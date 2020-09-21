---
title: वास्तविक
description: यह विषय परियोजना के वास्तविक आंकड़ों के बारे में जानकारी प्रदान करता है।
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 44c6e85f-5b21-4e24-999c-15a2f065d977
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8291e0eb8531e8e9690368675f333c44b6e92e48
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3752078"
---
# <a name="actuals"></a><span data-ttu-id="654fa-103">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="654fa-103">Actuals</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="654fa-104">वास्तविक आंकड़े उस काम की राशि हैं जो एक प्रोजेक्ट में पूरा किया गया है।</span><span class="sxs-lookup"><span data-stu-id="654fa-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="654fa-105">परियोजना वास्तविक आंकड़ों को अपने स्रोत दस्तावेजों से पता लगाया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="654fa-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="654fa-106">उन स्रोत दस्तावेजों में समय, व्यय और जर्नल प्रविष्टियाँ और चालान भी शामिल हैं।</span><span class="sxs-lookup"><span data-stu-id="654fa-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![स्रोत दस्तावेज़ों से प्रोजेक्ट के वास्तविक आंकड़ों का पता कैसे लगाया जाता है](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="654fa-108">एक समय प्रविष्टि प्रस्तुत करना</span><span class="sxs-lookup"><span data-stu-id="654fa-108">Submitting a time entry</span></span>

<span data-ttu-id="654fa-109">PSA में, जब एक प्रोजेक्ट के लिए एक समय प्रविष्टि प्रस्तुत की जाती है, जो समय और सामग्री अनुबंध लाइन के लिए चिह्नांकित किया गया है, दो जर्नल लाइनें बनाई जाती हैं।</span><span class="sxs-lookup"><span data-stu-id="654fa-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="654fa-110">एक लाइन लागत के लिए है, और दूसरी लाइन बिना बिल की बिक्री के लिए है।</span><span class="sxs-lookup"><span data-stu-id="654fa-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="654fa-111">जब किसी निश्चित-मूल्य अनुबंध रेखा पर चिह्नांकित किए गये प्रोजेक्ट के लिए समय प्रविष्टि प्रस्तुत की जाती है, तो एक जर्नल लाइन केवल लागत के लिए बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="654fa-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="654fa-112">डिफ़ॉल्ट मूल्य दर्ज करने के लिए तर्क जर्नल लाइन पर रहता है।</span><span class="sxs-lookup"><span data-stu-id="654fa-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="654fa-113">समय प्रविष्टि से सभी फ़ील्ड मान जर्नल लाइन में कॉपी किए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="654fa-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="654fa-114">इन फील्ड में लेन-देन की तारीख, अनुबंध रेखा जिसे प्रोजेक्ट के लिए चिह्नांकित किया गया है, और उचित मूल्य सूची में मुद्रा परिणाम।</span><span class="sxs-lookup"><span data-stu-id="654fa-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="654fa-115">डिफ़ॉल्ट मूल्य को प्रभावित करने वाले फ़ील्ड, जैसे **भूमिका** और **संगठन इकाई** जर्नल लाइन पर डिफ़ॉल्ट रूप से एक उचित मूल्य दर्ज करने का कारण बनते हैं।</span><span class="sxs-lookup"><span data-stu-id="654fa-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="654fa-116">यदि आप समय प्रविष्टि पर कोई कस्टम फ़ील्ड जोड़ते हैं, और आप चाहते हैं कि फ़ील्ड मान वास्तविक रूप से प्रचारित किया जाए तो वास्तविक इकाई पर फ़ील्ड बनाएँ, और फ़ील्ड चिह्नांकन का उपयोग वास्तविक समय प्रविष्टि से फ़ील्ड की क़ॉपी बनाने के लिए करें।</span><span class="sxs-lookup"><span data-stu-id="654fa-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="654fa-117">व्यय प्रविष्टि प्रस्तुत करना</span><span class="sxs-lookup"><span data-stu-id="654fa-117">Submitting an expense entry</span></span>

<span data-ttu-id="654fa-118">PSA में, जब एक व्यय प्रविष्टि एक प्रोजेक्ट के लिए प्रस्तुत की जाती है जिसे एक समय-और-सामग्री अनुबंध लाइन में चिह्नांकित किया जाता है, दो जर्नल लाइनें बनाई जाती हैं।</span><span class="sxs-lookup"><span data-stu-id="654fa-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="654fa-119">एक लाइन लागत के लिए है, और दूसरी लाइन बिना बिल की बिक्री के लिए है।</span><span class="sxs-lookup"><span data-stu-id="654fa-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="654fa-120">जब एक व्यय प्रविष्टि एक निश्चित-मूल्य अनुबंध लाइन के लिए चिह्नांकित किए गये प्रोजेक्ट के लिए प्रस्तुत की जाती है, तो एक जर्नल लाइन केवल लागत के लिए बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="654fa-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="654fa-121">व्यय के लिए डिफ़ॉल्ट मूल्य दर्ज करने के लिए तर्क व्यय श्रेणी पर आधारित है जिसे **व्यय प्रविष्टि** पृष्ठ पर चुना गया है।</span><span class="sxs-lookup"><span data-stu-id="654fa-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="654fa-122">लेन-देन की तारीख, अनुबंध रेखा जिसे प्रोजेक्ट के लिए चिह्नांकित किया गया है, और मुद्रा-सभी का उपयोग उचित मूल्य सूची निर्धारित करने के लिए किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="654fa-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="654fa-123">हालांकि, मूल्य के लिए, उपयोगकर्ता द्वारा दर्ज की गई राशि डिफ़ॉल्ट रूप से लागत और बिक्री के लिए संबंधित व्यय जर्नल लाइनों पर सीधे स्थापित की जाती है।</span><span class="sxs-lookup"><span data-stu-id="654fa-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="654fa-124">PSA के वर्तमान संस्करण में, व्यय प्रविष्टियों पर प्रति-इकाई डिफ़ॉल्ट कीमतों की श्रेणी-आधारित प्रविष्टि उपलब्ध नहीं है।</span><span class="sxs-lookup"><span data-stu-id="654fa-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-journals-to-record-costs"></a><span data-ttu-id="654fa-125">लागत रिकॉर्ड करने के लिए जर्नल का उपयोग करना</span><span class="sxs-lookup"><span data-stu-id="654fa-125">Using journals to record costs</span></span>

<span data-ttu-id="654fa-126">PSA में, आप जर्नल में सामग्री, शुल्क, समय, व्यय, या कर लेनदेन वर्गों में लागत या राजस्व रिकॉर्ड कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="654fa-126">In PSA, journals let you record cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="654fa-127">जर्नल में एक शीर्षक, लाइनें और एक **पुष्टि** क्रिया है।</span><span class="sxs-lookup"><span data-stu-id="654fa-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="654fa-128">यहां कुछ परिदृश्य दिए गए हैं जहां आप एक जर्नल का उपयोग कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="654fa-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="654fa-129">आपको किसी प्रोजेक्ट पर सामग्री की वास्तविक लागत और बिक्री रिकॉर्ड करनी चाहिए।</span><span class="sxs-lookup"><span data-stu-id="654fa-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="654fa-130">आपको किसी अन्य सिस्टम से PSA में लेनदेन के वास्तविक आंकड़ों को स्थानांतरित करना होगा।</span><span class="sxs-lookup"><span data-stu-id="654fa-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="654fa-131">आपको किसी अन्य सिस्टम में उत्पन्न होने वाली लागत को रिकॉर्ड करना होगा, जैसे कि खरीद या उप-अनुबंध लागत।</span><span class="sxs-lookup"><span data-stu-id="654fa-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="654fa-132">प्रोजेक्ट कार्यक्रमों के आधार पर वास्तविक आंकड़ों की रिकॉर्डिंग</span><span class="sxs-lookup"><span data-stu-id="654fa-132">Recording actuals based on project events</span></span>

<span data-ttu-id="654fa-133">PSA किसी प्रोजेक्ट के दौरान होने वाले वित्तीय लेनदेन को रिकॉर्ड करता है।</span><span class="sxs-lookup"><span data-stu-id="654fa-133">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="654fa-134">ये लेन-देन **वास्तविक** के रूप में दर्ज किए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="654fa-134">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="654fa-135">निम्न तालिकाएं विभिन्न प्रकार के बनाए गये वास्तविक आंकड़ों को दर्शाती हैं, इस पर निर्भर है कि क्या परियोजना एक समय-और-सामग्री है या फिक्स्ड-प्राइस प्रोजेक्ट बिक्री-पूर्व चरण में है, या एक आंतरिक परियोजना है।</span><span class="sxs-lookup"><span data-stu-id="654fa-135">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="654fa-136">**संसाधन, प्रोजेक्ट की अनुबंध इकाई के रूप में उसी संगठनात्मक इकाई से संबद्ध है**</span><span class="sxs-lookup"><span data-stu-id="654fa-136">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="654fa-137">ईवेंट</span><span class="sxs-lookup"><span data-stu-id="654fa-137">Event</span></span></th>
<th colspan="4"><span data-ttu-id="654fa-138">बिल योग्य या बेचा गया प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="654fa-138">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="654fa-139">प्रोजेक्ट बिक्री-पूर्व चरण में</span><span class="sxs-lookup"><span data-stu-id="654fa-139">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="654fa-140">आंतरिक प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="654fa-140">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="654fa-141">समय और सामग्री</span><span class="sxs-lookup"><span data-stu-id="654fa-141">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="654fa-142">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="654fa-142">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="654fa-143">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="654fa-143">Actuals</span></span></th>
<th><span data-ttu-id="654fa-144">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-144">Transaction currency</span></span></th>
<th><span data-ttu-id="654fa-145">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="654fa-145">Fixed price</span></span></th>
<th><span data-ttu-id="654fa-146">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-146">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="654fa-147">एक समय प्रविष्टि बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="654fa-147">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="654fa-148">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-148">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-149">एक समय प्रविष्टि प्रस्तुत की जाती है।</span><span class="sxs-lookup"><span data-stu-id="654fa-149">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="654fa-150">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-150">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="654fa-151">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कोई परिवर्तन या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="654fa-151">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="654fa-152">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-152">Cost actual</span></span></td>
<td><span data-ttu-id="654fa-153">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-153">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="654fa-154">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-154">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="654fa-155">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-155">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="654fa-156">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-156">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="654fa-157">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-157">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-158">वास्तविक बिक्री बिना बिल की (अनबिल्ड) – प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="654fa-158">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="654fa-159">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-159">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="654fa-160">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="654fa-160">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="654fa-161">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-161">Cost actual</span></span></td>
<td><span data-ttu-id="654fa-162">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-162">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="654fa-163">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-163">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="654fa-164">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-164">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="654fa-165">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-165">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="654fa-166">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-166">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-167">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="654fa-167">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="654fa-168">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-168">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-169">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="654fa-169">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="654fa-170">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-170">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="654fa-171">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कोई बदलाव या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="654fa-171">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="654fa-172">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="654fa-172">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="654fa-173">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-173">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="654fa-174">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री</span><span class="sxs-lookup"><span data-stu-id="654fa-174">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="654fa-175">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-175">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="654fa-176">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-176">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="654fa-177">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-177">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-178">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="654fa-178">Billed sales</span></span></td>
<td><span data-ttu-id="654fa-179">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-179">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="654fa-180">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="654fa-180">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="654fa-181">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="654fa-181">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="654fa-182">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-182">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="654fa-183">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-183">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="654fa-184">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-184">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="654fa-185">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-185">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="654fa-186">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-186">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-187">बिल की गयी बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="654fa-187">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="654fa-188">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-188">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-189">बिल की गयी बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="654fa-189">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="654fa-190">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-190">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="654fa-191">प्रभार्य मात्रा बढ़ाने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="654fa-191">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="654fa-192">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="654fa-192">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="654fa-193">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-193">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="654fa-194">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री का उलटाव (रिवर्सल)</span><span class="sxs-lookup"><span data-stu-id="654fa-194">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="654fa-195">माइलस्टोन स्थिति में परिवर्तन <strong>चालान</strong> से <strong>चालान के लिए तैयार</strong> तक</span><span class="sxs-lookup"><span data-stu-id="654fa-195">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="654fa-196">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-196">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="654fa-197">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-197">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="654fa-198">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-198">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-199">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="654fa-199">Billed sales</span></span></td>
<td><span data-ttu-id="654fa-200">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-200">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="654fa-201">प्रभार्य मात्रा को कम करने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="654fa-201">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="654fa-202">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="654fa-202">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="654fa-203">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-203">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-204">नई मात्रा के लिए बिल की गयी बिक्री</span><span class="sxs-lookup"><span data-stu-id="654fa-204">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="654fa-205">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-205">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-206">बिन न की गयी बिक्री - अंतर के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="654fa-206">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="654fa-207">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-207">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="654fa-208">**संसाधन एक संगठनात्मक इकाई के अंतर्गत आता है जो प्रोजेक्ट की अनुबंध इकाई से भिन्न होता है**</span><span class="sxs-lookup"><span data-stu-id="654fa-208">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="654fa-209">ईवेंट</span><span class="sxs-lookup"><span data-stu-id="654fa-209">Event</span></span></th>
<th colspan="4"><span data-ttu-id="654fa-210">बिल योग्य या बेचा गया प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="654fa-210">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="654fa-211">प्रोजेक्ट बिक्री-पूर्व चरण में</span><span class="sxs-lookup"><span data-stu-id="654fa-211">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="654fa-212">आंतरिक प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="654fa-212">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="654fa-213">समय और सामग्री</span><span class="sxs-lookup"><span data-stu-id="654fa-213">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="654fa-214">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="654fa-214">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="654fa-215">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="654fa-215">Actuals</span></span></th>
<th><span data-ttu-id="654fa-216">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-216">Transaction currency</span></span></th>
<th><span data-ttu-id="654fa-217">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="654fa-217">Fixed price</span></span></th>
<th><span data-ttu-id="654fa-218">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-218">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="654fa-219">एक समय प्रविष्टि बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="654fa-219">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="654fa-220">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-220">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-221">एक समय प्रविष्टि प्रस्तुत की जाती है।</span><span class="sxs-lookup"><span data-stu-id="654fa-221">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="654fa-222">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-222">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="654fa-223">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कोई परिवर्तन या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="654fa-223">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="654fa-224">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-224">Cost actual</span></span></td>
<td><span data-ttu-id="654fa-225">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-225">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="654fa-226">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-226">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="654fa-227">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-227">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="654fa-228">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-228">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="654fa-229">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-229">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-230">वास्तविक बिक्री बिना बिल की (अनबिल्ड) – प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="654fa-230">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="654fa-231">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-231">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-232">सोर्सिंग यूनिट की लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-232">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="654fa-233">संसाधनित इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-233">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-234">अंत: संगठनात्मक बिक्री</span><span class="sxs-lookup"><span data-stu-id="654fa-234">Interorganizational sales</span></span></td>
<td><span data-ttu-id="654fa-235">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-235">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="654fa-236">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="654fa-236">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="654fa-237">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-237">Cost actual</span></span></td>
<td><span data-ttu-id="654fa-238">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-238">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="654fa-239">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-239">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="654fa-240">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-240">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="654fa-241">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-241">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="654fa-242">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-242">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-243">सोर्सिंग यूनिट की लागत</span><span class="sxs-lookup"><span data-stu-id="654fa-243">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="654fa-244">संसाधनित इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-244">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-245">अंत: संगठनात्मक बिक्री</span><span class="sxs-lookup"><span data-stu-id="654fa-245">Interorganizational sales</span></span></td>
<td><span data-ttu-id="654fa-246">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-246">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-247">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="654fa-247">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="654fa-248">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-248">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-249">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="654fa-249">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="654fa-250">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-250">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="654fa-251">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कोई बदलाव या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="654fa-251">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="654fa-252">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="654fa-252">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="654fa-253">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-253">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="654fa-254">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री</span><span class="sxs-lookup"><span data-stu-id="654fa-254">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="654fa-255">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-255">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="654fa-256">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-256">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="654fa-257">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-257">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-258">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="654fa-258">Billed sales</span></span></td>
<td><span data-ttu-id="654fa-259">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-259">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="654fa-260">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="654fa-260">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="654fa-261">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="654fa-261">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="654fa-262">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-262">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="654fa-263">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-263">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="654fa-264">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-264">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="654fa-265">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-265">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="654fa-266">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-266">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-267">बिल की गयी बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="654fa-267">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="654fa-268">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-268">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-269">बिल की गयी बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="654fa-269">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="654fa-270">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-270">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="654fa-271">प्रभार्य मात्रा बढ़ाने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="654fa-271">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="654fa-272">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="654fa-272">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="654fa-273">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-273">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="654fa-274">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री का उलटाव (रिवर्सल)</span><span class="sxs-lookup"><span data-stu-id="654fa-274">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="654fa-275">माइलस्टोन स्थिति में परिवर्तन <strong>चालान</strong> से <strong>चालान के लिए तैयार</strong> तक</span><span class="sxs-lookup"><span data-stu-id="654fa-275">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="654fa-276">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-276">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="654fa-277">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-277">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="654fa-278">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="654fa-278">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-279">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="654fa-279">Billed sales</span></span></td>
<td><span data-ttu-id="654fa-280">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-280">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="654fa-281">प्रभार्य मात्रा को कम करने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="654fa-281">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="654fa-282">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="654fa-282">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="654fa-283">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-283">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-284">नई मात्रा के लिए बिल की गयी बिक्री</span><span class="sxs-lookup"><span data-stu-id="654fa-284">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="654fa-285">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-285">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="654fa-286">बिन न की गयी बिक्री - अंतर के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="654fa-286">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="654fa-287">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="654fa-287">Project contract currency</span></span></td>
</tr>
</tbody>
</table>
