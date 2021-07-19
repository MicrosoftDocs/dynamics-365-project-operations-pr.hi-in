---
title: उत्पाद-आधारित अनुबंध पंक्ति ओवरव्यू - लाइट
description: यह विषय, उत्पाद-आधारित अनुबंध पंक्ति के बारे में जानकारी प्रदान करता है.
author: rumant
ms.date: 10/07/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.custom: intro-internal
ms.openlocfilehash: 8464eefbce9ba266360e10039e2a0be78982d8fa
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 07/07/2021
ms.locfileid: "6369738"
---
# <a name="product-based-contract-lines-overview---lite"></a><span data-ttu-id="a2a6c-103">उत्पाद-आधारित अनुबंध पंक्ति ओवरव्यू - लाइट</span><span class="sxs-lookup"><span data-stu-id="a2a6c-103">Product-based contract lines overview - lite</span></span>

<span data-ttu-id="a2a6c-104">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="a2a6c-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a2a6c-105">आप Dynamics 365 Project Operations में उत्पाद-आधारित अनुबंध पंक्तियाँ बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-105">You can create product-based contract lines in Dynamics 365 Project Operations.</span></span> <span data-ttu-id="a2a6c-106">उत्पाद-आधारित अनुबंध क्षेत्र मैन्युअल रूप से निर्मित पंक्तियां हो सकती हैं, या वे उत्पाद कैटलॉग के आइटम हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-106">Product-based contract lines can be manually created lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="a2a6c-107">उत्पाद कैटलॉग</span><span class="sxs-lookup"><span data-stu-id="a2a6c-107">Product catalog</span></span>

<span data-ttu-id="a2a6c-108">उत्पाद कैटलॉग के उत्पादों में एक डिफ़ॉल्ट इकाई और इकाई समूह होता है।</span><span class="sxs-lookup"><span data-stu-id="a2a6c-108">The products in the product catalog have a default unit and unit group.</span></span> <span data-ttu-id="a2a6c-109">यदि कई उत्पाद एकसमान विशेषताओं के समुच्चय को साझा करते हैं, तो आप एक ऐसा उत्पाद परिवार बना सकते हैं जिसमें वे विशेषताएँ भी शामिल हों।</span><span class="sxs-lookup"><span data-stu-id="a2a6c-109">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="a2a6c-110">एक उत्पाद परिवार के सभी उत्पादों में एकसमान विशेषताओं का समुच्चय होता है।</span><span class="sxs-lookup"><span data-stu-id="a2a6c-110">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="a2a6c-111">उदाहरण के लिए, एक कंपनी विभिन्न सॉफ्टवेयरों के लिए सदस्यता लाइसेंस बेचती है।</span><span class="sxs-lookup"><span data-stu-id="a2a6c-111">For example, a company sells subscription licenses for different kinds of software.</span></span> <span data-ttu-id="a2a6c-112">सभी सदस्यता सॉफ्टवेयर में निम्नलिखित दो विशेषताएं होती हैं:</span><span class="sxs-lookup"><span data-stu-id="a2a6c-112">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="a2a6c-113">उपयोगकर्ताओं की संख्या</span><span class="sxs-lookup"><span data-stu-id="a2a6c-113">Number of users</span></span>
- <span data-ttu-id="a2a6c-114">सदस्यता अवधि (महीनों में)</span><span class="sxs-lookup"><span data-stu-id="a2a6c-114">Subscription duration (in months)</span></span>

<span data-ttu-id="a2a6c-115">इस प्रकार के कैटलॉग की देखरेख के लिए, उत्पाद परिवार बनाएं जिसका नाम **सदस्यता सॉफ़्टवेयर** है.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-115">To maintain this type of catalog, create a product family that is named **Subscription Software**.</span></span> <span data-ttu-id="a2a6c-116">उत्पाद परिवार में **उपयोगकर्ताओं की संख्या** और **सदस्यता अवधि** एट्रिब्यूट जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-116">Add the attributes, **Number of users** and **Subscription duration** to the product family.</span></span> <span data-ttu-id="a2a6c-117">फिर **सदस्यता सॉफ़्टवेयर** उत्पाद परिवार में अलग-अलग उत्पाद जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-117">Then, add individual products to the **Subscription Software** product family.</span></span>

## <a name="add-product-catalog-items-to-a-project-contract"></a><span data-ttu-id="a2a6c-118">किसी प्रोजेक्ट अनुबंध में उत्पाद कैटलॉग आइटम जोडे़ं</span><span class="sxs-lookup"><span data-stu-id="a2a6c-118">Add product catalog items to a project Contract</span></span>

<span data-ttu-id="a2a6c-119">परियोजना प्रतिबंध में दो तरह की पंक्तियां, परियोजना-आधारित और उत्पाद-आधारित के अनुभाग होते हैं.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-119">Project contracts have sections for two types of lines, project-based and product-based.</span></span> <span data-ttu-id="a2a6c-120">उत्पाद-आधारित पंक्तियों में अनुबंध पर उत्पाद मूल्य सूची में सभी उत्पाद और इकाइयां शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-120">Product-based lines include all of the products and units in the product price list on the contract.</span></span> <span data-ttu-id="a2a6c-121">ऐसे उत्पाद जो अनुबंध की उत्पाद मूल्य सूची का हिस्सा नहीं हैं, उनको जोड़ा जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-121">Products that aren't part of contract's product price list can be added.</span></span>

<span data-ttu-id="a2a6c-122">आप उत्पादों को अन्य मूल्य सूचियों से या सीधे उत्पाद कैटलॉग से चुन सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-122">You can select products from other price lists, or directly from the product catalog.</span></span> <span data-ttu-id="a2a6c-123">जब आप किसी उत्पाद कैटलॉग से सीधे उत्पादों चुनते हैं, तो उत्पाद की बिक्री मूल्य के लिए उस उत्पाद की डिफ़ॉल्ट मूल्य सूची को इस्तेमाल किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-123">When you select products directly from a product catalog, the default price list of that product is used for the product's sales price.</span></span> <span data-ttu-id="a2a6c-124">यदि कोई डिफ़ॉल्ट मूल्य सूची निर्धारित नहीं है, तो मूल्य 0 (शून्य) पर सेट होगा।</span><span class="sxs-lookup"><span data-stu-id="a2a6c-124">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="a2a6c-125">यदि एक अनुबंध पंक्ति कैटेलॉग पर आधारित है, तो आप पंक्ति पर बिक्री मूल्य को सीधे अधिरोहित(ओवरराइड) कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-125">If a contract line is based on a product catalog, you can override the sales price directly on the line.</span></span> <span data-ttu-id="a2a6c-126">अनुबंध पंक्ति में दो मूल्यों के साथ **मूल्य निर्धारण** फ़ील्ड है:</span><span class="sxs-lookup"><span data-stu-id="a2a6c-126">A contract line has the **Pricing** field with the two values:</span></span>

- <span data-ttu-id="a2a6c-127">**ओवरराइड मूल्य निर्धारण**</span><span class="sxs-lookup"><span data-stu-id="a2a6c-127">**Override pricing**</span></span>
- <span data-ttu-id="a2a6c-128">**डिफ़ॉल्ट का उपयोग करें**</span><span class="sxs-lookup"><span data-stu-id="a2a6c-128">**Use default**</span></span>

<span data-ttu-id="a2a6c-129">यदि आप **मूल्य निर्धारण** फ़ील्ड को **मूल्य-निर्धारण ओवरराइड करें** पर सेट करते हैं, तो डिफ़ॉल्ट मूल्य सेट नहीं किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-129">If you set the **Pricing** field to **Override pricing**, the default price isn't set.</span></span> <span data-ttu-id="a2a6c-130">अनुबंध पंक्ति पर उत्पाद के लिए मूल्य दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-130">Enter a price for the product on the contract line.</span></span> <span data-ttu-id="a2a6c-131">अगर आप **डिफ़ॉल्ट इस्तेमाल करें** फ़ील्ड पर सेट करते हैं तो डिफ़ॉल्ट बिक्री मूल्य को इस्तेमाल किया जाता है और फ़ील्ड को संपादित नहीं किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-131">If you set the field to **Use default**, the default sales price is used and the field can't be edited.</span></span>

<span data-ttu-id="a2a6c-132">आपके द्वारा परियोजना संचालन स्थापित करने के बाद, किसी अनुबंध पर डिफ़ॉल्ट बिक्री मूल्य उत्पाद-आधारित पद्धति पर दर्ज किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-132">After you install Project Operations, default sales prices are entered on the product-based lines on a contract.</span></span> <span data-ttu-id="a2a6c-133">**मूल्य निर्धारण** फ़ील्ड **मूल्य निर्धारण ओवरराइड करें** पर सेट है ताकि आप अनुबंध पंक्तियों पर डिफ़ॉल्ट मूल्य को संपादित कर सकें.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-133">The **Pricing** field is set to **Override pricing** so that you can edit the default price on the contract lines.</span></span> <span data-ttu-id="a2a6c-134">यह Dynamics 365 Sales में उत्पाद-आधारित पंक्तियों के व्यवहार के लिए Project Operations-विशिष्ट ओवरराइड है.</span><span class="sxs-lookup"><span data-stu-id="a2a6c-134">This is a Project Operations-specific override to product-based lines behavior in Dynamics 365 Sales.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]