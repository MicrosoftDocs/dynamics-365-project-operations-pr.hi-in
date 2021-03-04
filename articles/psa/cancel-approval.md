---
title: पहले से स्वीकृत समय और व्यय प्रविष्टियों को रद्द करें
description: यह विषय स्वीकृत प्रोजेक्ट समय और व्यय लेन-देन को रद्द करने के तरीके के बारे में जानकारी प्रदान करता है।
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/07/2019
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
ms.openlocfilehash: ea42c6755b4b48d986e385879607d659c57f483d
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/10/2021
ms.locfileid: "5150580"
---
# <a name="cancel-previously-approved-time-or-expense-entries"></a><span data-ttu-id="f669c-103">पहले से स्वीकृत समय या खर्च प्रविष्टियों को रद्द करें</span><span class="sxs-lookup"><span data-stu-id="f669c-103">Cancel previously approved time or expense entries</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="f669c-104">Dynamics 365 Project Service Automation के नवीनतम संस्करण में, अनुमोदनकर्ता उन समय या खर्च प्रविष्टियों को रद्द कर सकते हैं जो उन्होंने पहले अनुमोदित की थीं।</span><span class="sxs-lookup"><span data-stu-id="f669c-104">In the latest version of Dynamics 365 Project Service Automation, approvers can cancel time or expense entries that they previously approved.</span></span>

## <a name="cancel-a-previously-approved-time-or-expense-entry"></a><span data-ttu-id="f669c-105">पहले से स्वीकृत समय या खर्च प्रविष्टि रद्द करें</span><span class="sxs-lookup"><span data-stu-id="f669c-105">Cancel a previously approved time or expense entry</span></span>

<span data-ttu-id="f669c-106">आपके द्वारा पहले अनुमोदित किए गए समय या खर्च प्रविष्टि को रद्द करने के लिए इन चरणों का पालन करें।</span><span class="sxs-lookup"><span data-stu-id="f669c-106">Follow these steps to cancel a time or expense entry that you previously approved.</span></span>

1. <span data-ttu-id="f669c-107">**प्रोजेक्ट्स** \> **मेरे कार्य** \> **स्वीकृति** पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="f669c-107">Go to **Projects** \> **My Work** \> **Approvals**.</span></span>
2. <span data-ttu-id="f669c-108">**स्वीकृति** सूची पृष्ठ पर, दृश्य को **मेरे पिछले अनुमोदन** में बदल दें।</span><span class="sxs-lookup"><span data-stu-id="f669c-108">On the **Approvals** list page, change the view to **My past approvals**.</span></span> <span data-ttu-id="f669c-109">आपके द्वारा पहले अनुमोदित किए गए समय और खर्च प्रविष्टियों की एक सूची दिखाई जाती है।</span><span class="sxs-lookup"><span data-stu-id="f669c-109">A list of the time and expense entries that you previously approved is shown.</span></span>
3. <span data-ttu-id="f669c-110">एक या अधिक प्रविष्टियों का चयन करें, और फिर **अनुमोदन रद्द करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="f669c-110">Select one or more entries, and then select **Cancel approval**.</span></span> <span data-ttu-id="f669c-111">आपको एक चेतावनी संदेश प्राप्त होता है।</span><span class="sxs-lookup"><span data-stu-id="f669c-111">You receive a warning message.</span></span>
4. <span data-ttu-id="f669c-112">अनुमोदन रद्द करने के लिए **ठीक** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="f669c-112">Select **OK** to cancel the approval.</span></span>

## <a name="understand-the-impact-of-canceling-a-time-or-expense-entry-approval"></a><span data-ttu-id="f669c-113">एक समय या खर्च प्रविष्टि अनुमोदन को रद्द करने के प्रभाव को समझें</span><span class="sxs-lookup"><span data-stu-id="f669c-113">Understand the impact of canceling a time or expense entry approval</span></span>

<span data-ttu-id="f669c-114">जब कोई अनुमोदन रद्द किया जाता है, तो परिचालन प्रभाव और वित्तीय प्रभाव दोनों होते हैं।</span><span class="sxs-lookup"><span data-stu-id="f669c-114">When an approval is canceled, there is both operational impact and financial impact.</span></span>

### <a name="operational-impact"></a><span data-ttu-id="f669c-115">परिचालन प्रभाव</span><span class="sxs-lookup"><span data-stu-id="f669c-115">Operational impact</span></span>

<span data-ttu-id="f669c-116">परिचालन की तरफ, जब कोई अनुमोदन रद्द हो जाता है, तो रिकॉर्ड की स्थिति **ड्राफ्ट** पर रीसेट हो जाती है, और अनुमोदन अब **मेरे पिछले अनुमोदन** दृश्य में प्रकट नहीं होते हैं।</span><span class="sxs-lookup"><span data-stu-id="f669c-116">On the operations side, when an approval is canceled, the status of the record is reset to **Draft**, and the approval no longer appears in the **My past approvals** view.</span></span> <span data-ttu-id="f669c-117">इसके बजाय, रद्द की गई मंजूरी या तो **अनुमोदन के लिए समय प्रविष्टियों** दृश्य में दिखाई देती है या **अनुमोदन के लिए खर्च प्रविष्टियां** दृश्य, यह इस बात पर निर्भर करता है कि यह समय प्रविष्टि थी या खर्च प्रविष्टि थी।</span><span class="sxs-lookup"><span data-stu-id="f669c-117">Instead, the canceled approval appears in either the **Time entries for approval** view or the **Expense entries for approval** view, depending on whether it was a time entry or an expense entry.</span></span> <span data-ttu-id="f669c-118">इसके अतिरिक्त, संबंधित समय या खर्च प्रविष्टि की स्थिति को **सबमिशन** में बदल दिया जाता है, ताकि संबंधित प्रविष्टि उन अनुमोदनों के अनुरूप हो, जिनमें **ड्राफ्ट** की स्थिति है।</span><span class="sxs-lookup"><span data-stu-id="f669c-118">Additionally, the status of the related time or expense entry is changed to **Submitted**, so that the related entry is consistent with approvals that have a status of **Draft**.</span></span>

<span data-ttu-id="f669c-119">एक अनुमोदनकर्ता के रूप में, आप अनुमोदन के कुछ फ़ील्ड को संपादित कर सकते हैं जिनकी स्थिति **ड्राफ्ट** है।</span><span class="sxs-lookup"><span data-stu-id="f669c-119">As an approver, you can edit some of the fields of an approval that has a status of **Draft**.</span></span> <span data-ttu-id="f669c-120">इन फ़ील्ड में **बिलिंग प्रकार** और **समय प्रविष्टियों के लिए बिल योग्य घंटे** शामिल हैं।</span><span class="sxs-lookup"><span data-stu-id="f669c-120">These fields include **Billing Type** and **Billable Hours for Time Entries**.</span></span> <span data-ttu-id="f669c-121">आपके द्वारा बदलाव किए जाने के बाद, आप फिर से रिकॉर्ड को अनुमोदित कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="f669c-121">After you make changes, you can approve the record again.</span></span> <span data-ttu-id="f669c-122">वैकल्पिक रूप से, आप प्रविष्टि को अस्वीकार कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="f669c-122">Alternatively, you can reject the entry.</span></span> <span data-ttu-id="f669c-123">यदि आप किसी समय प्रविष्टि की स्वीकृति को अस्वीकार करते हैं, तो प्रविष्टि की स्थिति को **वापस की गई** में बदल दिया जाता है।</span><span class="sxs-lookup"><span data-stu-id="f669c-123">If you reject the approval of a time entry, the status of the entry is changed to **Returned**.</span></span> <span data-ttu-id="f669c-124">यदि आप किसी खर्च प्रविष्टि की स्वीकृति को अस्वीकार करते हैं, तो स्थिति को **अस्वीकृत** में बदल दिया जाता है।</span><span class="sxs-lookup"><span data-stu-id="f669c-124">If you reject the approval of an expense entry, the status is changed to **Rejected**.</span></span> <span data-ttu-id="f669c-125">कार्यात्मक रूप से, दोनों वापस की गई और अस्वीकृत प्रविष्टियां उसी प्रविष्टि के रूप में व्यवहार करती हैं जिसकी स्थिति **ड्राफ्ट** की होती है।</span><span class="sxs-lookup"><span data-stu-id="f669c-125">Functionally, both returned and rejected entries behave the same as an entry that has a status of **Draft**.</span></span> <span data-ttu-id="f669c-126">प्रोजेक्ट टीम का सदस्य या तो प्रविष्टि में कोई आवश्यक परिवर्तन कर सकता है और फिर उसे अनुमोदन के लिए पुनः सबमिट कर सकता है, या प्रविष्टि को पूरी तरह से हटा सकता है।</span><span class="sxs-lookup"><span data-stu-id="f669c-126">A project team member can either make any required changes to the entry and then resubmit it for approval, or delete the entry entirely.</span></span>

### <a name="financial-impact"></a><span data-ttu-id="f669c-127">वित्तीय प्रभाव</span><span class="sxs-lookup"><span data-stu-id="f669c-127">Financial impact</span></span>

<span data-ttu-id="f669c-128">स्वीकृति रद्द होने पर एक प्रोजेक्ट वित्तीय रूप से भी प्रभावित होता है।</span><span class="sxs-lookup"><span data-stu-id="f669c-128">A project is also affected financially when an approval is canceled.</span></span> <span data-ttu-id="f669c-129">सबसे पहले, लागत और बिक्री के लिए इसी वास्तविक तरीके को निम्नलिखित तरीके से अपडेट किया जाता है:</span><span class="sxs-lookup"><span data-stu-id="f669c-129">First, the corresponding actuals for cost and sales are updated in the following manner:</span></span>

- <span data-ttu-id="f669c-130">समायोजन की स्थिति **समायोजित** पर सेट है।</span><span class="sxs-lookup"><span data-stu-id="f669c-130">The adjustment status is set to **Adjusted**.</span></span>
- <span data-ttu-id="f669c-131">बिलिंग स्थिति **रद्द की गई** पर सेट है।</span><span class="sxs-lookup"><span data-stu-id="f669c-131">The billing status is set to **Canceled**.</span></span>

<span data-ttu-id="f669c-132">इसके बाद, वास्तविक तालिका में रिवर्सल प्रविष्टियां बनाई जाती हैं।</span><span class="sxs-lookup"><span data-stu-id="f669c-132">Next, reversal entries are created in the Actuals table.</span></span> <span data-ttu-id="f669c-133">पलटी गई प्रविष्टि बनाने के लिए, सिस्टम मूल वास्तविक से फ़ील्ड मानों को कॉपी करता है।</span><span class="sxs-lookup"><span data-stu-id="f669c-133">To create reversal entries, the system copies over the field values from the original actuals.</span></span> <span data-ttu-id="f669c-134">केवल उन मानों को कॉपी नहीं किया जाता है जो मात्रा मान हैं।</span><span class="sxs-lookup"><span data-stu-id="f669c-134">The only values that aren't copied over are the quantity values.</span></span> <span data-ttu-id="f669c-135">ये मान इसके बजाय प्रत्यावर्तित किए गए हैं।</span><span class="sxs-lookup"><span data-stu-id="f669c-135">These values are reversed instead.</span></span> <span data-ttu-id="f669c-136">प्रत्यावर्तित वास्तविकों को **लागत** और **बिल न की गई बिक्री** वास्तविक दोनों के लिए बनाया गया है।</span><span class="sxs-lookup"><span data-stu-id="f669c-136">Reversed actuals are created for both **Cost** and **Unbilled Sales** actuals.</span></span> <span data-ttu-id="f669c-137">प्रत्यावर्तित वास्तविक पर **समायोजन स्थिति** फ़ील्ड **समायोजन योग्य नहीं** पर सेट है, और बिलिंग स्थिति **रद्द** पर सेट है।</span><span class="sxs-lookup"><span data-stu-id="f669c-137">The **Adjustment Status** field on the reversed actuals is set to **Unadjustable**, and the billing status is set to **Canceled**.</span></span>

<span data-ttu-id="f669c-138">इन परिवर्तनों के बाद, वह राशि जो प्रोजेक्ट और प्रोजेक्ट पर राजस्व बैकलॉग पर खर्ची गई के रूप में दर्ज है अब इन राशियों का प्रतिनिधित्व करने वाली राशियों के लिए उत्तरदयी होगी।</span><span class="sxs-lookup"><span data-stu-id="f669c-138">After these changes are made, the amount that is recorded as spent on the project and the revenue backlog on the project will longer account for the amounts that these actuals represent.</span></span>
