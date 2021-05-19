---
title: परियोजनाओं पर सामग्री के लिए वित्तीय अनुमान
description: यह विषय परियोजना-आधारित सामग्रियों को परिभाषित करने या अनुमान लगाने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 98e3611b2b3948aab09a3eadeac7b95b893812e9
ms.sourcegitcommit: 504c09365bf404c1f1aa9b5034c1e1e5bc9d0d54
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/31/2021
ms.locfileid: "5788861"
---
# <a name="financial-estimates-for-materials-on-projects"></a><span data-ttu-id="72e15-103">परियोजनाओं पर सामग्री के लिए वित्तीय अनुमान</span><span class="sxs-lookup"><span data-stu-id="72e15-103">Financial estimates for materials on projects</span></span>

<span data-ttu-id="72e15-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="72e15-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="72e15-105">Dynamics 365 Project Operations परियोजना प्रबंधकों को प्रत्येक परियोजना या कार्य के लिए परियोजना-आधारित सामग्री की लागत को परिभाषित करने की अनुमति देता है.</span><span class="sxs-lookup"><span data-stu-id="72e15-105">Dynamics 365 Project Operations allows Project managers to define project-based material costs for each project or task.</span></span> <span data-ttu-id="72e15-106">सामग्री के लिए प्रत्येक अनुमान एक विशिष्ट परियोजना कार्य के साथ जुड़ा हो सकता है.</span><span class="sxs-lookup"><span data-stu-id="72e15-106">Each material estimate can be associated with a specific project task.</span></span> <span data-ttu-id="72e15-107">व्यय को विभिन्न व्यय श्रेणियों में वर्गीकृत किया जाता है, जिन्हें संगठनात्मक स्तर पर परिभाषित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="72e15-107">Expenses are categorized into different expense categories, which are defined at the organizational level.</span></span> <span data-ttu-id="72e15-108">प्रत्येक व्यय श्रेणी के लिए मूल्य निर्धारण और लागत निर्धारण प्राइस लिस्ट में परिभाषित किया गया है.</span><span class="sxs-lookup"><span data-stu-id="72e15-108">Pricing and costing for each expense category is defined in the price list.</span></span> 

<span data-ttu-id="72e15-109">किसी परियोजना के लिए सामग्री के अनुमान को देखने, जोड़ने या मिटाने के लिए निम्नलिखित चरणों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="72e15-109">Complete the following steps to view, add, or delete a project material estimate.</span></span>

1. <span data-ttu-id="72e15-110">**परियोजना** पर जाएं, और उस परियोजना का चयन करें जिसे आप अपडेट करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="72e15-110">Go to **Projects**, and select the project you want to update.</span></span>
2. <span data-ttu-id="72e15-111">**सामग्री का अनुमान** टैब पर, परियोजना के लिए सामग्री के अनुमानों की सूची देखें.</span><span class="sxs-lookup"><span data-stu-id="72e15-111">On the **Material Estimates** tab, view the list of project material estimates.</span></span>
3. <span data-ttu-id="72e15-112">सामग्री के लिए एक नया अनुमान बनाने के लिए **सामग्री के लिए नया अनुमान** चुनें.</span><span class="sxs-lookup"><span data-stu-id="72e15-112">Select **New Material estimate** to create a new material estimate.</span></span> <span data-ttu-id="72e15-113">या, मिटाने के लिए सामग्री का अनुमान का चयन करें, और फिर **सामग्री का अनुमान मिटाएं** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="72e15-113">Or, select a material estimate to delete, and then select **Delete Material Estimate**.</span></span>

<span data-ttu-id="72e15-114">निम्नलिखित तालिका किसी परियोजना पर **सामग्री अनुमान लाइन** पर फ़ील्ड के बारे में जानकारी प्रदान करती है.</span><span class="sxs-lookup"><span data-stu-id="72e15-114">The following table provides information about the fields on the **Material Estimate line** on a project.</span></span> 

| <span data-ttu-id="72e15-115">**फ़ील्ड**</span><span class="sxs-lookup"><span data-stu-id="72e15-115">**Field**</span></span> | <span data-ttu-id="72e15-116">**विवरण**</span><span class="sxs-lookup"><span data-stu-id="72e15-116">**Description**</span></span> | <span data-ttu-id="72e15-117">**डाउनस्ट्रीम प्रभाव**</span><span class="sxs-lookup"><span data-stu-id="72e15-117">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="72e15-118">कार्य</span><span class="sxs-lookup"><span data-stu-id="72e15-118">Task</span></span> | <span data-ttu-id="72e15-119">परियोजना में कार्यों की एक सूची.</span><span class="sxs-lookup"><span data-stu-id="72e15-119">A list of tasks in the project.</span></span> <span data-ttu-id="72e15-120">इसमें सारांश और लीफ़ नोड कार्य शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="72e15-120">This includes summary and leaf node tasks.</span></span> | <span data-ttu-id="72e15-121">जब आप किसी सामग्री अनुमान लाइन के लिए किसी कार्य का चयन करते हैं, तो किसी कार्य के लिए सामग्री की अनुमानित लागत और सामग्री की अनुमानित बिक्री प्रभावित होती है.</span><span class="sxs-lookup"><span data-stu-id="72e15-121">When you select a task for a material estimate line, the estimated material cost and estimated material sales for a task are impacted.</span></span> <span data-ttu-id="72e15-122">यदि यह फ़ील्ड खाली है, तो सामग्री के अनुमान को केवल परियोजना स्तर पर ट्रैक और संक्षेप में प्रस्तुत किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="72e15-122">If this field is empty, the material estimate is tracked and summarized only at the project level.</span></span> |
| <span data-ttu-id="72e15-123">उत्पाद का चयन करें</span><span class="sxs-lookup"><span data-stu-id="72e15-123">Select Product</span></span> |  <span data-ttu-id="72e15-124">आप निर्दिष्ट कर सकते हैं कि अनुमान लाइन मौजूदा (कैटलॉग) या राइट-इन प्रोडक्ट के लिए है या नहीं.</span><span class="sxs-lookup"><span data-stu-id="72e15-124">You can specify whether the estimate line is for an existing (catalog) or write-in product.</span></span> | <span data-ttu-id="72e15-125">यह फ़ील्ड यह निर्धारित करता है कि क्या आप कैटलॉग से किसी प्रोडक्ट का चयन करते हैं या किसी राइट-इन से.</span><span class="sxs-lookup"><span data-stu-id="72e15-125">This field determines if you select a product from the catalog or a write in product.</span></span> |
| <span data-ttu-id="72e15-126">उत्पाद</span><span class="sxs-lookup"><span data-stu-id="72e15-126">Product</span></span> | <span data-ttu-id="72e15-127">उत्पाद कैटलॉग से उत्पाद की ID.</span><span class="sxs-lookup"><span data-stu-id="72e15-127">The ID of the product from the product catalog.</span></span> <span data-ttu-id="72e15-128">जब आप किसी प्रोडक्ट आईडी का चयन करते हैं, तो **प्रोडक्ट चुनें** फ़ील्ड में मान स्वचालित रूप से **मौजूदा प्रोडक्ट** में अपडेट हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="72e15-128">When you select a product ID, the value in the **Select Product** field is automatically updated to **Existing product**.</span></span> <span data-ttu-id="72e15-129">आईडी का उपयोग प्राइस लिस्ट से लागत और बिक्री की कीमतों को फिर से प्राप्त करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="72e15-129">The ID is used to retrieve the cost and sales prices from the price list.</span></span> | <span data-ttu-id="72e15-130">इस फील्ड का प्रवाह की दिशा में कोई प्रभाव नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="72e15-130">There is no downstream impact for this field.</span></span> |
| <span data-ttu-id="72e15-131">राइट इन उत्पाद का वर्णन</span><span class="sxs-lookup"><span data-stu-id="72e15-131">Write In Product Description</span></span> | <span data-ttu-id="72e15-132">उत्पाद के नाम को लिखने के लिए टेक्स्ट फ़ील्ड.</span><span class="sxs-lookup"><span data-stu-id="72e15-132">A text field to write in the name of the product.</span></span> <span data-ttu-id="72e15-133">इस फ़ील्ड का उपयोग तब किया जाना चाहिए जब **प्रोडक्ट चुनें** फ़ील्ड में **राइट-इन** चुना जाता है.</span><span class="sxs-lookup"><span data-stu-id="72e15-133">This field should be used when **Write In** is selected in the **Select Product** field.</span></span>| <span data-ttu-id="72e15-134">इस फील्ड का प्रवाह की दिशा में कोई प्रभाव नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="72e15-134">There is no downstream impact for this field.</span></span> |
| <span data-ttu-id="72e15-135">प्रारंभ दिनांक</span><span class="sxs-lookup"><span data-stu-id="72e15-135">Start date</span></span> | <span data-ttu-id="72e15-136">पूर्वानुमानित तिथि जिस पर सामग्री का उपयोग किए जाने की उम्मीद है.</span><span class="sxs-lookup"><span data-stu-id="72e15-136">The forecasted date on which the material is expected to be used.</span></span> | <span data-ttu-id="72e15-137">इस फील्ड का प्रवाह की दिशा में कोई प्रभाव नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="72e15-137">There is no downstream impact for this field.</span></span> |
| <span data-ttu-id="72e15-138">इकाई समूह</span><span class="sxs-lookup"><span data-stu-id="72e15-138">Unit group</span></span> | <span data-ttu-id="72e15-139">इस फ़ील्ड में डिफ़ॉल्ट मान कैटलॉग प्रोडक्ट पर डिफ़ॉल्ट इकाई समूह से आता है.</span><span class="sxs-lookup"><span data-stu-id="72e15-139">The default value in this field comes from the default unit group on the catalog product.</span></span> <span data-ttu-id="72e15-140">आप किसी अन्य इकाई समूह का चयन करने के लिए इस फ़ील्ड को अपडेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="72e15-140">You can update this field to select another unit group.</span></span> | <span data-ttu-id="72e15-141">इस फील्ड का प्रवाह की दिशा में कोई प्रभाव नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="72e15-141">There is no downstream impact for this field.</span></span> |
| <span data-ttu-id="72e15-142">इकाई</span><span class="sxs-lookup"><span data-stu-id="72e15-142">Unit</span></span> | <span data-ttu-id="72e15-143">इस फ़ील्ड में मान चयनित प्रोडक्ट की डिफ़ॉल्ट इकाई से आता है.</span><span class="sxs-lookup"><span data-stu-id="72e15-143">The value in this field comes from the default unit of the selected product.</span></span> <span data-ttu-id="72e15-144">आप किसी अन्य इकाई का चयन करने के लिए इस फ़ील्ड को अपडेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="72e15-144">You can update this field to select another unit.</span></span> | <span data-ttu-id="72e15-145">इकाई बदलने के परिणामस्वरूप एक अलग डिफ़ॉल्ट इकाई मूल्य और लागत होती है.</span><span class="sxs-lookup"><span data-stu-id="72e15-145">Changing the unit results in a different default unit price and cost.</span></span> |
| <span data-ttu-id="72e15-146">मात्रा</span><span class="sxs-lookup"><span data-stu-id="72e15-146">Quantity</span></span> | <span data-ttu-id="72e15-147">परियोजना पर उपयोग किए जाने वाले प्रोडक्ट की अनुमानित मात्रा.</span><span class="sxs-lookup"><span data-stu-id="72e15-147">The estimated quantity of the product that will be used on the project.</span></span> | <span data-ttu-id="72e15-148">इस फील्ड का प्रवाह की दिशा में कोई प्रभाव नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="72e15-148">There is no downstream impact for this field.</span></span> |
| <span data-ttu-id="72e15-149">इकाई लागत</span><span class="sxs-lookup"><span data-stu-id="72e15-149">Unit Cost</span></span> | <span data-ttu-id="72e15-150">चयनित प्रोडक्ट और इकाई संयोजन की इकाई लागत उपयुक्त लागत की प्राइस लिस्ट में सेट की गई है.</span><span class="sxs-lookup"><span data-stu-id="72e15-150">The unit cost of the selected product and unit combination as set up in the applicable cost price list.</span></span> | <span data-ttu-id="72e15-151">इकाई लागत हमेशा परियोजना की लागत मुद्रा में दिखाई जाती है.</span><span class="sxs-lookup"><span data-stu-id="72e15-151">The unit cost is always shown in the project's cost currency.</span></span> <span data-ttu-id="72e15-152">यदि प्राइस लिस्ट में प्रोडक्ट और इकाई सेटअप के संयोजन के लिए इकाई लागत सेट नहीं किया गया है, तो इकाई लागत डिफ़ॉल्ट रूप से 0.00 हो जाएगी.</span><span class="sxs-lookup"><span data-stu-id="72e15-152">If there is no set up of unit cost for the combination of the product and unit setup in the price list, the unit cost will default to 0.00.</span></span> |
| <span data-ttu-id="72e15-153">इकाई मूल्य</span><span class="sxs-lookup"><span data-stu-id="72e15-153">Unit Price</span></span> | <span data-ttu-id="72e15-154">चयनित प्रोडक्ट और इकाई संयोजन की कीमत उपयुक्त सेल्स प्राइस लिस्ट में सेट की गई है.</span><span class="sxs-lookup"><span data-stu-id="72e15-154">The price of the selected product and unit combination as set up in the applicable sales price list.</span></span> | <span data-ttu-id="72e15-155">इकाई मूल्य हमेशा परियोजना की बिक्री मुद्रा में दिखाई जाती है.</span><span class="sxs-lookup"><span data-stu-id="72e15-155">The unit price is always shown in the project's sales currency.</span></span> <span data-ttu-id="72e15-156">यदि प्राइस लिस्ट में प्रोडक्ट और इकाई सेटअप के संयोजन के लिए इकाई मूल्य सेट नहीं किया गया है, तो इकाई मूल्य डिफ़ॉल्ट रूप से 0.00 हो जाएगी.</span><span class="sxs-lookup"><span data-stu-id="72e15-156">If there is no setup of unit price  for the combination of the product and unit setup in the price list, then unit price will default to 0.00.</span></span>|
| <span data-ttu-id="72e15-157">कुल लागत</span><span class="sxs-lookup"><span data-stu-id="72e15-157">Total Cost</span></span> | <span data-ttu-id="72e15-158">लागत राशि जिसकी गणना मात्रा \* इकाई लागत के रूप में की जाती है.</span><span class="sxs-lookup"><span data-stu-id="72e15-158">The cost amount that is calculated as quantity \* unit cost.</span></span>| <span data-ttu-id="72e15-159">लागत राशि हमेशा परियोजना की लागत मुद्रा में दिखाई जाती है.</span><span class="sxs-lookup"><span data-stu-id="72e15-159">The cost amount is always shown in the project's cost currency.</span></span> |
| <span data-ttu-id="72e15-160">कुल विक्रय</span><span class="sxs-lookup"><span data-stu-id="72e15-160">Total Sales</span></span> | <span data-ttu-id="72e15-161">बिक्री राशि जिसकी गणना मात्रा \* इकाई कीमत के रूप में की जाती है.</span><span class="sxs-lookup"><span data-stu-id="72e15-161">The sales amount that is calculated as quantity \* unit price.</span></span> | <span data-ttu-id="72e15-162">बिक्री राशि हमेशा परियोजना की बिक्री मुद्रा में दिखाई जाती है.</span><span class="sxs-lookup"><span data-stu-id="72e15-162">The sales amount is always shown in the project's sales currency.</span></span> |


[!INCLUDE[footer-include](../includes/footer-banner.md)]