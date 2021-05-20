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
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="142db-103">कॉपी प्रोजेक्ट के साथ प्रोजेक्ट टेम्पलेट विकसित करें</span><span class="sxs-lookup"><span data-stu-id="142db-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="142db-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="142db-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="142db-105">Dynamics 365 Project Operations परियोजना की प्रतिलिपि बनाने और भूमिका का प्रतिनिधित्व करने वाले जेनरिक संसाधनों पर किसी भी असाइनमेंट को वापस करने की क्षमता का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="142db-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="142db-106">ग्राहक इस कार्यक्षमता का उपयोग बुनियादी प्रोजेक्ट टेम्पलेट्स बनाने के लिए कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="142db-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="142db-107">जब आप **प्रोजेक्ट कॉपी करें** का चयन करते हैं, तो टारगेट प्रोजेक्ट की स्थिति अपडेट की जाती है.</span><span class="sxs-lookup"><span data-stu-id="142db-107">When you select **Copy Project**, the status of the target project is updated.</span></span> <span data-ttu-id="142db-108">कॉपी कार्रवाई कब पूरी हो जाए, यह निर्धारित करने के लिए **स्थिति कारण** का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="142db-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="142db-109">यदि टारगेट प्रोजेक्ट निकाय में कोई टारगेट तिथि का पता नहीं चला है **प्रोजेक्ट कॉपी करें** का चयन करना प्रोजेक्ट की शुरुआत की तिथि को वर्तमान प्रारंभ तिथि में भी अपडेट करता है.</span><span class="sxs-lookup"><span data-stu-id="142db-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="142db-110">प्रोजेक्ट कस्टम कार्रवाई कॉपी करें</span><span class="sxs-lookup"><span data-stu-id="142db-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="142db-111">नाम</span><span class="sxs-lookup"><span data-stu-id="142db-111">Name</span></span> 

<span data-ttu-id="142db-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="142db-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="142db-113">इनपुट पैरामीटर</span><span class="sxs-lookup"><span data-stu-id="142db-113">Input parameters</span></span>
<span data-ttu-id="142db-114">यहाँ तीन इनपुट पैरामीटर हैं:</span><span class="sxs-lookup"><span data-stu-id="142db-114">There are three input parameters:</span></span>

| <span data-ttu-id="142db-115">पैरामीटर</span><span class="sxs-lookup"><span data-stu-id="142db-115">Parameter</span></span>          | <span data-ttu-id="142db-116">प्रकार</span><span class="sxs-lookup"><span data-stu-id="142db-116">Type</span></span>   | <span data-ttu-id="142db-117">मान</span><span class="sxs-lookup"><span data-stu-id="142db-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="142db-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="142db-118">ProjectCopyOption</span></span>  | <span data-ttu-id="142db-119">String</span><span class="sxs-lookup"><span data-stu-id="142db-119">String</span></span> | <span data-ttu-id="142db-120">**{"removeNamedResources":true}** या **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="142db-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="142db-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="142db-121">SourceProject</span></span>      | <span data-ttu-id="142db-122">संदर्भ निकाय</span><span class="sxs-lookup"><span data-stu-id="142db-122">Entity Reference</span></span> | <span data-ttu-id="142db-123">स्रोत प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="142db-123">Source Project</span></span> |
| <span data-ttu-id="142db-124">लक्ष्य</span><span class="sxs-lookup"><span data-stu-id="142db-124">Target</span></span>             | <span data-ttu-id="142db-125">संदर्भ निकाय</span><span class="sxs-lookup"><span data-stu-id="142db-125">Entity Reference</span></span> | <span data-ttu-id="142db-126">टारगेट प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="142db-126">Target Project</span></span> |


- <span data-ttu-id="142db-127">**{"clearTeamsAndAssignments":true}**: वेब के लिए प्रोजेक्ट के लिए डिफ़ॉल्ट व्यवहार, और सभी असाइनमेंट और टीम के सदस्यों को हटा देंगे.</span><span class="sxs-lookup"><span data-stu-id="142db-127">**{"clearTeamsAndAssignments":true}**: Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="142db-128">**{"removeNamedResources":true}** Project Operations के लिए डिफ़ॉल्ट व्यवहार, और असाइनमेंटों को जेनेरिक संसाधनों पर वापस कर देगा.</span><span class="sxs-lookup"><span data-stu-id="142db-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="142db-129">कार्रवाइयों पर अधिक डिफ़ॉल्ट के लिए, देखें [वेब API कार्रवाइयों का उपयोग करें](/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span><span class="sxs-lookup"><span data-stu-id="142db-129">For more defaults on actions, see [Use Web API actions](/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="142db-130">कॉपी करने के लिए फ़ील्ड निर्दिष्ट करें</span><span class="sxs-lookup"><span data-stu-id="142db-130">Specify fields to copy</span></span> 
<span data-ttu-id="142db-131">जब कार्रवाई किया जाता है, तो **प्रोजेक्ट कॉपी करें** **प्रोजेक्ट कॉलम कॉपी करें** प्रोजेक्ट दृश्य को यह निर्धारित करने के लिए देखेगा कि प्रोजेक्ट को कॉपी करते समय किन फ़ील्डों को कॉपी करना है.</span><span class="sxs-lookup"><span data-stu-id="142db-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>


### <a name="example"></a><span data-ttu-id="142db-132">उदाहरण</span><span class="sxs-lookup"><span data-stu-id="142db-132">Example</span></span>
<span data-ttu-id="142db-133">निम्न उदाहरण **removeNamedResources** पैरामीटर के साथ **CopyProject** कस्टम क्रिया को कॉल करने का तरीका दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="142db-133">The following example shows how to call the **CopyProject** custom action with the **removeNamedResources** parameter set.</span></span>
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