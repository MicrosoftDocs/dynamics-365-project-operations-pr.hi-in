---
title: परियोजना-आधारित सुधारात्मक इनवॉइस
description: यह विषय Project Operations में परियोजना-आधारित सुधारात्मक इनवॉइस बनाने और पुष्टि करने के तरीके के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 03/29/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: fc96bb40f5207efc381986d46a3e37dfc1dc111c
ms.sourcegitcommit: ca0fc078d1a12484eca193fe051b8442c0559db8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/07/2021
ms.locfileid: "5867043"
---
# <a name="corrective-project-based-invoices"></a><span data-ttu-id="a76f8-103">परियोजना-आधारित सुधारात्मक इनवॉइस</span><span class="sxs-lookup"><span data-stu-id="a76f8-103">Corrective project-based invoices</span></span>

<span data-ttu-id="a76f8-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="a76f8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="a76f8-105">ग्राहक और प्रोजेक्ट मैनेजर के साथ बातचीत से तय किए गए परिवर्तनों या क्रेडिटों को संसाधित करने के लिए एक पुष्टिकृत प्रोजेक्ट इनवॉइस को ठीक किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="a76f8-105">A confirmed project invoice can be corrected to process changes or credits as negotiated with the customer and project manager.</span></span>

<span data-ttu-id="a76f8-106">किसी पुष्टिकृत इनवॉइस को संपादित करने के लिए पुष्टिकृत इनवॉइस खोलें और **इस इनवॉइस को सही करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="a76f8-106">To make edits to a confirmed invoice, open the confirmed invoice and select **Correct this Invoice**.</span></span> 

> [!NOTE]
> <span data-ttu-id="a76f8-107">यह चयन तब तक उपलब्ध नहीं है जब तक कि किसी परियोजना इनवॉइस की पुष्टि न हो या परियोजना-आधारित इनवॉइस में एडवांस या रिटेनर ना हो या एडवांस या रिटेनर की संगति न हो.</span><span class="sxs-lookup"><span data-stu-id="a76f8-107">This selection isn't available unless a project invoice is confirmed or the project-based invoice has advances or retainers or reconciliations of advances or retainers.</span></span>

<span data-ttu-id="a76f8-108">पुष्टिकृत इनवॉइस से नया ड्राफ्ट इनवॉइस बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="a76f8-108">A new draft invoice is created from the confirmed invoice.</span></span> <span data-ttu-id="a76f8-109">पहले से पुष्टिकृत इनवॉइस से सभी इनवॉइस लाइन विवरण नए ड्राफ्ट में कॉपी किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="a76f8-109">All invoice line details from the previously confirmed invoice are copied to the new draft.</span></span> <span data-ttu-id="a76f8-110">सही किए गए नए इनवॉइस पर लाइन विवरण के बारे में समझने के लिए कुछ प्रमुख बिंदु निम्नलिखित हैं:</span><span class="sxs-lookup"><span data-stu-id="a76f8-110">The following are some of the key points to understand about the line details on the new corrected invoice:</span></span>

- <span data-ttu-id="a76f8-111">सभी मात्रा शून्य के लिए अपडेट किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="a76f8-111">All quantities are updated to zero.</span></span> <span data-ttu-id="a76f8-112">Dynamics 365 Project Operations मानता है कि सभी इनवॉइस किए गए आइटम पूरी तरह से क्रेडिट किए होते हैं.</span><span class="sxs-lookup"><span data-stu-id="a76f8-112">Dynamics 365 Project Operations assumes that all invoiced items are fully credited.</span></span> <span data-ttu-id="a76f8-113">यदि आवश्यक हो, तो आप इन मात्राओं को मैन्युअल रूप से अपडेट कर सकते हैं ताकि इनवॉइस की जा रही मात्रा को दर्शाया जा सके, न कि क्रेडिट की जा रही मात्रा को.</span><span class="sxs-lookup"><span data-stu-id="a76f8-113">If needed, you can manually update these quantities to reflect the quantity that is being invoiced, and not the quantity that is being credited.</span></span> <span data-ttu-id="a76f8-114">आपके द्वारा दर्ज की गई मात्रा के आधार पर, एप्लिकेशन क्रेडिट की गई मात्रा की गणना करता है.</span><span class="sxs-lookup"><span data-stu-id="a76f8-114">Based on the quantity you enter, the application calculates the credited quantity.</span></span> <span data-ttu-id="a76f8-115">यह राशि सही की गई इनवॉइस की पुष्टि होने पर बनने वाले वास्तविक आँकड़ों में दर्शायी जाती है.</span><span class="sxs-lookup"><span data-stu-id="a76f8-115">This amount is reflected in the actuals that are created when the corrected invoice is confirmed.</span></span> <span data-ttu-id="a76f8-116">अगर आप टैक्स की रकम में बदलाव कर रहे हैं तो आपको सही टैक्स की रकम दर्ज करनी चाहिए न कि क्रेडिट की जा रही टैक्स की रकम.</span><span class="sxs-lookup"><span data-stu-id="a76f8-116">If you are making changes to the tax amount, you must enter the correct tax amount and not the tax amount that is being credited.</span></span>
- <span data-ttu-id="a76f8-117">उपलब्धि सुधार हमेशा पूर्ण क्रेडिट के रूप में संसाधित होते हैं.</span><span class="sxs-lookup"><span data-stu-id="a76f8-117">Milestone corrections are always processed as full credits.</span></span>


> [!IMPORTANT]
> <span data-ttu-id="a76f8-118">इनवॉइस लाइन के उन विवरणों के लिए जो पहले से ही इनवॉइस किए गए अन्य शुल्क के लिए सुधार के रूप में हैं, उनमें **सुधार** फ़ील्ड **हां** पर सेट है.</span><span class="sxs-lookup"><span data-stu-id="a76f8-118">For invoice line details that are corrections to other already invoiced charges, the **Correction** field is set to **Yes**.</span></span> <span data-ttu-id="a76f8-119">उन इनवॉइसों के लिए जिनमें सुधार की गई इनवॉइस लाइन के विवरण हैं, **सुधार** फ़ील्ड **हां** पर सेट है.</span><span class="sxs-lookup"><span data-stu-id="a76f8-119">For invoices that have corrected invoice line details, the **Has corrections** field is set to **Yes**.</span></span>

## <a name="actuals-created-when-a-corrective-invoice-is-confirmed"></a><span data-ttu-id="a76f8-120">सुधारात्मक इनवॉइस की पुष्टि होने पर बनाए गए एक्चुअल्स</span><span class="sxs-lookup"><span data-stu-id="a76f8-120">Actuals created when a corrective invoice is confirmed</span></span>

<span data-ttu-id="a76f8-121">निम्नलिखित तालिका में इनवॉइस के सुधार की पुष्टि होने पर बनाए गए एक्चुअल्स को सूचीबद्ध किया गया है.</span><span class="sxs-lookup"><span data-stu-id="a76f8-121">The following table lists the actuals that are created when a corrective invoice is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="216" valign="top">
                <p><span data-ttu-id="a76f8-122">
                    <strong>परिदृश्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a76f8-122">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="808" valign="top">
                <p><span data-ttu-id="a76f8-123">
                    <strong>पुष्टि होने पर बनाए गए वास्तविक</strong>
                </span><span class="sxs-lookup"><span data-stu-id="a76f8-123">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a76f8-124">पहले से इनवॉइस किए गए समय के लेन-देन का पूरा क्रेडिट इनवॉइस करना.</span><span class="sxs-lookup"><span data-stu-id="a76f8-124">Invoicing the full credit of a previously invoiced time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-125">समय के लिए मूल इनवॉइस लाइन विवरण पर घंटे और राशि के लिए बिल की गई सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="a76f8-125">A billed sales reversal for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-126">समय के लिए मूल इनवॉइस लाइन विवरण पर घंटे और राशि के लिए नई बिना बिल वाली सेल्स के वास्तविक आँकड़े.</span><span class="sxs-lookup"><span data-stu-id="a76f8-126">A new unbilled sales actual for the hours and amount on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="a76f8-127">एक समय लेनदेन पर आंशिक क्रेडिट इनवॉइस.</span><span class="sxs-lookup"><span data-stu-id="a76f8-127">Invoicing the partial credit on a time transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-128">समय के लिए मूल इनवॉइस लाइन विवरण पर इनवॉइस किए गए घंटे और राशि के लिए बिल की गई सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="a76f8-128">A billed sales reversal for the hours and amount invoiced on the original invoice line detail for time.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-129">एक नई बिना बिल की गई सेल्स के वास्तविक आँकड़े जो संपादित किए गए इनवॉइस लाइन विवरण पर घंटों और राशि के लिए चार्ज की जाती है, इसके विपरित, और एक समकक्ष बिल की गई सेल्स के वास्तविक आँकड़े.</span><span class="sxs-lookup"><span data-stu-id="a76f8-129">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-130">एक नई बिना बिल की गई सेल्स के वास्तविक आँकड़े जो इनवॉइस लाइन विवरण पर सही किए गए आंकड़ों को छांटने के बाद शेष घंटों और राशि के लिए चार्ज करने योग्य है.</span><span class="sxs-lookup"><span data-stu-id="a76f8-130">A new unbilled sales actual that is chargeable for the remaining hours and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a76f8-131">पहले से इनवॉइस किए गए ख़र्च लेनदेन का पूरा क्रेडिट इनवॉइस करना.</span><span class="sxs-lookup"><span data-stu-id="a76f8-131">Invoicing the full credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-132">ख़र्च के लिए मूल इनवॉइस लाइन विवरण पर मात्रा और राशि के लिए बिल की गई सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="a76f8-132">A billed sales reversal for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-133">खर्च के लिए मूल इनवॉइस लाइन विवरण पर मात्रा और राशि के लिए एक नई बिना बिल वाली सेल्स के वास्तविक आँकड़ें.</span><span class="sxs-lookup"><span data-stu-id="a76f8-133">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="a76f8-134">पहले से इनवॉइस किए गए ख़र्च लेनदेन का आंशिक क्रेडिट इनवॉइस करना.</span><span class="sxs-lookup"><span data-stu-id="a76f8-134">Invoicing the partial credit of a previously invoiced expense transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-135">एक खर्च के लिए मूल इनवॉइस लाइन विवरण पर इनवॉइस की गई मात्रा और राशि के लिए बिल की गई सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="a76f8-135">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for an expense.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-136">एक नई बिना बिल वाली सेल्स के वास्तविक आँकड़ें जो सही इनवॉइस लाइन विवरण पर मात्रा और राशि के लिए चार्ज की जाती है, इसके विपरित, और एक समकक्ष बिल की गई सेल्स के वास्तविक आँकड़े.</span><span class="sxs-lookup"><span data-stu-id="a76f8-136">A new unbilled sales actual that is chargeable for the quantity and amount on the corrected invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-137">एक नई बिना बिल वाली सेल्स के वास्तविक आँकड़े जो इनवॉइस लाइन विवरण पर सही किए गए आंकड़ों को छांटने के बाद शेष मात्रा और राशि के लिए चार्ज की जाती है.</span><span class="sxs-lookup"><span data-stu-id="a76f8-137">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
                <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a76f8-138">पहले से इनवॉइस किए गए मटिरियल ट्रांजैक्शन के पूरे क्रेडिट का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="a76f8-138">Invoicing the full credit of a previously invoiced material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-139">मटिरियल के लिए ओरिज़िनल इनवॉइस लाइन के विवरण पर मात्रा और राशि के लिए बिना बिल वाली सेल्स एक्चुअल्स.</span><span class="sxs-lookup"><span data-stu-id="a76f8-139">A billed sales reversal for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-140">मटिरियल के लिए ओरिज़िनल इनवॉइस लाइन के विवरण पर मात्रा और राशि के लिए बिना बिल वाली सेल्स एक्चुअल्स.</span><span class="sxs-lookup"><span data-stu-id="a76f8-140">A new unbilled sales actual for the quantity and amount on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="a76f8-141">किसी मटिरियल ट्रांजैक्शन पर आंशिक ऋण का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="a76f8-141">Invoicing the partial credit on a material transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-142">मटिरियल के लिए ओरिज़िनल इनवॉइस लाइन के विवरण पर इनवॉइस की गई मात्रा और राशि के लिए बिल वाली सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="a76f8-142">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for material.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-143">बिना बिल वाले नए सेल्स एक्चुअल्स जो संपादित किए गए इनवॉइस लाइन के विवरण पर, इसकी रिवर्सल पर और बिल की गई समकक्ष सेल्स एक्चुअल्स पर मात्रा और राशि के लिए चार्जेबल हैं.</span><span class="sxs-lookup"><span data-stu-id="a76f8-143">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-144">एक नई बिना बिल वाली सेल्स के वास्तविक आँकड़े जो इनवॉइस लाइन विवरण पर सही किए गए आंकड़ों को छांटने के बाद शेष मात्रा और राशि के लिए चार्ज की जाती है.</span><span class="sxs-lookup"><span data-stu-id="a76f8-144">A new unbilled sales actual that is chargeable for the remaining quantity and amount after deducting the corrected figures on the invoice line detail.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a76f8-145">पहले से इनवॉइस किए गए शुल्क लेनदेन का पूरा क्रेडिट इनवॉइस करना.</span><span class="sxs-lookup"><span data-stu-id="a76f8-145">Invoicing the full credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-146">शुल्क के लिए मूल इनवॉइस लाइन विवरण पर मात्रा और राशि के लिए एक बिल की गई सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="a76f8-146">A billed sales reversal for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-147">शुल्क के लिए मूल इनवॉइस लाइन विवरण पर मात्रा और राशि के लिए एक नई बिना बिल वाली सेल्स के वास्तविक आँकड़े.</span><span class="sxs-lookup"><span data-stu-id="a76f8-147">A new unbilled sales actual for the quantity and amount on the original invoice line detail for the fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="a76f8-148">पहले से इनवॉइस किए गए शुल्क लेनदेन का आंशिक क्रेडिट इनवॉइस करना.</span><span class="sxs-lookup"><span data-stu-id="a76f8-148">Invoicing the partial credit of a previously invoiced fee transaction.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-149">शुल्क के लिए मूल इनवॉइस लाइन विवरण पर इनवॉइस की गई मात्रा और राशि के लिए एक बिल की गई सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="a76f8-149">A billed sales reversal for the quantity and amount invoiced on the original invoice line detail for fee.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-150">एक नई बिना बिल की गई सेल्स के वास्तविक आँकड़े जो संपादित किए गए सुधार योग्य इनवॉइस लाइन विवरण पर मात्रा और राशि के लिए चार्ज की जाती है, इसके विपरित, और एक समकक्ष बिल की गई सेल्स के वास्तविक आँकड़े.</span><span class="sxs-lookup"><span data-stu-id="a76f8-150">A new unbilled sales actual that is chargeable for the quantity and amount on the edited corrective invoice line detail, a reversal of this, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="a76f8-151">पहले से इनवॉइस किए गए उपलब्धि का पूरा क्रेडिट इनवॉइस करना.</span><span class="sxs-lookup"><span data-stu-id="a76f8-151">Invoicing the full credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-152">उपलब्धि के लिए मूल इनवॉइस लाइन विवरण पर राशि के लिए एक बिल की गई सेल्स रिवर्सल.</span><span class="sxs-lookup"><span data-stu-id="a76f8-152">A billed sales reversal for the amount on the original invoice line detail for the milestone.</span></span>
                </p>
                <p>
<span data-ttu-id="a76f8-153">उपलब्धि के इनवॉइस की स्थिति, <b>ग्राहक के इनवॉइस</b> से अपडेट की जाती है जो <b>रेडी टू इनवॉइस</b> पर पोस्ट किया गया है.</span><span class="sxs-lookup"><span data-stu-id="a76f8-153">The invoice status of the milestone is updated from <b>Customer Invoice Posted</b> to <b>Ready to Invoice</b>.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="a76f8-154">पहले से इनवॉइस किए गए उपलब्धि के आंशिक क्रेडिट का इनवॉइस करना.</span><span class="sxs-lookup"><span data-stu-id="a76f8-154">Invoicing the partial credit of a previously invoiced milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="a76f8-155">यह परिदृश्य समर्थित नहीं है.</span><span class="sxs-lookup"><span data-stu-id="a76f8-155">This scenario isn't supported.</span></span>
                </p>
            </td>
        </tr>       
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
