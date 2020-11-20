---
title: कैटलॉग उत्पाद के लिए लागत और विक्रय दर सेट अप करें - लाइट
description: यह विषय उत्पाद कैटलॉग में लागत और विक्रय की दरों को सेट करने संबंधी जानकारी देता है.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 135b182af73bdab7a3520589431332ad059ec497
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176703"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products---lite"></a><span data-ttu-id="93ffa-103">कैटलॉग उत्पाद के लिए लागत और विक्रय दर सेट अप करें - लाइट</span><span class="sxs-lookup"><span data-stu-id="93ffa-103">Set up cost and sales rates for catalog products - lite</span></span>

<span data-ttu-id="93ffa-104">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="93ffa-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="93ffa-105">Dynamics 365 प्रकल्प परिचालन में उत्पाद कैटलॉग वस्तुओं के मूल्य तय करन Dynamics 365 Sales के समान है.</span><span class="sxs-lookup"><span data-stu-id="93ffa-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="93ffa-106">चूंकि उत्पादों का अनुमान नही लगाया जा सकता या उन्हे प्रकल्प परिचालनों में इस्तेमाल नही किया जा सकता, ऎसे में उत्पाद कैटलॉग मूल्य को प्रकल्प मूल्य सूची में कोट और अनुबन्ध के लिये सेट करने की आवश्यकता नही होती है.</span><span class="sxs-lookup"><span data-stu-id="93ffa-106">Because products can't be estimated or used on projects in Project Operations, there is no need to set product catalog prices on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="93ffa-107">उत्पाद कैटलॉग मूल्य को **उत्पाद मूल्य** के अनुरुप सेट किया जाना चाहिये जो कि कोट फील्ड, अनुबन्ध या खाते के अनुसार हो.</span><span class="sxs-lookup"><span data-stu-id="93ffa-107">Product catalog prices should be set up in the **Product Price** field of a quote, contract, or account.</span></span> <span data-ttu-id="93ffa-108">उत्पाद कैटलॉग मूल्य को उत्पाद मूल्य सूची के अनुसार इन निकायों के अनुसार सेट नही करें.</span><span class="sxs-lookup"><span data-stu-id="93ffa-108">Don't set up product catalog prices in the project price lists for these entities.</span></span> <span data-ttu-id="93ffa-109">उत्पाद मूल्य सूची प्रकल्प परिचालन के लिये अलग होती है.</span><span class="sxs-lookup"><span data-stu-id="93ffa-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="93ffa-110">ये परिचालन विशेष व्यवसाय तर्क होता है जो कोट से अनुबन्ध तक मूल्य सूची की प्रति बनाता है.</span><span class="sxs-lookup"><span data-stu-id="93ffa-110">There is application-specific business logic that copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="93ffa-111">इसका परिणाम है अनुबंध आधारित प्रकल्प मूल्य सूची.</span><span class="sxs-lookup"><span data-stu-id="93ffa-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="93ffa-112">कॉपी परिचालन से कोट प्राप्त करने की प्रक्रिया धीमी हो सकती है यदि कोट पर दी गई प्रकल्प मूल्य सूची काफी बड़ी हो.</span><span class="sxs-lookup"><span data-stu-id="93ffa-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="93ffa-113">उत्पाद मूल्य सूची अनुबन्ध में मौजूद प्रमुख मूल्य सूची के लिये कॉपी नही की गई है.</span><span class="sxs-lookup"><span data-stu-id="93ffa-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="93ffa-114">इसका अर्थ है कि उत्पाद मूल्य सूची का प्रभाव कोट प्राप्त करने की प्रक्रिया पर नही पड़ता है.</span><span class="sxs-lookup"><span data-stu-id="93ffa-114">This means that product price lists don't impact the performance of the quote win process.</span></span>
