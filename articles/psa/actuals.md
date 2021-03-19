---
title: वास्तविक अवलोकन
description: यह विषय परियोजना के वास्तविक आंकड़ों के बारे में जानकारी प्रदान करता है।
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 08/03/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: c4a3424bed704243dfb5524fa541c3fcc0899e57
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5285620"
---
# <a name="actuals-overview"></a><span data-ttu-id="57fd9-103">वास्तविक अवलोकन</span><span class="sxs-lookup"><span data-stu-id="57fd9-103">Actuals overview</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="57fd9-104">वास्तविक आंकड़े उस काम की राशि हैं जो एक प्रोजेक्ट में पूरा किया गया है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="57fd9-105">परियोजना वास्तविक आंकड़ों को अपने स्रोत दस्तावेजों से पता लगाया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="57fd9-106">उन स्रोत दस्तावेजों में समय, व्यय और जर्नल प्रविष्टियाँ और चालान भी शामिल हैं।</span><span class="sxs-lookup"><span data-stu-id="57fd9-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![स्रोत दस्तावेज़ों से प्रोजेक्ट के वास्तविक आंकड़ों का पता कैसे लगाया जाता है](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="57fd9-108">एक समय प्रविष्टि प्रस्तुत करना</span><span class="sxs-lookup"><span data-stu-id="57fd9-108">Submitting a time entry</span></span>

<span data-ttu-id="57fd9-109">PSA में, जब एक प्रोजेक्ट के लिए एक समय प्रविष्टि प्रस्तुत की जाती है, जो समय और सामग्री अनुबंध लाइन के लिए चिह्नांकित किया गया है, दो जर्नल लाइनें बनाई जाती हैं।</span><span class="sxs-lookup"><span data-stu-id="57fd9-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="57fd9-110">एक लाइन लागत के लिए है, और दूसरी लाइन बिना बिल की बिक्री के लिए है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="57fd9-111">जब किसी निश्चित-मूल्य अनुबंध रेखा पर चिह्नांकित किए गये प्रोजेक्ट के लिए समय प्रविष्टि प्रस्तुत की जाती है, तो एक जर्नल लाइन केवल लागत के लिए बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="57fd9-112">डिफ़ॉल्ट मूल्य दर्ज करने के लिए तर्क जर्नल लाइन पर रहता है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="57fd9-113">समय प्रविष्टि से सभी फ़ील्ड मान जर्नल लाइन में कॉपी किए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="57fd9-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="57fd9-114">इन फील्ड में लेन-देन की तारीख, अनुबंध रेखा जिसे प्रोजेक्ट के लिए चिह्नांकित किया गया है, और उचित मूल्य सूची में मुद्रा परिणाम।</span><span class="sxs-lookup"><span data-stu-id="57fd9-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="57fd9-115">डिफ़ॉल्ट मूल्य को प्रभावित करने वाले फ़ील्ड, जैसे **भूमिका** और **संगठन इकाई** जर्नल लाइन पर डिफ़ॉल्ट रूप से एक उचित मूल्य दर्ज करने का कारण बनते हैं।</span><span class="sxs-lookup"><span data-stu-id="57fd9-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="57fd9-116">यदि आप समय प्रविष्टि पर कोई कस्टम फ़ील्ड जोड़ते हैं, और आप चाहते हैं कि फ़ील्ड मान वास्तविक रूप से प्रचारित किया जाए तो वास्तविक इकाई पर फ़ील्ड बनाएँ, और फ़ील्ड चिह्नांकन का उपयोग वास्तविक समय प्रविष्टि से फ़ील्ड की क़ॉपी बनाने के लिए करें।</span><span class="sxs-lookup"><span data-stu-id="57fd9-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="57fd9-117">व्यय प्रविष्टि प्रस्तुत करना</span><span class="sxs-lookup"><span data-stu-id="57fd9-117">Submitting an expense entry</span></span>

<span data-ttu-id="57fd9-118">PSA में, जब एक व्यय प्रविष्टि एक प्रोजेक्ट के लिए प्रस्तुत की जाती है जिसे एक समय-और-सामग्री अनुबंध लाइन में चिह्नांकित किया जाता है, दो जर्नल लाइनें बनाई जाती हैं।</span><span class="sxs-lookup"><span data-stu-id="57fd9-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="57fd9-119">एक लाइन लागत के लिए है, और दूसरी लाइन बिना बिल की बिक्री के लिए है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="57fd9-120">जब एक व्यय प्रविष्टि एक निश्चित-मूल्य अनुबंध लाइन के लिए चिह्नांकित किए गये प्रोजेक्ट के लिए प्रस्तुत की जाती है, तो एक जर्नल लाइन केवल लागत के लिए बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="57fd9-121">व्यय के लिए डिफ़ॉल्ट मूल्य दर्ज करने के लिए तर्क व्यय श्रेणी पर आधारित है जिसे **व्यय प्रविष्टि** पृष्ठ पर चुना गया है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="57fd9-122">लेन-देन की तारीख, अनुबंध रेखा जिसे प्रोजेक्ट के लिए चिह्नांकित किया गया है, और मुद्रा-सभी का उपयोग उचित मूल्य सूची निर्धारित करने के लिए किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="57fd9-123">हालांकि, मूल्य के लिए, उपयोगकर्ता द्वारा दर्ज की गई राशि डिफ़ॉल्ट रूप से लागत और बिक्री के लिए संबंधित व्यय जर्नल लाइनों पर सीधे स्थापित की जाती है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="57fd9-124">PSA के वर्तमान संस्करण में, व्यय प्रविष्टियों पर प्रति-इकाई डिफ़ॉल्ट कीमतों की श्रेणी-आधारित प्रविष्टि उपलब्ध नहीं है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-entry-journals-to-record-costs"></a><span data-ttu-id="57fd9-125">लागत रिकॉर्ड करने के लिए प्रविष्टि जर्नल का उपयोग करना</span><span class="sxs-lookup"><span data-stu-id="57fd9-125">Using Entry journals to record costs</span></span>

<span data-ttu-id="57fd9-126">PSA में, आप प्रविष्टि जर्नल के चलते सामग्री, शुल्क, समय, व्यय या कर लेनदेन वर्गों में लागत या राजस्व रिकॉर्ड कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="57fd9-126">In PSA, Entry journals let you record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="57fd9-127">जर्नल में एक शीर्षक, लाइनें और एक **पुष्टि** क्रिया है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="57fd9-128">यहां कुछ परिदृश्य दिए गए हैं जहां आप एक जर्नल का उपयोग कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="57fd9-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="57fd9-129">आपको किसी प्रोजेक्ट पर सामग्री की वास्तविक लागत और बिक्री रिकॉर्ड करनी चाहिए।</span><span class="sxs-lookup"><span data-stu-id="57fd9-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="57fd9-130">आपको किसी अन्य सिस्टम से PSA में लेनदेन के वास्तविक आंकड़ों को स्थानांतरित करना होगा।</span><span class="sxs-lookup"><span data-stu-id="57fd9-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="57fd9-131">आपको किसी अन्य सिस्टम में उत्पन्न होने वाली लागत को रिकॉर्ड करना होगा, जैसे कि खरीद या उप-अनुबंध लागत।</span><span class="sxs-lookup"><span data-stu-id="57fd9-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="57fd9-132">वास्तविक बनाने के लिए प्रविष्टि जर्नल का उपयोग केवल उस उपयोगकर्ता द्वारा किया जाना चाहिए, जो वास्तविक रूप से परियोजना पर लेखांकन प्रभाव के बारे में जानता हो.</span><span class="sxs-lookup"><span data-stu-id="57fd9-132">Using Entry journals to create actuals should be done only by a user who is fully aware of the accounting impact the Actuals have on the project.</span></span> <span data-ttu-id="57fd9-133">ऐसा इसलिए है, क्योंकि एप्लिकेशन जर्नल पंक्ति प्रकार या जर्नल पंक्ति पर दर्ज संबंधित मूल्य निर्धारण को सत्यापित नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="57fd9-133">This is because the application does not validate the journal line type, or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="57fd9-134">इस जर्नल प्रकार के प्रभाव के कारण, इस बात विशेष ध्यान दें कि किस व्यक्ति को प्रविष्टि जर्नल बनाने की पहुँच दी गई है.</span><span class="sxs-lookup"><span data-stu-id="57fd9-134">Because of the impact of this journal type, exercise adequate caution in who is given access to create Entry journals.</span></span>     


## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="57fd9-135">प्रोजेक्ट कार्यक्रमों के आधार पर वास्तविक आंकड़ों की रिकॉर्डिंग</span><span class="sxs-lookup"><span data-stu-id="57fd9-135">Recording actuals based on project events</span></span>

<span data-ttu-id="57fd9-136">PSA किसी प्रोजेक्ट के दौरान होने वाले वित्तीय लेनदेन को रिकॉर्ड करता है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-136">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="57fd9-137">ये लेन-देन **वास्तविक** के रूप में दर्ज किए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="57fd9-137">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="57fd9-138">निम्न तालिकाएं विभिन्न प्रकार के बनाए गये वास्तविक आंकड़ों को दर्शाती हैं, इस पर निर्भर है कि क्या परियोजना एक समय-और-सामग्री है या फिक्स्ड-प्राइस प्रोजेक्ट बिक्री-पूर्व चरण में है, या एक आंतरिक परियोजना है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-138">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="57fd9-139">**संसाधन, प्रोजेक्ट की अनुबंध इकाई के रूप में उसी संगठनात्मक इकाई से संबद्ध है**</span><span class="sxs-lookup"><span data-stu-id="57fd9-139">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="57fd9-140">ईवेंट</span><span class="sxs-lookup"><span data-stu-id="57fd9-140">Event</span></span></th>
<th colspan="4"><span data-ttu-id="57fd9-141">बिल योग्य या बेचा गया प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="57fd9-141">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="57fd9-142">प्रोजेक्ट बिक्री-पूर्व चरण में</span><span class="sxs-lookup"><span data-stu-id="57fd9-142">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="57fd9-143">आंतरिक प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="57fd9-143">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="57fd9-144">समय और सामग्रियां</span><span class="sxs-lookup"><span data-stu-id="57fd9-144">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="57fd9-145">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-145">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="57fd9-146">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="57fd9-146">Actuals</span></span></th>
<th><span data-ttu-id="57fd9-147">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-147">Transaction currency</span></span></th>
<th><span data-ttu-id="57fd9-148">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-148">Fixed price</span></span></th>
<th><span data-ttu-id="57fd9-149">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-149">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="57fd9-150">एक समय प्रविष्टि बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-150">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="57fd9-151">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-151">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-152">एक समय प्रविष्टि प्रस्तुत की जाती है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-152">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="57fd9-153">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-153">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="57fd9-154">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कोई परिवर्तन या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-154">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="57fd9-155">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-155">Cost actual</span></span></td>
<td><span data-ttu-id="57fd9-156">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-156">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="57fd9-157">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-157">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="57fd9-158">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-158">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="57fd9-159">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-159">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="57fd9-160">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-160">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-161">वास्तविक बिक्री बिना बिल की (अनबिल्ड) – प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-161">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="57fd9-162">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-162">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="57fd9-163">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-163">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="57fd9-164">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-164">Cost actual</span></span></td>
<td><span data-ttu-id="57fd9-165">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-165">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="57fd9-166">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-166">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="57fd9-167">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-167">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="57fd9-168">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-168">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="57fd9-169">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-169">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-170">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-170">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="57fd9-171">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-171">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-172">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-172">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="57fd9-173">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-173">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="57fd9-174">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कोई बदलाव या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-174">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="57fd9-175">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="57fd9-175">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="57fd9-176">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-176">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="57fd9-177">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री</span><span class="sxs-lookup"><span data-stu-id="57fd9-177">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="57fd9-178">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-178">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="57fd9-179">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-179">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="57fd9-180">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-180">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-181">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="57fd9-181">Billed sales</span></span></td>
<td><span data-ttu-id="57fd9-182">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-182">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="57fd9-183">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-183">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="57fd9-184">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="57fd9-184">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="57fd9-185">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-185">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="57fd9-186">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-186">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="57fd9-187">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-187">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="57fd9-188">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-188">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="57fd9-189">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-189">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-190">बिल की गयी बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-190">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="57fd9-191">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-191">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-192">बिल की गयी बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-192">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="57fd9-193">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-193">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="57fd9-194">प्रभार्य मात्रा बढ़ाने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-194">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="57fd9-195">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="57fd9-195">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="57fd9-196">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-196">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="57fd9-197">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री का उलटाव (रिवर्सल)</span><span class="sxs-lookup"><span data-stu-id="57fd9-197">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="57fd9-198">माइलस्टोन स्थिति में परिवर्तन <strong>चालान</strong> से <strong>चालान के लिए तैयार</strong> तक</span><span class="sxs-lookup"><span data-stu-id="57fd9-198">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="57fd9-199">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-199">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="57fd9-200">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-200">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="57fd9-201">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-201">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-202">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="57fd9-202">Billed sales</span></span></td>
<td><span data-ttu-id="57fd9-203">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-203">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="57fd9-204">प्रभार्य मात्रा को कम करने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-204">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="57fd9-205">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="57fd9-205">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="57fd9-206">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-206">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-207">नई मात्रा के लिए बिल की गयी बिक्री</span><span class="sxs-lookup"><span data-stu-id="57fd9-207">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="57fd9-208">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-208">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-209">बिन न की गयी बिक्री - अंतर के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-209">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="57fd9-210">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-210">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="57fd9-211">**संसाधन एक संगठनात्मक इकाई के अंतर्गत आता है जो प्रोजेक्ट की अनुबंध इकाई से भिन्न होता है**</span><span class="sxs-lookup"><span data-stu-id="57fd9-211">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="57fd9-212">ईवेंट</span><span class="sxs-lookup"><span data-stu-id="57fd9-212">Event</span></span></th>
<th colspan="4"><span data-ttu-id="57fd9-213">बिल योग्य या बेचा गया प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="57fd9-213">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="57fd9-214">प्रोजेक्ट बिक्री-पूर्व चरण में</span><span class="sxs-lookup"><span data-stu-id="57fd9-214">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="57fd9-215">आंतरिक प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="57fd9-215">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="57fd9-216">समय और सामग्रियां</span><span class="sxs-lookup"><span data-stu-id="57fd9-216">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="57fd9-217">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-217">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="57fd9-218">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="57fd9-218">Actuals</span></span></th>
<th><span data-ttu-id="57fd9-219">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-219">Transaction currency</span></span></th>
<th><span data-ttu-id="57fd9-220">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-220">Fixed price</span></span></th>
<th><span data-ttu-id="57fd9-221">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-221">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="57fd9-222">एक समय प्रविष्टि बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-222">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="57fd9-223">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-223">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-224">एक समय प्रविष्टि प्रस्तुत की जाती है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-224">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="57fd9-225">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-225">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="57fd9-226">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कोई परिवर्तन या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-226">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="57fd9-227">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-227">Cost actual</span></span></td>
<td><span data-ttu-id="57fd9-228">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-228">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="57fd9-229">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-229">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="57fd9-230">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-230">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="57fd9-231">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-231">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="57fd9-232">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-232">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-233">वास्तविक बिक्री बिना बिल की (अनबिल्ड) – प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-233">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="57fd9-234">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-235">सोर्सिंग यूनिट की लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-235">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="57fd9-236">संसाधनित इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-236">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-237">अंत: संगठनात्मक बिक्री</span><span class="sxs-lookup"><span data-stu-id="57fd9-237">Interorganizational sales</span></span></td>
<td><span data-ttu-id="57fd9-238">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-238">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="57fd9-239">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-239">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="57fd9-240">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-240">Cost actual</span></span></td>
<td><span data-ttu-id="57fd9-241">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-241">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="57fd9-242">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-242">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="57fd9-243">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-243">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="57fd9-244">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-244">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="57fd9-245">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-245">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-246">सोर्सिंग यूनिट की लागत</span><span class="sxs-lookup"><span data-stu-id="57fd9-246">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="57fd9-247">संसाधनित इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-247">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-248">अंत: संगठनात्मक बिक्री</span><span class="sxs-lookup"><span data-stu-id="57fd9-248">Interorganizational sales</span></span></td>
<td><span data-ttu-id="57fd9-249">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-249">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-250">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-250">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="57fd9-251">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-251">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-252">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-252">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="57fd9-253">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-253">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="57fd9-254">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कोई बदलाव या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-254">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="57fd9-255">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="57fd9-255">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="57fd9-256">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-256">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="57fd9-257">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री</span><span class="sxs-lookup"><span data-stu-id="57fd9-257">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="57fd9-258">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-258">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="57fd9-259">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-259">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="57fd9-260">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-260">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-261">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="57fd9-261">Billed sales</span></span></td>
<td><span data-ttu-id="57fd9-262">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-262">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="57fd9-263">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-263">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="57fd9-264">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="57fd9-264">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="57fd9-265">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-265">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="57fd9-266">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-266">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="57fd9-267">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-267">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="57fd9-268">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-268">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="57fd9-269">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-269">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-270">बिल की गयी बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-270">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="57fd9-271">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-271">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-272">बिल की गयी बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-272">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="57fd9-273">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-273">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="57fd9-274">प्रभार्य मात्रा बढ़ाने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-274">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="57fd9-275">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="57fd9-275">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="57fd9-276">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-276">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="57fd9-277">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री का उलटाव (रिवर्सल)</span><span class="sxs-lookup"><span data-stu-id="57fd9-277">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="57fd9-278">माइलस्टोन स्थिति में परिवर्तन <strong>चालान</strong> से <strong>चालान के लिए तैयार</strong> तक</span><span class="sxs-lookup"><span data-stu-id="57fd9-278">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="57fd9-279">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-279">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="57fd9-280">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-280">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="57fd9-281">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="57fd9-281">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-282">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="57fd9-282">Billed sales</span></span></td>
<td><span data-ttu-id="57fd9-283">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-283">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="57fd9-284">प्रभार्य मात्रा को कम करने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="57fd9-284">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="57fd9-285">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="57fd9-285">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="57fd9-286">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-286">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-287">नई मात्रा के लिए बिल की गयी बिक्री</span><span class="sxs-lookup"><span data-stu-id="57fd9-287">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="57fd9-288">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-288">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="57fd9-289">बिन न की गयी बिक्री - अंतर के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="57fd9-289">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="57fd9-290">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="57fd9-290">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]