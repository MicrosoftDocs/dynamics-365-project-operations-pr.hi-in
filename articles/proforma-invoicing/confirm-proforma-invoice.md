---
title: एक प्रोफ़ॉर्मा इनवॉइस की पुष्टि करें
description: यह विषय प्रोफॉर्मा इनवॉइस की पुष्टि की जानकारी देता है.
author: rumant
manager: AnnBe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 560bb68cba865a6af60504114126ae6ea73dde2d
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077545"
---
# <a name="confirm-a-proforma-invoice"></a><span data-ttu-id="881d4-103">एक प्रोफ़ॉर्मा इनवॉइस की पुष्टि करें</span><span class="sxs-lookup"><span data-stu-id="881d4-103">Confirm a proforma invoice</span></span>

<span data-ttu-id="881d4-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="881d4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="881d4-105">प्रोफोर्मा इनवॉइस की पुष्टि के बाद परियोजना इनवॉइस की स्थिति **पुष्ट हुआ** में अपडेट हो जाएगी.</span><span class="sxs-lookup"><span data-stu-id="881d4-105">After a proforma invoice is confirmed, the status of the project invoice updates to **Confirmed**.</span></span> <span data-ttu-id="881d4-106">जब एक इनवॉइस की पुष्टि होती है, तो यह केवल पढ़ने के लायक ही रहता है.</span><span class="sxs-lookup"><span data-stu-id="881d4-106">When an invoice is confirmed, it becomes read-only.</span></span> <span data-ttu-id="881d4-107">आगे जाने पर, इनवॉइस को तभी सही किया जा सकता है, जब कोई ग्राहक सुधार या क्रेडिट की शुरुआत करता है, या जब इसे भुगतान हुआ के रूप में चिह्नित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="881d4-107">Going forward, the invoice can only be corrected if there are any customer-initiated corrections or credits, or when it's marked as paid.</span></span>

<span data-ttu-id="881d4-108">निम्नलिखित तालिका सिस्टम द्वारा निर्मित वास्तविक को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="881d4-108">The following table lists the actuals created by the system.</span></span> <span data-ttu-id="881d4-109">इन वास्तविक को तभी बनाया गया है जब ड्राफ़्ट परियोजना इनवॉइस की पुष्टि से पहले कुछ संचालनों को प्रदर्शित किया गया था.</span><span class="sxs-lookup"><span data-stu-id="881d4-109">These actuals are created when certain operations are performed on the draft project invoice before it is confirmed.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="416" valign="top">
                <p><span data-ttu-id="881d4-110">
                    <strong>परिदृश्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="881d4-110">
                    <strong>Scenario</strong>
                </span></span></p>
            </td>
            <td width="608" valign="top">
                <p><span data-ttu-id="881d4-111">
                    <strong>पुष्टि होने पर बनाए गए वास्तविक</strong>
                </span><span class="sxs-lookup"><span data-stu-id="881d4-111">
                    <strong>Actuals created on confirmation</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="881d4-112">ड्राफ्ट इनवॉइस पर बिना किसी संपादन/बदलाव के समय लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="881d4-112">Invoicing a time transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-113">असल समय अनुमोदन पर घंटे और राशि के लिए एक बिना बिल वाली बिक्री की तबदीली.</span><span class="sxs-lookup"><span data-stu-id="881d4-113">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-114">असल समय अनुमोदन पर घंटे और राशि के लिए वास्तविक बिल बिक्री.</span><span class="sxs-lookup"><span data-stu-id="881d4-114">A billed sales actual for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="881d4-115">मात्रा को कम करने के लिए संपादित किए/बदले गए समय लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="881d4-115">Invoicing a time transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-116">असल समय अनुमोदन पर घंटे और राशि के लिए एक बिना बिल वाली बिक्री की तबदीली.</span><span class="sxs-lookup"><span data-stu-id="881d4-116">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-117">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर घंटों और राशि के लिए प्रभार्य है, बिना बिल वाली वास्तविक बिक्री के उल्टा और बिल वाली वास्तविक बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="881d4-117">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-118">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर सही आंकड़े काटने के बाद बचे हुए घंटों और राशि के लिए प्रभार्य है, वास्तविक बिना बिल बिक्री के उल्टा और वास्तविक बिल बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="881d4-118">A new unbilled sales actual that is non-chargeable for the remaining hours and amount after deducting the corrected figures on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="881d4-119">मात्रा बढ़ाने के लिए संपादित किए गए एक/ किसी समय के लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="881d4-119">Invoicing a time transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-120">असल समय अनुमोदन पर घंटे और राशि के लिए एक बिना बिल वाली बिक्री की तबदीली.</span><span class="sxs-lookup"><span data-stu-id="881d4-120">An unbilled sales reversal for the hours and amount on the original time approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-121">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर घंटों और राशि के लिए प्रभार्य है, बिना बिल वाली वास्तविक बिक्री के उल्टा और बिल वाली वास्तविक बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="881d4-121">A new unbilled sales actual that is chargeable for the hours and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="881d4-122">ड्राफ़्ट इनवॉइस पर बिना किसी संपादन के किसी खर्च के लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="881d4-122">Invoicing an expense transaction without any edits on the draft invoice.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-123">असल/मूल खर्च अनुमोदन पर मात्रा और राशि के लिए वास्तविक बिना बिल बिक्री.</span><span class="sxs-lookup"><span data-stu-id="881d4-123">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-124">असल/मूल खर्च अनुमोदन पर मात्रा और राशि के लिए वास्तविक बिल बिक्री.</span><span class="sxs-lookup"><span data-stu-id="881d4-124">A billed sales actual for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="3" valign="top">
                <p>
<span data-ttu-id="881d4-125">मात्रा कम करने के लिए संपादित किए गए किसी खर्च के लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="881d4-125">Invoicing an expense transaction that was edited to reduce the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-126">असल/मूल खर्च अनुमोदन पर मात्रा और राशि के लिए वास्तविक बिना बिल बिक्री.</span><span class="sxs-lookup"><span data-stu-id="881d4-126">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-127">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर मात्रा और राशि के लिए प्रभार्य है, बिना बिल वाली वास्तविक बिक्री के उल्टा और वास्तविक बिल वास्तविक बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="881d4-127">A new unbilled sales actual that is chargeable for the quantity and amount on the edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent billed sales actual.</span></span> 
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-128">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर सही आंकड़े काटने के बाद बची हुई मात्रा और राशि के लिए गैर-प्रभार्य है, वास्तविक बिना बिल बिक्री के उल्टा और वास्तविक बिल बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="881d4-128">A new unbilled sales actual that is non-chargeable for the remaining quantity and amount after deducting the corrected figures on edited invoice line detail, a reversal of the unbilled sales actual, and an equivalent of the billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="881d4-129">मात्रा बढ़ाने के लिए संपादित किए गए किसी खर्च के लेनदेन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="881d4-129">Invoicing an expense transaction that was edited to increase the quantity.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-130">असल/मूल खर्च अनुमोदन पर मात्रा और राशि के लिए वास्तविक बिना बिल बिक्री.</span><span class="sxs-lookup"><span data-stu-id="881d4-130">An unbilled sales reversal for the quantity and amount on the original expense approval.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-131">एक नई वास्तविक बिना बिल बिक्री जो संपादित इनवॉइस पंक्ति विवरण पर मात्रा और राशि के लिए प्रभार्य है, वास्तविक बिना बिल बिक्री के उल्टा और वास्तविक बिल बिक्री के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="881d4-131">A new unbilled sales actual that is chargeable for quantity and amount on the edited invoice line detail, a reversal of the untilled sales actual, and an equivalent billed sales actual.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" rowspan="2" valign="top">
                <p>
<span data-ttu-id="881d4-132">शुल्क का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="881d4-132">Invoicing a fee.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-133">असल/मूल बहीखाता पंक्ति पर शुल्क राशि के लिए बिना बिल वाली उलट बिक्री.</span><span class="sxs-lookup"><span data-stu-id="881d4-133">An unbilled sales reversal for the fee amount on the original journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-134">असल/मूल बहीखाता पंक्ति पर मात्रा और राशि के लिए वास्तविक बिक्री बिल.</span><span class="sxs-lookup"><span data-stu-id="881d4-134">A billed sales actual for the quantity and amount on the original fee journal line.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="216" valign="top">
                <p>
<span data-ttu-id="881d4-135">किसी/एक माइलस्टोन का इनवॉइस बनाना.</span><span class="sxs-lookup"><span data-stu-id="881d4-135">Invoicing a milestone.</span></span>
                </p>
            </td>
            <td width="408" valign="top">
                <p>
<span data-ttu-id="881d4-136">परियोजना अनुबंध पंक्ति पर मूल माइलस्टोन पर माइलस्टोन की राशि के लिए वास्तविक बिक्री बिल.</span><span class="sxs-lookup"><span data-stu-id="881d4-136">A billed sales actual for the milestone amount on the original milestone on the project contract line.</span></span>
                </p>
            </td>
        </tr>
    </tbody>
</table>
