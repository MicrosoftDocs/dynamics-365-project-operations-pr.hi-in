---
title: संसाधन का अनुमान
description: यह विषय परियोजना संचालन में संसाधन अनुमान की गणना के बारे में जानकारी देता है।
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 454b8931db53739a7bc19364911109802a1ed087
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127364"
---
# <a name="resource-estimates"></a><span data-ttu-id="e2751-103">संसाधन का अनुमान</span><span class="sxs-lookup"><span data-stu-id="e2751-103">Resource estimates</span></span>

<span data-ttu-id="e2751-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="e2751-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e2751-105">संसाधन के अनुमान चरणबद्ध प्रयासों से आते हैं, जो लागू मूल्य निर्धारण आयामों के साथ-साथ काम के रुकने की संरचना में परिभाषित होते हैं।</span><span class="sxs-lookup"><span data-stu-id="e2751-105">Resource estimates come from time-phased effort that is defined in the work breakdown structure along with applicable pricing dimensions.</span></span> <span data-ttu-id="e2751-106">आमतौर पर, गणना **प्रत्येक भूमिका x घंटे के लिए दर/घंटा है।**</span><span class="sxs-lookup"><span data-stu-id="e2751-106">Typically, the calculation is **rate/hr for each role x hours.**</span></span> <span data-ttu-id="e2751-107">प्रत्येक संसाधन के लिए चरणबद्ध प्रयास संसाधन को असाइनमेंट रिकॉर्ड में रखा जाता है।</span><span class="sxs-lookup"><span data-stu-id="e2751-107">The time-phased effort for each resource is stored in the resource assignment record.</span></span> <span data-ttu-id="e2751-108">मूल्य निर्धारण को पूर्व-निर्धारित मूल्य सूची में रखा जाता है।</span><span class="sxs-lookup"><span data-stu-id="e2751-108">The pricing is stored in a pre-defined price list.</span></span> <span data-ttu-id="e2751-109">लागू मूल्य सूची के आधार पर इकाई रूपांतरण लागू किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="e2751-109">Unit conversion is applied based on the applicable price list.</span></span>

![संसाधन का अनुमान](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a><span data-ttu-id="e2751-111">डिफ़ॉल्ट लागत मूल्य और लागत मुद्रा</span><span class="sxs-lookup"><span data-stu-id="e2751-111">Default cost price and cost currency</span></span>

<span data-ttu-id="e2751-112">संगठनात्मक इकाई से लागत मूल्य डिफ़ॉल्ट हैं।</span><span class="sxs-lookup"><span data-stu-id="e2751-112">Cost prices are defaulted from the Organizational Unit.</span></span>

## <a name="default-bill-rate-and-sales-currency"></a><span data-ttu-id="e2751-113">डिफ़ॉल्ट बिल दर और बिक्री मुद्रा</span><span class="sxs-lookup"><span data-stu-id="e2751-113">Default bill rate and sales currency</span></span>

<span data-ttu-id="e2751-114">बिक्री मूल्य प्रति सौदा एक बार लागू होते हैं।</span><span class="sxs-lookup"><span data-stu-id="e2751-114">Sales prices are applied once per deal.</span></span> <span data-ttu-id="e2751-115">बिक्री मूल्य सूची डिफ़ॉल्ट के लिए पदानुक्रम इस प्रकार है:</span><span class="sxs-lookup"><span data-stu-id="e2751-115">The hierarchy for sale price list defaulting is as follows:</span></span>

1. <span data-ttu-id="e2751-116">संगठन</span><span class="sxs-lookup"><span data-stu-id="e2751-116">Organization</span></span>
2. <span data-ttu-id="e2751-117">ग्राहक</span><span class="sxs-lookup"><span data-stu-id="e2751-117">Customer</span></span>
3. <span data-ttu-id="e2751-118">कोट/अनुबंध</span><span class="sxs-lookup"><span data-stu-id="e2751-118">Quote/contract</span></span>
