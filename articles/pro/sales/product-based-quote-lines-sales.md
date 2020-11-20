---
title: उत्पाद-आधारित कोट पंक्तियाँ ओवरव्यू - लाइट
description: यह विषय उत्पाद-आधारित कोट पंक्तियों के साथ कार्य करने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/30/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: f6aa428c486f149308ad078f9d7a80a0be0f0f04
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/30/2020
ms.locfileid: "4178190"
---
# <a name="product-based-quote-lines-overview---lite"></a><span data-ttu-id="03ca6-103">उत्पाद-आधारित कोट पंक्तियाँ ओवरव्यू - लाइट</span><span class="sxs-lookup"><span data-stu-id="03ca6-103">Product-based quote lines overview - lite</span></span>

<span data-ttu-id="03ca6-104">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="03ca6-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="03ca6-105">आप Dynamics 365 Project Operations में उत्पाद-आधारित कोट पंक्तियाँ बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="03ca6-105">You can create product-based quote lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="03ca6-106">उत्पाद-आधारित कोट पंक्तियों को मैनुअल रूप से जोड़ा जा सकता है या वे उत्पाद कैटलॉग का आइटम हो सकती हैं.</span><span class="sxs-lookup"><span data-stu-id="03ca6-106">Product-based quote lines can be manually added, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="03ca6-107">उत्पाद कैटलॉग</span><span class="sxs-lookup"><span data-stu-id="03ca6-107">Product catalog</span></span>

<span data-ttu-id="03ca6-108">उत्पाद कैटलॉग के प्रत्येक उत्पाद की एक डिफ़ॉल्ट इकाई और इकाई समूह होता है.</span><span class="sxs-lookup"><span data-stu-id="03ca6-108">Each product in the product catalog has a default unit and unit group.</span></span> <span data-ttu-id="03ca6-109">यदि कई उत्पाद एट्रिब्यूट के समान सेट को साझा करते हैं, तो आप एक ऐसा उत्पाद समूह बना सकते हैं, जो उन एट्रिब्यूट को साझा करता है.</span><span class="sxs-lookup"><span data-stu-id="03ca6-109">If multiple products share the same set of attributes, you can create a product family that share those attributes.</span></span> 

<span data-ttu-id="03ca6-110">उदाहरण के लिए, एक कंपनी विभिन्न सॉफ्टवेयरों के लिए सदस्यता लाइसेंस बेचती है।</span><span class="sxs-lookup"><span data-stu-id="03ca6-110">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="03ca6-111">सभी सदस्यता सॉफ्टवेयर में निम्नलिखित दो विशेषताएं होती हैं:</span><span class="sxs-lookup"><span data-stu-id="03ca6-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="03ca6-112">उपयोगकर्ताओं की संख्या</span><span class="sxs-lookup"><span data-stu-id="03ca6-112">Number of users</span></span>
- <span data-ttu-id="03ca6-113">सदस्यता अवधि महीनों में मापी जाती है</span><span class="sxs-lookup"><span data-stu-id="03ca6-113">A subscription duration measured in months</span></span>

<span data-ttu-id="03ca6-114">इस प्रकार के कैटलॉग को कायम रखने के लिए, **सदस्यता सॉफ़्टवेयर** नामक एक उत्पाद समूह बनाएँ और उपयोगकर्ताओं की संख्या और सदस्यता अवधि को एट्रिब्यूट के रूप में जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="03ca6-114">To maintain this type of catalog, create a product family named **Subscription Software** and add the number of users and the subscription duration as attributes.</span></span> <span data-ttu-id="03ca6-115">उसके बाद, आप अलग-अलग उत्पादों को **सदस्यता सॉफ़्टवेयर** उत्पाद समूह में जोड़ सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="03ca6-115">Next, you can add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="03ca6-116">परियोजना कोट में उत्पाद कैटलॉग आइटम जोड़ें</span><span class="sxs-lookup"><span data-stu-id="03ca6-116">Add product catalog items to a project quote</span></span>

<span data-ttu-id="03ca6-117">**परियोजना कोट** और **परियोजना अनुबंध** पृष्ठ में परियोजना-आधारित पंक्तियों और उत्पाद-आधारित पंक्तियों के लिए अनुभाग होते हैं.</span><span class="sxs-lookup"><span data-stu-id="03ca6-117">The **Project Quote** and **Project Contract** pages have sections for project-based lines and product-based lines.</span></span> <span data-ttu-id="03ca6-118">उत्पाद-आधारित पंक्तियों के लिए, कोट पंक्ति या परियोजना अनुबंध पंक्ति की ड्रॉप-डाउन सूची, उत्पाद मूल्य सूची में सभी उत्पाद और इकाइयों को शामिल करती है.</span><span class="sxs-lookup"><span data-stu-id="03ca6-118">For product-based lines, the drop-down list on the quote line or project contract line includes all the products and units in the product price list.</span></span> <span data-ttu-id="03ca6-119">आप उन उत्पादों को भी जोड़ सकते हैं, जो उत्पाद मूल्य सूची का हिस्सा नहीं हैं.</span><span class="sxs-lookup"><span data-stu-id="03ca6-119">You can also add products that aren't part of the product price list.</span></span>

<span data-ttu-id="03ca6-120">इसके अतिरिक्त, आप अन्य मूल्य सूचियों से उत्पादों का चयन कर सकते हैं या आप सीधे उत्पाद कैटेलॉग से भी उत्पादों का चयन कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="03ca6-120">Additionally, you can select products from other price lists or directly from the product catalog.</span></span> <span data-ttu-id="03ca6-121">जब आप कैटेलॉग से सीधे उत्पादों का चयन तो करते हैं, उत्पाद का बिक्री मूल्य प्राप्त करने के लिए उस उत्पाद की डिफ़ॉल्ट मूल्य सूची का उपयोग किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="03ca6-121">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="03ca6-122">यदि डिफ़ॉल्ट मूल्य सूची सेट नहीं है, तो मूल्य शून्य (0) पर सेट होता है.</span><span class="sxs-lookup"><span data-stu-id="03ca6-122">If a default price list isn't set, the price is set to zero (0).</span></span>

<span data-ttu-id="03ca6-123">जब कोट पंक्ति उत्पाद कैटेलॉग पर आधारित होती है, तो आप विक्रय मूल्य को सीधे कोट पंक्ति पर ओवरराइड कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="03ca6-123">When a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="03ca6-124">दो उपलब्ध मानों के साथ **मूल्य निर्धारण** फ़ील्ड में एक कोट पंक्ति:</span><span class="sxs-lookup"><span data-stu-id="03ca6-124">A quote line in **Pricing** field with two available values:</span></span>

- <span data-ttu-id="03ca6-125">**ओवरराइड मूल्य निर्धारण**</span><span class="sxs-lookup"><span data-stu-id="03ca6-125">**Override Pricing**</span></span>
- <span data-ttu-id="03ca6-126">**डिफ़ॉल्ट का उपयोग करें**</span><span class="sxs-lookup"><span data-stu-id="03ca6-126">**Use Default**</span></span>

<span data-ttu-id="03ca6-127">यदि आप **ओवरराइड मूल्य निर्धारण** चुनते हैं, तो डिफ़ॉल्ट मूल्य सेट नहीं है.</span><span class="sxs-lookup"><span data-stu-id="03ca6-127">If you select **Override Pricing**, the default price isn't set.</span></span> <span data-ttu-id="03ca6-128">इसके बजाए, आपको कोट पंक्ति पर उत्पाद के लिए एक मूल्य दर्ज करना होगा.</span><span class="sxs-lookup"><span data-stu-id="03ca6-128">Instead, you must enter a price for the product on the quote line.</span></span> <span data-ttu-id="03ca6-129">यदि आप **डिफ़ॉल्ट का उपयोग करें** चुनते हैं, तो डिफ़ॉल्ट विक्रय मूल्य का उपयोग किया जाता है और फ़ील्ड संपादन के लिए लॉक हो जाती है.</span><span class="sxs-lookup"><span data-stu-id="03ca6-129">If you select **Use Default**, the default sales price is used and the field is locked for editing.</span></span>

<span data-ttu-id="03ca6-130">डिफ़ॉल्ट विक्रय मूल्य कोट की उत्पाद-आधारित पंक्तियों पर दर्ज किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="03ca6-130">Default sales prices are entered on the product-based lines of a quote.</span></span> <span data-ttu-id="03ca6-131">उसके बाद **मूल्य निर्धारण** फ़ील्ड को **ओवरराइड मूल्य निर्धारण** पर सेट किया जाता है, ताकि आप कोट पंक्तियों पर डिफ़ॉल्ट मूल्य को संपादित कर सकें.</span><span class="sxs-lookup"><span data-stu-id="03ca6-131">The **Pricing** field is then set to **Override Pricing** so that you can edit the default price on the quote lines.</span></span> <span data-ttu-id="03ca6-132">यह Dynamics 365 Sales में उत्पाद-आधारित पंक्ति पर Project Operations-विशिष्ट ओवरराइड व्यवहार है.</span><span class="sxs-lookup"><span data-stu-id="03ca6-132">This is a Project Operations-specific override to the product-based lines behavior in Dynamics 365 Sales.</span></span>
