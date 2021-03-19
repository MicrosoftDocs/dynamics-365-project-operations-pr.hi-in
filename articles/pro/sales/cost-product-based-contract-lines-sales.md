---
title: उत्पाद-आधारित अनुबंध पंक्ति लागत - लाइट
description: यह विषय बनाने के बारे में जानकारी प्रदान करता है
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 001b0b54abcdd5fcd1eca7f3271cc78392f68860
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5273695"
---
# <a name="cost-product-based-contract-lines---lite"></a><span data-ttu-id="f7d40-103">उत्पाद-आधारित अनुबंध पंक्ति लागत - लाइट</span><span class="sxs-lookup"><span data-stu-id="f7d40-103">Cost product-based contract lines - lite</span></span>

<span data-ttu-id="f7d40-104">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="f7d40-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="f7d40-105">Dynamics 365 Project Operations में उत्पाद आधारित अनुबंध पंक्तियों में **लागत मूल्य** फ़ील्ड शामिल होती है, जो डाउनस्ट्रीम लाभप्रदता गणना के लिए उत्पाद की लागत मूल्य को संग्रहित करती है.</span><span class="sxs-lookup"><span data-stu-id="f7d40-105">Product-based contract lines in Dynamics 365 Project Operations include the **Cost Price** field, which stores the cost price of the product for downstream profitability calculations.</span></span>

<span data-ttu-id="f7d40-106">जब कैटलॉग उत्पाद के लिए उत्पाद-आधारित अनुबंध पंक्ति बनाई जाती है, तो उत्पाद कैटलॉग में पंक्ति की लागत **मानक लागत** से डिफ़ॉल्ट होती है.</span><span class="sxs-lookup"><span data-stu-id="f7d40-106">When a product-based contract line is created for a catalog product, the cost of the line defaults from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="f7d40-107">उत्पाद कैटलॉग में **मानक लागत** फ़ील्ड संगठन की आधार मुद्रा में सेट किया गया है.</span><span class="sxs-lookup"><span data-stu-id="f7d40-107">The **Standard Cost** field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="f7d40-108">जब अनुबंध लाइन पर इकाई लागत डिफ़ॉल्ट होती है, तो यह अनुबंध पर बिक्री मुद्रा में बदल गया होता है.</span><span class="sxs-lookup"><span data-stu-id="f7d40-108">When the unit cost defaults on the contract line, it's converted into the sales currency on the contract.</span></span>

## <a name="unit-cost-on-a-product-based-contract-line"></a><span data-ttu-id="f7d40-109">उत्पाद-आधारित अनुबंध लाइन पर इकाई लागत</span><span class="sxs-lookup"><span data-stu-id="f7d40-109">Unit cost on a product-based contract line</span></span>

<span data-ttu-id="f7d40-110">उत्पाद-आधारित अनुबंध लाइन पर एक इकाई लागत होने से एक इकाई की प्रत्येक बिक्री के लिए विभिन्न उत्पाद लागतों की अनुमति मिलती है.</span><span class="sxs-lookup"><span data-stu-id="f7d40-110">Having a unit cost on a product-based contract line allows for different product costs for each sale of a unit.</span></span> <span data-ttu-id="f7d40-111">जबकि हमेशा आवश्यक नहीं है, कुछ परिदृश्य हैं जहां आपूर्तिकर्ता द्वारा ग्राहक के लिए उत्पाद की लागत में छूट दी जा सकती है.</span><span class="sxs-lookup"><span data-stu-id="f7d40-111">While not always necessary, there are certain scenarios where the cost of the product may be discounted for the customer by the supplier.</span></span> <span data-ttu-id="f7d40-112">निम्न परिदृश्य पर विचार करें:</span><span class="sxs-lookup"><span data-stu-id="f7d40-112">Consider the following scenario:</span></span>

<span data-ttu-id="f7d40-113">Fabrikam Robotics, Adatum कॉर्पोरेशन की असेंबली लाइनों में रोबोटिक टुकड़ियाँ इंस्टॉल कर रहा है.</span><span class="sxs-lookup"><span data-stu-id="f7d40-113">Fabrikam Robotics is installing robotic arms at Adatum Corporation's assembly lines.</span></span> <span data-ttu-id="f7d40-114">Fabrikam स्थापना सेवाएं प्रदान करता है, लेकिन Robotic Arms, Trey Research से है.</span><span class="sxs-lookup"><span data-stu-id="f7d40-114">Fabrikam provides installation services but the robotic arms are from Trey Research.</span></span> <span data-ttu-id="f7d40-115">यदि Adatum कॉर्पोरेशन में रोबोटिक टुकड़ियाँ का इंस्टॉलेशन Trey Research के लिए एक नया उद्योग सिरा खोलता है, तो वे Fabrikam को इस सौदे के लिए एक विशेष छूट की पेशकश कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="f7d40-115">If the installation of robotic arms at Adatum Corporation opens a new industry vertical for Trey Research, they could offer a special discount for this deal to Fabrikam.</span></span> <span data-ttu-id="f7d40-116">इस मामले में, Fabrikam, Robotic Arms के लिए उत्पाद-आधारित अनुबंध पंक्ति बनाता है.</span><span class="sxs-lookup"><span data-stu-id="f7d40-116">In this case, Fabrikam creates a product-based contract line for Robotic Arms.</span></span> <span data-ttu-id="f7d40-117">इस अनुबंध के लिए प्रति इकाई लागत दर्ज की जाती है.</span><span class="sxs-lookup"><span data-stu-id="f7d40-117">A per unit cost is entered for this contract.</span></span> <span data-ttu-id="f7d40-118">लागत Trey Research से Robotic Arms की लागत से अलग है.</span><span class="sxs-lookup"><span data-stu-id="f7d40-118">The cost is different from the cost of robotic arms from Trey Research.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]