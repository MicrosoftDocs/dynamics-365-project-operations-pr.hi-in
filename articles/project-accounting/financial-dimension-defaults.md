---
title: वित्तीय आयाम डिफ़ॉल्ट
description: यह विषय वित्तीय आयाम डिफ़ॉल्ट सेट अप करने के तरीके के बारे में जानकारी प्रदान करता है.
author: sigitac
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 03b9a9028c1610b191db9c1bfb0163adc88bdf3e
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642365"
---
# <a name="financial-dimension-defaults"></a><span data-ttu-id="2e976-103">वित्तीय आयाम डिफ़ॉल्ट</span><span class="sxs-lookup"><span data-stu-id="2e976-103">Financial dimension defaults</span></span>

<span data-ttu-id="2e976-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="2e976-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="2e976-105">परियोजना सबलेज़र और सामान्य लेज़र लेनदेन पर अतिरिक्त जानकारी प्रदान करने के लिए Dynamics 365 Project Operations, Dynamics 365 Finance में [वित्तीय आयाम](https://docs.microsoft.com/dynamics365/finance/general-ledger/financial-dimensions) फ़्रेमवर्क का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="2e976-105">Dynamics 365 Project Operations uses the [Financial dimensions](https://docs.microsoft.com/dynamics365/finance/general-ledger/financial-dimensions) framework in Dynamics 365 Finance to provide additional insights on project subledger and general ledger transactions.</span></span>

<span data-ttu-id="2e976-106">डिफ़ॉल्ट वित्तीय आयाम को ग्राहक, परियोजना फ़ंडिंग स्रोत, माइलस्टोन, परियोजना अनुबंध पंक्ति या परियोजना पर सेट किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="2e976-106">Default financial dimensions can be set on a customer, project funding source, milestone, project contract line, or project.</span></span>

## <a name="define-default-financial-dimensions-for-a-customer"></a><span data-ttu-id="2e976-107">ग्राहक के लिए डिफ़ॉल्ट वित्तीय आयामों को परिभाषित करें</span><span class="sxs-lookup"><span data-stu-id="2e976-107">Define default financial dimensions for a customer</span></span>

<span data-ttu-id="2e976-108">ग्राहक आयाम डिफ़ॉल्ट वित्तिय में निर्दिष्ट हैं.</span><span class="sxs-lookup"><span data-stu-id="2e976-108">Customer dimension defaults are specified in Finance.</span></span> <span data-ttu-id="2e976-109">आयाम डिफ़ॉल्ट सेट करने के लिए निम्न चरणों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="2e976-109">Complete the following steps to set dimension defaults.</span></span>

1. <span data-ttu-id="2e976-110">**लेनदारी लेखे** > **ग्राहक** > **सभी ग्राहक** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="2e976-110">Go to **Accounts receivable** > **Customers** > **All customers**.</span></span>
2. <span data-ttu-id="2e976-111">**ग्राहक** पृष्ठ, **वित्तीय आयाम** टैब पर, विशिष्ट ग्राहक के लिए वित्तीय आयाम मान सेट करें.</span><span class="sxs-lookup"><span data-stu-id="2e976-111">On the **Customers** page, on the **Financial dimensions** tab, set the financial dimension values for specific customer.</span></span>

## <a name="define-default-financial-dimensions-for-project-contracts"></a><span data-ttu-id="2e976-112">परियोजना अनुबंधों के लिए डिफ़ॉल्ट वित्तीय आयामों को परिभाषित करें</span><span class="sxs-lookup"><span data-stu-id="2e976-112">Define default financial dimensions for project contracts</span></span>

<span data-ttu-id="2e976-113">Common Data Service (CDS) में परियोजना अनुबंध बनाए और कायम रखे जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="2e976-113">Project contracts are created and maintained in Common Data Service (CDS).</span></span> <span data-ttu-id="2e976-114">परियोजना अनुबंधों के लिए लेखांकन एट्रिब्यूट को वित्तिय में **परियोजना प्रबंधन और लेखांकन** मॉड्यूल में सेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="2e976-114">Accounting attributes for project contracts are set in the **Project management and accounting** module in Finance.</span></span>

### <a name="set-financial-dimensions-for-a-project-funding-source"></a><span data-ttu-id="2e976-115">परियोजना फ़ंडिंग स्रोत के लिए वित्तीय आयाम सेट करें</span><span class="sxs-lookup"><span data-stu-id="2e976-115">Set financial dimensions for a project funding source</span></span>

1. <span data-ttu-id="2e976-116">**परियोजना प्रबंधन और लेखांकन** > **परियोजना** > **परियोजना अनुबंध** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="2e976-116">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="2e976-117">वह रिकॉर्ड चुनें जिसे आप अद्यतन करना चाहते हैं और **परियोजना अनुबंध** टैब पर, **डिफ़ॉल्ट लेखांकन दिखाएं** चुनें.</span><span class="sxs-lookup"><span data-stu-id="2e976-117">Select the record you want to update, and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="2e976-118">**संबंधित जानकारी** विस्तृत करें और **फ़ंडिंग स्रोत** टैब चुनें.</span><span class="sxs-lookup"><span data-stu-id="2e976-118">Expand **Related information** and select the **Funding sources** tab.</span></span>
4. <span data-ttu-id="2e976-119">वित्तीय आयाम डिफ़ॉल्ट सेट करें.</span><span class="sxs-lookup"><span data-stu-id="2e976-119">Set the financial dimension defaults.</span></span> <span data-ttu-id="2e976-120">ध्यान दें कि ग्राहक खाते से वित्तीय आयाम डिफ़ॉल्ट होते हैं.</span><span class="sxs-lookup"><span data-stu-id="2e976-120">Notice that the financial dimensions default from the customer account.</span></span>

### <a name="set-financial-dimensions-for-a-project-contract-line"></a><span data-ttu-id="2e976-121">परियोजना अनुबंध पंक्ति के लिए वित्तीय आयाम सेट करें</span><span class="sxs-lookup"><span data-stu-id="2e976-121">Set financial dimensions for a project contract line</span></span>

1. <span data-ttu-id="2e976-122">**परियोजना प्रबंधन और लेखांकन** > **परियोजना** > **परियोजना अनुबंध** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="2e976-122">Go to **Project management and accounting** > **Projects** > **Project contracts**.</span></span>
2. <span data-ttu-id="2e976-123">वह रिकॉर्ड चुनें जिसे आप अद्यतन करना चाहते हैं और **परियोजना अनुबंध** टैब पर, **डिफ़ॉल्ट लेखांकन दिखाएं** चुनें.</span><span class="sxs-lookup"><span data-stu-id="2e976-123">Select the record you want to update and on the **Project contract** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="2e976-124">**संबंधित जानकारी** विस्तृत करें और **अनुबंध पंक्तियाँ** टैब चुनें.</span><span class="sxs-lookup"><span data-stu-id="2e976-124">Expand **Related information** and select the **Contract lines** tab.</span></span>
4. <span data-ttu-id="2e976-125">वित्तीय आयाम डिफ़ॉल्ट सेट करें.</span><span class="sxs-lookup"><span data-stu-id="2e976-125">Set the financial dimension defaults.</span></span> <span data-ttu-id="2e976-126">वित्तीय आयाम डिफ़ॉल्ट लागू होते हैं और केवल निश्चित मूल्य (माइलस्टोन) अनुबंध पंक्तियों के साथ उपयोग किए जा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="2e976-126">The financial dimension defaults are applicable and can be used only with Fixed price (milestone) contract lines.</span></span>

<span data-ttu-id="2e976-127">इन डिफ़ॉल्ट का उपयोग संबंधित परियोजना ऑन-अकाउंट ट्रांज़ैक्शन और इनवॉइस पंक्तियों पर किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="2e976-127">These defaults are used on related project on-account transactions and invoice lines.</span></span>

## <a name="define-default-financial-dimensions-for-projects"></a><span data-ttu-id="2e976-128">परियोजनाओं के लिए डिफ़ॉल्ट वित्तीय आयामों को परिभाषित करें</span><span class="sxs-lookup"><span data-stu-id="2e976-128">Define default financial dimensions for projects</span></span>

<span data-ttu-id="2e976-129">CDS में परियोजना बनाई और कायम रखी जाती हैं.</span><span class="sxs-lookup"><span data-stu-id="2e976-129">Projects are created and maintained in CDS.</span></span> <span data-ttu-id="2e976-130">परियोजनाओं के लिए लेखांकन एट्रिब्यूट को वित्तिय में **परियोजना प्रबंधन और लेखांकन** मॉड्यूल में सेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="2e976-130">Accounting attributes for projects are set in the **Project management and accounting** module in Finance.</span></span>

1. <span data-ttu-id="2e976-131">**परियोजना प्रबंधन और लेखांकन** > **परियोजना** > **सभी परियोजना** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="2e976-131">Go to **Project management and accounting** > **Projects** > **All projects**.</span></span>
2. <span data-ttu-id="2e976-132">वह रिकॉर्ड चुनें जिसे आप अद्यतन करना चाहते हैं और **परियोजना** टैब पर, **डिफ़ॉल्ट लेखांकन दिखाएं** चुनें.</span><span class="sxs-lookup"><span data-stu-id="2e976-132">Select the record that you want to update and on the **Project** tab, select **Show default accounting**.</span></span>
3. <span data-ttu-id="2e976-133">**संबंधित जानकारी** विस्तृत करें और **सेटअप** टैब चुनें.</span><span class="sxs-lookup"><span data-stu-id="2e976-133">Expand **Related information** and select the **Setup** tab.</span></span>
4. <span data-ttu-id="2e976-134">वित्तीय आयाम डिफ़ॉल्ट सेट करें.</span><span class="sxs-lookup"><span data-stu-id="2e976-134">Set the financial dimension defaults.</span></span> <span data-ttu-id="2e976-135">ध्यान दें कि ग्राहक खाते से वित्तीय आयाम डिफ़ॉल्ट होते हैं.</span><span class="sxs-lookup"><span data-stu-id="2e976-135">Notice that financial dimensions default from the customer account.</span></span> <span data-ttu-id="2e976-136">यदि परियोजना एकाधिक परियोजना अनुबंध ग्राहकों के साथ अनुबंध पंक्ति से संबद्ध है, तो प्राथमिक ग्राहक का उपयोग वित्तीय आयामों को डिफ़ॉल्ट करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="2e976-136">If the project is associated with a contract line with multiple project contract customers, the primary customer is used to default financial dimensions.</span></span>

<span data-ttu-id="2e976-137">परियोजना डिफ़ॉल्ट वित्तीय आयामों का उपयोग **Project Operations एकीकरण जर्नल** और संबंधित परियोजना इनवॉइस पंक्तियों पर समय, व्यय और शुल्क ट्रांज़ैक्शन के लिए जर्नल पंक्ति डिफ़ॉल्ट को सेट करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="2e976-137">Project default financial dimensions are used to set journal line defaults for time, expense, and fee transactions in the **Project Operations Integration Journal** and on related project invoice lines.</span></span>
