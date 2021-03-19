---
title: कैटलॉग उत्पाद के लिए लागत और विक्रय दर सेट अप करें - लाइट
description: यह विषय उत्पाद कैटलॉग में लागत और विक्रय की दरों को सेट करने संबंधी जानकारी देता है.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f0941c549cc38f0938a5819e8cb6ca9912f14790
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5274460"
---
# <a name="set-up-cost-and-sales-rates-for-catalog-products---lite"></a><span data-ttu-id="a42f7-103">कैटलॉग उत्पाद के लिए लागत और विक्रय दर सेट अप करें - लाइट</span><span class="sxs-lookup"><span data-stu-id="a42f7-103">Set up cost and sales rates for catalog products - lite</span></span>

<span data-ttu-id="a42f7-104">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="a42f7-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="a42f7-105">Dynamics 365 Project Operations में उत्पाद कैटलॉग के लिए मूल्य निर्धारण सेट अप करना Dynamics 365 Sales में सेट अप करने के समान होता है.</span><span class="sxs-lookup"><span data-stu-id="a42f7-105">Setting up pricing for product catalog items in Dynamics 365 Project Operations is the same as in Dynamics 365 Sales.</span></span>

<span data-ttu-id="a42f7-106">Project Operations में, उत्पादों का परियोजनाओं पर अनुमान नहीं लगाया जा सकता है या उपयोग नहीं किया जा सकता है, इसलिए कोट और अनुबंधों के लिए उत्पाद कैटलॉग मूल्यों को परियोजना मूल्य सूचियों पर सेट किए जाने की आवश्यकता नहीं होती है.</span><span class="sxs-lookup"><span data-stu-id="a42f7-106">In Project Operations, products can't be estimated or used on projects, so product catalog prices don't need to be set on project price lists for quotes and contracts.</span></span>

<span data-ttu-id="a42f7-107">उत्पाद कैटलॉग मूल्य सेट अप करने के लिए, कोट, अनुबंध या खाते की **उत्पाद मूल्य** फ़ील्ड का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="a42f7-107">Use the **Product Price** field of a quote, contract, or account to set up product catalog prices.</span></span> <span data-ttu-id="a42f7-108">परियोजना मूल्य सूची में उत्पाद कैटलॉग मूल्य सेट अप न करें.</span><span class="sxs-lookup"><span data-stu-id="a42f7-108">Don't set up product catalog prices in the project price lists.</span></span> <span data-ttu-id="a42f7-109">उत्पाद मूल्य सूची प्रकल्प परिचालन के लिये अलग होती है.</span><span class="sxs-lookup"><span data-stu-id="a42f7-109">Project price lists are exclusive to Project Operations.</span></span> <span data-ttu-id="a42f7-110">एप्लिकेशन-विशिष्ट व्यावसायिक तर्क मूल्य सूची की कोट से अनुबंध पर प्रतिलिपि बनाते हैं.</span><span class="sxs-lookup"><span data-stu-id="a42f7-110">Application-specific business logic copies the price lists from a quote to a contract.</span></span> <span data-ttu-id="a42f7-111">इसका परिणाम है अनुबंध आधारित प्रकल्प मूल्य सूची.</span><span class="sxs-lookup"><span data-stu-id="a42f7-111">The result is a contract-specific project price list.</span></span> <span data-ttu-id="a42f7-112">कॉपी परिचालन से कोट प्राप्त करने की प्रक्रिया धीमी हो सकती है यदि कोट पर दी गई प्रकल्प मूल्य सूची काफी बड़ी हो.</span><span class="sxs-lookup"><span data-stu-id="a42f7-112">The copy operation can delay the quote win process if the project price list on the quote gets too large.</span></span> <span data-ttu-id="a42f7-113">उत्पाद मूल्य सूची अनुबन्ध में मौजूद प्रमुख मूल्य सूची के लिये कॉपी नही की गई है.</span><span class="sxs-lookup"><span data-stu-id="a42f7-113">Product price lists aren't copied to create custom price lists on contracts.</span></span> <span data-ttu-id="a42f7-114">क्योंकि इसमें कोई प्रतिलिपि बनाना शामिल नहीं है, इसलिए कोट प्रक्रिया का प्रदर्शन प्रभावित नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="a42f7-114">Because there's no copying involved, the performance of the quote process isn't affected.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]