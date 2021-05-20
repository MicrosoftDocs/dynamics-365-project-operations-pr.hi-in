---
title: कॉपी प्रोजेक्ट के साथ प्रोजेक्ट टेम्पलेट विकसित करें
description: यह विषय कॉपी प्रोजेक्ट कस्टम कार्रवाई का उपयोग करके प्रोजेक्ट टेम्पलेट बनाने के तरीके के बारे में जानकारी प्रदान करता है.
author: stsporen
manager: Annbe
ms.date: 01/21/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cc17df0c73b276048f7c4b04bd9dc6644e828dc0
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949816"
---
# <a name="develop-project-templates-with-copy-project"></a>कॉपी प्रोजेक्ट के साथ प्रोजेक्ट टेम्पलेट विकसित करें

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

Dynamics 365 Project Operations परियोजना की प्रतिलिपि बनाने और भूमिका का प्रतिनिधित्व करने वाले जेनरिक संसाधनों पर किसी भी असाइनमेंट को वापस करने की क्षमता का समर्थन करता है. ग्राहक इस कार्यक्षमता का उपयोग बुनियादी प्रोजेक्ट टेम्पलेट्स बनाने के लिए कर सकते हैं.

जब आप **प्रोजेक्ट कॉपी करें** का चयन करते हैं, तो टारगेट प्रोजेक्ट की स्थिति अपडेट की जाती है. कॉपी कार्रवाई कब पूरी हो जाए, यह निर्धारित करने के लिए **स्थिति कारण** का उपयोग करें. यदि टारगेट प्रोजेक्ट निकाय में कोई टारगेट तिथि का पता नहीं चला है **प्रोजेक्ट कॉपी करें** का चयन करना प्रोजेक्ट की शुरुआत की तिथि को वर्तमान प्रारंभ तिथि में भी अपडेट करता है.

## <a name="copy-project-custom-action"></a>प्रोजेक्ट कस्टम कार्रवाई कॉपी करें 

### <a name="name"></a>नाम 

**msdyn_CopyProjectV2**

### <a name="input-parameters"></a>इनपुट पैरामीटर
यहाँ तीन इनपुट पैरामीटर हैं:

| पैरामीटर          | प्रकार   | मान                                                   | 
|--------------------|--------|----------------------------------------------------------|
| ProjectCopyOption  | String | **{"removeNamedResources":true}** या **{"clearTeamsAndAssignments":true}** |
| SourceProject      | संदर्भ निकाय | स्रोत प्रोजेक्ट |
| लक्ष्य             | संदर्भ निकाय | टारगेट प्रोजेक्ट |


- **{"clearTeamsAndAssignments":true}**: वेब के लिए प्रोजेक्ट के लिए डिफ़ॉल्ट व्यवहार, और सभी असाइनमेंट और टीम के सदस्यों को हटा देंगे.
- **{"removeNamedResources":true}** Project Operations के लिए डिफ़ॉल्ट व्यवहार, और असाइनमेंटों को जेनेरिक संसाधनों पर वापस कर देगा.

कार्रवाइयों पर अधिक डिफ़ॉल्ट के लिए, देखें [वेब API कार्रवाइयों का उपयोग करें](/powerapps/developer/common-data-service/webapi/use-web-api-actions)

## <a name="specify-fields-to-copy"></a>कॉपी करने के लिए फ़ील्ड निर्दिष्ट करें 
जब कार्रवाई किया जाता है, तो **प्रोजेक्ट कॉपी करें** **प्रोजेक्ट कॉलम कॉपी करें** प्रोजेक्ट दृश्य को यह निर्धारित करने के लिए देखेगा कि प्रोजेक्ट को कॉपी करते समय किन फ़ील्डों को कॉपी करना है.


### <a name="example"></a>उदाहरण
निम्न उदाहरण **removeNamedResources** पैरामीटर के साथ **CopyProject** कस्टम क्रिया को कॉल करने का तरीका दिखाता है.
```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

    [DataContract]
    public class ProjectCopyOption
    {
        /// <summary>
        /// Clear teams and assignments.
        /// </summary>
        [DataMember(Name = "clearTeamsAndAssignments")]
        public bool ClearTeamsAndAssignments { get; set; }

        /// <summary>
        /// Replace named resource with generic resource.
        /// </summary>
        [DataMember(Name = "removeNamedResources")]
        public bool ReplaceNamedResources { get; set; }
    }

    public class CopyProjectSample
    {
        private IOrganizationService organizationService;

        public CopyProjectSample(IOrganizationService organizationService)
        {
            this.organizationService = organizationService;
        }

        public void SampleRun()
        {
            // Example source project GUID
            Guid sourceProjectId = new Guid("11111111-1111-1111-1111-111111111111");
            var sourceProject = new Entity("msdyn_project", sourceProjectId);

            Entity targetProject = new Entity("msdyn_project");
            targetProject["msdyn_subject"] = "Example Project";
            targetProject.Id = organizationService.Create(targetProject);

            ProjectCopyOption copyOption = new ProjectCopyOption();
            copyOption.ReplaceNamedResources = true;

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, ProjectCopyOption projectCopyOption)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV2");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;
            req["ProjectCopyOption"] = JsonConvert.SerializeObject(projectCopyOption);
            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```


[!INCLUDE[footer-include](../includes/footer-banner.md)]