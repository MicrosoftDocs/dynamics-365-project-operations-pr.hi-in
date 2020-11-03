---
title: कॉपी प्रोजेक्ट के साथ प्रोजेक्ट टेम्पलेट विकसित करें
description: यह विषय कॉपी प्रोजेक्ट कस्टम कार्रवाई का उपयोग करके प्रोजेक्ट टेम्पलेट बनाने के तरीके के बारे में जानकारी प्रदान करता है.
author: stsporen
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: cb49109e8c199bc4569702ae844a19985534294d
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077640"
---
# <a name="develop-project-templates-with-copy-project"></a><span data-ttu-id="fb0b1-103">कॉपी प्रोजेक्ट के साथ प्रोजेक्ट टेम्पलेट विकसित करें</span><span class="sxs-lookup"><span data-stu-id="fb0b1-103">Develop project templates with Copy Project</span></span>

<span data-ttu-id="fb0b1-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="fb0b1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="fb0b1-105">Dynamics 365 Project Operations किसी प्रोजेक्ट को कॉपी करने और किसी भी असाइनमेंट को जेनेरिक संसाधनों पर वापस करने की क्षमता का समर्थन करता है जो भूमिका का प्रतिनिधित्व करते हैं.</span><span class="sxs-lookup"><span data-stu-id="fb0b1-105">Dynamics 365 Project Operations supports the ability to copy a project and revert any assignments back to the generic resources that represent the role.</span></span> <span data-ttu-id="fb0b1-106">ग्राहक इस कार्यक्षमता का उपयोग बुनियादी प्रोजेक्ट टेम्पलेट्स बनाने के लिए कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="fb0b1-106">Customers can use this functionality to build basic project templates.</span></span>

<span data-ttu-id="fb0b1-107">जब आप **प्रोजेक्ट कॉपी करें** का चयन करते हैं, तो टारगेट प्रोजेक्ट की स्थिति अपडेट की जाती है.</span><span class="sxs-lookup"><span data-stu-id="fb0b1-107">When you select **Copy Project** , the status of the target project is updated.</span></span> <span data-ttu-id="fb0b1-108">कॉपी कार्रवाई कब पूरी हो जाए, यह निर्धारित करने के लिए **स्थिति कारण** का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="fb0b1-108">Use **Status Reason** to determine when the copy action is complete.</span></span> <span data-ttu-id="fb0b1-109">यदि टारगेट प्रोजेक्ट निकाय में कोई टारगेट तिथि का पता नहीं चला है **प्रोजेक्ट कॉपी करें** का चयन करना प्रोजेक्ट की शुरुआत की तिथि को वर्तमान प्रारंभ तिथि में भी अपडेट करता है.</span><span class="sxs-lookup"><span data-stu-id="fb0b1-109">Selecting **Copy Project** also updates the start date of the project to the current start date if no target date is detected in the target project entity.</span></span>

## <a name="copy-project-custom-action"></a><span data-ttu-id="fb0b1-110">प्रोजेक्ट कस्टम कार्रवाई कॉपी करें</span><span class="sxs-lookup"><span data-stu-id="fb0b1-110">Copy Project custom action</span></span> 

### <a name="name"></a><span data-ttu-id="fb0b1-111">नाम</span><span class="sxs-lookup"><span data-stu-id="fb0b1-111">Name</span></span> 

<span data-ttu-id="fb0b1-112">**msdyn_CopyProjectV2**</span><span class="sxs-lookup"><span data-stu-id="fb0b1-112">**msdyn_CopyProjectV2**</span></span>

### <a name="input-parameters"></a><span data-ttu-id="fb0b1-113">इनपुट पैरामीटर</span><span class="sxs-lookup"><span data-stu-id="fb0b1-113">Input parameters</span></span>
<span data-ttu-id="fb0b1-114">यहाँ तीन इनपुट पैरामीटर हैं:</span><span class="sxs-lookup"><span data-stu-id="fb0b1-114">There are three input parameters:</span></span>

| <span data-ttu-id="fb0b1-115">पैरामीटर</span><span class="sxs-lookup"><span data-stu-id="fb0b1-115">Parameter</span></span>          | <span data-ttu-id="fb0b1-116">प्रकार</span><span class="sxs-lookup"><span data-stu-id="fb0b1-116">Type</span></span>   | <span data-ttu-id="fb0b1-117">मान</span><span class="sxs-lookup"><span data-stu-id="fb0b1-117">Values</span></span>                                                   | 
|--------------------|--------|----------------------------------------------------------|
| <span data-ttu-id="fb0b1-118">ProjectCopyOption</span><span class="sxs-lookup"><span data-stu-id="fb0b1-118">ProjectCopyOption</span></span>  | <span data-ttu-id="fb0b1-119">String</span><span class="sxs-lookup"><span data-stu-id="fb0b1-119">String</span></span> | <span data-ttu-id="fb0b1-120">**{"removeNamedResources":true}** या **{"clearTeamsAndAssignments":true}**</span><span class="sxs-lookup"><span data-stu-id="fb0b1-120">**{"removeNamedResources":true}** or **{"clearTeamsAndAssignments":true}**</span></span> |
| <span data-ttu-id="fb0b1-121">SourceProject</span><span class="sxs-lookup"><span data-stu-id="fb0b1-121">SourceProject</span></span>      | <span data-ttu-id="fb0b1-122">संदर्भ निकाय</span><span class="sxs-lookup"><span data-stu-id="fb0b1-122">Entity Reference</span></span> | <span data-ttu-id="fb0b1-123">स्रोत प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="fb0b1-123">Source Project</span></span> |
| <span data-ttu-id="fb0b1-124">लक्ष्य</span><span class="sxs-lookup"><span data-stu-id="fb0b1-124">Target</span></span>             | <span data-ttu-id="fb0b1-125">संदर्भ निकाय</span><span class="sxs-lookup"><span data-stu-id="fb0b1-125">Entity Reference</span></span> | <span data-ttu-id="fb0b1-126">टारगेट प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="fb0b1-126">Target Project</span></span> |


- <span data-ttu-id="fb0b1-127">**{"clearTeamsAndAssignments":true}** : वेब के लिए प्रोजेक्ट के लिए डिफ़ॉल्ट व्यवहार, और सभी असाइनमेंट और टीम के सदस्यों को हटा देंगे.</span><span class="sxs-lookup"><span data-stu-id="fb0b1-127">**{"clearTeamsAndAssignments":true}** : Thee default behavior for Project for the Web, and will remove all assignments and team members.</span></span>
- <span data-ttu-id="fb0b1-128">**{"removeNamedResources":true}** Project Operations के लिए डिफ़ॉल्ट व्यवहार, और असाइनमेंटों को जेनेरिक संसाधनों पर वापस कर देगा.</span><span class="sxs-lookup"><span data-stu-id="fb0b1-128">**{"removeNamedResources":true}** The default behavior for Project Operations, and will revert assignments to generic resources.</span></span>

<span data-ttu-id="fb0b1-129">कार्रवाइयों पर अधिक डिफ़ॉल्ट के लिए, देखें [वेब API कार्रवाइयों का उपयोग करें](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span><span class="sxs-lookup"><span data-stu-id="fb0b1-129">For more defaults on actions, see [Use Web API actions](https://docs.microsoft.com/powerapps/developer/common-data-service/webapi/use-web-api-actions)</span></span>

## <a name="specify-fields-to-copy"></a><span data-ttu-id="fb0b1-130">कॉपी करने के लिए फ़ील्ड निर्दिष्ट करें</span><span class="sxs-lookup"><span data-stu-id="fb0b1-130">Specify fields to copy</span></span> 
<span data-ttu-id="fb0b1-131">जब कार्रवाई किया जाता है, तो **प्रोजेक्ट कॉपी करें** **प्रोजेक्ट कॉलम कॉपी करें** प्रोजेक्ट दृश्य को यह निर्धारित करने के लिए देखेगा कि प्रोजेक्ट को कॉपी करते समय किन फ़ील्डों को कॉपी करना है.</span><span class="sxs-lookup"><span data-stu-id="fb0b1-131">When the action is called, **Copy Project** will look at the project view **Copy Project Columns** to determine which fields to copy when the project is copied.</span></span>
