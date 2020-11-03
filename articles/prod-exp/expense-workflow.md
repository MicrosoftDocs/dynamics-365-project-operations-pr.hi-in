---
title: ख़र्च प्रबंधन कार्यप्रवाह
description: यह विषय बताता है कि आप ख़र्च प्रबंधन में ख़र्च रिपोर्ट के लिए समीक्षा प्रक्रिया सेट करने के लिए Microsoft Dynamics 365 Finance में कार्यप्रवाह प्रणाली का उपयोग कैसे कर सकते हैं.
author: ShylaThompson
manager: AnnBe
ms.date: 09/13/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WorkflowtableListPageRnr
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 5207be92cb58d8ab2658096b3e0f3fc81d73d91e
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077855"
---
# <a name="expense-management-workflow"></a><span data-ttu-id="40ad6-103">ख़र्च प्रबंधन कार्यप्रवाह</span><span class="sxs-lookup"><span data-stu-id="40ad6-103">Expense management workflow</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="40ad6-104">आप ख़र्च प्रबंधन में ख़र्च रिपोर्ट के लिए समीक्षा प्रक्रिया सेट करने के लिए कार्यप्रवाह प्रणाली का उपयोग कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="40ad6-104">You can use the workflow system to set up a review process for expense reports in Expense management.</span></span> <span data-ttu-id="40ad6-105">आप एक कार्यप्रवाह सेट कर सकते हैं जो यह निर्धारित करने के लिए निम्नलिखित मानदंडों का उपयोग करता है कि ख़र्च रिपोर्ट को कौन स्वीकृति देता है:</span><span class="sxs-lookup"><span data-stu-id="40ad6-105">You can set up a workflow that uses the following criteria to determine who approves expense reports:</span></span>

- <span data-ttu-id="40ad6-106">कर्मचारी रिपोर्टिंग पदानुक्रम और पूर्वनिर्धारित अनुमोदन सीमाएं</span><span class="sxs-lookup"><span data-stu-id="40ad6-106">The employee reporting hierarchy and predefined approval limits</span></span>
- <span data-ttu-id="40ad6-107">अंतरिम अनुमोदनकर्ताओं और अंतिम अनुमोदक का समर्थन करने वाली बहु-स्तरीय अनुमोदन</span><span class="sxs-lookup"><span data-stu-id="40ad6-107">Multi-level approval that supports interim approvers and a final approver</span></span>
- <span data-ttu-id="40ad6-108">वित्तीय आयाम और परियोजना की जिम्मेदारी</span><span class="sxs-lookup"><span data-stu-id="40ad6-108">Financial dimensions and project responsibility</span></span>
- <span data-ttu-id="40ad6-109">विशिष्ट उपयोगकर्ताओं या उपयोगकर्ता समूहों को असाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="40ad6-109">Assignment to specific users or user groups</span></span>

<span data-ttu-id="40ad6-110">ख़र्च रिपोर्ट, यात्रा मांग, नकद अग्रिम, और मूल्य वर्धित कर (VAT) वसूली के लिए कार्यप्रवाह अनुमोदन बनाए जा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="40ad6-110">Workflow approvals can be created for expense reports, travel requisitions, cash advances, and value-added tax (VAT) recovery.</span></span>

<span data-ttu-id="40ad6-111">**उदाहरण**</span><span class="sxs-lookup"><span data-stu-id="40ad6-111">**Example**</span></span>

<span data-ttu-id="40ad6-112">निम्नलिखित प्रक्रिया ख़र्च रिपोर्ट के लिए ख़र्च प्रबंधन कार्यप्रवाह का एक उदाहरण है.</span><span class="sxs-lookup"><span data-stu-id="40ad6-112">The following process is an example of the expense management workflow for an expense report.</span></span>

1. <span data-ttu-id="40ad6-113">एक ख़र्च रिपोर्ट को एक कर्मचारी बनाता है और सहेजता है.</span><span class="sxs-lookup"><span data-stu-id="40ad6-113">An employee creates and saves an expense report.</span></span>
2. <span data-ttu-id="40ad6-114">कर्मचारी अनुमोदन के लिए ख़र्च रिपोर्ट प्रस्तुत करता है.</span><span class="sxs-lookup"><span data-stu-id="40ad6-114">The employee submits the expense report for approval.</span></span> <span data-ttu-id="40ad6-115">अनुमोदक की पहचान उस नियमों के आधार पर की जाती है जिसे कार्यप्रवाह स्थापित होने पर परिभाषित किया गया था.</span><span class="sxs-lookup"><span data-stu-id="40ad6-115">The approver is identified based on the rules that were defined when the workflow was set up.</span></span>
3. <span data-ttu-id="40ad6-116">अनुमोदक को एक अधिसूचना प्राप्त होती है कि एक ख़र्च रिपोर्ट अनुमोदन के लिए तैयार है.</span><span class="sxs-lookup"><span data-stu-id="40ad6-116">The approver receives a notification that an expense report is ready for approval.</span></span> <span data-ttu-id="40ad6-117">अनुमोदक ख़र्च रिपोर्ट की समीक्षा करता है और यह सत्यापित करता है कि निम्नलिखित शर्तों को पूरा किया गया है:</span><span class="sxs-lookup"><span data-stu-id="40ad6-117">The approver reviews the expense report and verifies that the following conditions are met:</span></span>

    - <span data-ttu-id="40ad6-118">ख़र्च किसी भी ख़र्च नीतियों का उल्लंघन नहीं करते हैं.</span><span class="sxs-lookup"><span data-stu-id="40ad6-118">The expenses don't violate any expense policies.</span></span> <span data-ttu-id="40ad6-119">यदि कोई ख़र्च किसी नीति का उल्लंघन करता है, तो अनुमोदक यह सत्यापित करता है कि ख़र्च रिपोर्ट में वैध व्यावसायिक औचित्य शामिल है.</span><span class="sxs-lookup"><span data-stu-id="40ad6-119">If an expense violates a policy, the approver verifies that the expense report includes a valid business justification.</span></span>
    - <span data-ttu-id="40ad6-120">ख़र्च रिपोर्ट से इलेक्ट्रॉनिक रसीदें संलग्न हैं.</span><span class="sxs-lookup"><span data-stu-id="40ad6-120">Electronic receipts are attached to the expense report.</span></span>

4. <span data-ttu-id="40ad6-121">अनुमोदक ख़र्च रिपोर्ट को स्वीकृत करता है.</span><span class="sxs-lookup"><span data-stu-id="40ad6-121">The approver approves the expense report.</span></span>
5. <span data-ttu-id="40ad6-122">ख़र्च रिपोर्ट पोस्टिंग के लिए लेखा देय समन्वयक को सौंपी जाती है.</span><span class="sxs-lookup"><span data-stu-id="40ad6-122">The expense report is assigned to the Accounts payable coordinator for posting.</span></span>
6. <span data-ttu-id="40ad6-123">क्या स्वचालित पोस्टिंग कॉन्फ़िगर की गई है के आधार पर निम्नलिखित चरणों में से एक होता है:</span><span class="sxs-lookup"><span data-stu-id="40ad6-123">One of the following steps occurs, depending on whether automatic posting is configured:</span></span>

    - <span data-ttu-id="40ad6-124">यदि स्वचालित पोस्टिंग को कॉन्फ़िगर किया गया है, तो ख़र्च रिपोर्ट को भुगतान के लिए संसाधित किया जाता है, और ख़र्च रिपोर्ट की स्थिति अपडेट की जाती है.</span><span class="sxs-lookup"><span data-stu-id="40ad6-124">If automatic posting is configured, the expense report is processed for payment, and the status of the expense report is updated.</span></span>
    - <span data-ttu-id="40ad6-125">यदि स्वचालित पोस्टिंग कॉन्फ़िगर नहीं की गई है, तो लेखा देय समन्वयक यह सत्यापित करता है कि सभी मूल रसीदें प्रस्तुत की गई हैं, और यह कि रसीदें ख़र्च रिपोर्ट पर ख़र्चों के साथ पंक्तिबध्द हैं.</span><span class="sxs-lookup"><span data-stu-id="40ad6-125">If automatic posting isn't configured, the Accounts payable coordinator verifies that all original receipts have been submitted, and that the receipts are aligned with the expenses on the expense report.</span></span> <span data-ttu-id="40ad6-126">ख़र्च रिपोर्ट पर दर्ज किए गए सभी कर कोड को भी सही के रूप में सत्यापित किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="40ad6-126">All tax codes that are entered on the expense report must also be verified as correct.</span></span>

<span data-ttu-id="40ad6-127">इन आवश्यकताओं को सत्यापित किए जाने के बाद, ख़र्च रिपोर्ट पोस्ट की जाती है.</span><span class="sxs-lookup"><span data-stu-id="40ad6-127">After these requirements are verified, the expense report is posted.</span></span>

<span data-ttu-id="40ad6-128">ख़र्च रिपोर्ट पोस्ट किए जाने के बाद, ख़र्च रिपोर्ट के लिए भुगतान अधिकृत किया जाता है, और कर्मचारी की प्रतिपूर्ति की जाती है.</span><span class="sxs-lookup"><span data-stu-id="40ad6-128">After the expense report is posted, payment is authorized for the expense report, and the employee is reimbursed.</span></span>
