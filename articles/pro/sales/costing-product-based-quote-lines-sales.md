---
title: उत्पाद-आधारित कोट लागत
description: यह विषय उत्पाद-आधारित कोट लाइन पर लागत मूल्य लागू करने के बारे में जानकारी देता है.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 1fa7896e249abfefd3e93cba4bad789e67e14f31
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003453"
---
# <a name="costing-product-based-quote-lines"></a><span data-ttu-id="ccb2a-103">उत्पाद-आधारित कोट लागत</span><span class="sxs-lookup"><span data-stu-id="ccb2a-103">Costing product-based quote lines</span></span>

<span data-ttu-id="ccb2a-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="ccb2a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="ccb2a-105">Dynamics 365 Project Operations में उत्पाद-आधारित कोट लाइनों की भी एक **लागत मूल्य** फ़ील्ड होती है.</span><span class="sxs-lookup"><span data-stu-id="ccb2a-105">Product-based quote lines in Dynamics 365 Project Operations also have a **Cost Price** field.</span></span> <span data-ttu-id="ccb2a-106">इस फ़ील्ड का इस्तेमाल उत्पाद की कोट लाइन पर और डाउनस्ट्रीम लाभ क्षमता की गणना के लिए लागत मूल्य पर नज़र रखने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="ccb2a-106">This field is used to track the cost price for the product on the quote line and for downstream profitability calculations.</span></span>

<span data-ttu-id="ccb2a-107">जब कैटलॉग उत्पाद के लिए उत्पाद-आधारित कोट लाइन बनाई जाती है, उत्पाद-आधारित कोट लाइन की लागत उत्पाद सूची में **मानक लागत** फ़ील्ड से डिफ़ॉल्ट होती है.</span><span class="sxs-lookup"><span data-stu-id="ccb2a-107">When a product-based quote line is created for a catalog product, the cost of the product-based quote line is defaulted from the **Standard Cost** field in the product catalog.</span></span> <span data-ttu-id="ccb2a-108">उत्पाद कैटलॉग में मानक लागत फ़ील्ड संगठन की आधार मुद्रा में सेट किया गया है.</span><span class="sxs-lookup"><span data-stu-id="ccb2a-108">The standard cost field in the product catalog is set up in the Organization's base currency.</span></span> <span data-ttu-id="ccb2a-109">उत्पाद-आधारित कोट लाइन पर डिफ़ॉल्ट इकाई लागत कोट पर बिक्री मुद्रा में परिवर्तित हो जाती है.</span><span class="sxs-lookup"><span data-stu-id="ccb2a-109">The default unit cost on the product-based quote line is converted to the sales currency on the quote.</span></span>

## <a name="unit-cost-on-a-product-based-quote-line"></a><span data-ttu-id="ccb2a-110">उत्पाद-आधारित कोट लाइन पर इकाई लागत</span><span class="sxs-lookup"><span data-stu-id="ccb2a-110">Unit cost on a product-based quote line</span></span>

<span data-ttu-id="ccb2a-111">उत्पाद-आधारित कोट लाइन पर इकाई लागत होने का उद्देश्य प्रत्येक बिक्री के लिए उत्पाद हेतु अलग-अलग लागतों की अनुमति देना है.</span><span class="sxs-lookup"><span data-stu-id="ccb2a-111">The purpose of having a unit cost on a product-based quote line is to allow for different costs for a product for each sale.</span></span> <span data-ttu-id="ccb2a-112">यह विशिष्ट परिदृश्य नहीं है, लेकिन कभी-कभी अंतिम बिक्री के ग्राहक के आधार पर आपूर्तिकर्ता द्वारा उत्पाद की लागत में छूट दी जा सकती है.</span><span class="sxs-lookup"><span data-stu-id="ccb2a-112">This is not a typical scenario, but sometimes the cost of the product may be discounted by the supplier depending on the customer of the final sale.</span></span>

<span data-ttu-id="ccb2a-113">उदाहरण के लिए:</span><span class="sxs-lookup"><span data-stu-id="ccb2a-113">For example:</span></span>

<span data-ttu-id="ccb2a-114">Fabrikam Robotics, Adatum कॉर्पोरेशन की असेंबली लाइनों में रोबोटिक टुकड़ियाँ इंस्टॉल कर रहा है.</span><span class="sxs-lookup"><span data-stu-id="ccb2a-114">Fabrikam Robotics is installing robotic arms at A Datum Corporation's assembly lines.</span></span> <span data-ttu-id="ccb2a-115">Fabrikam इंस्टॉलेशन सेवाएं प्रदान करता है, लेकिन रोबोटिक आर्म्स Trey robotics से खरीदे जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="ccb2a-115">Fabrikam provides installation services but the robotic arms are procured from Trey robotics.</span></span> <span data-ttu-id="ccb2a-116">यदि A Datum Corporation में रोबोटिक आर्म्स का इंस्टॉलेशन,Trey के रोबोटिक आर्म्स के लिए नया उद्योग परिक्षेत्र खोलती है, Trey इस डील के लिए Fabrikam को विशेष छूट दे सकता है.</span><span class="sxs-lookup"><span data-stu-id="ccb2a-116">If the installation of robotic arms at A Datum Corporation opens a new industry vertical for Trey's robotic arms, Trey could give a special discount for this deal to Fabrikam.</span></span>

<span data-ttu-id="ccb2a-117">इस मामले में, Fabrikam रोबोटिक आर्म्स के लिए उत्पाद-आधारित कोट लाइन बनाएगा और इस कोट के लिए विशेष प्रति इकाई लागत इनपुट देगा.</span><span class="sxs-lookup"><span data-stu-id="ccb2a-117">In this case, Fabrikam will create product-based quote line for Robotic Arms and input a special per unit cost for this quote.</span></span> <span data-ttu-id="ccb2a-118">यह लागत Trey रोबोटिक आर्म्स की मानक लागत से अलग है.</span><span class="sxs-lookup"><span data-stu-id="ccb2a-118">This cost is different from the standard cost of Trey Robotic Arms.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]