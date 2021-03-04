---
title: प्रोजेक्टस और प्रोजेक्ट कॉन्ट्रेक्ट पर इनवॉइस के बैकलॉग की समीक्षा करें
description: इस टॉपिक में समय, व्यय और उत्पाद से जुड़े बैकलॉग की समीक्षा करने और उन्हें इनवॉयस बनाने के लिए तैयार करने के तरीके के बारे में जानकारी प्रदान की गई है।
author: rumant
manager: kfend
ms.service: project-operations
ms.custom: ''
ms.author: rumant
ms.date: 03/11/2019
ms.topic: article
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 092455a131f556e4f943f6bb89d7e38358f0a697
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/10/2021
ms.locfileid: "5150490"
---
# <a name="review-the-invoicing-backlog-on-projects-and-project-contracts"></a><span data-ttu-id="8e49f-103">प्रोजेक्टस और प्रोजेक्ट कॉन्ट्रेक्ट पर इनवॉइस के बैकलॉग की समीक्षा करें</span><span class="sxs-lookup"><span data-stu-id="8e49f-103">Review the invoicing backlog on projects and project contracts</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="8e49f-104">जब किसी लेनदेन का इनवॉयस बनने और प्रोसेस होने को तैयार हो तो लेनदेन पर **इन्वॉयसिंग हेतु तैयार** चिह्नित किया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="8e49f-104">When a transaction is ready to have an invoice created and processed, the transaction should be marked **Ready to invoice**.</span></span> <span data-ttu-id="8e49f-105">इस टॉपिक में संभावित प्रकार के लेनदेन का वर्णन किया गया है।</span><span class="sxs-lookup"><span data-stu-id="8e49f-105">This topic describes the types of transactions that can be created.</span></span>

## <a name="review-the-time-and-material-billing-backlog"></a><span data-ttu-id="8e49f-106">समय और सामग्री की बिलिंग के बैकलॉग की समीक्षा करें</span><span class="sxs-lookup"><span data-stu-id="8e49f-106">Review the time and material billing backlog</span></span>

<span data-ttu-id="8e49f-107">जब किसी प्रोजेक्ट से जुड़े समय या व्यय की प्रविष्टि प्रस्तुत होने के बाद अनुमोदित की जाती है तो PSA द्वारा प्रोजेक्ट के लिए वास्तविक आंकड़े बनाये जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="8e49f-107">When a time or expense entry is submitted and approved for a project, PSA creates a project actual.</span></span> <span data-ttu-id="8e49f-108">यदि प्रोजेक्ट और लेनदेन की श्रेणी के संयोजन को समय -और -सामग्री प्रोजेक्ट की कॉन्ट्रेक्ट रेखा पर मैप किया जाता है, तो प्रविष्टि स्वीकृत होने पर दो वास्तविक आंकड़े बनाए जाते हैं:</span><span class="sxs-lookup"><span data-stu-id="8e49f-108">If the combination of the project and the transaction class are mapped to a contract line for a time-and-materials project, two actuals are created when the entry is approved:</span></span>

- <span data-ttu-id="8e49f-109">वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="8e49f-109">Cost actual</span></span> 
- <span data-ttu-id="8e49f-110">वास्तविक अनबिल्ड बिक्री</span><span class="sxs-lookup"><span data-stu-id="8e49f-110">Unbilled sales actual</span></span>

<span data-ttu-id="8e49f-111">वास्तविक अनबिल्ड बिक्री बिलिंग में बैकलॉग का सूचक है और उनकी बिलिंग की स्थिति को **इनवॉयसिंग के लिए तैयार** पर सेट की जानी चाहिए।</span><span class="sxs-lookup"><span data-stu-id="8e49f-111">Unbilled sales actuals represent the billing backlog, and their billing status must be set to **Ready to Invoice**.</span></span> <span data-ttu-id="8e49f-112">जब किसी प्रोजेक्ट का इनवॉइस बनाया जाता है तो **इनवॉयसिंग के लिए तैयार** चिन्हित की गई वास्तविक अनबिल्ड बिक्री को इनवॉयस लाइन विवरण के तौर पर कॉपी किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="8e49f-112">When a project invoice is created, unbilled sales actuals that are marked **Ready to Invoice** are copied over as invoice line details.</span></span>

<span data-ttu-id="8e49f-113">समय और सामग्री के लिए बिलिंग के बैकलॉग की समीक्षा करने हेतु **बिक्री** \> **बिलिंग** \> **समय और सामग्री की बिलिंग का बैकलॉग** पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="8e49f-113">To review the billing backlog for time and materials, go to **Sales** \> **Billing** \> **Time and Material Billing Backlog**.</span></span> <span data-ttu-id="8e49f-114">इन्वॉयसिंग के लिए तैयार सभी वास्तविक अनबिल्ड बिक्री का चुनाव करें और फिर **इन्वॉयसिंग के लिए तैयार** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="8e49f-114">Select all the unbilled sales actuals that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="8e49f-115">इन वास्तविक आंकड़ों की बिलिंग की स्थिति को परिवर्तित कर **इन्वॉयसिंग के लिए तैयार** किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="8e49f-115">The billing status of these actuals is changed to **Ready to Invoice**.</span></span>

![समय और सामग्री की बिलिंग का बैकलॉग](media/TMBacklog.png)

## <a name="review-the-product-billing-backlog"></a><span data-ttu-id="8e49f-117">उत्पाद की बिलिंग के बैकलॉग की समीक्षा करें</span><span class="sxs-lookup"><span data-stu-id="8e49f-117">Review the product billing backlog</span></span>

<span data-ttu-id="8e49f-118">PSA में जब किसे प्रोजेक्ट के कॉन्ट्रेक्ट में उत्पाद-आधारित कॉन्ट्रेक्ट लाइनें होती हैं तो उन लाइनों को प्रोजेक्ट कॉन्ट्रेक्ट के लिए इनवॉयस बनाते समय ध्यान में रखा जाता है।</span><span class="sxs-lookup"><span data-stu-id="8e49f-118">In PSA, when a project contract has product-based contract lines, those lines are considered for invoicing whenever an invoice is created for the project contract.</span></span> <span data-ttu-id="8e49f-119">कोई भी उत्पाद जिसमें **इन्वॉयसिंग के लिए तैयार** के तौर पर चिह्नित कॉन्ट्रेक्ट लाइनें होती हैं, उन्हें प्रोजेक्ट की इनवॉइस लाइनों के तौर पर प्रोजेक्ट के इनवॉयस में कॉपी किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="8e49f-119">Any product that has contract lines that are marked **Ready to Invoice** is copied over to the project invoice as project invoice lines.</span></span>

<span data-ttu-id="8e49f-120">उत्पादों की बिलिंग के बैकलॉग की समीक्षा करने के लिए **बिक्री** \> **बिलिंग** \> **उत्पाद की बिलिंग का बैकलॉग** पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="8e49f-120">To review the billing backlog for products, go to **Sales** \> **Billing** \> **Product Billing Backlog**.</span></span> <span data-ttu-id="8e49f-121">सभी उत्पाद-आधारित कॉन्ट्रेक्ट लाइनों का चुनाव करें जो इन्वॉयसिंग के लिए तैयार हैं, और फिर **इन्वॉयसिंग के लिए तैयार** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="8e49f-121">Select all the product-based contract lines that are ready to be invoiced, and then select **Ready to Invoice**.</span></span> <span data-ttu-id="8e49f-122">इन लाइनों की बिलिंग की स्थिति को परिवर्तित कर **इन्वॉयसिंग के लिए तैयार** कर दिया गया है।</span><span class="sxs-lookup"><span data-stu-id="8e49f-122">The billing status of these lines is changed to **Ready to Invoice**.</span></span>

![उत्पाद की बिलिंग का बैकलॉग](media/ProductBacklog.png)

## <a name="review-billing-milestones-on-fixed-price-contracts"></a><span data-ttu-id="8e49f-124">फिक्स्ड-प्राइस कॉन्ट्रेक्ट के मामले में बिलिंग के महत्वपूर्ण चरणों की समीक्षा करें</span><span class="sxs-lookup"><span data-stu-id="8e49f-124">Review billing milestones on fixed-price contracts</span></span>

<span data-ttu-id="8e49f-125">फिक्स्ड-प्राइस बिलिंग विधि वाली प्रत्येक प्रोजेक्ट कॉन्ट्रेक्ट लाइन में कॉन्ट्रेक्ट से जुड़े महत्त्वपूर्ण चरण परिभाषित किये जाने चाहिए।</span><span class="sxs-lookup"><span data-stu-id="8e49f-125">Each project contract line that has a fixed-price billing method must define contract milestones.</span></span> <span data-ttu-id="8e49f-126">कॉन्ट्रेक्ट से जुड़े इन महत्त्वपूर्ण चरणों की इन्वॉयसिंग तभी की जा सकती है जब वे **इनवॉयसिंग के लिए तैयार** चिह्नित किये गए हों।</span><span class="sxs-lookup"><span data-stu-id="8e49f-126">These contract milestones can be invoiced only if they are marked **Ready to Invoice**.</span></span> 

<span data-ttu-id="8e49f-127">बिलिंग के महत्त्वपूर्ण चरणों की समीक्षा करने के लिए **बिक्री** \> **बिलिंग** \> **फिक्स्ड प्राइस के महत्त्वपूर्ण चरण** पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="8e49f-127">To review billing milestones, go to **Sales** \> **Billing** \> **Fixed Price Milestones**.</span></span> <span data-ttu-id="8e49f-128">इन्वॉयसिंग के लिए तैयार महत्त्वपूर्ण चरणों का चयन करें और फिर **इन्वॉयसिंग के लिए तैयार** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="8e49f-128">Select the milestones that are ready to be invoiced, and then select **Ready to invoice**.</span></span> <span data-ttu-id="8e49f-129">इन महत्त्वपूर्ण चरणों की बिलिंग की स्थिति परिवर्तित होकर **इन्वॉयसिंग के लिए तैयार** हो जाती है।</span><span class="sxs-lookup"><span data-stu-id="8e49f-129">The billing status of these milestones is changed to **Ready to Invoice**.</span></span>

![फिक्स्ड-प्राइस के मामले में महत्त्वपूर्ण चरण](media/FPBacklog.png)
