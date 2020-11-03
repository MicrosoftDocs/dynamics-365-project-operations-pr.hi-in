---
title: वास्तविक
description: यह विषय Microsoft Dynamics 365 परियोजना संचालन में वास्तविक के साथ काम करने के तरीके के बारे में सूचना देता है.
author: rumant
manager: AnnBe
ms.date: 09/16/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 93a945ffbe9c6dd998456b506b95e717ab8fbab7
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077690"
---
# <a name="actuals"></a><span data-ttu-id="3a982-103">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="3a982-103">Actuals</span></span> 

<span data-ttu-id="3a982-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="3a982-104">_**Applies to:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="3a982-105">वास्तविक आंकड़े उस काम की राशि हैं जो एक प्रोजेक्ट में पूरा किया गया है।</span><span class="sxs-lookup"><span data-stu-id="3a982-105">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="3a982-106">वे समय और व्यय प्रविष्टियों और जर्नल प्रविष्टियों और चालान के परिणामस्वरूप बनाए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="3a982-106">They are created as a result of time and expense entries, and journal entries and invoices.</span></span>

## <a name="journal-lines-and-time-submission"></a><span data-ttu-id="3a982-107">जर्नल लाइन और समय सबमिशन</span><span class="sxs-lookup"><span data-stu-id="3a982-107">Journal lines and time submission</span></span>

<span data-ttu-id="3a982-108">समय प्रविष्टि के बारे में अधिक जानकारी के लिए, [समय प्रविष्टि संक्षिप्त विवरण](../time/time-entry-overview.md) देखें।</span><span class="sxs-lookup"><span data-stu-id="3a982-108">For more information about time entry, see [Time entry overview](../time/time-entry-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="3a982-109">समय और सामग्रियां</span><span class="sxs-lookup"><span data-stu-id="3a982-109">Time and materials</span></span>

<span data-ttu-id="3a982-110">जब एक समय प्रविष्टि, जो सबमिट की जाती है वह ऐसी परियोजना से जुड़ी होती है जिसे समय-और-सामग्री अनुबंध लाइन में मैप किया जाता है, तो सिस्टम दो जर्नल लाइन बनाता है, एक लागत के लिए और एक गैर-बिल बिक्री के लिए।</span><span class="sxs-lookup"><span data-stu-id="3a982-110">When a time entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="3a982-111">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="3a982-111">Fixed price</span></span>

<span data-ttu-id="3a982-112">जब एक समय प्रविष्टि, जो सबमिट की जाती है वह एक ऐसी परियोजना से जुड़ी होती है जिसे एक निश्चित मूल्य अनुबंध लाइन पर मैप किया जाता है, तो सिस्टम लागत के लिए एक जर्नल लाइन बनाता है।</span><span class="sxs-lookup"><span data-stu-id="3a982-112">When a time entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="3a982-113">डिफ़ॉल्ट मूल्य निर्धारण</span><span class="sxs-lookup"><span data-stu-id="3a982-113">Default pricing</span></span>

<span data-ttu-id="3a982-114">डिफ़ॉल्ट मूल्य बनाने के लिए तर्क जर्नल पंक्ति पर रहता है.</span><span class="sxs-lookup"><span data-stu-id="3a982-114">The logic for creating default prices resides on the journal line.</span></span> <span data-ttu-id="3a982-115">समय प्रविष्टि से फ़ील्ड मान जर्नल पंक्ति में कॉपी किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="3a982-115">The field values from the time entry are copied to the journal line.</span></span> <span data-ttu-id="3a982-116">इन मान में लेन-देन की तारीख, अनुबंध रेखा जिसे प्रोजेक्ट के लिए चिह्नांकित किया गया है, और उचित मूल्य सूची में मुद्रा परिणाम।</span><span class="sxs-lookup"><span data-stu-id="3a982-116">These values include the transaction date, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span>

<span data-ttu-id="3a982-117">डिफ़ॉल्ट मूल्य निर्धारण को प्रभावित करने वाले फ़ील्ड, जैसे **भूमिका** और **संगठन इकाई** जर्नल लाइन पर उपयोग किसी के लिए मूल्य दर्ज करने का कारण बनते हैं।</span><span class="sxs-lookup"><span data-stu-id="3a982-117">The fields that affect default pricing, such as **Role** and **Org Unit** , are used to determine the appropriate price on the journal line.</span></span> <span data-ttu-id="3a982-118">आप समय प्रविष्टि पर एक कस्टम क्षेत्र को जोड़ सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="3a982-118">You can add a custom field on the time entry.</span></span> <span data-ttu-id="3a982-119">यदि आप चाहते हैं कि फ़ील्ड मान वास्तविक रूप से प्रचारित किया जाए तो वास्तविक निकाय पर फ़ील्ड बनाएँ, और फ़ील्ड चिह्नांकन का उपयोग वास्तविक समय प्रविष्टि से फ़ील्ड की क़ॉपी बनाने के लिए करें।</span><span class="sxs-lookup"><span data-stu-id="3a982-119">If you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="journal-lines-and-basic-expense-submission"></a><span data-ttu-id="3a982-120">जर्नल पंक्ति और मूल व्यय प्रस्तुत करना</span><span class="sxs-lookup"><span data-stu-id="3a982-120">Journal lines and basic expense submission</span></span>

<span data-ttu-id="3a982-121">व्यय प्रविष्टि के बारे में अधिक जानकारी के लिए, देखें [व्यय प्रविष्टि अवलोकन](../expense/expense-overview.md).</span><span class="sxs-lookup"><span data-stu-id="3a982-121">For more information about expense entry, see [Expense overview](../expense/expense-overview.md).</span></span>

### <a name="time-and-materials"></a><span data-ttu-id="3a982-122">समय और सामग्रियां</span><span class="sxs-lookup"><span data-stu-id="3a982-122">Time and materials</span></span>

<span data-ttu-id="3a982-123">जब एक मूल व्यय प्रविष्टि, जो सबमिट की जाती है वह एक ऐसी परियोजना से जुड़ी होती है जिसे समय-और-सामग्री अनुबंध लाइन में मैप किया जाता है, तो सिस्टम दो जर्नल लाइन बनाता है, एक लागत के लिए और एक गैर-बिल बिक्री के लिए।</span><span class="sxs-lookup"><span data-stu-id="3a982-123">When a basic expense entry that is submitted is linked to a project that is mapped to a time-and-materials contract line, the system creates two journal lines, one for cost and one for unbilled sales.</span></span>

### <a name="fixed-price"></a><span data-ttu-id="3a982-124">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="3a982-124">Fixed price</span></span>

<span data-ttu-id="3a982-125">जब एक मूल व्यय प्रविष्टि, जो सबमिट की जाती है, वह एक निश्चित मूल्य अनुबंध लाइन पर मैप की गई परियोजना से जुड़ी होती है, तो सिस्टम लागत के लिए एक जर्नल लाइन बनाता है।</span><span class="sxs-lookup"><span data-stu-id="3a982-125">When a basic expense entry that is submitted is linked to a project that is mapped to a fixed-price contract line, the system creates one journal line for cost.</span></span>

### <a name="default-pricing"></a><span data-ttu-id="3a982-126">डिफ़ॉल्ट मूल्य निर्धारण</span><span class="sxs-lookup"><span data-stu-id="3a982-126">Default pricing</span></span>

<span data-ttu-id="3a982-127">खर्चों के लिए डिफ़ॉल्ट मूल्य दर्ज करने का तर्क व्यय श्रेणी पर आधारित है।</span><span class="sxs-lookup"><span data-stu-id="3a982-127">The logic for entering default prices for expenses is based on the expense category.</span></span> <span data-ttu-id="3a982-128">लेन-देन की तारीख, अनुबंध रेखा जिसे प्रोजेक्ट के लिए चिह्नांकित किया गया है, और मुद्रा-सभी का उपयोग उचित मूल्य सूची निर्धारित करने के लिए किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="3a982-128">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="3a982-129">हालांकि, मूल्य के लिए, दर्ज की गई राशि डिफ़ॉल्ट रूप से लागत और बिक्री के लिए संबंधित व्यय जर्नल लाइनों पर सीधे स्थापित की जाती है।</span><span class="sxs-lookup"><span data-stu-id="3a982-129">However, by default, the amount that is entered for the price itself is set directly on the related expense journal lines for cost and sales.</span></span>

<span data-ttu-id="3a982-130">व्यय प्रविष्टियों पर प्रति-इकाई डिफ़ॉल्ट कीमतों की श्रेणी-आधारित प्रविष्टि उपलब्ध नहीं है.</span><span class="sxs-lookup"><span data-stu-id="3a982-130">Category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="use-entry-journals-to-record-costs"></a><span data-ttu-id="3a982-131">लागत रिकॉर्ड करने के लिए जर्नल प्रविष्टि का उपयोग करना</span><span class="sxs-lookup"><span data-stu-id="3a982-131">Use entry journals to record costs</span></span>

<span data-ttu-id="3a982-132">आप सामग्री, शुल्क, समय, व्यय, या कर लेन-देन वर्गों में लागत या राजस्व रिकॉर्ड करने के लिए प्रविष्टि जर्नल का उपयोग कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="3a982-132">You can use entry journals to record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="3a982-133">जर्नल का उपयोग निम्नलिखित उद्देश्यों के लिए किया जा सकता है:</span><span class="sxs-lookup"><span data-stu-id="3a982-133">Journals can be used for the following purposes:</span></span>

- <span data-ttu-id="3a982-134">किसी प्रोजेक्ट पर सामग्री की वास्तविक लागत और बिक्री रिकॉर्ड करें.</span><span class="sxs-lookup"><span data-stu-id="3a982-134">Record the actual cost of materials and sales on a project.</span></span>
- <span data-ttu-id="3a982-135">आपको किसी अन्य सिस्टम से Microsoft Dynamics 365 Project Operations में लेनदेन के वास्तविक आंकड़ों को स्थानांतरित करना होगा.</span><span class="sxs-lookup"><span data-stu-id="3a982-135">Move transaction actuals from another system to Microsoft Dynamics 365 Project Operations.</span></span>
- <span data-ttu-id="3a982-136">उस लागत को रिकॉर्ड करें जो किसी अन्य सिस्टम में हुई।</span><span class="sxs-lookup"><span data-stu-id="3a982-136">Record costs that occurred in another system.</span></span> <span data-ttu-id="3a982-137">इन लागतों में खरीद या उप-लागतों को शामिल किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="3a982-137">These costs can include procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="3a982-138">एप्लिकेशन उस जर्नल लाइन प्रकार या संबंधित मूल्य निर्धारण को मान्य नहीं करता है, जो जर्नल लाइन पर दर्ज किया गया है।</span><span class="sxs-lookup"><span data-stu-id="3a982-138">The application doesn't validate the journal line type or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="3a982-139">इसलिए, केवल वह उपयोगकर्ता जो पूरी तरह से लेखांकन असर जानता है, जो वास्तविक रूप से परियोजना पर होता है, को वास्तविक बनाने के लिए प्रविष्टि जर्नल का उपयोग करना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="3a982-139">Therefore, only a user who is fully aware of the accounting impact that actuals have on the project should use entry journals to create actuals.</span></span> <span data-ttu-id="3a982-140">इस जर्नल प्रकार के असर के कारण, आपको सावधानीपूर्वक यह चुनना चाहिए कि प्रविष्टि जर्नल को बनाने की पहुंच किसके पास है।</span><span class="sxs-lookup"><span data-stu-id="3a982-140">Because of the impact of this journal type, you should carefully choose who has access to create entry journals.</span></span>
## <a name="record-actuals-based-on-project-events"></a><span data-ttu-id="3a982-141">प्रोजेक्ट कार्यक्रमों के आधार पर वास्तविक आंकड़ों की रिकॉर्ड</span><span class="sxs-lookup"><span data-stu-id="3a982-141">Record actuals based on project events</span></span>

<span data-ttu-id="3a982-142">Project Operations किसी प्रोजेक्ट के दौरान होने वाले वित्तीय लेनदेन को रिकॉर्ड करता है.</span><span class="sxs-lookup"><span data-stu-id="3a982-142">Project Operations records the financial transactions that occur during a project.</span></span> <span data-ttu-id="3a982-143">ये लेन-देन वास्तविक के रूप में दर्ज किए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="3a982-143">These transactions are recorded as actuals.</span></span> <span data-ttu-id="3a982-144">निम्न तालिकाएं विभिन्न प्रकार के बनाए गये वास्तविक आंकड़ों को दर्शाती हैं, इस पर निर्भर है कि क्या परियोजना एक समय-और-सामग्री है या फिक्स्ड-प्राइस प्रोजेक्ट बिक्री-पूर्व चरण में है, या एक आंतरिक परियोजना है।</span><span class="sxs-lookup"><span data-stu-id="3a982-144">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

### <a name="the-resource-belongs-to-same-organizational-unit-as-the-projects-contracting-unit"></a><span data-ttu-id="3a982-145">संसाधन, प्रोजेक्ट की अनुबंध इकाई के रूप में उसी संगठनात्मक इकाई से संबद्ध है</span><span class="sxs-lookup"><span data-stu-id="3a982-145">The resource belongs to same organizational unit as the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="3a982-146">ईवेंट</span><span class="sxs-lookup"><span data-stu-id="3a982-146">Event</span></span></th>
<th colspan="4"><span data-ttu-id="3a982-147">बिल योग्य या बेचा गया प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="3a982-147">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="3a982-148">प्रोजेक्ट बिक्री-पूर्व चरण में</span><span class="sxs-lookup"><span data-stu-id="3a982-148">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="3a982-149">आंतरिक प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="3a982-149">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="3a982-150">समय और सामग्रियां</span><span class="sxs-lookup"><span data-stu-id="3a982-150">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="3a982-151">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="3a982-151">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="3a982-152">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="3a982-152">Actuals</span></span></th>
<th><span data-ttu-id="3a982-153">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-153">Transaction currency</span></span></th>
<th><span data-ttu-id="3a982-154">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="3a982-154">Fixed price</span></span></th>
<th><span data-ttu-id="3a982-155">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-155">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="3a982-156">एक समय प्रविष्टि बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="3a982-156">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="3a982-157">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-157">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-158">एक समय प्रविष्टि प्रस्तुत की जाती है।</span><span class="sxs-lookup"><span data-stu-id="3a982-158">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="3a982-159">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-159">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="3a982-160">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कोई परिवर्तन या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="3a982-160">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="3a982-161">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-161">Cost actual</span></span></td>
<td><span data-ttu-id="3a982-162">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-162">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="3a982-163">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-163">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="3a982-164">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-164">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="3a982-165">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-165">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="3a982-166">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-167">वास्तविक बिक्री बिना बिल की (अनबिल्ड) – प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="3a982-167">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="3a982-168">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-168">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="3a982-169">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="3a982-169">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="3a982-170">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-170">Cost actual</span></span></td>
<td><span data-ttu-id="3a982-171">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-171">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="3a982-172">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-172">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="3a982-173">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-173">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="3a982-174">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-174">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="3a982-175">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-175">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-176">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="3a982-176">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="3a982-177">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-177">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-178">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="3a982-178">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="3a982-179">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="3a982-180">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कोई बदलाव या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="3a982-180">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="3a982-181">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="3a982-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="3a982-182">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-182">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="3a982-183">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री</span><span class="sxs-lookup"><span data-stu-id="3a982-183">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="3a982-184">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-184">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="3a982-185">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-185">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="3a982-186">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-187">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="3a982-187">Billed sales</span></span></td>
<td><span data-ttu-id="3a982-188">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-188">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="3a982-189">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="3a982-189">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="3a982-190">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="3a982-190">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="3a982-191">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-191">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="3a982-192">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-192">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="3a982-193">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-193">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="3a982-194">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-194">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="3a982-195">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-195">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-196">बिल की गयी बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="3a982-196">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="3a982-197">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-197">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-198">बिल की गयी बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="3a982-198">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="3a982-199">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-199">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="3a982-200">प्रभार्य मात्रा बढ़ाने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="3a982-200">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="3a982-201">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="3a982-201">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="3a982-202">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-202">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="3a982-203">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री का उलटाव (रिवर्सल)</span><span class="sxs-lookup"><span data-stu-id="3a982-203">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="3a982-204">माइलस्टोन स्थिति में परिवर्तन <strong>चालान</strong> से <strong>चालान के लिए तैयार</strong> तक</span><span class="sxs-lookup"><span data-stu-id="3a982-204">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="3a982-205">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-205">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="3a982-206">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-206">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="3a982-207">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-207">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-208">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="3a982-208">Billed sales</span></span></td>
<td><span data-ttu-id="3a982-209">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-209">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="3a982-210">प्रभार्य मात्रा को कम करने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="3a982-210">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="3a982-211">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="3a982-211">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="3a982-212">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-212">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-213">नई मात्रा के लिए बिल की गयी बिक्री</span><span class="sxs-lookup"><span data-stu-id="3a982-213">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="3a982-214">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-214">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-215">बिन न की गयी बिक्री - अंतर के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="3a982-215">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="3a982-216">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-216">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

### <a name="the-resource-belongs-to-an-organizational-unit-that-differs-from-the-projects-contracting-unit"></a><span data-ttu-id="3a982-217">संसाधन एक संगठनात्मक इकाई के अंतर्गत आता है जो प्रोजेक्ट की अनुबंध इकाई से भिन्न होता है</span><span class="sxs-lookup"><span data-stu-id="3a982-217">The resource belongs to an organizational unit that differs from the project's contracting unit</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="3a982-218">ईवेंट</span><span class="sxs-lookup"><span data-stu-id="3a982-218">Event</span></span></th>
<th colspan="4"><span data-ttu-id="3a982-219">बिल योग्य या बेचा गया प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="3a982-219">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="3a982-220">प्रोजेक्ट बिक्री-पूर्व चरण में</span><span class="sxs-lookup"><span data-stu-id="3a982-220">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="3a982-221">आंतरिक प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="3a982-221">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="3a982-222">समय और सामग्रियां</span><span class="sxs-lookup"><span data-stu-id="3a982-222">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="3a982-223">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="3a982-223">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="3a982-224">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="3a982-224">Actuals</span></span></th>
<th><span data-ttu-id="3a982-225">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-225">Transaction currency</span></span></th>
<th><span data-ttu-id="3a982-226">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="3a982-226">Fixed price</span></span></th>
<th><span data-ttu-id="3a982-227">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-227">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="3a982-228">एक समय प्रविष्टि बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="3a982-228">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="3a982-229">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-229">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-230">एक समय प्रविष्टि प्रस्तुत की जाती है।</span><span class="sxs-lookup"><span data-stu-id="3a982-230">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="3a982-231">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-231">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="3a982-232">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कोई परिवर्तन या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="3a982-232">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="3a982-233">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-233">Cost actual</span></span></td>
<td><span data-ttu-id="3a982-234">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-234">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="3a982-235">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-235">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="3a982-236">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-236">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="3a982-237">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-237">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="3a982-238">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-238">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-239">वास्तविक बिक्री बिना बिल की (अनबिल्ड) – प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="3a982-239">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="3a982-240">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-240">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-241">सोर्सिंग यूनिट की लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-241">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="3a982-242">संसाधनित इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-242">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-243">अंत: संगठनात्मक बिक्री</span><span class="sxs-lookup"><span data-stu-id="3a982-243">Interorganizational sales</span></span></td>
<td><span data-ttu-id="3a982-244">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-244">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="3a982-245">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="3a982-245">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="3a982-246">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-246">Cost actual</span></span></td>
<td><span data-ttu-id="3a982-247">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-247">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="3a982-248">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-248">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="3a982-249">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-249">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="3a982-250">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-250">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="3a982-251">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-251">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-252">सोर्सिंग यूनिट की लागत</span><span class="sxs-lookup"><span data-stu-id="3a982-252">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="3a982-253">संसाधनित इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-253">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-254">अंत: संगठनात्मक बिक्री</span><span class="sxs-lookup"><span data-stu-id="3a982-254">Interorganizational sales</span></span></td>
<td><span data-ttu-id="3a982-255">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-255">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-256">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="3a982-256">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="3a982-257">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-257">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-258">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="3a982-258">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="3a982-259">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="3a982-260">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कोई बदलाव या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="3a982-260">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="3a982-261">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="3a982-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="3a982-262">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-262">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="3a982-263">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री</span><span class="sxs-lookup"><span data-stu-id="3a982-263">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="3a982-264">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-264">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="3a982-265">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-265">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="3a982-266">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-267">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="3a982-267">Billed sales</span></span></td>
<td><span data-ttu-id="3a982-268">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-268">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="3a982-269">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="3a982-269">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="3a982-270">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="3a982-270">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="3a982-271">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-271">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="3a982-272">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-272">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="3a982-273">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-273">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="3a982-274">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-274">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="3a982-275">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-275">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-276">बिल की गयी बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="3a982-276">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="3a982-277">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-277">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-278">बिल की गयी बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="3a982-278">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="3a982-279">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-279">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="3a982-280">प्रभार्य मात्रा बढ़ाने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="3a982-280">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="3a982-281">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="3a982-281">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="3a982-282">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-282">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="3a982-283">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री का उलटाव (रिवर्सल)</span><span class="sxs-lookup"><span data-stu-id="3a982-283">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="3a982-284">माइलस्टोन स्थिति में परिवर्तन <strong>चालान</strong> से <strong>चालान के लिए तैयार</strong> तक</span><span class="sxs-lookup"><span data-stu-id="3a982-284">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="3a982-285">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-285">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="3a982-286">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-286">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="3a982-287">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="3a982-287">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-288">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="3a982-288">Billed sales</span></span></td>
<td><span data-ttu-id="3a982-289">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-289">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="3a982-290">प्रभार्य मात्रा को कम करने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="3a982-290">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="3a982-291">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="3a982-291">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="3a982-292">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-292">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-293">नई मात्रा के लिए बिल की गयी बिक्री</span><span class="sxs-lookup"><span data-stu-id="3a982-293">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="3a982-294">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-294">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="3a982-295">बिन न की गयी बिक्री - अंतर के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="3a982-295">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="3a982-296">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="3a982-296">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
