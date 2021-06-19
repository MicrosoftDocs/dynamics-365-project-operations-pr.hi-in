---
title: प्रोफ़ॉर्मा परियोजना इनवॉइस की पुष्टि करें
description: यह विषय Project Operations में प्रोफार्मा परियोजना इनवॉइस की पुष्टि करने के बारे में जानकारी प्रदान करता है.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 0ab40e38f221e57368949b7491578caa8ba88c02
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004128"
---
# <a name="confirm-a-proforma-project-invoice"></a><span data-ttu-id="f65ed-103">प्रोफ़ॉर्मा परियोजना इनवॉइस की पुष्टि करें</span><span class="sxs-lookup"><span data-stu-id="f65ed-103">Confirm a proforma project invoice</span></span> 

<span data-ttu-id="f65ed-104">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="f65ed-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="f65ed-105">प्रोफोर्मा इनवॉइस की पुष्टि के बाद परियोजना इनवॉइस की स्थिति **पुष्ट हुआ** में अपडेट हो जाएगी.</span><span class="sxs-lookup"><span data-stu-id="f65ed-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="f65ed-106">जब एक इनवॉइस की पुष्टि होती है, तो यह केवल पढ़ने के लायक ही रहता है.</span><span class="sxs-lookup"><span data-stu-id="f65ed-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="f65ed-107">अब से, इनवॉइस को केवल तभी सुधारा जा सकता है जब किसी ग्राहक की ओर से शुरू किए गए सुधार या क्रेडिट हों.</span><span class="sxs-lookup"><span data-stu-id="f65ed-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits.</span></span>

<span data-ttu-id="f65ed-108">निम्नलिखित तालिका सिस्टम द्वारा निर्मित वास्तविक को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="f65ed-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="f65ed-109">इन वास्तविक को तभी बनाया गया है जब ड्राफ़्ट परियोजना इनवॉइस की पुष्टि से पहले कुछ संचालनों को प्रदर्शित किया गया था.</span><span class="sxs-lookup"><span data-stu-id="f65ed-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="f65ed-110">
                    <strong>परिदृश्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f65ed-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="f65ed-111">
                    <strong>पुष्टि होने पर बनाए गए वास्तविक</strong>
                </span><span class="sxs-lookup"><span data-stu-id="f65ed-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f65ed-112">अग्रिम या शुल्क का इनवॉइस बनाना</span><span class="sxs-lookup"><span data-stu-id="f65ed-112">Invoicing an advance or retainer</span></span> </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-113">एक वास्तविक बिल बिक्री का प्रकार, <strong>रिटेनर</strong> शुल्क को अग्रिम या शुल्क पर राशि के लिए बनाया गया है.</span><span class="sxs-lookup"><span data-stu-id="f65ed-113">A billed sales actual of type, <strong>Retainer</strong> is created for the amount on the advance or retainer.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-114">शुल्क के लिए नकारात्मक राशि या सही करने के लिए उपयोग में लाए जाने के लिए अग्रिम का वास्तविक बिल बिक्री का प्रकार.</span><span class="sxs-lookup"><span data-stu-id="f65ed-114">An unbilled sales actual of a negative amount of the retainer or advance to be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f65ed-115">किसी इनवॉइस पर शुल्क या अग्रिम के पूरी तरह से सही हो जाने के बाद.</span><span class="sxs-lookup"><span data-stu-id="f65ed-115">After fully reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-116">शुल्क या अग्रिम का वास्तविक बिल बिक्री का उलट जो सही करने के लिए बनाया गया था.</span><span class="sxs-lookup"><span data-stu-id="f65ed-116">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="f65ed-117">यह राशि सकारात्मक है क्योंकि यह उस नकारात्मक को रद्द करने के लिए है जो शुल्क या अग्रिम द्वारा इनवॉइस बनाए जाने पर बनाई गई थी.</span><span class="sxs-lookup"><span data-stu-id="f65ed-117">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-118">इस इनवॉइस पर राशि के लिए वास्तविक बिक्री बिल.</span><span class="sxs-lookup"><span data-stu-id="f65ed-118">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="f65ed-119">किसी इनवॉइस पर आंशिक रूप से एक शुल्क या अग्रिम को सही करने के बाद.</span><span class="sxs-lookup"><span data-stu-id="f65ed-119">After partially reconciling a retainer or advance on an invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-120">शुल्क या अग्रिम का वास्तविक बिल बिक्री का उलट जो सही करने के लिए बनाया गया था.</span><span class="sxs-lookup"><span data-stu-id="f65ed-120">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="f65ed-121">यह राशि सकारात्मक है क्योंकि यह उस नकारात्मक को रद्द करने के लिए है जो शुल्क या अग्रिम द्वारा इनवॉइस बनाए जाने पर बनाई गई थी.</span><span class="sxs-lookup"><span data-stu-id="f65ed-121">This amount is positive as it's meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-122">इस इनवॉइस पर राशि के लिए वास्तविक बिक्री बिल.</span><span class="sxs-lookup"><span data-stu-id="f65ed-122">A billed sales actual for the amount on this invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-123">भविष्य के इनवॉइस पर सामंजस्य स्थापित करने के लिए शेष शुल्क या अग्रिम राशि का नकारात्मक वास्तविक ऋण रहित बिक्री है.</span><span class="sxs-lookup"><span data-stu-id="f65ed-123">A negative unbilled sales actual of the remaining retainer or advance amount to be used for reconciliation on future invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f65ed-124">ड्राफ्ट इनवॉइस पर बिना किसी संपादन/बदलाव के समय लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="f65ed-124">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-125">असल समय अनुमोदन पर घंटे और राशि के लिए एक बिना बिल वाली बिक्री की तबदीली.</span><span class="sxs-lookup"><span data-stu-id="f65ed-125">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-126">असल समय अनुमोदन पर घंटे और राशि के लिए वास्तविक बिल बिक्री.</span><span class="sxs-lookup"><span data-stu-id="f65ed-126">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="f65ed-127">मात्रा को कम करने के लिए संपादित किए/बदले गए समय लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="f65ed-127">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-128">असल समय अनुमोदन पर घंटे और राशि के लिए एक बिना बिल वाली बिक्री की तबदीली.</span><span class="sxs-lookup"><span data-stu-id="f65ed-128">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-129">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर घंटों और राशि के लिए प्रभार्य है, वास्तविक बिना बिल बिक्री के उल्टा और वास्तविक बिल बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="f65ed-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-130">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर सही आंकड़े काटने के बाद शेष घंटों और राशि के लिए प्रभार्य है, वास्तविक बिक्री के उल्टा और वास्तविक बिल बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="f65ed-130">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on edited invoice line detail, a reversal of the sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f65ed-131">मात्रा बढ़ाने के लिए संपादित किए गए एक/ किसी समय के लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="f65ed-131">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-132">असल समय अनुमोदन पर घंटे और राशि के लिए एक बिना बिल वाली बिक्री की तबदीली.</span><span class="sxs-lookup"><span data-stu-id="f65ed-132">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-133">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर घंटों और राशि के लिए प्रभार्य है, बिना बिल वाली वास्तविक बिक्री के उल्टा और बिल वाली वास्तविक बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="f65ed-133">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f65ed-134">ड्राफ्ट इनवॉइस पर बिना किसी संपादन/बदलाव के खर्च के लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="f65ed-134">Invoicing an expense transaction without any edits on draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-135">असल/मूल खर्च अनुमोदन पर मात्रा और राशि के लिए वास्तविक बिना बिल बिक्री.</span><span class="sxs-lookup"><span data-stu-id="f65ed-135">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-136">असल/मूल खर्च अनुमोदन पर मात्रा और राशि के लिए वास्तविक बिल बिक्री</span><span class="sxs-lookup"><span data-stu-id="f65ed-136">A billed sales actual for the quantity and amount on the original expense approval</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="f65ed-137">मात्रा कम करने के लिए संपादित किए गए किसी खर्च के लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="f65ed-137">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-138">असल/मूल खर्च अनुमोदन पर मात्रा और राशि के लिए वास्तविक बिना बिल बिक्री.</span><span class="sxs-lookup"><span data-stu-id="f65ed-138">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-139">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर मात्रा और राशि के लिए प्रभार्य है, बिना बिल वाली वास्तविक बिक्री के उल्टा और वास्तविक बिल वास्तविक बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="f65ed-139">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-140">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर सही आंकड़े काटने के बाद शेष मात्रा और राशि के लिए प्रभार्य है, वास्तविक बिना बिल बिक्री के उल्टा और वास्तविक बिल बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="f65ed-140">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f65ed-141">मात्रा बढ़ाने के लिए संपादित किए गए किसी खर्च के लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="f65ed-141">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-142">असल/मूल खर्च अनुमोदन पर मात्रा और राशि के लिए वास्तविक बिना बिल बिक्री.</span><span class="sxs-lookup"><span data-stu-id="f65ed-142">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-143">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर मात्रा और राशि के लिए प्रभार्य है, वास्तविक बिना बिल बिक्री के उल्टा और वास्तविक बिल बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="f65ed-143">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f65ed-144">ड्राफ्ट इनवॉइस पर बिना किसी संपादन के मटिरियल ट्रांजैक्शन (अधिग्रहण) का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="f65ed-144">Invoicing a material transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-145">ओरिज़िनल मटिरियल के उपयोग के अनुमोदन पर मात्रा और राशि के लिए एक बिना बिल वाली सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="f65ed-145">An unbilled sales reversal for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-146">ओरिज़िनल मटिरियल के उपयोग के अनुमोदन पर मात्रा और राशि के लिए बिल वाले सेल्स एक्चुअल्स.</span><span class="sxs-lookup"><span data-stu-id="f65ed-146">A billed sales actual for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="f65ed-147">मात्रा बढ़ाने के लिए संपादित किए गए मटिरियल ट्रांजैक्शन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="f65ed-147">Invoicing a material transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-148">ओरिज़िनल समय के अनुमोदन पर मात्रा और राशि के लिए एक बिना बिल वाली सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="f65ed-148">An unbilled sales reversal for the quantity and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-149">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर मात्रा और राशि के लिए प्रभार्य है, बिना बिल वाली वास्तविक बिक्री के उल्टा और वास्तविक बिल वास्तविक बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="f65ed-149">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-150">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर सही आंकड़े काटने के बाद शेष मात्रा और राशि के लिए प्रभार्य है, वास्तविक बिना बिल बिक्री के उल्टा और वास्तविक बिल बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="f65ed-150">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f65ed-151">मात्रा बढ़ाने के लिए संपादित किए गए मटिरियल ट्रांजैक्शन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="f65ed-151">Invoicing a material transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-152">ओरिज़िनल मटिरियल के उपयोग के अनुमोदन पर मात्रा और राशि के लिए एक बिना बिल वाली सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="f65ed-152">An unbilled sales reversal for the quantity and amount on the original material usage approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-153">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर मात्रा और राशि के लिए प्रभार्य है, बिना बिल वाली वास्तविक बिक्री के उल्टा और वास्तविक बिल वास्तविक बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="f65ed-153">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="f65ed-154">शुल्क का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="f65ed-154">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-155">असल/मूल बहीखाता पंक्ति पर शुल्क राशि के लिए बिना बिल वाली उलट बिक्री.</span><span class="sxs-lookup"><span data-stu-id="f65ed-155">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-156">असल/मूल बहीखाता पंक्ति पर मात्रा और राशि के लिए वास्तविक बिक्री बिल.</span><span class="sxs-lookup"><span data-stu-id="f65ed-156">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="f65ed-157">किसी/एक माइलस्टोन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="f65ed-157">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-158">परियोजना अनुबंध पंक्ति पर मूल माइलस्टोन पर माइलस्टोन की राशि के लिए वास्तविक बिक्री बिल.</span><span class="sxs-lookup"><span data-stu-id="f65ed-158">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="f65ed-159">उत्पाद-आधारित अनुबंध पंक्ति का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="f65ed-159">Invoicing a product-based contract line.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="f65ed-160">उत्पाद-आधारित अनुबंध पंक्ति से आने वाली मात्रा और राशि के साथ उत्पाद लाइन के लिए वास्तविक बिक्री बिल.</span><span class="sxs-lookup"><span data-stu-id="f65ed-160">A billed sales actual for the product line with the quantity and amount coming from the product-based contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
