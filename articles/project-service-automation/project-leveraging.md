---
title: विक्रय अनुमान और प्रोजेक्ट
description: इस विषय में बिक्री की प्रक्रिया में शेड्यूल और आकलनों का लाभ लेने के बारे में जानकारी दी गई है।
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: eb5ab6a1-fdff-490e-9c2a-19aef493de11
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 4431c1c894a01bfecc132575d8981ebc9fe50b51
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751994"
---
# <a name="sales-estimates-and-projects"></a><span data-ttu-id="869e2-103">विक्रय अनुमान और प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="869e2-103">Sales estimates and projects</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="869e2-104">बिक्री की प्रक्रिया के दौरान, आप प्रोजेक्ट को बिक्री के कोट से जोड़ते हुए बिक्री के आकलन तैयार कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="869e2-104">During the sales process, you can create sales estimates by linking a project to a sales quote.</span></span> <span data-ttu-id="869e2-105">इस तरह, प्रोजेक्ट की शेड्यूलिंग और आकलन सुविधाओं का लाभ लेने के लिए बिक्री की प्रक्रिया के दौरान बेहतर आकलन किए जा सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="869e2-105">In this way, deterministic estimation can occur during the sales process, to take advantage of project scheduling and estimation capabilities.</span></span> <span data-ttu-id="869e2-106">यदि बिक्री अच्छी होती है तो बिक्री आकलन के प्रयोजन के लिए इस्तेमाल किए जाने वाला शेड्यूल का इस्तेमाल प्रोजेक्ट की योजना को बेहतर करने के लिए किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="869e2-106">If the sale goes through, the schedule that was used for sales estimation purposes can be used as the basis for further refinement of the project plan.</span></span>

## <a name="linking-a-project-to-a-quote-line"></a><span data-ttu-id="869e2-107">एक प्रोजेक्ट को कोट लाइन से जोड़ना</span><span class="sxs-lookup"><span data-stu-id="869e2-107">Linking a project to a quote line</span></span>

<span data-ttu-id="869e2-108">जब आप प्रोजेक्ट-आधारित कोट लाइन बनाते हैं, आप **कोट लाइन** पेज पर नया प्रोजेक्ट बना सकते हैं या मौजूदा प्रोजेक्ट का एसोसिएट बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="869e2-108">When you create a project-based quote line, you can create a new project or associate an existing project pn the **Quote Line** page.</span></span> 

> ![कोट लाइन फार्म](media/project-8.png)
 
<span data-ttu-id="869e2-110">जब आप कोट लाइन विवरण से नया प्रोजेक्ट बनाते हैं तो आप प्रोजेक्ट के टैम्पलेट का लाभ ले सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="869e2-110">When you create a new project from the quote line details, you can take advantage of project templates.</span></span> <span data-ttu-id="869e2-111">प्रोजेक्ट टैम्पलेट मॉडल प्रोजेक्ट होते हैं जो किसी संगठन में सामान्य मानक प्रोजेक्ट योजनाओं और वितीय आकलनों को दर्शाते हैं।</span><span class="sxs-lookup"><span data-stu-id="869e2-111">Project templates are model projects that represent standard project plans and financial estimates that are typical in an organization.</span></span> <span data-ttu-id="869e2-112">वे पिछले प्रोजेक्ट की योजनाओं और आकलनों की कॉपी भी हो सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="869e2-112">They can also represent copies of project plans and estimates from past projects.</span></span>

> ![कोटेशन लाइन का विवरण](media/project-9.png)
  
<span data-ttu-id="869e2-114">जब आप किसी कोट से प्रोजेक्ट तैयार करते हैं तो यह प्रोजेक्ट अपने आप कोट लाइन से जुड़ जाता है।</span><span class="sxs-lookup"><span data-stu-id="869e2-114">When you create the project from the quote, the project is automatically associated with the quote line.</span></span>

## <a name="components-of-estimates-in-a-project"></a><span data-ttu-id="869e2-115">एक प्रोजेक्ट के आकलनों के घटक</span><span class="sxs-lookup"><span data-stu-id="869e2-115">Components of estimates in a project</span></span>

<span data-ttu-id="869e2-116">शेड्यूल से आप कार्य को टास्क में विभाजित कर सकते हैं, टास्क का पदानुक्रम बनाए रख सकते हैं, यह तय कर सकते हैं कि टास्क को पूरा करने के लिए किन संसाधन की आवश्यकता है और उस टास्क को पूरा करने के लिए आवश्यक प्रयास का आकलन कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="869e2-116">A schedule lets you divide work into tasks, maintain a hierarchy of tasks, determine what resources are required to complete a task, and assign an estimate of the effort that is required to complete a task.</span></span>

<span data-ttu-id="869e2-117">आप **प्रोजेक्ट** पेज के **शेड्यूल** टैब पर फील्ड का इस्तेमाल करते हुए कार्य के प्रयास और शेड्यूल के आकलनों को परिभाषित कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="869e2-117">You can define the work effort and schedule estimates by using the fields on the **Schedule** tab of the **Project** page.</span></span> <span data-ttu-id="869e2-118">चूँकि कीमत सूची प्रोजेक्ट से जुड़ी होती है, वित्तीय आकलनों का परिकलन लागत और बिक्री की कीमत जो कीमत सूची में परिभाषित होते हैं, का इस्तेमाल करते हुए किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="869e2-118">Because a price list is associated with the project, financial estimates are calculated by using cost and sales prices that are defined in the price list.</span></span>

## <a name="importing-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="869e2-119">आकलनों को प्रोजेक्ट से कोट में लाना</span><span class="sxs-lookup"><span data-stu-id="869e2-119">Importing estimates from a project into a quote</span></span>

<span data-ttu-id="869e2-120">प्रोजेक्ट के आकलनों को परिभाषित करने के बाद, आप उन्हें कोट लाइन में ला सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="869e2-120">After you define project estimates, you can import them into the quote line.</span></span> <span data-ttu-id="869e2-121">**कोट लाइन डीटेल्स** पेज पर, प्रकार, भूमिका या टास्क स्तर द्वारा प्रोजेक्ट को आकलनों का विवरण बनाने के लिए रिब्बन पर **अनुमानों से आयात करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="869e2-121">On the **Quote Line Details** page, select **Import from estimates** on the ribbon to summarize project estimates by transaction type, role, or task level.</span></span>
