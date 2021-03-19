---
title: अनुबंध पर एक एड-हॉक उन्नत बनाना
description: यह विषय आवश्यकतानुसार अनुबंध पर एडवांस बनाने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 2f0a6391a3bf6dd39d21504a6f286e4ff1954183
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5273599"
---
# <a name="creating-an-ad-hoc-advance-on-a-contract"></a><span data-ttu-id="983ae-103">अनुबंध पर एक एड-हॉक उन्नत बनाना</span><span class="sxs-lookup"><span data-stu-id="983ae-103">Creating an ad hoc advance on a contract</span></span>

<span data-ttu-id="983ae-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="983ae-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="983ae-105">Microsoft Dynamics 365 Project Operations उन इनवॉइसिंग परिदृश्यों का समर्थन करता है, जिनमें पूर्व-भुगतान और एडवांस शामिल होते हैं.</span><span class="sxs-lookup"><span data-stu-id="983ae-105">Microsoft Dynamics 365 Project Operations supports invoicing scenarios that involve pre-payments and advances.</span></span> <span data-ttu-id="983ae-106">**Project Operations** में **एडवांस** उपयोग करने की प्रक्रिया **रिटेनर** अनुबंधों के समान है.</span><span class="sxs-lookup"><span data-stu-id="983ae-106">The process for using **Advances** in **Project Operations** is similar to **Retainer** contracts.</span></span> 

<span data-ttu-id="983ae-107">एडवांस के लिए ग्राहक को इनवॉइस करने हेतु निम्न चरणों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="983ae-107">Complete the following steps to invoice the customer for an advance.</span></span>

1. <span data-ttu-id="983ae-108">**परियोजना अनुबंध** पृष्ठ पर जाएँ और उसके बाद **एडवांस और रिटेनर्स** टैब चुनें.</span><span class="sxs-lookup"><span data-stu-id="983ae-108">Go to the **Project Contract** page, and then select the **Advances and Retainers** tab.</span></span>
2. <span data-ttu-id="983ae-109">उस सब-ग्रिड में, जो पहले रिकॉर्ड किए गए सभी एडवांस और पूर्व भुगतानों को सूचीबद्ध करती है, **+ नई परियोजना अनुबंध रिटेनर** चुनें.</span><span class="sxs-lookup"><span data-stu-id="983ae-109">In the subgrid that lists all the previously recorded advances and prepayments, select **+ New Project contract retainer**.</span></span> 

    <span data-ttu-id="983ae-110">पूर्व भुगतान और एडवांस को रिकॉर्ड करने के लिए, **त्वरित बनाएँ** प्रपत्र खुलता है.</span><span class="sxs-lookup"><span data-stu-id="983ae-110">The **Quick Create** form opens for recording a prepayment or advance.</span></span>
    
3. <span data-ttu-id="983ae-111">नीचे दी गई तालिका एडवांस को रिकॉर्ड करने के लिए फ़ील्ड और नए बनाने के लिए ध्यान में रखने वाले विचारों को सूचीबद्ध करती है:</span><span class="sxs-lookup"><span data-stu-id="983ae-111">The table below lists the fields for recording an advance and the considerations to keep in mind as you create new ones:</span></span>

    | <span data-ttu-id="983ae-112">क्षेत्र</span><span class="sxs-lookup"><span data-stu-id="983ae-112">Field</span></span> | <span data-ttu-id="983ae-113">विवरण</span><span class="sxs-lookup"><span data-stu-id="983ae-113">Description</span></span> | <span data-ttu-id="983ae-114">डाउनस्ट्रीम प्रभाव</span><span class="sxs-lookup"><span data-stu-id="983ae-114">Downstream impact</span></span> |
    | --- | --- | --- |
    | <span data-ttu-id="983ae-115">**परियोजना अनुबंध ग्राहक**</span><span class="sxs-lookup"><span data-stu-id="983ae-115">**Project Contract Customer**</span></span> | <span data-ttu-id="983ae-116">यह फ़ील्ड इंगित करती है कि अनुबंध पर किस ग्राहक को इस एडवांस के लिए इनवॉइस किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="983ae-116">This field indicates which customer on the contract will be invoiced for this advance.</span></span> | <span data-ttu-id="983ae-117">यदि आपके पास अनुबंध पर एकाधिक ग्राहक हैं और उनमें से प्रत्येक को एक विशिष्ट रिटेनर या एडवांस राशि के लिए इनवॉइस करना चाहते हैं, तो प्रत्येक ग्राहक के लिए व्यक्तिगत रूप से एडवांस बनाएं.</span><span class="sxs-lookup"><span data-stu-id="983ae-117">If you have multiple customers on the contract and want to invoice each of them for a specific retainer or advance amount, create an advance for each customer individually.</span></span> |
    | <span data-ttu-id="983ae-118">**वर्णन**</span><span class="sxs-lookup"><span data-stu-id="983ae-118">**Description**</span></span> | <span data-ttu-id="983ae-119">इस एडवांस को पहचानने में सहायता के लिए एडवांस के उद्देश्य या समय का विवरण.</span><span class="sxs-lookup"><span data-stu-id="983ae-119">The description of the purpose or timing of the advance to help identify this advance.</span></span> | <span data-ttu-id="983ae-120">यह विवरण इस एडवांस के लिए इनवॉइस पंक्ति पर प्रदर्शित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="983ae-120">This description is displayed on the invoice line for this advance.</span></span> |
    | <span data-ttu-id="983ae-121">**राशि**</span><span class="sxs-lookup"><span data-stu-id="983ae-121">**Amount**</span></span> | <span data-ttu-id="983ae-122">पूर्व भुगतान या एडवांस के लिए राशि.</span><span class="sxs-lookup"><span data-stu-id="983ae-122">The amount for the pre-payment or advance.</span></span> | <span data-ttu-id="983ae-123">यह राशि इस एडवांस के लिए इनवॉइस पंक्ति पर प्रदर्शित की गई है.</span><span class="sxs-lookup"><span data-stu-id="983ae-123">This amount is displayed on the invoice line for this advance.</span></span> |
    | <span data-ttu-id="983ae-124">**इनवॉइस की तिथि**</span><span class="sxs-lookup"><span data-stu-id="983ae-124">**Invoice Date**</span></span> | <span data-ttu-id="983ae-125">वह दिनांक, जब इस एडवांस को ग्राहक को इनवॉइस किया गया.</span><span class="sxs-lookup"><span data-stu-id="983ae-125">The date on which this advance is invoiced to the customer.</span></span> | <span data-ttu-id="983ae-126">यह इस एडवांस के लिए एक इनवॉइस पंक्ति बनाने हेतु स्वचालित इनवॉइस निर्माण प्रक्रिया का दिनांक है.</span><span class="sxs-lookup"><span data-stu-id="983ae-126">This is the date for the automated invoice creation process to create an invoice line for this advance.</span></span> |
    | <span data-ttu-id="983ae-127">**इनवॉइस स्थिति**</span><span class="sxs-lookup"><span data-stu-id="983ae-127">**Invoice Status**</span></span> | <span data-ttu-id="983ae-128">यह एक विकल्प सेटिंग है, जो इंगित करती है कि यह एडवांस इस ग्राहक के लिए ड्राफ़्ट इनवॉइस में जोड़ा गया है या नहीं.</span><span class="sxs-lookup"><span data-stu-id="983ae-128">This is an option setting that indicates whether this advance is added to a draft invoice for this customer.</span></span> <span data-ttu-id="983ae-129">संभावित मान हैं:</span><span class="sxs-lookup"><span data-stu-id="983ae-129">The possible values are:</span></span></br><span data-ttu-id="983ae-130">- **इनवॉइस करने के लिए तैयार नहीं**</span><span class="sxs-lookup"><span data-stu-id="983ae-130">- **Not ready to invoice**</span></span></br><span data-ttu-id="983ae-131">- **इनवॉइस करने के लिए तैयार**</span><span class="sxs-lookup"><span data-stu-id="983ae-131">- **Ready to invoice**</span></span> | <span data-ttu-id="983ae-132">जब किसी एडवांस या पूर्व भुगतान को **इनवॉइस के लिए तैयार** के रूप में चिह्नित किया जाता है, तो उसे ड्राफ़्ट इनवॉइस पर एक पंक्ति समय के रूप में जोड़ा जाता है.</span><span class="sxs-lookup"><span data-stu-id="983ae-132">When an advance or pre-payment is marked as **Ready to invoice**, it is added as a line time on a draft invoice.</span></span> <span data-ttu-id="983ae-133">केवल एक पूरी तरह से इनवॉइस किए गए एडवांस का उपयोग अगली इनवॉइस अवधि के लिए परियोजना लागतों के विरुद्ध मिलान करने के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="983ae-133">Only a fully invoiced advance can be used to reconcile against project costs for the next invoice period.</span></span> |

4. <span data-ttu-id="983ae-134">एडवांस या पूर्व भुगतान को रिकॉर्ड करने के लिए, त्वरित बनाएँ संवाद पर **सहेजें और बंद करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="983ae-134">Select **Save and close** on the quick create dialog to record the advance or the pre-payment.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]