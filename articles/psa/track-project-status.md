---
title: परियोजना की स्थिति ट्रैक करें
description: Project Service में परियोजना की स्थिति को ट्रैक करने का तरीका
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: e9c8b594d468016264d0b4d9745597a35f55e50e
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149590"
---
# <a name="track-a-projects-status-project-service"></a><span data-ttu-id="859ae-103">परियोजना की स्थिति ट्रैक करना (Project Service)</span><span class="sxs-lookup"><span data-stu-id="859ae-103">Track a project’s status (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="859ae-104">किसी क्लाइंट की परियोजना की प्रगति को ट्रैक करने के लिए [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="859ae-104">Use the [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] to track the progress of a client’s project.</span></span>  

<span data-ttu-id="859ae-105">व्‍यस्‍तता बढ़ने के साथ-साथ, परियोजना अवस्‍थाएँ अद्यतन होती हैं ताकि व्‍यस्‍तता की अवस्‍था दर्शाई जा सके:</span><span class="sxs-lookup"><span data-stu-id="859ae-105">As the engagement progresses, the project stages update to reflect the stage of the engagement:</span></span>  


|              |                                                                                                                                                                                                                                                                                                  |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   <span data-ttu-id="859ae-106">**नया**</span><span class="sxs-lookup"><span data-stu-id="859ae-106">**New**</span></span>    | <span data-ttu-id="859ae-107">जब आप एक परियोजना बनाते हैं, तो अवस्‍था को **नया** पर सेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="859ae-107">When you create a project, the stage is set to **New**.</span></span> <span data-ttu-id="859ae-108">यदि आपने परियोजना एक टेम्‍पलेट से बनाई है, तो इस अवस्‍था पर परियोजना के पास एक शेड्यूल, अनुमान और टीम डेटा हो सकता है.</span><span class="sxs-lookup"><span data-stu-id="859ae-108">If you created the project from a template, at this stage the project may have a schedule, estimates, and team data.</span></span> <span data-ttu-id="859ae-109">अन्यथा, परियोजना की रूपरेखा मौजूद होगी और आपको शेष परियोजना घटक मैन्युअल रूप से दर्ज करना पड़ेगा.</span><span class="sxs-lookup"><span data-stu-id="859ae-109">Otherwise, it will be the outline of the project and you need to manually enter the rest of the project components.</span></span> |
|  <span data-ttu-id="859ae-110">**कोट**</span><span class="sxs-lookup"><span data-stu-id="859ae-110">**Quote**</span></span>   |      <span data-ttu-id="859ae-111">जब आप किसी परियोजना को एक कोट से संबद्ध करते हैं, या इसे कोट से बनाते हैं, तो परियोजना अवस्‍था **कोट** पर सेट की जाती है, और अनुमानित प्रारंभ और समाप्ति दिनांक का अद्यतन भी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="859ae-111">When you associate a project to a quote or create it from a quote, the project stage is set to **Quote**, and the estimated start and end datesare updated as well.</span></span> <span data-ttu-id="859ae-112">जब परियोजना एक कोट अवस्‍था में है, तो कोट पर विवरण **परियोजना** पृष्ठ पर **विक्रय** टैब पर प्रदर्शित होता है.</span><span class="sxs-lookup"><span data-stu-id="859ae-112">When the project is in the quote stage, details on the quote display on the **Sales** tab on the **Project** page.</span></span>      |
|   <span data-ttu-id="859ae-113">**योजना**</span><span class="sxs-lookup"><span data-stu-id="859ae-113">**Plan**</span></span>   |                                     <span data-ttu-id="859ae-114">जब आप किसी परियोजना के साथ संबद्ध कोट जीतते हैं, और जब व्‍यस्‍तताएँ अनुबंध अवस्‍था पर बढ़ती हैं, तो परियोजना अवस्‍था **योजना** पर अद्यतन करती है.</span><span class="sxs-lookup"><span data-stu-id="859ae-114">When you win a quote associated with a project, and when the engagement progresses to the contract stage, the project stage updates to **Plan**.</span></span> <span data-ttu-id="859ae-115">**परियोजना** पृष्ठ पर, अनुबंध विवरण **विक्रय** टैब पर प्रदर्शित होते हैं.</span><span class="sxs-lookup"><span data-stu-id="859ae-115">Contract details display on the **Sales** tab on the **Project** page.</span></span>                                      |
| <span data-ttu-id="859ae-116">**पूर्ण**</span><span class="sxs-lookup"><span data-stu-id="859ae-116">**Complete**</span></span> |                    <span data-ttu-id="859ae-117">जब परियोजना पूर्ण होती है, तो आप अवस्था को **पूर्ण** पर फ़्लिप कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="859ae-117">When the project work is complete, you can flip the stage to **Complete**.</span></span> <span data-ttu-id="859ae-118">जब परियोजना चरण पर सेट होता है, तो यह समझा जाता है कि कार्य 100% पूर्ण हो गया है, परंतु परियोजना किसी भी लंबित समय या व्‍यय प्रविष्टि रिकार्ड किए जाने के लिए खुली रखी जाती है.</span><span class="sxs-lookup"><span data-stu-id="859ae-118">When the project stage is set to complete, it’s understood that the work is 100% complete but the project is kept open for any pending time or expense entries to be recorded.</span></span>                     |
|  <span data-ttu-id="859ae-119">**बंद करें**</span><span class="sxs-lookup"><span data-stu-id="859ae-119">**Close**</span></span>   |           <span data-ttu-id="859ae-120">जब परियोजना में सभी लेन-देन को रिकॉर्ड कर लिया जाता है, और आप इसके बाद और लॉग ऑन करने की अपेक्षा नहीं करते, तो आप अवस्‍था को मैन्‍युअल रूप से **बंद** पर सेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="859ae-120">When all transactions have been recorded on the project and you don't expect any more to be logged, you can manually set the stage to **Close**.</span></span> <span data-ttu-id="859ae-121">जब परियोजना **बंद** पर सेट कर दिया जाता है, किसी परियोजना पर कोई और लेन-देन लॉग नहीं कर सकते और परियोजना केवल पढ़ने के लिए हो जाएगी.</span><span class="sxs-lookup"><span data-stu-id="859ae-121">When the project is set to **Close**, you can’t log any more transactions on the project and the project will be read only.</span></span>           |

## <a name="to-track-a-projects-status"></a><span data-ttu-id="859ae-122">एक परियोजना स्थिति ट्रैक करना</span><span class="sxs-lookup"><span data-stu-id="859ae-122">To track a project’s status</span></span>  

1.  <span data-ttu-id="859ae-123">**Project Service > परियोजना** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="859ae-123">Go to **Project Service > Projects**.</span></span>  

2.  <span data-ttu-id="859ae-124">जिस परियोजना पर आप काम करना चाहते हैं, उस पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="859ae-124">Click the project you want to work on.</span></span>  

3.  <span data-ttu-id="859ae-125">स्क्रीन के ऊपर पट्टी में, परियोजना नाम के आगे स्थित नीचे तीर का चयन करें, और उसके बाद **परियोजना ट्रैकिंग** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="859ae-125">In the bar across the top of the screen, select the down arrow next to the project name, and then click **Project Tracking**.</span></span>  

4.  <span data-ttu-id="859ae-126">कार्य सूची के ऊपर ड्रॉप डाउन सूची में **प्रयास ट्रैकिंग** या **लागत ट्रैकिंग** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="859ae-126">Select **Effort Tracking** or **Cost Tracking** in the drop-down list above the task list.</span></span>  

5.  <span data-ttu-id="859ae-127">किसी भी कार्य को संपादित करने के लिए उसे डबल-क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="859ae-127">Double-click any task to edit it.</span></span> <span data-ttu-id="859ae-128">आप कार्य के समय और प्रगति में परिवर्तन करने के लिए गैंट चार्ट पर स्‍तंभों को स्‍थानांतरित कर सकते हैं या उनका आकार बदल सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="859ae-128">You can also move or resize the bars in the Gantt chart to change the time and progress for a task.</span></span>  

### <a name="see-also"></a><span data-ttu-id="859ae-129">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="859ae-129">See Also</span></span>  
 [<span data-ttu-id="859ae-130">परियोजना प्रबंधक मार्गदर्शिका</span><span class="sxs-lookup"><span data-stu-id="859ae-130">Project Manager Guide</span></span>](../psa/project-manager-guide.md)
