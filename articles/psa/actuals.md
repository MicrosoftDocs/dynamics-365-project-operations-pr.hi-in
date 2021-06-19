---
title: वास्तविक अवलोकन
description: यह विषय परियोजना के वास्तविक आंकड़ों के बारे में जानकारी प्रदान करता है।
author: rumant
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
ms.openlocfilehash: 73f1b14bbb4cc53111a1b3a93756a86db04475ab
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6014658"
---
# <a name="actuals-overview"></a><span data-ttu-id="7603c-103">वास्तविक अवलोकन</span><span class="sxs-lookup"><span data-stu-id="7603c-103">Actuals overview</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="7603c-104">वास्तविक आंकड़े उस काम की राशि हैं जो एक प्रोजेक्ट में पूरा किया गया है।</span><span class="sxs-lookup"><span data-stu-id="7603c-104">Actuals are the amount of work that has been completed on a project.</span></span> <span data-ttu-id="7603c-105">परियोजना वास्तविक आंकड़ों को अपने स्रोत दस्तावेजों से पता लगाया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="7603c-105">Project actuals can be traced back to their source documents.</span></span> <span data-ttu-id="7603c-106">उन स्रोत दस्तावेजों में समय, व्यय और जर्नल प्रविष्टियाँ और चालान भी शामिल हैं।</span><span class="sxs-lookup"><span data-stu-id="7603c-106">Those source documents include time, expense, and journal entries, and also invoices.</span></span>

![स्रोत दस्तावेज़ों से प्रोजेक्ट के वास्तविक आंकड़ों का पता कैसे लगाया जाता है](media/basic-guide-18.png)

## <a name="submitting-a-time-entry"></a><span data-ttu-id="7603c-108">एक समय प्रविष्टि प्रस्तुत करना</span><span class="sxs-lookup"><span data-stu-id="7603c-108">Submitting a time entry</span></span>

<span data-ttu-id="7603c-109">PSA में, जब एक प्रोजेक्ट के लिए एक समय प्रविष्टि प्रस्तुत की जाती है, जो समय और सामग्री अनुबंध लाइन के लिए चिह्नांकित किया गया है, दो जर्नल लाइनें बनाई जाती हैं।</span><span class="sxs-lookup"><span data-stu-id="7603c-109">In PSA, when a time entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="7603c-110">एक लाइन लागत के लिए है, और दूसरी लाइन बिना बिल की बिक्री के लिए है।</span><span class="sxs-lookup"><span data-stu-id="7603c-110">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="7603c-111">जब किसी निश्चित-मूल्य अनुबंध रेखा पर चिह्नांकित किए गये प्रोजेक्ट के लिए समय प्रविष्टि प्रस्तुत की जाती है, तो एक जर्नल लाइन केवल लागत के लिए बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="7603c-111">When a time entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span> 

<span data-ttu-id="7603c-112">डिफ़ॉल्ट मूल्य दर्ज करने के लिए तर्क जर्नल लाइन पर रहता है।</span><span class="sxs-lookup"><span data-stu-id="7603c-112">Logic for entering default prices resides on the journal line.</span></span> <span data-ttu-id="7603c-113">समय प्रविष्टि से सभी फ़ील्ड मान जर्नल लाइन में कॉपी किए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="7603c-113">All the field values from a time entry are copied to the journal line.</span></span> <span data-ttu-id="7603c-114">इन फील्ड में लेन-देन की तारीख, अनुबंध रेखा जिसे प्रोजेक्ट के लिए चिह्नांकित किया गया है, और उचित मूल्य सूची में मुद्रा परिणाम।</span><span class="sxs-lookup"><span data-stu-id="7603c-114">These fields include the date of the transaction, the contract line that the project is mapped to, and the currency result in the appropriate price list.</span></span> 

<span data-ttu-id="7603c-115">डिफ़ॉल्ट मूल्य को प्रभावित करने वाले फ़ील्ड, जैसे **भूमिका** और **संगठन इकाई** जर्नल लाइन पर डिफ़ॉल्ट रूप से एक उचित मूल्य दर्ज करने का कारण बनते हैं।</span><span class="sxs-lookup"><span data-stu-id="7603c-115">The fields that affect default prices, such as **Role** and **Org Unit**, cause an appropriate price to be entered by default on the journal line.</span></span> <span data-ttu-id="7603c-116">यदि आप समय प्रविष्टि पर कोई कस्टम फ़ील्ड जोड़ते हैं, और आप चाहते हैं कि फ़ील्ड मान वास्तविक रूप से प्रचारित किया जाए तो वास्तविक इकाई पर फ़ील्ड बनाएँ, और फ़ील्ड चिह्नांकन का उपयोग वास्तविक समय प्रविष्टि से फ़ील्ड की क़ॉपी बनाने के लिए करें।</span><span class="sxs-lookup"><span data-stu-id="7603c-116">If you add a custom field on the time entry, and you want the field value to be propagated to actuals, create the field on the Actuals entity, and use field mappings to copy the field from the time entry to the actual.</span></span>

## <a name="submitting-an-expense-entry"></a><span data-ttu-id="7603c-117">व्यय प्रविष्टि प्रस्तुत करना</span><span class="sxs-lookup"><span data-stu-id="7603c-117">Submitting an expense entry</span></span>

<span data-ttu-id="7603c-118">PSA में, जब एक व्यय प्रविष्टि एक प्रोजेक्ट के लिए प्रस्तुत की जाती है जिसे एक समय-और-सामग्री अनुबंध लाइन में चिह्नांकित किया जाता है, दो जर्नल लाइनें बनाई जाती हैं।</span><span class="sxs-lookup"><span data-stu-id="7603c-118">In PSA, when an expense entry is submitted for a project that is mapped to a time-and-materials contract line, two journal lines are created.</span></span> <span data-ttu-id="7603c-119">एक लाइन लागत के लिए है, और दूसरी लाइन बिना बिल की बिक्री के लिए है।</span><span class="sxs-lookup"><span data-stu-id="7603c-119">One line is for cost, and the other line is for unbilled sales.</span></span> <span data-ttu-id="7603c-120">जब एक व्यय प्रविष्टि एक निश्चित-मूल्य अनुबंध लाइन के लिए चिह्नांकित किए गये प्रोजेक्ट के लिए प्रस्तुत की जाती है, तो एक जर्नल लाइन केवल लागत के लिए बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="7603c-120">When an expense entry is submitted for a project that is mapped to a fixed-price contract line, a journal line is created only for cost.</span></span>

<span data-ttu-id="7603c-121">व्यय के लिए डिफ़ॉल्ट मूल्य दर्ज करने के लिए तर्क व्यय श्रेणी पर आधारित है जिसे **व्यय प्रविष्टि** पृष्ठ पर चुना गया है।</span><span class="sxs-lookup"><span data-stu-id="7603c-121">Logic for entering default prices for expenses is based on the expense category that is selected on the **Expense entry** page.</span></span> <span data-ttu-id="7603c-122">लेन-देन की तारीख, अनुबंध रेखा जिसे प्रोजेक्ट के लिए चिह्नांकित किया गया है, और मुद्रा-सभी का उपयोग उचित मूल्य सूची निर्धारित करने के लिए किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="7603c-122">The transaction date, the contract line that the project is mapped to, and the currency are all used to determine the appropriate price list.</span></span> <span data-ttu-id="7603c-123">हालांकि, मूल्य के लिए, उपयोगकर्ता द्वारा दर्ज की गई राशि डिफ़ॉल्ट रूप से लागत और बिक्री के लिए संबंधित व्यय जर्नल लाइनों पर सीधे स्थापित की जाती है।</span><span class="sxs-lookup"><span data-stu-id="7603c-123">However, for the price itself, the amount that the user entered is set directly on the related expense journal lines for cost and sales by default.</span></span>

<span data-ttu-id="7603c-124">PSA के वर्तमान संस्करण में, व्यय प्रविष्टियों पर प्रति-इकाई डिफ़ॉल्ट कीमतों की श्रेणी-आधारित प्रविष्टि उपलब्ध नहीं है।</span><span class="sxs-lookup"><span data-stu-id="7603c-124">In the current version of PSA, category-based entry of per-unit default prices on expense entries isn't available.</span></span>

## <a name="using-entry-journals-to-record-costs"></a><span data-ttu-id="7603c-125">लागत रिकॉर्ड करने के लिए प्रविष्टि जर्नल का उपयोग करना</span><span class="sxs-lookup"><span data-stu-id="7603c-125">Using Entry journals to record costs</span></span>

<span data-ttu-id="7603c-126">PSA में, आप प्रविष्टि जर्नल के चलते सामग्री, शुल्क, समय, व्यय या कर लेनदेन वर्गों में लागत या राजस्व रिकॉर्ड कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="7603c-126">In PSA, Entry journals let you record the cost or revenue in the material, fee, time, expense, or tax transaction classes.</span></span> <span data-ttu-id="7603c-127">जर्नल में एक शीर्षक, लाइनें और एक **पुष्टि** क्रिया है।</span><span class="sxs-lookup"><span data-stu-id="7603c-127">A journal has a header, lines, and a **Confirm** action.</span></span> <span data-ttu-id="7603c-128">यहां कुछ परिदृश्य दिए गए हैं जहां आप एक जर्नल का उपयोग कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="7603c-128">Here are some scenarios where you might use a journal:</span></span>

- <span data-ttu-id="7603c-129">आपको किसी प्रोजेक्ट पर सामग्री की वास्तविक लागत और बिक्री रिकॉर्ड करनी चाहिए।</span><span class="sxs-lookup"><span data-stu-id="7603c-129">You must record material actual costs and sales on a project.</span></span>
- <span data-ttu-id="7603c-130">आपको किसी अन्य सिस्टम से PSA में लेनदेन के वास्तविक आंकड़ों को स्थानांतरित करना होगा।</span><span class="sxs-lookup"><span data-stu-id="7603c-130">You must move transaction actuals from another system to PSA.</span></span>
- <span data-ttu-id="7603c-131">आपको किसी अन्य सिस्टम में उत्पन्न होने वाली लागत को रिकॉर्ड करना होगा, जैसे कि खरीद या उप-अनुबंध लागत।</span><span class="sxs-lookup"><span data-stu-id="7603c-131">You must record costs that occurred in another system, such as procurement or subcontracting costs.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7603c-132">वास्तविक बनाने के लिए प्रविष्टि जर्नल का उपयोग केवल उस उपयोगकर्ता द्वारा किया जाना चाहिए, जो वास्तविक रूप से परियोजना पर लेखांकन प्रभाव के बारे में जानता हो.</span><span class="sxs-lookup"><span data-stu-id="7603c-132">Using Entry journals to create actuals should be done only by a user who is fully aware of the accounting impact the Actuals have on the project.</span></span> <span data-ttu-id="7603c-133">ऐसा इसलिए है, क्योंकि एप्लिकेशन जर्नल पंक्ति प्रकार या जर्नल पंक्ति पर दर्ज संबंधित मूल्य निर्धारण को सत्यापित नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="7603c-133">This is because the application does not validate the journal line type, or the related pricing that is entered on the journal line.</span></span> <span data-ttu-id="7603c-134">इस जर्नल प्रकार के प्रभाव के कारण, इस बात विशेष ध्यान दें कि किस व्यक्ति को प्रविष्टि जर्नल बनाने की पहुँच दी गई है.</span><span class="sxs-lookup"><span data-stu-id="7603c-134">Because of the impact of this journal type, exercise adequate caution in who is given access to create Entry journals.</span></span>     


## <a name="recording-actuals-based-on-project-events"></a><span data-ttu-id="7603c-135">प्रोजेक्ट कार्यक्रमों के आधार पर वास्तविक आंकड़ों की रिकॉर्डिंग</span><span class="sxs-lookup"><span data-stu-id="7603c-135">Recording actuals based on project events</span></span>

<span data-ttu-id="7603c-136">PSA किसी प्रोजेक्ट के दौरान होने वाले वित्तीय लेनदेन को रिकॉर्ड करता है।</span><span class="sxs-lookup"><span data-stu-id="7603c-136">PSA records the financial transactions that occur during a project.</span></span> <span data-ttu-id="7603c-137">ये लेन-देन **वास्तविक** के रूप में दर्ज किए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="7603c-137">These transactions are recorded as **actuals**.</span></span> <span data-ttu-id="7603c-138">निम्न तालिकाएं विभिन्न प्रकार के बनाए गये वास्तविक आंकड़ों को दर्शाती हैं, इस पर निर्भर है कि क्या परियोजना एक समय-और-सामग्री है या फिक्स्ड-प्राइस प्रोजेक्ट बिक्री-पूर्व चरण में है, या एक आंतरिक परियोजना है।</span><span class="sxs-lookup"><span data-stu-id="7603c-138">The following tables show the different types of actuals that are created, depending on whether the project is a time-and-materials or fixed-price project, is in the presales stage, or is an internal project.</span></span>

<span data-ttu-id="7603c-139">**संसाधन, प्रोजेक्ट की अनुबंध इकाई के रूप में उसी संगठनात्मक इकाई से संबद्ध है**</span><span class="sxs-lookup"><span data-stu-id="7603c-139">**The resource belongs to same organizational unit as the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="7603c-140">ईवेंट</span><span class="sxs-lookup"><span data-stu-id="7603c-140">Event</span></span></th>
<th colspan="4"><span data-ttu-id="7603c-141">बिल योग्य या बेचा गया प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="7603c-141">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="7603c-142">प्रोजेक्ट बिक्री-पूर्व चरण में</span><span class="sxs-lookup"><span data-stu-id="7603c-142">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="7603c-143">आंतरिक प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="7603c-143">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="7603c-144">समय और सामग्रियां</span><span class="sxs-lookup"><span data-stu-id="7603c-144">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="7603c-145">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="7603c-145">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="7603c-146">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="7603c-146">Actuals</span></span></th>
<th><span data-ttu-id="7603c-147">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-147">Transaction currency</span></span></th>
<th><span data-ttu-id="7603c-148">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="7603c-148">Fixed price</span></span></th>
<th><span data-ttu-id="7603c-149">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-149">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="7603c-150">एक समय प्रविष्टि बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="7603c-150">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="7603c-151">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-151">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-152">एक समय प्रविष्टि प्रस्तुत की जाती है।</span><span class="sxs-lookup"><span data-stu-id="7603c-152">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="7603c-153">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-153">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7603c-154">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कोई परिवर्तन या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="7603c-154">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7603c-155">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-155">Cost actual</span></span></td>
<td><span data-ttu-id="7603c-156">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-156">Contracting unit currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7603c-157">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-157">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="7603c-158">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-158">Contracting unit currency</span></span>
<td rowspan="2"><span data-ttu-id="7603c-159">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-159">Cost actual</span></span></td>
<td rowspan="2"><span data-ttu-id="7603c-160">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-160">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-161">वास्तविक बिक्री बिना बिल की (अनबिल्ड) – प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="7603c-161">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="7603c-162">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-162">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7603c-163">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="7603c-163">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7603c-164">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-164">Cost actual</span></span></td>
<td><span data-ttu-id="7603c-165">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-165">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7603c-166">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-166">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="7603c-167">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-167">Contracting unit currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7603c-168">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-168">Cost actual</span></span></td>
<td rowspan="3"><span data-ttu-id="7603c-169">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-169">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-170">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="7603c-170">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7603c-171">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-171">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-172">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="7603c-172">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7603c-173">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-173">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7603c-174">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कोई बदलाव या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="7603c-174">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7603c-175">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="7603c-175">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7603c-176">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-176">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7603c-177">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री</span><span class="sxs-lookup"><span data-stu-id="7603c-177">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="7603c-178">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-178">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7603c-179">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-179">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="7603c-180">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-180">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-181">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="7603c-181">Billed sales</span></span></td>
<td><span data-ttu-id="7603c-182">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-182">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7603c-183">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="7603c-183">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7603c-184">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="7603c-184">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7603c-185">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-185">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7603c-186">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-186">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7603c-187">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-187">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7603c-188">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-188">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7603c-189">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-189">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-190">बिल की गयी बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="7603c-190">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7603c-191">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-191">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-192">बिल की गयी बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="7603c-192">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7603c-193">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-193">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7603c-194">प्रभार्य मात्रा बढ़ाने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="7603c-194">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7603c-195">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="7603c-195">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7603c-196">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-196">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="7603c-197">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री का उलटाव (रिवर्सल)</span><span class="sxs-lookup"><span data-stu-id="7603c-197">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="7603c-198">माइलस्टोन स्थिति में परिवर्तन <strong>चालान</strong> से <strong>चालान के लिए तैयार</strong> तक</span><span class="sxs-lookup"><span data-stu-id="7603c-198">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="7603c-199">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-199">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7603c-200">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-200">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="7603c-201">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-201">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-202">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="7603c-202">Billed sales</span></span></td>
<td><span data-ttu-id="7603c-203">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-203">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7603c-204">प्रभार्य मात्रा को कम करने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="7603c-204">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7603c-205">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="7603c-205">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7603c-206">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-206">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-207">नई मात्रा के लिए बिल की गयी बिक्री</span><span class="sxs-lookup"><span data-stu-id="7603c-207">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="7603c-208">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-208">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-209">बिन न की गयी बिक्री - अंतर के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="7603c-209">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="7603c-210">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-210">Project contract currency</span></span></td>
</tr>
</tbody>
</table>

<span data-ttu-id="7603c-211">**संसाधन एक संगठनात्मक इकाई के अंतर्गत आता है जो प्रोजेक्ट की अनुबंध इकाई से भिन्न होता है**</span><span class="sxs-lookup"><span data-stu-id="7603c-211">**The resource belongs to an organizational unit that differs from the project's contracting unit**</span></span>

<table>
<thead>
<tr>
<th rowspan="3"><span data-ttu-id="7603c-212">ईवेंट</span><span class="sxs-lookup"><span data-stu-id="7603c-212">Event</span></span></th>
<th colspan="4"><span data-ttu-id="7603c-213">बिल योग्य या बेचा गया प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="7603c-213">Billable or sold project</span></span></th>
<th rowspan="3"><span data-ttu-id="7603c-214">प्रोजेक्ट बिक्री-पूर्व चरण में</span><span class="sxs-lookup"><span data-stu-id="7603c-214">Project in the presales stage</span></span></th>
<th rowspan="3"><span data-ttu-id="7603c-215">आंतरिक प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="7603c-215">Internal project</span></span></th>
</tr>
<tr>
<th colspan="2"><span data-ttu-id="7603c-216">समय और सामग्रियां</span><span class="sxs-lookup"><span data-stu-id="7603c-216">Time and materials</span></span></th>
<th colspan="2"><span data-ttu-id="7603c-217">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="7603c-217">Fixed price</span></span></th>
</tr>
<tr>
<th><span data-ttu-id="7603c-218">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="7603c-218">Actuals</span></span></th>
<th><span data-ttu-id="7603c-219">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-219">Transaction currency</span></span></th>
<th><span data-ttu-id="7603c-220">निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="7603c-220">Fixed price</span></span></th>
<th><span data-ttu-id="7603c-221">लेन देन मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-221">Transaction currency</span></span></th>
</tr>
</thead>
<tbody>
<tr>
<td><span data-ttu-id="7603c-222">एक समय प्रविष्टि बनाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="7603c-222">A time entry is created.</span></span></td>
<td colspan="6"><span data-ttu-id="7603c-223">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-223">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-224">एक समय प्रविष्टि प्रस्तुत की जाती है।</span><span class="sxs-lookup"><span data-stu-id="7603c-224">A time entry is submitted.</span></span></td>
<td colspan="6"><span data-ttu-id="7603c-225">वास्तविक इकाई में कोई गतिविधि नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-225">No activity in the Actuals entity</span></span></td>
</tr>
<tr>
<td rowspan="4"><span data-ttu-id="7603c-226">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कोई परिवर्तन या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="7603c-226">Time is approved, and no change to or increase in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7603c-227">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-227">Cost actual</span></span></td>
<td><span data-ttu-id="7603c-228">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-228">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="7603c-229">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-229">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="7603c-230">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-230">Contracting unit currency</span></span></td>
<td rowspan="4"><span data-ttu-id="7603c-231">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-231">Cost actual</span></span></td>
<td rowspan="4"><span data-ttu-id="7603c-232">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-232">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-233">वास्तविक बिक्री बिना बिल की (अनबिल्ड) – प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="7603c-233">Unbilled sales actual – Chargeable</span></span></td>
<td><span data-ttu-id="7603c-234">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-234">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-235">सोर्सिंग यूनिट की लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-235">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="7603c-236">संसाधनित इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-236">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-237">अंत: संगठनात्मक बिक्री</span><span class="sxs-lookup"><span data-stu-id="7603c-237">Interorganizational sales</span></span></td>
<td><span data-ttu-id="7603c-238">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-238">Contracting unit currency</span></span></td>
</tr>
<tr>
<td rowspan="5"><span data-ttu-id="7603c-239">समय स्वीकृत है, और अनुमोदन के दौरान बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="7603c-239">Time is approved, and a decrease in billable hours occurs during approval.</span></span></td>
<td><span data-ttu-id="7603c-240">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-240">Cost actual</span></span></td>
<td><span data-ttu-id="7603c-241">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-241">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7603c-242">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-242">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="7603c-243">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-243">Contracting unit currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7603c-244">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-244">Cost actual</span></span></td>
<td rowspan="5"><span data-ttu-id="7603c-245">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-245">Cost actual</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-246">सोर्सिंग यूनिट की लागत</span><span class="sxs-lookup"><span data-stu-id="7603c-246">Resourcing unit cost</span></span></td>
<td><span data-ttu-id="7603c-247">संसाधनित इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-247">Resourcing unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-248">अंत: संगठनात्मक बिक्री</span><span class="sxs-lookup"><span data-stu-id="7603c-248">Interorganizational sales</span></span></td>
<td><span data-ttu-id="7603c-249">अनुबंध इकाई मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-249">Contracting unit currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-250">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="7603c-250">Unbilled sales actual – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7603c-251">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-251">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-252">बिना बिल की (अनबिल्ड) वास्तविक बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="7603c-252">Unbilled sales actual – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7603c-253">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-253">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7603c-254">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कोई बदलाव या वृद्धि नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="7603c-254">An invoice is confirmed, and no change to or increase in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7603c-255">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="7603c-255">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7603c-256">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-256">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7603c-257">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री</span><span class="sxs-lookup"><span data-stu-id="7603c-257">Billed sales for milestone</span></span></td>
<td rowspan="2"><span data-ttu-id="7603c-258">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-258">Project contract currency</span></span></td>
<td rowspan="2"><span data-ttu-id="7603c-259">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-259">Not applicable</span></span></td>
<td rowspan="2"><span data-ttu-id="7603c-260">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-260">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-261">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="7603c-261">Billed sales</span></span></td>
<td><span data-ttu-id="7603c-262">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-262">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7603c-263">चालान की पुष्टि की जाती है, और बिल योग्य घंटों में कमी होती है।</span><span class="sxs-lookup"><span data-stu-id="7603c-263">An invoice is confirmed, and a decrease in billable hours occurs.</span></span></td>
<td><span data-ttu-id="7603c-264">बिना बिल की (अनबिल्ड) बिक्री रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="7603c-264">Unbilled sales reversal</span></span></td>
<td><span data-ttu-id="7603c-265">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-265">Project contract currency</span></span></td>
<td rowspan="3"><span data-ttu-id="7603c-266">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-266">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7603c-267">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-267">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7603c-268">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-268">Not applicable</span></span></td>
<td rowspan="3"><span data-ttu-id="7603c-269">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-269">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-270">बिल की गयी बिक्री - नई मात्रा के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="7603c-270">Billed sales – Chargeable for the new quantity</span></span></td>
<td><span data-ttu-id="7603c-271">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-271">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-272">बिल की गयी बिक्री - अंतर के लिए गैर-प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="7603c-272">Billed sales – Non-chargeable for the difference</span></span></td>
<td><span data-ttu-id="7603c-273">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-273">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="2"><span data-ttu-id="7603c-274">प्रभार्य मात्रा बढ़ाने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="7603c-274">An invoice is corrected to increase the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7603c-275">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="7603c-275">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7603c-276">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-276">Project contract currency</span></span></td>
<td rowspan="5">
<ul>
<li><span data-ttu-id="7603c-277">माइलस्टोन के लिए बिल्ड (बिल की गयी) बिक्री का उलटाव (रिवर्सल)</span><span class="sxs-lookup"><span data-stu-id="7603c-277">Billed sales reversal for milestone</span></span></li>
<li><span data-ttu-id="7603c-278">माइलस्टोन स्थिति में परिवर्तन <strong>चालान</strong> से <strong>चालान के लिए तैयार</strong> तक</span><span class="sxs-lookup"><span data-stu-id="7603c-278">Change in milestone status from <strong>Invoiced</strong> to <strong>Ready for invoice</strong></span></span></li>
</ul>
</td>
<td rowspan="5"><span data-ttu-id="7603c-279">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-279">Project contract currency</span></span></td>
<td rowspan="5"><span data-ttu-id="7603c-280">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-280">Not applicable</span></span></td>
<td rowspan="5"><span data-ttu-id="7603c-281">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="7603c-281">Not applicable</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-282">बिल की गई विक्रय</span><span class="sxs-lookup"><span data-stu-id="7603c-282">Billed sales</span></span></td>
<td><span data-ttu-id="7603c-283">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-283">Project contract currency</span></span></td>
</tr>
<tr>
<td rowspan="3"><span data-ttu-id="7603c-284">प्रभार्य मात्रा को कम करने के लिए चालान को सुधारा जाता है।</span><span class="sxs-lookup"><span data-stu-id="7603c-284">An invoice is corrected to decrease the chargeable quantity.</span></span></td>
<td><span data-ttu-id="7603c-285">बिल की गयी बिक्री - रिवर्सल</span><span class="sxs-lookup"><span data-stu-id="7603c-285">Billed sales – Reversal</span></span></td>
<td><span data-ttu-id="7603c-286">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-286">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-287">नई मात्रा के लिए बिल की गयी बिक्री</span><span class="sxs-lookup"><span data-stu-id="7603c-287">Billed sales for the new quantity</span></span></td>
<td><span data-ttu-id="7603c-288">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-288">Project contract currency</span></span></td>
</tr>
<tr>
<td><span data-ttu-id="7603c-289">बिन न की गयी बिक्री - अंतर के लिए प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="7603c-289">Unbilled sales – Chargeable for the difference</span></span></td>
<td><span data-ttu-id="7603c-290">प्रोजेक्ट अनुबंध मुद्रा</span><span class="sxs-lookup"><span data-stu-id="7603c-290">Project contract currency</span></span></td>
</tr>
</tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]