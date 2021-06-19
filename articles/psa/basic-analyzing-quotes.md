---
title: प्रोजेक्ट कोटेशन का विश्लेषण
description: यह विषय प्रोजेक्ट कोटेशन के विश्लेषण के बारे में जानकारी प्रदान करता है।
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
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
ms.openlocfilehash: acb3f1a2020cfd59f60f828e9092bd7ccde00077
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012453"
---
# <a name="analysis-of-project-quotes"></a><span data-ttu-id="a1545-103">प्रोजेक्ट कोटेशन का विश्लेषण</span><span class="sxs-lookup"><span data-stu-id="a1545-103">Analysis of project quotes</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a1545-104">Dynamics 365 Project Service Automation लाभप्रदता का अनुमान लगाने के लिए प्रोजेक्ट कोटेशन का विश्लेषण करता है।</span><span class="sxs-lookup"><span data-stu-id="a1545-104">Dynamics 365 Project Service Automation analyzes project quotes to estimate profitability.</span></span> <span data-ttu-id="a1545-105">यह भी विश्लेषण करता है कि डिलीवरी की तारीख या पूर्णता तिथि और बजट के बारे में ग्राहकों की अपेक्षाओं के साथ कोटेशन कितनी अच्छी तरह से मेल खाता है।</span><span class="sxs-lookup"><span data-stu-id="a1545-105">It also analyzes how well the quote is aligned with customer expectations about the delivery date or completion date, and about the budget.tions.</span></span>

## <a name="profitability-analysis"></a><span data-ttu-id="a1545-106">लाभप्रदता का विश्लेषण</span><span class="sxs-lookup"><span data-stu-id="a1545-106">Profitability analysis</span></span>

<span data-ttu-id="a1545-107">Project Service Automation सकल मार्जिन और समायोजित सकल मार्जिन का उपयोग करके लाभप्रदता का विश्लेषण करता है।</span><span class="sxs-lookup"><span data-stu-id="a1545-107">Project Service Automation analyzes profitability by using the gross margin and the adjusted gross margin.</span></span>

- <span data-ttu-id="a1545-108">सकल मार्जिन की गणना निम्न सूत्र का उपयोग करके की जाती है:</span><span class="sxs-lookup"><span data-stu-id="a1545-108">Gross margins are calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- <span data-ttu-id="a1545-109">समायोजित सकल मार्जिन की गणना निम्न सूत्र का उपयोग करके की जाती है:</span><span class="sxs-lookup"><span data-stu-id="a1545-109">The adjusted gross margin is calculated by using the following formula:</span></span>

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

<span data-ttu-id="a1545-110">यदि सकल मार्जिन और समायोजित सकल मार्जिन के लिए मान एक विस्तृत मार्जिन से भिन्न होते हैं, तो कोटेशन में अधिकांश काम गैर-प्रभार्य के रूप में वर्गीकृत किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="a1545-110">If the values for gross margin and adjusted gross margin differ by a wide margin, much of the work in the quote is classified as non-chargeable.</span></span>

## <a name="analysis-of-customer-expectations"></a><span data-ttu-id="a1545-111">ग्राहक की उम्मीदों का विश्लेषण</span><span class="sxs-lookup"><span data-stu-id="a1545-111">Analysis of customer expectations</span></span>

<span data-ttu-id="a1545-112">यदि आप निम्न फ़ील्ड के लिए मान दर्ज करते हैं, तो शेड्यूल और बजट के बारे में ग्राहकों की अपेक्षाओं के लिए आप कोटेशन का विश्लेषण और चार्ट तैयार कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="a1545-112">You can analyze quotes and generate charts for customer expectations about the schedule and budget if you enter values for the following fields:</span></span>

- <span data-ttu-id="a1545-113">कोटेशन हेडर पर **अनुरोधित डिलीवरी की तिथि** फ़ील्ड.</span><span class="sxs-lookup"><span data-stu-id="a1545-113">The **Requested delivery date** field on the quote header.</span></span>
- <span data-ttu-id="a1545-114">**ग्राहक बजट** प्रत्येक कोटेशन लाइन (प्रोजेक्ट-आधारित लाइनों और उत्पाद-आधारित लाइनों के लिए)।</span><span class="sxs-lookup"><span data-stu-id="a1545-114">The **Customer budget** field for each quote line (for project-based lines and product-based lines).</span></span>

<span data-ttu-id="a1545-115">शेड्यूल के बारे में ग्राहकों की अपेक्षाओं का विश्लेषण कोटेशन लाइन की नवीनतम अंतिम तिथि को कोटेशन में सभी कोटेशन लाइनों में अनुरोधित डिलीवरी तिथि के साथ तुलना करके किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="a1545-115">Analysis of customer expectations about the schedule is done by comparing the latest end date of the quote line detail with the requested delivery date across all quote lines in the quote.</span></span>

<span data-ttu-id="a1545-116">बजट के बारे में ग्राहकों की अपेक्षाओं का विश्लेषण कुल ग्राहक बजट के योग की तुलना में सभी कोटेशन लाइनों में कोटेशन की राशि के साथ किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="a1545-116">Analysis of customer expectations about the budget is done by comparing the sum of the total customer budget with the quoted amount across all quote lines.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]