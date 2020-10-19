---
title: व्यय श्रेणियाँ सेटअप करें
description: यह विषय व्यय रिपोर्ट और साझा रिपोर्ट के लिए साझा श्रेणियां सेट करने के तरीके के बारे में जानकारी प्रदान करता है।
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: f051d70f3dfe3b241dc0a206c0cdfda000f87c76
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896688"
---
# <a name="set-up-expense-categories"></a><span data-ttu-id="e1c81-103">व्यय श्रेणियाँ सेटअप करें</span><span class="sxs-lookup"><span data-stu-id="e1c81-103">Set up expense categories</span></span>

<span data-ttu-id="e1c81-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="e1c81-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="e1c81-105">जब कर्मचारी व्यय रिपोर्ट बनाते हैं, तो प्रत्येक व्यय जो वे रिकॉर्ड करते हैं, को एक व्यय श्रेणी से जुड़ा होना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="e1c81-105">When employees create expense reports, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="e1c81-106">व्यय श्रेणियों को साझा की गई श्रेणियों से प्राप्त किया जाता है, जिन्हें आपके संगठन में कानूनी निकायों के बीच साझा किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="e1c81-106">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="e1c81-107">आपके संगठन को कैसे परिभाषित किया जाता है, इसके आधार पर, इन व्यय श्रेणियों को अन्य क्षेत्रों में भी साझा किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="e1c81-107">Depending on how your organization is defined, these expense categories can also be shared in other areas.</span></span> <span data-ttu-id="e1c81-108">आपके संगठन की परिभाषा और कार्यान्वयन टीम से मार्गदर्शन के आधार पर, आपको यह निर्धारित करना होगा कि क्या व्यय प्रबंधन में उपयोग की जाने वाली श्रेणियां केवल व्यय प्रबंधन में उपयोग की जाएंगी या उनको अन्य क्षेत्रों में साझा किया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="e1c81-108">Based on the definition of your organization and guidance from the implementation team, you must determine whether the categories that are used in Expense management will be used only in Expense management or should be shared in other areas.</span></span>

> [!NOTE]
> <span data-ttu-id="e1c81-109">इन श्रेणियों को परियोजना प्रबंधन और लेखांकन और व्यय प्रबंधन, या परियोजना प्रबंधन और लेखा और उत्पादन के बीच साझा किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="e1c81-109">These categories can be shared between Project management and accounting and Expense management, or between Project management and accounting and Production.</span></span> <span data-ttu-id="e1c81-110">हालांकि, उन्हें व्यय प्रबंधन और उत्पादन के बीच साझा नहीं किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="e1c81-110">However, they can't be shared between Expense management and Production.</span></span>

<span data-ttu-id="e1c81-111">सेटअप प्रक्रिया शुरू करने से पहले, प्रत्येक व्यय श्रेणी के लिए निम्नलिखित निर्णय लिए जाने चाहिए:</span><span class="sxs-lookup"><span data-stu-id="e1c81-111">Before you can begin the setup process, the following decisions must be made for each expense category:</span></span>

- <span data-ttu-id="e1c81-112">व्यय श्रेणी क्या है?</span><span class="sxs-lookup"><span data-stu-id="e1c81-112">What is the expense category?</span></span> <span data-ttu-id="e1c81-113">उदाहरणों में उड़ानों, होटल या माइलेज के लिए श्रेणियां शामिल हैं।</span><span class="sxs-lookup"><span data-stu-id="e1c81-113">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="e1c81-114">क्या व्यय श्रेणी का उपयोग परियोजना प्रबंधन और लेखा में भी किया जा सकता है?</span><span class="sxs-lookup"><span data-stu-id="e1c81-114">Can the expense category also be used in Project management and accounting?</span></span> <span data-ttu-id="e1c81-115">यदि यह हो सकता है, तो आपको निम्नलिखित निर्णय भी करने होंगे:</span><span class="sxs-lookup"><span data-stu-id="e1c81-115">If it can, you must also make the following decisions:</span></span>

    - <span data-ttu-id="e1c81-116">निम्नलिखित खर्चों के लिए किन व्यय खातों का उपयोग किया जाएगा?</span><span class="sxs-lookup"><span data-stu-id="e1c81-116">Which cost accounts will be used for the following expenses?</span></span>

        - <span data-ttu-id="e1c81-117">लागत</span><span class="sxs-lookup"><span data-stu-id="e1c81-117">Cost</span></span>
        - <span data-ttu-id="e1c81-118">पेरोल आवंटन</span><span class="sxs-lookup"><span data-stu-id="e1c81-118">Payroll allocation</span></span>
        - <span data-ttu-id="e1c81-119">WIP-लागत मूल्य</span><span class="sxs-lookup"><span data-stu-id="e1c81-119">WIP-cost value</span></span>
        - <span data-ttu-id="e1c81-120">लागत-आइटम</span><span class="sxs-lookup"><span data-stu-id="e1c81-120">Cost-item</span></span>
        - <span data-ttu-id="e1c81-121">WIP-लागत मूल्य-आइटम</span><span class="sxs-lookup"><span data-stu-id="e1c81-121">WIP-cost value-item</span></span>
        - <span data-ttu-id="e1c81-122">उपार्जित नुकसान</span><span class="sxs-lookup"><span data-stu-id="e1c81-122">Accrued loss</span></span>
        - <span data-ttu-id="e1c81-123">WIP-उपार्जित नुकसान</span><span class="sxs-lookup"><span data-stu-id="e1c81-123">WIP-accrued loss</span></span>

    - <span data-ttu-id="e1c81-124">राजस्व के निम्नलिखित स्रोतों के लिए कौन से राजस्व खातों का उपयोग किया जाएगा?</span><span class="sxs-lookup"><span data-stu-id="e1c81-124">Which revenue accounts will be used for the following sources of revenue?</span></span>

        - <span data-ttu-id="e1c81-125">इनवॉइस की गई आमदनी</span><span class="sxs-lookup"><span data-stu-id="e1c81-125">Invoiced revenue</span></span>
        - <span data-ttu-id="e1c81-126">उपार्जित राजस्व-बिक्री मूल्य</span><span class="sxs-lookup"><span data-stu-id="e1c81-126">Accrued revenue-sales value</span></span>
        - <span data-ttu-id="e1c81-127">WIP-विक्रय मूल्य</span><span class="sxs-lookup"><span data-stu-id="e1c81-127">WIP-sales value</span></span>
        - <span data-ttu-id="e1c81-128">उपार्जित राजस्व-उत्पादन</span><span class="sxs-lookup"><span data-stu-id="e1c81-128">Accrued revenue-production</span></span>
        - <span data-ttu-id="e1c81-129">WIP-उत्पादन</span><span class="sxs-lookup"><span data-stu-id="e1c81-129">WIP-production</span></span>
        - <span data-ttu-id="e1c81-130">उपार्जित राजस्व-लाभ</span><span class="sxs-lookup"><span data-stu-id="e1c81-130">Accrued revenue-profit</span></span>
        - <span data-ttu-id="e1c81-131">WIP-लाभ</span><span class="sxs-lookup"><span data-stu-id="e1c81-131">WIP-profit</span></span>
        - <span data-ttu-id="e1c81-132">उपार्जित राजस्व-सदस्यता</span><span class="sxs-lookup"><span data-stu-id="e1c81-132">Accrued revenue-subscription</span></span>
        - <span data-ttu-id="e1c81-133">WIP-सदस्यता</span><span class="sxs-lookup"><span data-stu-id="e1c81-133">WIP-subscription</span></span>

- <span data-ttu-id="e1c81-134">व्यय प्रकार क्या है?</span><span class="sxs-lookup"><span data-stu-id="e1c81-134">What is the expense type?</span></span>
- <span data-ttu-id="e1c81-135">व्यय श्रेणी के लिए डिफ़ॉल्ट भुगतान विधि क्या है?</span><span class="sxs-lookup"><span data-stu-id="e1c81-135">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="e1c81-136">क्या व्यय श्रेणी वाले खर्चों को अलग-अलग करना होगा?</span><span class="sxs-lookup"><span data-stu-id="e1c81-136">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="e1c81-137">व्यय श्रेणी के लिए मुख्य डिफ़ॉल्ट खाता क्या है?</span><span class="sxs-lookup"><span data-stu-id="e1c81-137">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="e1c81-138">व्यय श्रेणी के लिए डिफ़ॉल्ट आइटम बिक्री कर समूह क्या है?</span><span class="sxs-lookup"><span data-stu-id="e1c81-138">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="e1c81-139">क्या अतिरिक्त भुगतान विधियां व्यय श्रेणी के लिए अनुमत हैं?</span><span class="sxs-lookup"><span data-stu-id="e1c81-139">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="e1c81-140">यदि ऐसा है, तो वो क्या हैं?</span><span class="sxs-lookup"><span data-stu-id="e1c81-140">If so, what are they?</span></span>
- <span data-ttu-id="e1c81-141">क्या इस व्यय श्रेणी में उपश्रेणियां हैं?</span><span class="sxs-lookup"><span data-stu-id="e1c81-141">Are there subcategories in this expense category?</span></span> <span data-ttu-id="e1c81-142">यदि उपश्रेणियां हैं, तो आपको निम्नलिखित निर्णय भी करने होंगे:</span><span class="sxs-lookup"><span data-stu-id="e1c81-142">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="e1c81-143">क्या किसी भी उपश्रेणी को कर वसूली से बाहर रखा गया है?</span><span class="sxs-lookup"><span data-stu-id="e1c81-143">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="e1c81-144">उपश्रेणियों का आइटम विक्रय कर समूह क्या है?</span><span class="sxs-lookup"><span data-stu-id="e1c81-144">What is the item sales tax group of the subcategories?</span></span>
