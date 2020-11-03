---
title: कोटिंग, मूल्य निर्धारण और बिलिंग के लिए मूल मार्गदर्शिका
description: यह विषय Project Service Automation में मूल कोटिंग, मूल्य निर्धारण और बिलिंग के बारे में जानकारी प्रदान करता है।
author: kfend
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 2/14/2019
ms.topic: article
ms.author: kfend
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 986b073e7ee13b88f8516f92220b1e313a083bc0
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077803"
---
# <a name="basic-guide-to-quoting-pricing-and-billing"></a><span data-ttu-id="c2e2a-103">कोटिंग, मूल्य निर्धारण और बिलिंग के लिए मूल मार्गदर्शिका</span><span class="sxs-lookup"><span data-stu-id="c2e2a-103">Basic guide to quoting, pricing and billing</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="c2e2a-104">सही समय पर सही संसाधन खोजने की क्षमता, उन संसाधनों को प्रोजेक्ट पर बुक करना और संसाधनों का उपयोग करना संगठनों को राजस्व लक्ष्य और ग्राहक संतुष्टि लक्ष्यों को पूरा करने में मदद करता है।</span><span class="sxs-lookup"><span data-stu-id="c2e2a-104">The ability to find the right resources at the right time, book those resources on projects, and keep resources utilized helps organizations meet revenue targets and customer satisfaction goals.</span></span> 

<span data-ttu-id="c2e2a-105">इस विषय में पहले जो PDF लिंक था उसे हटा दिया गया है और सामग्री को निम्नलिखित विषयों में ले जाया गया है:</span><span class="sxs-lookup"><span data-stu-id="c2e2a-105">The PDF link that was previously in this topic has been removed and the content has been moved to the following topics:</span></span>

- [<span data-ttu-id="c2e2a-106">कोटिंग, मूल्य निर्धारण और बिलिंग</span><span class="sxs-lookup"><span data-stu-id="c2e2a-106">Quoting, pricing, and billing</span></span>](../quote-bill-price.md)
- [<span data-ttu-id="c2e2a-107">बिक्री प्रक्रियाएँ</span><span class="sxs-lookup"><span data-stu-id="c2e2a-107">Sales processes</span></span>](../basic-sales-process.md)
- [<span data-ttu-id="c2e2a-108">कोट और कोट पंक्तियाँ</span><span class="sxs-lookup"><span data-stu-id="c2e2a-108">Quotes and quote lines</span></span>](../basic-quote-lines.md)
- [<span data-ttu-id="c2e2a-109">उत्पाद-आधारित कोट पंक्तियाँ</span><span class="sxs-lookup"><span data-stu-id="c2e2a-109">Product-based quote lines</span></span>](../product-based-quote-lines.md)
- [<span data-ttu-id="c2e2a-110">मूल्य लगाना</span><span class="sxs-lookup"><span data-stu-id="c2e2a-110">Pricing</span></span>](../basic-pricing.md)
- [<span data-ttu-id="c2e2a-111">उत्पाद कैटलॉग मूल्य निर्धारण</span><span class="sxs-lookup"><span data-stu-id="c2e2a-111">Product catalog pricing</span></span>](../product-catalog-pricing.md)
- [<span data-ttu-id="c2e2a-112">व्यावसायिक लेनदेन</span><span class="sxs-lookup"><span data-stu-id="c2e2a-112">Business transactions</span></span>](../basic-business-transactions.md)
- [<span data-ttu-id="c2e2a-113">अनुमान</span><span class="sxs-lookup"><span data-stu-id="c2e2a-113">Estimates</span></span>](../estimates.md)
- [<span data-ttu-id="c2e2a-114">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="c2e2a-114">Actuals</span></span>](../actuals.md)
- [<span data-ttu-id="c2e2a-115">प्रोजेक्ट कोट का विश्लेषण करना</span><span class="sxs-lookup"><span data-stu-id="c2e2a-115">Analyzing project quotes</span></span>](../basic-analyzing-quotes.md)
- [<span data-ttu-id="c2e2a-116">संगठनात्मक इकाइयाँ</span><span class="sxs-lookup"><span data-stu-id="c2e2a-116">Organizational units</span></span>](../advanced-organizational.md)
- [<span data-ttu-id="c2e2a-117">इकाई समूह और इकाइयाँ</span><span class="sxs-lookup"><span data-stu-id="c2e2a-117">Unit groups and units</span></span>](../advanced-units.md)
- [<span data-ttu-id="c2e2a-118">Multi-currency परिदृश्य</span><span class="sxs-lookup"><span data-stu-id="c2e2a-118">Multi-currency scenarios</span></span>](../advanced-currency.md)
- [<span data-ttu-id="c2e2a-119">वास्तविक की रिकॉर्डिंग</span><span class="sxs-lookup"><span data-stu-id="c2e2a-119">Recording actuals</span></span>](../advanced-actuals.md)

> [!NOTE]
> <span data-ttu-id="c2e2a-120">यह विषय भविष्य के दस्तावेज़ अपडेट में हटा दिया जाएगा।</span><span class="sxs-lookup"><span data-stu-id="c2e2a-120">This topic will be removed in a future documentation update.</span></span> 
