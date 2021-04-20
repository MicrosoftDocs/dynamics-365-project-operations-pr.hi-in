---
title: सुधारात्मक परियोजना-आधारित इनवॉइस बनाएँ
description: यह विषय Project Operations में इनवॉइस के सुधार के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 03/29/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 32772d64b3fc77f0af9618edff40e3b295593454
ms.sourcegitcommit: 504c09365bf404c1f1aa9b5034c1e1e5bc9d0d54
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/31/2021
ms.locfileid: "5788862"
---
# <a name="create-corrective-project-based-invoices"></a><span data-ttu-id="20e5d-103">सुधारात्मक परियोजना-आधारित इनवॉइस बनाएँ</span><span class="sxs-lookup"><span data-stu-id="20e5d-103">Create corrective project-based invoices</span></span> 

<span data-ttu-id="20e5d-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="20e5d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="20e5d-105">ग्राहक और प्रोजेक्ट मैनेजर के साथ बातचीत से तय किए गए परिवर्तनों या क्रेडिटों को संसाधित करने के लिए एक पुष्टिकृत प्रोजेक्ट इनवॉइस को ठीक किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="20e5d-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="20e5d-106">किसी पुष्टिकृत इनवॉइस को संपादित करने के लिए पुष्टिकृत इनवॉइस खोलें और **इस इनवॉइस को सही करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="20e5d-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="20e5d-107">यह चयन तब तक उपलब्ध नहीं है जब तक कि किसी प्रोजेक्ट इनवॉइस की पुष्टि न हो जाए.</span><span class="sxs-lookup"><span data-stu-id="20e5d-107">This selection isn't available unless a project invoice is confirmed.</span></span>

<span data-ttu-id="20e5d-108">पुष्टिकृत इनवॉइस से नया ड्राफ्ट इनवॉइस बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="20e5d-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="20e5d-109">पहले से पुष्टिकृत इनवॉइस से सभी इनवॉइस लाइन विवरण नए ड्राफ्ट में कॉपी किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="20e5d-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="20e5d-110">नए सुधारे गए इनवॉइस लाइन के बारे में अधिक समझने में आपकी मदद करने के लिए कुछ महत्वपूर्ण बिंदु निम्नलिखित हैं:</span><span class="sxs-lookup"><span data-stu-id="20e5d-110">The following are some key points to help you understand more about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="20e5d-111">सभी मात्रा शून्य के लिए अपडेट किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="20e5d-111">All quantities are updated to zero.</span></span> <span data-ttu-id="20e5d-112">यह माना जाता है कि इनवॉइस किए गए सभी आइटम पूरी तरह से क्रेडिट किए होते हैं.</span><span class="sxs-lookup"><span data-stu-id="20e5d-112">This assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="20e5d-113">यदि आवश्यक हो, तो आप इन मात्राओं को मैन्युअल रूप से अपडेट कर सकते हैं ताकि इनवॉइस की जा रही मात्रा को दर्शाया जा सके, न कि क्रेडिट की जा रही मात्रा को.</span><span class="sxs-lookup"><span data-stu-id="20e5d-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="20e5d-114">आपके द्वारा दर्ज की गई मात्रा के आधार पर, एप्लिकेशन क्रेडिट की गई मात्रा की गणना करता है.</span><span class="sxs-lookup"><span data-stu-id="20e5d-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="20e5d-115">यह राशि सही की गई इनवॉइस की पुष्टि होने पर बनने वाले वास्तविक आँकड़ों में दर्शायी जाती है.</span><span class="sxs-lookup"><span data-stu-id="20e5d-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="20e5d-116">अगर आप टैक्स की रकम में बदलाव कर रहे हैं तो आपको सही टैक्स की रकम दर्ज करनी चाहिए न कि क्रेडिट की जा रही टैक्स की रकम.</span><span class="sxs-lookup"><span data-stu-id="20e5d-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="20e5d-117">उपलब्धि सुधार हमेशा पूर्ण क्रेडिट के रूप में संसाधित होते हैं.</span><span class="sxs-lookup"><span data-stu-id="20e5d-117">Milestone corrections are always processed as full credits.</span></span>
- <span data-ttu-id="20e5d-118">यदि ग्राहक को गलत राशि के लिए इनवॉइस दिया गया था तो रिटेनर या अग्रिम राशि को ठीक किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="20e5d-118">Retainer or advance amounts can be corrected if the customer was invoiced for an incorrect amount.</span></span>
- <span data-ttu-id="20e5d-119">यदि पहले से पुष्टि किए गए इनवॉइस पर शुल्कों के प्रति मिलान करने के लिए गलत राशि का उपयोग किया गया था तो रिटेनरों और अग्रिमों के मिलान को ठीक किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="20e5d-119">Reconciliations of retainers and advances can be corrected if an incorrect amount was used to reconcile against the charges on a previously confirmed invoice.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="20e5d-120">इनवॉइस लाइन के विवरण जो पहले से ही इनवॉइस किए गए शुल्कों में सुधार के रूप में हैं, उनमें **सुधार** फ़ील्ड **हां** पर सेट होता है.</span><span class="sxs-lookup"><span data-stu-id="20e5d-120">Invoice line details that are corrections to other already invoiced charges have the **Correction** field set to **Yes**.</span></span> <span data-ttu-id="20e5d-121">उन इनवॉइसों में जिनमें सही किए गए इनवॉइस लाइन विवरण होते हैं, उनमें **सुधार है** नामक एक फ़ील्ड होता है जो **हाँ** के लिए सेट भी होता है.</span><span class="sxs-lookup"><span data-stu-id="20e5d-121">Invoices that have corrected invoice line details have a field called **Has corrections** that is also set to **Yes**.</span></span>

## <a name="actuals-created-on-confirmation-of-a-corrective-invoice"></a><span data-ttu-id="20e5d-122">सुधार करने योग्य इनवॉइस की पुष्टि पर बनाए गए वास्तविक आँकड़ें</span><span class="sxs-lookup"><span data-stu-id="20e5d-122">Actuals created on confirmation of a corrective invoice</span></span>

<span data-ttu-id="20e5d-123">निम्नलिखित तालिका में इनवॉइस के सुधार की पुष्टि होने पर बनाए गए एक्चुअल्स को सूचीबद्ध किया गया है.</span><span class="sxs-lookup"><span data-stu-id="20e5d-123">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="20e5d-124">
                    <strong>परिदृश्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="20e5d-124">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="20e5d-125">
                    <strong>पुष्टि होने पर बनाए गए वास्तविक</strong>
                </span><span class="sxs-lookup"><span data-stu-id="20e5d-125">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="20e5d-126">इनवॉइस किए गए अग्रिम या रिटेनर के सुधार की पुष्टि करें.<strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="20e5d-126">Confirm the correction of an invoiced advance or retainer.<strong></strong>
                </span></span></p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-127">शुल्क या अग्रिम का वास्तविक बिल बिक्री का उलट जो सही करने के लिए बनाया गया था.</span><span class="sxs-lookup"><span data-stu-id="20e5d-127">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="20e5d-128">यह राशि सकारात्मक है क्योंकि यह उस नकारात्मक को रद्द करने के लिए है जो रिटेनर या अग्रिम को इनवॉइस किए जाने पर बनाया गया था.</span><span class="sxs-lookup"><span data-stu-id="20e5d-128">This amount is positive because it is meant to cancel out the negative that was created when the retainer or advance was invoiced.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-129">एक बिल की गई सेल्स रिवर्सल के वास्तविक आँकड़ों को रिटेनर या अग्रिम पर उपलब्ध राशि के लिए बिल की गई मूल सेल्स को रिवर्स करने के लिए बनाया गया है.</span><span class="sxs-lookup"><span data-stu-id="20e5d-129">A billed sales reversal actual is created for the amount on the retainer or advance to reverse the original billed sales.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-130">रिटेनर या अग्रिम-आधारित सही की गई इनवॉइस लाइन पर सही की गई राशि के लिए नई बिल की गई सेल्स के वास्तविक आँकड़े उत्पन्न किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="20e5d-130">A new billed sales actual is created for the corrected amount on the retainer or advance-based corrected invoice line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-131">रिटेनर या अग्रिम-आधारित सही की गई इनवॉइस लाइन के नकारात्मक राशि की बिना बिल की गई सेल्स के वास्तविक आँकड़े, जिनका उपयोग मिलान के लिए किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="20e5d-131">An unbilled sales actual of negative amount of the retainer or advance-based corrected invoice line, which will be used for reconciliation.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="4" valign="top">
                <p>
<span data-ttu-id="20e5d-132">पहले से मिलान किए गए रिटेनर या अग्रिम के सुधार की पुष्टि.</span><span class="sxs-lookup"><span data-stu-id="20e5d-132">A confirmation of the correction of a previously reconciled retainer or advance.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-133">शुल्क या अग्रिम का वास्तविक बिल बिक्री का उलट जो सही करने के लिए बनाया गया था.</span><span class="sxs-lookup"><span data-stu-id="20e5d-133">An unbilled sales reversal of the retainer or advance that was created for reconciliation.</span></span> <span data-ttu-id="20e5d-134">यह राशि सकारात्मक है और पिछला मिलान होने पर बनाए गए नकारात्मक को रद्द करने के लिए होती है.</span><span class="sxs-lookup"><span data-stu-id="20e5d-134">This amount is positive and is meant to cancel out the negative that was created when the previous reconciliation occurred.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-135">पिछले इनवॉइस पर राशि के लिए बिल की गई सेल्स रिवर्सल के वास्तविक आँकड़े.</span><span class="sxs-lookup"><span data-stu-id="20e5d-135">A billed sales reversal actual for the amount on the previous invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-136">सही किए गए रिटेनर राशि के लिए नई बिल की गई सेल्स के वास्तविक आँकड़े जो सही की गई इनवॉइस पर लागू होती है.</span><span class="sxs-lookup"><span data-stu-id="20e5d-136">A new billed sales actual for the corrected retainer amount that is applied on the corrected invoice.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-137">सही बचे हुए रिटेनर या अग्रिम से नकारात्मक राशि के साथ बिना बिल की गई सेल्स के वास्तविक आँकड़े, जिसका उपयोग बाद के इनवॉइसों पर मिलान के लिए किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="20e5d-137">An unbilled sales actual with a negative amount from the corrected leftover retainer or advance, which will be used for reconciliation on later invoices.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="20e5d-138">पहले से इनवॉइस किए गए समय के लेन-देन का पूरा क्रेडिट इनवॉइस करना.</span><span class="sxs-lookup"><span data-stu-id="20e5d-138">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-139">समय के लिए मूल इनवॉइस लाइन विवरण पर घंटे और राशि के लिए बिल की गई सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="20e5d-139">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-140">समय के लिए मूल इनवॉइस लाइन विवरण पर घंटे और राशि के लिए नई बिना बिल वाली सेल्स के वास्तविक आँकड़े.</span><span class="sxs-lookup"><span data-stu-id="20e5d-140">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="20e5d-141">एक समय लेनदेन पर आंशिक क्रेडिट इनवॉइस.</span><span class="sxs-lookup"><span data-stu-id="20e5d-141">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-142">समय के लिए मूल इनवॉइस लाइन विवरण पर इनवॉइस किए गए घंटे और राशि के लिए बिल की गई सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="20e5d-142">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-143">एक नई बिना बिल की गई सेल्स के वास्तविक आँकड़े जो संपादित किए गए इनवॉइस लाइन विवरण पर घंटों और राशि के लिए चार्ज की जाती है, इसके विपरित, और एक समकक्ष बिल की गई सेल्स के वास्तविक आँकड़े.</span><span class="sxs-lookup"><span data-stu-id="20e5d-143">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-144">एक नई बिना बिल की गई सेल्स के वास्तविक आँकड़े जो इनवॉइस लाइन विवरण पर सही किए गए आंकड़ों को छांटने के बाद शेष घंटों और राशि के लिए चार्ज करने योग्य है.</span><span class="sxs-lookup"><span data-stu-id="20e5d-144">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="20e5d-145">पहले से इनवॉइस किए गए ख़र्च लेनदेन का पूरा क्रेडिट इनवॉइस करना.</span><span class="sxs-lookup"><span data-stu-id="20e5d-145">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-146">ख़र्च के लिए मूल इनवॉइस लाइन विवरण पर मात्रा और राशि के लिए बिल की गई सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="20e5d-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-147">खर्च के लिए मूल इनवॉइस लाइन विवरण पर मात्रा और राशि के लिए एक नई बिना बिल वाली सेल्स के वास्तविक आँकड़ें.</span><span class="sxs-lookup"><span data-stu-id="20e5d-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="20e5d-148">पहले से इनवॉइस किए गए ख़र्च लेनदेन का आंशिक क्रेडिट इनवॉइस करना.</span><span class="sxs-lookup"><span data-stu-id="20e5d-148">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-149">एक खर्च के लिए मूल इनवॉइस लाइन विवरण पर इनवॉइस की गई मात्रा और राशि के लिए बिल की गई सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="20e5d-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-150">एक नई बिना बिल वाली सेल्स के वास्तविक आँकड़ें जो सही इनवॉइस लाइन विवरण पर मात्रा और राशि के लिए चार्ज की जाती है, इसके विपरित, और एक समकक्ष बिल की गई सेल्स के वास्तविक आँकड़े.</span><span class="sxs-lookup"><span data-stu-id="20e5d-150">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-151">एक नई बिना बिल वाली सेल्स के वास्तविक आँकड़े जो इनवॉइस लाइन विवरण पर सही किए गए आंकड़ों को छांटने के बाद शेष मात्रा और राशि के लिए चार्ज की जाती है.</span><span class="sxs-lookup"><span data-stu-id="20e5d-151">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="20e5d-152">पहले से इनवॉइस किए गए शुल्क लेनदेन का पूरा क्रेडिट इनवॉइस करना.</span><span class="sxs-lookup"><span data-stu-id="20e5d-152">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-153">शुल्क के लिए मूल इनवॉइस लाइन विवरण पर मात्रा और राशि के लिए एक बिल की गई सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="20e5d-153">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-154">शुल्क के लिए मूल इनवॉइस लाइन विवरण पर मात्रा और राशि के लिए एक नई बिना बिल वाली सेल्स के वास्तविक आँकड़े.</span><span class="sxs-lookup"><span data-stu-id="20e5d-154">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="20e5d-155">पहले से इनवॉइस किए गए शुल्क लेनदेन का आंशिक क्रेडिट इनवॉइस करना.</span><span class="sxs-lookup"><span data-stu-id="20e5d-155">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-156">शुल्क के लिए मूल इनवॉइस लाइन विवरण पर इनवॉइस की गई मात्रा और राशि के लिए एक बिल की गई सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="20e5d-156">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-157">एक नई बिना बिल की गई सेल्स के वास्तविक आँकड़े जो संपादित किए गए सुधार योग्य इनवॉइस लाइन विवरण पर मात्रा और राशि के लिए चार्ज की जाती है, इसके विपरित, और एक समकक्ष बिल की गई सेल्स के वास्तविक आँकड़े.</span><span class="sxs-lookup"><span data-stu-id="20e5d-157">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="20e5d-158">पहले से इनवॉइस किए गए उपलब्धि का पूरा क्रेडिट इनवॉइस करना.</span><span class="sxs-lookup"><span data-stu-id="20e5d-158">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-159">उपलब्धि के लिए मूल इनवॉइस लाइन विवरण पर राशि के लिए एक बिल की गई सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="20e5d-159">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="20e5d-160">उपलब्धि पर इनवॉइस की स्थिति <b>ग्राहक के इनवॉइस</b> से अपडेट की जाती है जो <b>रेडी टू इनवॉइस</b> पर पोस्ट किया गया है.</span><span class="sxs-lookup"><span data-stu-id="20e5d-160">The invoice status on the milestone is updated from <b>Customer invoice posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="20e5d-161">पहले से इनवॉइस किए गए उपलब्धि के आंशिक क्रेडिट का इनवॉइस करना.</span><span class="sxs-lookup"><span data-stu-id="20e5d-161">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="20e5d-162">असमर्थित</span><span class="sxs-lookup"><span data-stu-id="20e5d-162">Unsupported</span></span> </p>
            </td>
        </tr>        
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
