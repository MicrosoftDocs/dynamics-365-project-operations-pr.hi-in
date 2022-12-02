---
title: कॉपी प्रोजेक्ट के साथ प्रोजेक्ट टेम्पलेट विकसित करें
description: यह आलेख कॉपी प्रोजेक्ट कस्टम कार्रवाई का उपयोग करके प्रोजेक्ट टेम्पलेट बनाने के तरीके के बारे में जानकारी प्रदान करता है.
author: stsporen
ms.date: 03/10/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 47c1023bbc4c21e3571bffbf3670bf0f7854f81d
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8923834"
---
# <a name="develop-project-templates-with-copy-project"></a>कॉपी प्रोजेक्ट के साथ प्रोजेक्ट टेम्पलेट विकसित करें

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

Dynamics 365 Project Operations परियोजना की प्रतिलिपि बनाने और भूमिका का प्रतिनिधित्व करने वाले जेनरिक संसाधनों पर किसी भी असाइनमेंट को वापस करने की क्षमता का समर्थन करता है. ग्राहक इस कार्यक्षमता का उपयोग बुनियादी प्रोजेक्ट टेम्पलेट्स बनाने के लिए कर सकते हैं.

जब आप **प्रोजेक्ट कॉपी करें** का चयन करते हैं, तो टारगेट प्रोजेक्ट की स्थिति अपडेट की जाती है. कॉपी कार्रवाई कब पूरी हो जाए, यह निर्धारित करने के लिए **स्थिति कारण** का उपयोग करें. यदि टारगेट प्रोजेक्ट निकाय में कोई टारगेट तिथि का पता नहीं चला है **प्रोजेक्ट कॉपी करें** का चयन करना प्रोजेक्ट की शुरुआत की तिथि को वर्तमान प्रारंभ तिथि में भी अपडेट करता है.

## <a name="copy-project-custom-action"></a>प्रोजेक्ट कस्टम कार्रवाई कॉपी करें

### <a name="name"></a>Name 

msdyn\_CopyProjectV3

### <a name="input-parameters"></a>इनपुट पैरामीटर

यहाँ तीन इनपुट पैरामीटर हैं:

- **ReplaceNamedResources** या **ClearTeamsAndAssignments** - विकल्पों में से केवल एक सेट करें. दोनों सेट मत करो.

    - **\{"ReplaceNamedResources":सच\}** - Project Operations के लिए डिफ़ॉल्ट व्यवहार. कोई नाम युक्त संसाधनों को सामान्य संसाधनों से स्थानापन्न किया जाता है.
    - **\{"ClearTeamsAndAssignments":सच\}** - Project for the Web के लिए डिफ़ॉल्ट व्यवहार. सभी असाइनमेंट और टीम के सदस्यों को हटा दिया जाता है.

- **SourceProject** - कॉपी करने के लिए स्रोत प्रोजेक्ट का निकाय संदर्भ. यह पैरामीटर शून्य नहीं हो सकता.
- **लक्ष्‍य** - कॉपी करने के लिए लक्षित प्रोजेक्ट का इकाई संदर्भ. यह पैरामीटर शून्य नहीं हो सकता.

निम्न तालिका तीन मापदंडों का सारांश प्रदान करती है.

| मापदंड                | Type             | मान                 |
|--------------------------|------------------|-----------------------|
| ReplaceNamedResources    | Boolean          | **सही** या **गलत** |
| ClearTeamsAndAssignments | Boolean          | **सही** या **गलत** |
| SourceProject            | निकाय संदर्भ | स्रोत परियोजना    |
| लक्ष्य                   | निकाय संदर्भ | टारगेट प्रोजेक्ट    |

कार्रवाइयों पर अधिक डिफ़ॉल्ट के लिए, देखें [वेब API कार्रवाइयों का उपयोग करें](/powerapps/developer/common-data-service/webapi/use-web-api-actions).

### <a name="validations"></a>सत्यापन

निम्नलिखित सत्यापन किए जाते हैं.

1. संगठन में दोनों परियोजनाओं के अस्तित्व की पुष्टि करने के लिए नल जांच और स्रोत और लक्ष्य परियोजनाओं को पुनः प्राप्त करता है.
2. सिस्टम पुष्टि करता है कि लक्ष्य परियोजना निम्नलिखित शर्तों की पुष्टि करके प्रतिलिपि बनाने के लिए मान्य है:

    - परियोजना पर कोई पिछली गतिविधि नहीं है (के चयन सहित **कार्य** टैब), और परियोजना नव निर्मित है.
    - इस परियोजना पर कोई पिछली प्रति नहीं है, किसी आयात का अनुरोध नहीं किया गया है, और परियोजना की **असफल** स्थिति नहीं है.

3. HTTP का उपयोग करके ऑपरेशन को कॉल नहीं किया जाता है.

## <a name="specify-fields-to-copy"></a>कॉपी करने के लिए फ़ील्ड निर्दिष्ट करें

जब कार्रवाई किया जाता है, तो **प्रोजेक्ट कॉपी करें** **प्रोजेक्ट कॉलम कॉपी करें** प्रोजेक्ट दृश्य को यह निर्धारित करने के लिए देखेगा कि प्रोजेक्ट को कॉपी करते समय किन फ़ील्डों को कॉपी करना है.

### <a name="example"></a>उदाहरण

निम्न उदाहरण **removeNamedResources** पैरामीटर के साथ **CopyProjectV3** कस्टम क्रिया को कॉल करने का तरीका दिखाता है.

```C#
{
    using System;
    using System.Runtime.Serialization;
    using Microsoft.Xrm.Sdk;
    using Newtonsoft.Json;

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
            targetProject["msdyn_subject"] = "Example Project - Copy";
            targetProject.Id = organizationService.Create(targetProject);

            CallCopyProjectAPI(sourceProject.ToEntityReference(), targetProject.ToEntityReference(), copyOption, true, false);
            Console.WriteLine("Done ...");
        }

        private void CallCopyProjectAPI(EntityReference sourceProject, EntityReference TargetProject, bool replaceNamedResources = true, bool clearTeamsAndAssignments = false)
        {
            OrganizationRequest req = new OrganizationRequest("msdyn_CopyProjectV3");
            req["SourceProject"] = sourceProject;
            req["Target"] = TargetProject;

            if (replaceNamedResources)
            {
                req["ReplaceNamedResources"] = true;
            }
            else
            {
                req["ClearTeamsAndAssignments"] = true;
            }

            OrganizationResponse response = organizationService.Execute(req);
        }
    }
}
```

[!INCLUDE[footer-include](../includes/footer-banner.md)]
