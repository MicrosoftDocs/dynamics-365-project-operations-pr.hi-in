---
title: एक प्रोफ़ॉर्मा इनवॉइस की पुष्टि करें
description: यह विषय प्रोफॉर्मा इनवॉइस की पुष्टि की जानकारी देता है.
author: rumant
manager: AnnBe
ms.date: 10/13/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b2ed241509d2643d841ce55777e6e316612f70b8
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287870"
---
# <a name="confirm-a-proforma-invoice"></a><span data-ttu-id="4bbcf-103">एक प्रोफ़ॉर्मा इनवॉइस की पुष्टि करें</span><span class="sxs-lookup"><span data-stu-id="4bbcf-103">Confirm a proforma invoice</span></span>

<span data-ttu-id="4bbcf-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="4bbcf-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="4bbcf-105">प्रोफोर्मा इनवॉइस की पुष्टि के बाद परियोजना इनवॉइस की स्थिति **पुष्ट हुआ** में अपडेट हो जाएगी.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="4bbcf-106">जब एक इनवॉइस की पुष्टि होती है, तो यह केवल पढ़ने के लायक ही रहता है.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="4bbcf-107">आगे जाने पर, इनवॉइस को तभी सही किया जा सकता है, जब कोई ग्राहक सुधार या क्रेडिट की शुरुआत करता है, या जब इसे भुगतान हुआ के रूप में चिह्नित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, or when it's marked as paid.</span></span>

<span data-ttu-id="4bbcf-108">निम्नलिखित तालिका सिस्टम द्वारा निर्मित वास्तविक को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="4bbcf-109">इन वास्तविक को तभी बनाया गया है जब ड्राफ़्ट परियोजना इनवॉइस की पुष्टि से पहले कुछ संचालनों को प्रदर्शित किया गया था.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="416" valign="top">
                <p><span data-ttu-id="4bbcf-110">
                    <strong>परिदृश्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4bbcf-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="608" valign="top">
                <p><span data-ttu-id="4bbcf-111">
                    <strong>पुष्टि होने पर बनाए गए वास्तविक</strong>
                </span><span class="sxs-lookup"><span data-stu-id="4bbcf-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4bbcf-112">ड्राफ्ट इनवॉइस पर बिना किसी संपादन/बदलाव के समय लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-112">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-113">असल समय अनुमोदन पर घंटे और राशि के लिए एक बिना बिल वाली बिक्री की तबदीली.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-113">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-114">असल समय अनुमोदन पर घंटे और राशि के लिए वास्तविक बिल बिक्री.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-114">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="4bbcf-115">मात्रा को कम करने के लिए संपादित किए/बदले गए समय लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-115">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-116">असल समय अनुमोदन पर घंटे और राशि के लिए एक बिना बिल वाली बिक्री की तबदीली.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-116">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-117">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर घंटों और राशि के लिए प्रभार्य है, बिना बिल वाली वास्तविक बिक्री के उल्टा और बिल वाली वास्तविक बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-117">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-118">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर सही आंकड़े काटने के बाद बचे हुए घंटों और राशि के लिए प्रभार्य है, वास्तविक बिना बिल बिक्री के उल्टा और वास्तविक बिल बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-118">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4bbcf-119">मात्रा बढ़ाने के लिए संपादित किए गए एक/ किसी समय के लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-119">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-120">असल समय अनुमोदन पर घंटे और राशि के लिए एक बिना बिल वाली बिक्री की तबदीली.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-120">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-121">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर घंटों और राशि के लिए प्रभार्य है, बिना बिल वाली वास्तविक बिक्री के उल्टा और बिल वाली वास्तविक बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-121">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4bbcf-122">ड्राफ़्ट इनवॉइस पर बिना किसी संपादन के किसी खर्च के लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-122">Invoicing an expense transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-123">असल/मूल खर्च अनुमोदन पर मात्रा और राशि के लिए वास्तविक बिना बिल बिक्री.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-123">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-124">असल/मूल खर्च अनुमोदन पर मात्रा और राशि के लिए वास्तविक बिल बिक्री.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-124">A billed sales actual for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="4bbcf-125">मात्रा कम करने के लिए संपादित किए गए किसी खर्च के लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-125">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-126">असल/मूल खर्च अनुमोदन पर मात्रा और राशि के लिए वास्तविक बिना बिल बिक्री.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-126">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-127">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर मात्रा और राशि के लिए प्रभार्य है, बिना बिल वाली वास्तविक बिक्री के उल्टा और वास्तविक बिल वास्तविक बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-127">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-128">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर सही आंकड़े काटने के बाद बची हुई मात्रा और राशि के लिए गैर-प्रभार्य है, वास्तविक बिना बिल बिक्री के उल्टा और वास्तविक बिल बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-128">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent of the billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4bbcf-129">मात्रा बढ़ाने के लिए संपादित किए गए किसी खर्च के लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-129">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-130">असल/मूल खर्च अनुमोदन पर मात्रा और राशि के लिए वास्तविक बिना बिल बिक्री.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-130">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-131">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर मात्रा और राशि के लिए प्रभार्य है, वास्तविक बिना बिल बिक्री के उल्टा और वास्तविक बिल बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-131">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the untilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="4bbcf-132">शुल्क का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-132">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-133">असल/मूल बहीखाता पंक्ति पर शुल्क राशि के लिए बिना बिल वाली उलट बिक्री.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-133">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-134">असल/मूल बहीखाता पंक्ति पर मात्रा और राशि के लिए वास्तविक बिक्री बिल.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-134">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="4bbcf-135">किसी/एक माइलस्टोन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-135">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="4bbcf-136">परियोजना अनुबंध पंक्ति पर मूल माइलस्टोन पर माइलस्टोन की राशि के लिए वास्तविक बिक्री बिल.</span><span class="sxs-lookup"><span data-stu-id="4bbcf-136">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../includes/footer-banner.md)]