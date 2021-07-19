---
title: वास्तविक
description: यह विषय Microsoft Dynamics 365 Project Operations में वास्तविक के साथ काम करने के तरीके के बारे में जानकारी प्रदान करता है.
author: rumant
ms.date: 04/01/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: intro-internal
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 9e046602a3005930c41ab8c50472d5b1a72303c6
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368613"
---
# <a name="actuals"></a><span data-ttu-id="fe27a-103">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="fe27a-103">Actuals</span></span> 

<span data-ttu-id="fe27a-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="fe27a-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="fe27a-105">वास्तविक किसी प्रोज़ेक्ट पर समीक्षा और अनुमोदित वित्तीय और अनुसूची प्रगति का प्रतिनिधित्व करते हैं.</span><span class="sxs-lookup"><span data-stu-id="fe27a-105">Actuals represent the reviewed and approved financial and schedule progress on a project.</span></span> <span data-ttu-id="fe27a-106">वे समय, व्यय, सामग्री उपयोग प्रविष्टियों, और जर्नल प्रविष्टियों और इनवॉइस के अनुमोदन का एक परिणाम के रूप में बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="fe27a-106">They are created as a result of approval of time, expense, material usage entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="fe27a-107">जर्नल लाइन और समय सबमिशन</span><span class="sxs-lookup"><span data-stu-id="fe27a-107">Journal lines and time submission</span></span>

<span data-ttu-id="fe27a-108">समय प्रविष्टि के बारे में अधिक जानकारी के लिए, [समय प्रविष्टि संक्षिप्त विवरण](../time/time-entry-overview.md) देखें।</span><span class="sxs-lookup"><span data-stu-id="fe27a-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="fe27a-109">समय और सामग्रियां</span><span class="sxs-lookup"><span data-stu-id="fe27a-109">Time and materials</span></span>

<span data-ttu-id="fe27a-110">जब एक समय प्रविष्टि, जो सबमिट की जाती है वह ऐसी परियोजना से जुड़ी होती है जिसे समय-और-सामग्री अनुबंध लाइन में मैप किया जाता है, तो सिस्टम दो जर्नल लाइन बनाता है, एक लागत के लिए और एक गैर-बिल बिक्री के लिए।</span><span class="sxs-lookup"><span data-stu-id="fe27a-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="fe27a-111">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-111">Fixed price</span></span>

<span data-ttu-id="fe27a-112">जब एक समय प्रविष्टि, जो सबमिट की जाती है वह एक ऐसी परियोजना से जुड़ी होती है जिसे एक निश्चित मूल्य अनुबंध लाइन पर मैप किया जाता है, तो सिस्टम लागत के लिए एक जर्नल लाइन बनाता है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="fe27a-113">डिफ़ॉल्ट मूल्य निर्धारण</span><span class="sxs-lookup"><span data-stu-id="fe27a-113">Default pricing</span></span>

<span data-ttu-id="fe27a-114">डिफ़ॉल्ट मूल्य बनाने के लिए तर्क जर्नल पंक्ति पर रहता है.</span><span class="sxs-lookup"><span data-stu-id="fe27a-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="fe27a-115">समय प्रविष्टि से फ़ील्ड मान जर्नल पंक्ति में कॉपी किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="fe27a-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="fe27a-116">इन मान में लेन-देन की तारीख, अनुबंध रेखा जिसे प्रोजेक्ट के लिए चिह्नांकित किया गया है, और उचित मूल्य सूची में मुद्रा परिणाम।</span><span class="sxs-lookup"><span data-stu-id="fe27a-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="fe27a-117">डिफ़ॉल्ट मूल्य निर्धारण को प्रभावित करने वाले फ़ील्ड जैसे **भूमिका** और **रिसोर्सिंग यूनिट**, का उपयोग जर्नल लाइन पर उचित मूल्य निर्धारित करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="fe27a-117">The fields that affect default pricing, such as **Role** and **Resourcing Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="fe27a-118">आप समय प्रविष्टि पर एक कस्टम क्षेत्र को जोड़ सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="fe27a-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="fe27a-119">यदि आप चाहते हैं कि फ़ील्ड मूल्य को वास्तविक रूप में प्रचारित किया जाए, तो **वास्ताविक** और **जर्नल लाइन** तालिकाओं में फ़ील्ड बनाएं.</span><span class="sxs-lookup"><span data-stu-id="fe27a-119">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="fe27a-120">लेन-देन मूल का उपयोग करके जर्नल लाइन के माध्यम से समय प्रविष्टि से वास्तविक तक चयनित फ़ील्ड वैल्यू का प्रचार करने के लिए कस्टम कोड का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="fe27a-120">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="fe27a-121">लेनदेन मूल और कनेक्शन के बारे में अधिक जानकारी के लिए, देखें [वास्तविक को मूल रिकॉर्ड से जोड़ना](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="fe27a-121">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="fe27a-122">जर्नल पंक्ति और मूल व्यय प्रस्तुत करना</span><span class="sxs-lookup"><span data-stu-id="fe27a-122">Journal lines and basic expense submission</span></span>

<span data-ttu-id="fe27a-123">व्यय प्रविष्टि के बारे में अधिक जानकारी के लिए, देखें [व्यय प्रविष्टि अवलोकन](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="fe27a-123">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="fe27a-124">समय और सामग्रियां</span><span class="sxs-lookup"><span data-stu-id="fe27a-124">Time and materials</span></span>

<span data-ttu-id="fe27a-125">जब एक मूल व्यय प्रविष्टि, जो सबमिट की जाती है वह एक ऐसी परियोजना से जुड़ी होती है जिसे समय-और-सामग्री अनुबंध लाइन में मैप किया जाता है, तो सिस्टम दो जर्नल लाइन बनाता है, एक लागत के लिए और एक गैर-बिल बिक्री के लिए।</span><span class="sxs-lookup"><span data-stu-id="fe27a-125">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="fe27a-126">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-126">Fixed price</span></span>

<span data-ttu-id="fe27a-127">जब सबमिट की गई बेसिक खर्च एंट्री किसी ऐसी प्रोज़ेक्ट से जुड़ी होती है, जिसे फिक्स्ड प्राइस कॉन्ट्रैक्ट लाइन में मैप किया जाता है, तो सिस्टम लागत के लिए एक जर्नल लाइन बनाता है.</span><span class="sxs-lookup"><span data-stu-id="fe27a-127">When a submitted basic expense entry is linked to a project that's mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="fe27a-128">डिफ़ॉल्ट मूल्य निर्धारण</span><span class="sxs-lookup"><span data-stu-id="fe27a-128">Default pricing</span></span>

<span data-ttu-id="fe27a-129">खर्चों के लिए डिफ़ॉल्ट मूल्य दर्ज करने का तर्क व्यय श्रेणी पर आधारित है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-129">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="fe27a-130">लेन-देन की तारीख, अनुबंध रेखा जिसे प्रोजेक्ट के लिए चिह्नांकित किया गया है, और मुद्रा, सभी का उपयोग उचित मूल्य सूची निर्धारित करने के लिए किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-130">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="fe27a-131">डिफ़ॉल्ट मूल्य निर्धारण को प्रभावित करने वाले फ़ील्ड, जैसे **लेनदेन श्रेणी** और **यूनिट**, का उपयोग जर्नल लाइन पर उचित मूल्य निर्धारित करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="fe27a-131">The fields that affect default pricing, such as **Transaction Category** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="fe27a-132">हालांकि, यह केवल तभी काम करता है जब मूल्य सूची में मूल्य निर्धारण विधि **मूल्य प्रति यूनिट** है.</span><span class="sxs-lookup"><span data-stu-id="fe27a-132">However, this only works when the pricing method in the price list is **Price per unit**.</span></span> <span data-ttu-id="fe27a-133">यदि मूल्य निर्धारण विधि **लागत** या **मार्कअप ओवर कॉस्ट** है, तो खर्च प्रविष्टि बनाए जाने पर दर्ज की गई कीमत का उपयोग लागत के लिए किया जाता है और विक्रय जर्नल लाइन पर मूल्य की गणना मूल्य निर्धारण विधि के आधार पर की जाती है.</span><span class="sxs-lookup"><span data-stu-id="fe27a-133">If pricing method is **At cost** or **Markup over cost**, the price entered when the expense entry is created is used for cost and the price on the sales journal line is calculated based on the pricing method.</span></span> 

<span data-ttu-id="fe27a-134">आप व्यय प्रविष्टि पर कस्टम फ़ील्ड जोड़ सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="fe27a-134">You can add a custom field on the expense entry.</span></span> <span data-ttu-id="fe27a-135">यदि आप चाहते हैं कि फ़ील्ड मूल्य को वास्तविक रूप में प्रचारित किया जाए, तो **वास्ताविक** और **जर्नल लाइन** तालिकाओं में फ़ील्ड बनाएं.</span><span class="sxs-lookup"><span data-stu-id="fe27a-135">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="fe27a-136">लेन-देन मूल का उपयोग करके जर्नल लाइन के माध्यम से समय प्रविष्टि से वास्तविक तक चयनित फ़ील्ड वैल्यू का प्रचार करने के लिए कस्टम कोड का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="fe27a-136">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="fe27a-137">लेनदेन मूल और कनेक्शन के बारे में अधिक जानकारी के लिए, देखें [वास्तविक को मूल रिकॉर्ड से जोड़ना](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="fe27a-137">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="journal-lines-and-material-usage-log-submission"></a><span data-ttu-id="fe27a-138">जर्नल लाइनें और सामग्री उपयोग लॉग सबमिशन</span><span class="sxs-lookup"><span data-stu-id="fe27a-138">Journal lines and material usage log submission</span></span>

<span data-ttu-id="fe27a-139">व्यय प्रविष्टि के बारे में अधिक जानकारी के लिए [सामग्री उपयोग लॉग](../material/material-usage-log.md) देखें.</span><span class="sxs-lookup"><span data-stu-id="fe27a-139">For more information about expense entry, see [Material Usage Log](../material/material-usage-log.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="fe27a-140">समय और सामग्रियां</span><span class="sxs-lookup"><span data-stu-id="fe27a-140">Time and materials</span></span>

<span data-ttu-id="fe27a-141">जब प्रस्तुत सामग्री उपयोग लॉग प्रविष्टि को ऐसी परियोजना से जोड़ा जाता है, जिसमें समय और सामग्री अनुबंध लाइन से मैप होता है, तो सिस्टम दो जर्नल लाइनों, लागत के लिए एक और बिना बिल बिक्री के लिए एक बनाता है.</span><span class="sxs-lookup"><span data-stu-id="fe27a-141">When a submitted material usage log entry is linked to a project that is mapped to a time and materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="fe27a-142">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-142">Fixed price</span></span>

<span data-ttu-id="fe27a-143">जब सबमिट की गई सामग्री उपयोग लॉग एंट्री को ऐसी परियोजना से जोड़ा जाता है, जिसे निश्चित मूल्य अनुबंध लाइन में मैप किया जाता है, तो सिस्टम लागत के लिए एक जर्नल लाइन बनाता है.</span><span class="sxs-lookup"><span data-stu-id="fe27a-143">When a submitted material usage log entry is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="fe27a-144">डिफ़ॉल्ट मूल्य निर्धारण</span><span class="sxs-lookup"><span data-stu-id="fe27a-144">Default pricing</span></span>

<span data-ttu-id="fe27a-145">सामग्री के लिए डिफ़ॉल्ट कीमतों में प्रवेश करने के लिए तर्क उत्पाद और इकाई संयोजन पर आधारित है.</span><span class="sxs-lookup"><span data-stu-id="fe27a-145">The logic for entering default prices for material is based on the product and unit combination.</span></span> <span data-ttu-id="fe27a-146">लेन-देन की तारीख, अनुबंध रेखा जिसे प्रोजेक्ट के लिए चिह्नांकित किया गया है, और मुद्रा, सभी का उपयोग उचित मूल्य सूची निर्धारित करने के लिए किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-146">The transaction date, the contract line that the project is mapped to, and the currency, are all used to determine the appropriate price list.</span></span> <span data-ttu-id="fe27a-147">डिफ़ॉल्ट मूल्य निर्धारण को प्रभावित करने वाले फ़ील्ड, जैसे **उत्पाद ID** और **इकाई**, का उपयोग जर्नल लाइन पर उचित मूल्य निर्धारित करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="fe27a-147">The fields that affect default pricing, such as **Product ID** and **Unit**, are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="fe27a-148">हालांकि, यह केवल सूची उत्पादों के लिए काम करता है.</span><span class="sxs-lookup"><span data-stu-id="fe27a-148">However, this only works for catalog products.</span></span> <span data-ttu-id="fe27a-149">लिखने के उत्पादों के लिए, सामग्री उपयोग लॉग प्रविष्टि बनाए जाने पर दर्ज की गई कीमत का उपयोग जर्नल लाइनों पर लागत और बिक्री मूल्य के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="fe27a-149">For write-in products, the price entered when the material usage log entry is created is used for cost and sales price on the journal lines.</span></span> 

<span data-ttu-id="fe27a-150">आप **सामग्री उपयोग लॉग** प्रविष्टि पर एक कस्टम फ़ील्ड जोड़ सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="fe27a-150">You can add a custom field on the **Material Usage Log** entry.</span></span> <span data-ttu-id="fe27a-151">यदि आप चाहते हैं कि फ़ील्ड मूल्य को वास्तविक रूप में प्रचारित किया जाए, तो **वास्ताविक** और **जर्नल लाइन** तालिकाओं में फ़ील्ड बनाएं.</span><span class="sxs-lookup"><span data-stu-id="fe27a-151">If you want the field value to be propagated to actuals, create the field in the **Actuals** and **Journal Line** tables.</span></span> <span data-ttu-id="fe27a-152">लेन-देन मूल का उपयोग करके जर्नल लाइन के माध्यम से समय प्रविष्टि से वास्तविक तक चयनित फ़ील्ड वैल्यू का प्रचार करने के लिए कस्टम कोड का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="fe27a-152">Use custom code to propagate the selected field value from Time Entry to Actuals through the journal line using transaction origins.</span></span> <span data-ttu-id="fe27a-153">लेनदेन मूल और कनेक्शन के बारे में अधिक जानकारी के लिए, देखें [वास्तविक को मूल रिकॉर्ड से जोड़ना](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span><span class="sxs-lookup"><span data-stu-id="fe27a-153">For more information about transaction origins and connections, see [Linking Actuals to original records](linkingactuals.md#example-how-transaction-origin-works-with-transaction-connection).</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="fe27a-154">लागत रिकॉर्ड करने के लिए जर्नल प्रविष्टि का उपयोग करना</span><span class="sxs-lookup"><span data-stu-id="fe27a-154">Use entry journals to record costs</span></span>

<span data-ttu-id="fe27a-155">आप सामग्री, शुल्क, समय, व्यय, या कर लेन-देन वर्गों में लागत या राजस्व रिकॉर्ड करने के लिए प्रविष्टि जर्नल का उपयोग कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="fe27a-155">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="fe27a-156">जर्नल का उपयोग निम्नलिखित उद्देश्यों के लिए किया जा सकता है:</span><span class="sxs-lookup"><span data-stu-id="fe27a-156">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="fe27a-157">लेनदेन के वास्तविक को अन्य सिस्टम से Microsoft Dynamics 365 Project Operations में स्थानांतरित करें.</span><span class="sxs-lookup"><span data-stu-id="fe27a-157">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="fe27a-158">उस लागत को रिकॉर्ड करें जो किसी अन्य सिस्टम में हुई।</span><span class="sxs-lookup"><span data-stu-id="fe27a-158">Record costs that occurred in another system.</span></span> <span data-ttu-id="fe27a-159">इन लागतों में खरीद या उप-लागतों को शामिल किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-159">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="fe27a-160">एप्लिकेशन उस जर्नल लाइन प्रकार या संबंधित मूल्य निर्धारण को मान्य नहीं करता है, जो जर्नल लाइन पर दर्ज किया गया है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-160">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="fe27a-161">इसलिए, केवल वह उपयोगकर्ता जो पूरी तरह से लेखांकन असर जानता है, जो वास्तविक रूप से परियोजना पर होता है, को वास्तविक बनाने के लिए प्रविष्टि जर्नल का उपयोग करना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="fe27a-161">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="fe27a-162">इस जर्नल प्रकार के असर के कारण, आपको सावधानीपूर्वक यह चुनना चाहिए कि प्रविष्टि जर्नल को बनाने की पहुंच किसके पास है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-162">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>

## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="fe27a-163">प्रोजेक्ट कार्यक्रमों के आधार पर वास्तविक आंकड़ों की रिकॉर्ड</span><span class="sxs-lookup"><span data-stu-id="fe27a-163">Record actuals based on project events</span></span>

<span data-ttu-id="fe27a-164">Project Operations किसी प्रोजेक्ट के दौरान होने वाले वित्तीय लेनदेन को रिकॉर्ड करता है.</span><span class="sxs-lookup"><span data-stu-id="fe27a-164">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="fe27a-165">ये लेन-देन वास्तविक के रूप में दर्ज किए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="fe27a-165">These transactions are recorded as actuals.</span></span> <span data-ttu-id="fe27a-166">निम्न तालिकाएं विभिन्न प्रकार के बनाए गये वास्तविक आंकड़ों को दर्शाती हैं, इस पर निर्भर है कि क्या परियोजना एक समय-और-सामग्री है या फिक्स्ड-प्राइस प्रोजेक्ट बिक्री-पूर्व चरण में है, या एक आंतरिक परियोजना है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-166">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="fe27a-167">संसाधन, प्रोजेक्ट की अनुबंध इकाई के रूप में उसी संगठनात्मक इकाई से संबद्ध है</span><span class="sxs-lookup"><span data-stu-id="fe27a-167">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="fe27a-168">ईवेंट</span><span class="sxs-lookup"><span data-stu-id="fe27a-168">Event</span></span></th>
<th colspan="4"><span data-ttu-id="fe27a-169">बिल योग्य या बेचा गया प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="fe27a-169">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="fe27a-170">प्रोजेक्ट बिक्री-पूर्व चरण में</span><span class="sxs-lookup"><span data-stu-id="fe27a-170">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="fe27a-171">आंतरिक प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="fe27a-171">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="fe27a-172">समय और सामग्रियां</span><span class="sxs-lookup"><span data-stu-id="fe27a-172">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="fe27a-173">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-173">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="fe27a-174">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="fe27a-174">Actuals</span></span></th>
<th><span data-ttu-id="fe27a-175">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-175">Transaction currency</span></span></th>
<th><span data-ttu-id="fe27a-176">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-176">Fixed price</span></span></th>
<th><span data-ttu-id="fe27a-177">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-177">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="fe27a-178">एक समय प्रविष्टि बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-178">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="fe27a-179">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-179">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-180">एक समय प्रविष्टि प्रस्तुत की जाती है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-180">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="fe27a-181">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-181">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="fe27a-182">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कोई परिवर्तन या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-182">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="fe27a-183">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-183">Cost actual</span></span></td>
<td><span data-ttu-id="fe27a-184">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-184">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="fe27a-185">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-185">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="fe27a-186">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-186">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="fe27a-187">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-187">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="fe27a-188">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-188">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-189">वास्तविक बिक्री बिना बिल की (अनबिल्ड) – प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-189">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="fe27a-190">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="fe27a-191">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-191">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="fe27a-192">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-192">Cost actual</span></span></td>
<td><span data-ttu-id="fe27a-193">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-193">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="fe27a-194">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-194">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="fe27a-195">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-195">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="fe27a-196">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-196">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="fe27a-197">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-197">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-198">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-198">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="fe27a-199">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-199">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-200">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-200">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="fe27a-201">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-201">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="fe27a-202">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कोई बदलाव या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-202">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="fe27a-203">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="fe27a-203">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="fe27a-204">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-204">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="fe27a-205">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री</span><span class="sxs-lookup"><span data-stu-id="fe27a-205">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="fe27a-206">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-206">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="fe27a-207">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-207">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="fe27a-208">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-208">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-209">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="fe27a-209">Billed sales</span></span></td>
<td><span data-ttu-id="fe27a-210">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-210">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="fe27a-211">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-211">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="fe27a-212">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="fe27a-212">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="fe27a-213">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-213">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="fe27a-214">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-214">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="fe27a-215">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-215">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="fe27a-216">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-216">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="fe27a-217">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-217">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-218">बिल की गयी बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-218">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="fe27a-219">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-219">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-220">बिल की गयी बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-220">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="fe27a-221">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-221">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="fe27a-222">प्रभार्य मात्रा बढ़ाने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-222">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="fe27a-223">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="fe27a-223">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="fe27a-224">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-224">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="fe27a-225">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री का उलटाव (रिवर्सल)</span><span class="sxs-lookup"><span data-stu-id="fe27a-225">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="fe27a-226">माइलस्टोन स्थिति में परिवर्तन <strong>चालान</strong> से <strong>चालान के लिए तैयार</strong> तक</span><span class="sxs-lookup"><span data-stu-id="fe27a-226">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="fe27a-227">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-227">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="fe27a-228">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-228">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="fe27a-229">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-229">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-230">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="fe27a-230">Billed sales</span></span></td>
<td><span data-ttu-id="fe27a-231">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-231">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="fe27a-232">प्रभार्य मात्रा को कम करने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-232">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="fe27a-233">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="fe27a-233">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="fe27a-234">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-235">नई मात्रा के लिए बिल की गयी बिक्री</span><span class="sxs-lookup"><span data-stu-id="fe27a-235">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="fe27a-236">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-236">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-237">बिन न की गयी बिक्री - अंतर के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-237">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="fe27a-238">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-238">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="fe27a-239">संसाधन एक संगठनात्मक इकाई के अंतर्गत आता है जो प्रोजेक्ट की अनुबंध इकाई से भिन्न होता है</span><span class="sxs-lookup"><span data-stu-id="fe27a-239">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="fe27a-240">ईवेंट</span><span class="sxs-lookup"><span data-stu-id="fe27a-240">Event</span></span></th>
<th colspan="4"><span data-ttu-id="fe27a-241">बिल योग्य या बेचा गया प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="fe27a-241">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="fe27a-242">प्रोजेक्ट बिक्री-पूर्व चरण में</span><span class="sxs-lookup"><span data-stu-id="fe27a-242">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="fe27a-243">आंतरिक प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="fe27a-243">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="fe27a-244">समय और सामग्रियां</span><span class="sxs-lookup"><span data-stu-id="fe27a-244">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="fe27a-245">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-245">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="fe27a-246">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="fe27a-246">Actuals</span></span></th>
<th><span data-ttu-id="fe27a-247">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-247">Transaction currency</span></span></th>
<th><span data-ttu-id="fe27a-248">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-248">Fixed price</span></span></th>
<th><span data-ttu-id="fe27a-249">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-249">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="fe27a-250">एक समय प्रविष्टि बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-250">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="fe27a-251">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-251">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-252">एक समय प्रविष्टि प्रस्तुत की जाती है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-252">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="fe27a-253">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-253">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="fe27a-254">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कोई परिवर्तन या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-254">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="fe27a-255">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-255">Cost actual</span></span></td>
<td><span data-ttu-id="fe27a-256">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-256">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="fe27a-257">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-257">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="fe27a-258">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-258">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="fe27a-259">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-259">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="fe27a-260">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-260">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-261">वास्तविक बिक्री बिना बिल की (अनबिल्ड) – प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-261">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="fe27a-262">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-262">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-263">सोर्सिंग यूनिट की लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-263">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="fe27a-264">संसाधनित इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-264">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-265">अंत: संगठनात्मक बिक्री</span><span class="sxs-lookup"><span data-stu-id="fe27a-265">Interorganizational sales</span></span></td>
<td><span data-ttu-id="fe27a-266">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-266">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="fe27a-267">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-267">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="fe27a-268">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-268">Cost actual</span></span></td>
<td><span data-ttu-id="fe27a-269">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-269">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="fe27a-270">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-270">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="fe27a-271">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-271">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="fe27a-272">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-272">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="fe27a-273">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-273">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-274">सोर्सिंग यूनिट की लागत</span><span class="sxs-lookup"><span data-stu-id="fe27a-274">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="fe27a-275">संसाधनित इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-275">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-276">अंत: संगठनात्मक बिक्री</span><span class="sxs-lookup"><span data-stu-id="fe27a-276">Interorganizational sales</span></span></td>
<td><span data-ttu-id="fe27a-277">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-277">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-278">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-278">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="fe27a-279">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-279">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-280">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-280">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="fe27a-281">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-281">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="fe27a-282">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कोई बदलाव या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-282">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="fe27a-283">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="fe27a-283">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="fe27a-284">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-284">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="fe27a-285">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री</span><span class="sxs-lookup"><span data-stu-id="fe27a-285">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="fe27a-286">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-286">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="fe27a-287">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-287">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="fe27a-288">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-288">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-289">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="fe27a-289">Billed sales</span></span></td>
<td><span data-ttu-id="fe27a-290">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-290">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="fe27a-291">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-291">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="fe27a-292">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="fe27a-292">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="fe27a-293">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-293">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="fe27a-294">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-294">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="fe27a-295">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-295">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="fe27a-296">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-296">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="fe27a-297">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-297">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-298">बिल की गयी बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-298">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="fe27a-299">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-299">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-300">बिल की गयी बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-300">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="fe27a-301">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-301">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="fe27a-302">प्रभार्य मात्रा बढ़ाने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-302">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="fe27a-303">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="fe27a-303">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="fe27a-304">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-304">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="fe27a-305">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री का उलटाव (रिवर्सल)</span><span class="sxs-lookup"><span data-stu-id="fe27a-305">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="fe27a-306">माइलस्टोन स्थिति में परिवर्तन <strong>चालान</strong> से <strong>चालान के लिए तैयार</strong> तक</span><span class="sxs-lookup"><span data-stu-id="fe27a-306">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="fe27a-307">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-307">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="fe27a-308">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-308">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="fe27a-309">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="fe27a-309">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-310">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="fe27a-310">Billed sales</span></span></td>
<td><span data-ttu-id="fe27a-311">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-311">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="fe27a-312">प्रभार्य मात्रा को कम करने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="fe27a-312">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="fe27a-313">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="fe27a-313">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="fe27a-314">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-314">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-315">नई मात्रा के लिए बिल की गयी बिक्री</span><span class="sxs-lookup"><span data-stu-id="fe27a-315">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="fe27a-316">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-316">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="fe27a-317">बिन न की गयी बिक्री - अंतर के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="fe27a-317">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="fe27a-318">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="fe27a-318">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
