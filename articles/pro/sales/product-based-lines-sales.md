---
title: उत्पाद-आधारित अवसर पंक्तियाँ - लाइट
description: यह विषय Project Operations में उत्पाद आधारित अवसर लाइन आइटम के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 4f8da5258a1dd0aa4229654c0e1e222b8cf3a21a
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5272615"
---
# <a name="product-based-opportunity-lines---lite"></a><span data-ttu-id="e5cf5-103">उत्पाद-आधारित अवसर पंक्तियाँ - लाइट</span><span class="sxs-lookup"><span data-stu-id="e5cf5-103">Product-based opportunity lines - lite</span></span>

<span data-ttu-id="e5cf5-104">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="e5cf5-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e5cf5-105">उत्पाद आधारित अवसर लाइनें, अवसर पर लाइन आइटम हैं.</span><span class="sxs-lookup"><span data-stu-id="e5cf5-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="e5cf5-106">ये अलग-अलग पंक्ति आइटम उस संभावित इनवॉइस पर मौजूद हैं, जो ग्राहक को प्रदान किया गया.</span><span class="sxs-lookup"><span data-stu-id="e5cf5-106">These distinct line items are on the eventual invoice that is provided to the customer.</span></span> <span data-ttu-id="e5cf5-107">इनवॉइस में कोई अन्य अतिरिक्त सेवाएँ शामिल नहीं होती हैं.</span><span class="sxs-lookup"><span data-stu-id="e5cf5-107">The invoice doesn't include any other additional services.</span></span> <span data-ttu-id="e5cf5-108">संबद्ध ख़र्च और खपत किसी भी संबंधित परियोजनाओं के कार्यों पर ट्रैक नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="e5cf5-108">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="e5cf5-109">उत्पाद-आधारित लाइनें, कैटलॉग आइटम या राइट-इन उत्पाद हो सकती हैं.</span><span class="sxs-lookup"><span data-stu-id="e5cf5-109">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="e5cf5-110">अवसर के उत्पाद-आधारित लाइनों पर अधिकांश कार्यक्षमता Dynamics 365 Sales एप्लिकेशन द्वारा प्रदान की गई कार्यक्षमता का पालन करती है.</span><span class="sxs-lookup"><span data-stu-id="e5cf5-110">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="e5cf5-111">उत्पाद-आधारित अवसर लाइनों के बारे में अधिक जानकारी के लिए, देखें [एक अवसर के लिए उत्पादों को जोड़ें](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="e5cf5-111">For more information about product-based opportunity lines, see [Add products to an opportunity](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="e5cf5-112">**ग्राहक बजट** एक अवधारणा है, जो परियोजना-आधारित अवसर पंक्तियों के लिए विशिष्ट है.</span><span class="sxs-lookup"><span data-stu-id="e5cf5-112">**Customer budget** is a concept that is specific to project-based opportunity lines.</span></span> <span data-ttu-id="e5cf5-113">**ग्राहक बजट** फ़ील्ड उस राशि को ट्रैक करती है, जो ग्राहक आइटम के लिए भुगतान करने के लिए तैयार है.</span><span class="sxs-lookup"><span data-stu-id="e5cf5-113">The **Customer budget** field tracks the amount the customer is willing to pay for the item.</span></span>

<span data-ttu-id="e5cf5-114">जब अवसर सारांश की आय विधि **सिस्टम परिकलित** होती है, तो अवसर पंक्तियों पर ग्राहक बजट मान अनुमानित आय को परिकलित करने के लिए सारांशित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="e5cf5-114">When the revenue method of the Opportunity summary is **System Calculated**, the customer budget values across the opportunity lines are summarized to calculate the estimated revenue.</span></span> 



[!INCLUDE[footer-include](../../includes/footer-banner.md)]