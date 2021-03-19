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
ms.openlocfilehash: 98a61746f172b50bf6fa29cb0d21462cd616f417
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286520"
---
# <a name="resource-estimates"></a><span data-ttu-id="71891-103">संसाधन का अनुमान</span><span class="sxs-lookup"><span data-stu-id="71891-103">Resource estimates</span></span>

<span data-ttu-id="71891-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="71891-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="71891-105">संसाधन के अनुमान चरणबद्ध प्रयासों से आते हैं, जो लागू मूल्य निर्धारण आयामों के साथ-साथ काम के रुकने की संरचना में परिभाषित होते हैं।</span><span class="sxs-lookup"><span data-stu-id="71891-105">Resource estimates come from time-phased effort that is defined in the work breakdown structure along with applicable pricing dimensions.</span></span> <span data-ttu-id="71891-106">आमतौर पर, गणना **प्रत्येक भूमिका x घंटे के लिए दर/घंटा है।**</span><span class="sxs-lookup"><span data-stu-id="71891-106">Typically, the calculation is **rate/hr for each role x hours.**</span></span> <span data-ttu-id="71891-107">प्रत्येक संसाधन के लिए चरणबद्ध प्रयास संसाधन को असाइनमेंट रिकॉर्ड में रखा जाता है।</span><span class="sxs-lookup"><span data-stu-id="71891-107">The time-phased effort for each resource is stored in the resource assignment record.</span></span> <span data-ttu-id="71891-108">मूल्य निर्धारण को पूर्व-निर्धारित मूल्य सूची में रखा जाता है।</span><span class="sxs-lookup"><span data-stu-id="71891-108">The pricing is stored in a pre-defined price list.</span></span> <span data-ttu-id="71891-109">लागू मूल्य सूची के आधार पर इकाई रूपांतरण लागू किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="71891-109">Unit conversion is applied based on the applicable price list.</span></span>

![संसाधन का अनुमान](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a><span data-ttu-id="71891-111">डिफ़ॉल्ट लागत मूल्य और लागत मुद्रा</span><span class="sxs-lookup"><span data-stu-id="71891-111">Default cost price and cost currency</span></span>

<span data-ttu-id="71891-112">संगठनात्मक इकाई से लागत मूल्य डिफ़ॉल्ट हैं।</span><span class="sxs-lookup"><span data-stu-id="71891-112">Cost prices are defaulted from the Organizational Unit.</span></span>

## <a name="default-bill-rate-and-sales-currency"></a><span data-ttu-id="71891-113">डिफ़ॉल्ट बिल दर और बिक्री मुद्रा</span><span class="sxs-lookup"><span data-stu-id="71891-113">Default bill rate and sales currency</span></span>

<span data-ttu-id="71891-114">बिक्री मूल्य प्रति सौदा एक बार लागू होते हैं।</span><span class="sxs-lookup"><span data-stu-id="71891-114">Sales prices are applied once per deal.</span></span> <span data-ttu-id="71891-115">बिक्री मूल्य सूची डिफ़ॉल्ट के लिए पदानुक्रम इस प्रकार है:</span><span class="sxs-lookup"><span data-stu-id="71891-115">The hierarchy for sale price list defaulting is as follows:</span></span>

1. <span data-ttu-id="71891-116">संगठन</span><span class="sxs-lookup"><span data-stu-id="71891-116">Organization</span></span>
2. <span data-ttu-id="71891-117">ग्राहक</span><span class="sxs-lookup"><span data-stu-id="71891-117">Customer</span></span>
3. <span data-ttu-id="71891-118">कोट/अनुबंध</span><span class="sxs-lookup"><span data-stu-id="71891-118">Quote/contract</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]