---
title: उत्पाद-आधारित कोट पंक्तियाँ
description: यह विषय, उत्पाद-आधारित उद्धृत पंक्तियों के बारे में जानकारी प्रदान करता है।
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 03/06/2019
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
ms.openlocfilehash: 1bd789f4ee4d5b4603093be24aa25addafa9e8e8
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998503"
---
# <a name="product-based-quote-lines"></a><span data-ttu-id="f1160-103">उत्पाद-आधारित कोट पंक्तियाँ</span><span class="sxs-lookup"><span data-stu-id="f1160-103">Product-based quote lines</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]


<span data-ttu-id="f1160-104">आप Dynamics 365 Project Service Automation में उत्पाद-आधारित उद्धरण लाइनें बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="f1160-104">You can create product-based quote lines in Dynamics 365 Project Service Automation.</span></span> <span data-ttu-id="f1160-105">उत्पाद-आधारित उद्धरण लाइनें "राइट-इन" लाइनें हो सकती हैं,या वे उत्पाद सूची की आइटम हो सकती हैं।</span><span class="sxs-lookup"><span data-stu-id="f1160-105">Product-based quote lines can be "write-in" lines, or they can be items from the product catalog.</span></span>

## <a name="product-catalog"></a><span data-ttu-id="f1160-106">उत्पाद कैटलॉग</span><span class="sxs-lookup"><span data-stu-id="f1160-106">Product catalog</span></span>

<span data-ttu-id="f1160-107">Dynamics 365 उत्पाद कैटलॉग के उत्पादों में एक डिफ़ॉल्ट इकाई और इकाई समूह होता है।</span><span class="sxs-lookup"><span data-stu-id="f1160-107">The products in a Dynamics 365 product catalog have a default unit and unit group.</span></span> <span data-ttu-id="f1160-108">यदि कई उत्पाद एकसमान विशेषताओं के समुच्चय को साझा करते हैं, तो आप एक ऐसा उत्पाद परिवार बना सकते हैं जिसमें वे विशेषताएँ भी शामिल हों।</span><span class="sxs-lookup"><span data-stu-id="f1160-108">If several products share the same set of attributes, you can create a product family that also has those attributes.</span></span> <span data-ttu-id="f1160-109">एक उत्पाद परिवार के सभी उत्पादों में एकसमान विशेषताओं का समुच्चय होता है।</span><span class="sxs-lookup"><span data-stu-id="f1160-109">All the products in one product family inherit the same set of attributes.</span></span>

<span data-ttu-id="f1160-110">उदाहरण के लिए, एक कंपनी विभिन्न सॉफ्टवेयरों के लिए सदस्यता लाइसेंस बेचती है।</span><span class="sxs-lookup"><span data-stu-id="f1160-110">For example, a company sells subscription licenses for a variety of software.</span></span> <span data-ttu-id="f1160-111">सभी सदस्यता सॉफ्टवेयर में निम्नलिखित दो विशेषताएं होती हैं:</span><span class="sxs-lookup"><span data-stu-id="f1160-111">All subscription software has the following two attributes:</span></span>

- <span data-ttu-id="f1160-112">उपयोगकर्ताओं की संख्या</span><span class="sxs-lookup"><span data-stu-id="f1160-112">Number of users</span></span> 
- <span data-ttu-id="f1160-113">सदस्यता अवधि (महीनों में)</span><span class="sxs-lookup"><span data-stu-id="f1160-113">Subscription duration (in months)</span></span>

<span data-ttu-id="f1160-114">इस प्रकार के कैटलॉग को बनाने का एक अच्छा तरीका है कि एक ऐसा उत्पाद परिवार बनाया जाए जिसका नाम **सदस्यता सॉफ्टवेयर** है, और जिसकी विशेषता **उपयोगकर्ताओं की संख्या** और **सदस्यता अवधि** है।</span><span class="sxs-lookup"><span data-stu-id="f1160-114">A good way to maintain this type of catalog is to create a product family that is named **Subscription Software**, and that has **Number of users** and **Subscription duration** as attributes.</span></span> <span data-ttu-id="f1160-115">फिर आप **सब्सक्रिप्शन सॉफ्टवेयर** उत्पाद परिवार में व्यक्तिगत उत्पाद जोड़ सकते हैं, जैसे **Dynamics 365 Sales** या **Dynamics 365 Field Service**।</span><span class="sxs-lookup"><span data-stu-id="f1160-115">You can then add individual products, such as **Dynamics 365 Sales** or **Dynamics 365 Field Service** to the **Subscription Software** product family.</span></span>

## <a name="adding-product-catalog-items-to-a-project-quote"></a><span data-ttu-id="f1160-116">किसी प्रोजेक्ट कोट में उत्पाद कैटलॉग आइटम जोड़ना</span><span class="sxs-lookup"><span data-stu-id="f1160-116">Adding product catalog items to a project quote</span></span>

<span data-ttu-id="f1160-117">प्रोजेक्ट उद्धरण और प्रोजेक्ट कॉन्ट्रैक्ट पेज में दो प्रकार की पद्धतियां होती हैं: प्रोजेक्ट-आधारित पद्धतियां और उत्पाद-आधारित पद्धतियां।</span><span class="sxs-lookup"><span data-stu-id="f1160-117">Project quote and project contract pages have sections for two types of lines: project-based lines and product-based lines.</span></span> <span data-ttu-id="f1160-118">उत्पाद-आधारित पद्धतियों के लिए, Dynamics 365 का उपयोग उत्पाद कैटलॉग से आइटम को एक उद्धरण में जोड़ने के लिए किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="f1160-118">For product-based lines, Dynamics 365 is used to add items from a product catalog to a quote.</span></span> <span data-ttu-id="f1160-119">उद्धरण पद्धति या प्रोजेक्ट अनुबंध पद्धति में ड्रॉप-डाउन सूची में उत्पाद मूल्य सूची में वे सभी उत्पाद और इकाइयां शामिल होते हैं, जो उद्धरण या परियोजना अनुबंध से जुड़े हुए है।</span><span class="sxs-lookup"><span data-stu-id="f1160-119">The drop-down list on the quote line or project contract line includes all the products and units in the product price list that is attached to the quote or project contract.</span></span> <span data-ttu-id="f1160-120">आप उन उत्पादों को भी जोड़ सकते हैं जो उद्धरण के उत्पाद मूल्य सूची का हिस्सा नहीं हैं।</span><span class="sxs-lookup"><span data-stu-id="f1160-120">You can also add products that aren't part of quote's product price list.</span></span>

<span data-ttu-id="f1160-121">इसके अतिरिक्त, आप अन्य मूल्य सूचियों से उत्पादों का चयन कर सकते हैं, या आप सीधे उत्पाद कैटेलॉग से भी उत्पादों का चयन कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="f1160-121">Additionally, you can select products from other price lists, or you can select products directly from the product catalog.</span></span> <span data-ttu-id="f1160-122">जब आप कैटेलॉग से सीधे उत्पादों का चयन तो करते हैं, उत्पाद का बिक्री मूल्य प्राप्त करने के लिए उस उत्पाद की डिफ़ॉल्ट मूल्य सूची का उपयोग किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="f1160-122">When you select products directly from a product catalog, the default price list of that product is used to get the product's sales price.</span></span> <span data-ttu-id="f1160-123">यदि कोई डिफ़ॉल्ट मूल्य सूची निर्धारित नहीं है, तो मूल्य 0 (शून्य) पर सेट होगा।</span><span class="sxs-lookup"><span data-stu-id="f1160-123">If a default price list isn't set, the price is set to 0 (zero).</span></span>

<span data-ttu-id="f1160-124">यदि एक उद्धरण पद्धति कैटेलॉग पर आधारित है, तो आप उद्धरण पद्धति पर बिक्री मूल्य को सीधे अधिरोहित(ओवरराइड) कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="f1160-124">If a quote line is based on a product catalog, you can override the sales price directly on the quote line.</span></span> <span data-ttu-id="f1160-125">ध्यान दें कि Dynamics 365 में उद्धरण पद्धति एक **मूल्य निर्धारण** क्षेत्र है।</span><span class="sxs-lookup"><span data-stu-id="f1160-125">Note that a quote line in Dynamics 365 has a **Pricing** field.</span></span> <span data-ttu-id="f1160-126">दो मान उपलब्ध हैं:</span><span class="sxs-lookup"><span data-stu-id="f1160-126">Two values are available:</span></span>

- <span data-ttu-id="f1160-127">ओवरराइड मूल्य निर्धारण</span><span class="sxs-lookup"><span data-stu-id="f1160-127">Override pricing</span></span>  
- <span data-ttu-id="f1160-128">डिफ़ॉल्ट का उपयोग करें</span><span class="sxs-lookup"><span data-stu-id="f1160-128">Use default</span></span>

<span data-ttu-id="f1160-129">यदि आप इस क्षेत्र को **ओवरराइड मूल्य निर्धारण** पर निर्धारित करते हैं, तो Dynamics 365 डिफ़ॉल्ट मूल्य निर्धारित नहीं करता है।</span><span class="sxs-lookup"><span data-stu-id="f1160-129">If you set this field to **Override pricing**, Dynamics 365 doesn't set a default price.</span></span> <span data-ttu-id="f1160-130">आपको उद्धरण पद्धति पर किसी उत्पाद के लिए एक मूल्य दर्ज करना होगा।</span><span class="sxs-lookup"><span data-stu-id="f1160-130">You must enter a price for the product on the quote line.</span></span> <span data-ttu-id="f1160-131">यदि आप इस फ़ील्ड को **डिफ़ॉल्ट का उपयोग करें** पर निर्धारित करते हैं, Dynamics 365 डिफ़ॉल्ट बिक्री मूल्य का उपयोग करता है और और संपादन को रोकने के लिए फ़ील्ड में अवरोध लगा देता है।</span><span class="sxs-lookup"><span data-stu-id="f1160-131">If you set this field to **Use default**, Dynamics 365 uses the default sales price and locks the field to prevent editing.</span></span>

<span data-ttu-id="f1160-132">आपके द्वारा PSA स्थापित करने के बाद, किसी कोट पर डिफ़ॉल्ट बिक्री मूल्य उत्पाद-आधारित पद्धति पर दर्ज किए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="f1160-132">After you install PSA, default sales prices are entered on the product-based lines on a quote.</span></span> <span data-ttu-id="f1160-133">तब **मूल्य निर्धारण** क्षेत्र **ओवरराइड मूल्य निर्धारण** पर निर्धारित किया जाता है, ताकि आप उद्धरण पद्धित पर डिफ़ॉल्ट मूल्य को संपादित कर सकें।</span><span class="sxs-lookup"><span data-stu-id="f1160-133">The **Pricing** field is then set to **Override pricing** so that you can edit the default price on the quote lines.</span></span>

> ![ओवरराइड मूल्य निर्धारण निर्धारित करना](media/basic-guide-10.png)
 
## <a name="quantity-factors-for-products"></a><span data-ttu-id="f1160-135">उत्पादों के लिए मात्रा कारक</span><span class="sxs-lookup"><span data-stu-id="f1160-135">Quantity factors for products</span></span>

<span data-ttu-id="f1160-136">PSA, सदस्यता-आधारित उत्पादों की बिक्री की मदद करने के लिए मात्रा कारकों का उपयोग करता है।</span><span class="sxs-lookup"><span data-stu-id="f1160-136">PSA uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="f1160-137">सदस्यता-आधारित उत्पादों के लिए उद्धरण पर या प्रोजेक्ट अनुबंध पद्धति पर मात्रा, उपयोगकर्ता महीनों की संख्या के रूप में व्यक्त की जाती है।</span><span class="sxs-lookup"><span data-stu-id="f1160-137">For subscription-based products, the quantity on the quote or project contract line is expressed as the number of user months.</span></span>

<span data-ttu-id="f1160-138">आमतौर पर, सदस्यता सॉफ़्टवेयर की कीमत कैटलॉग में प्रति माह प्रति उपयोगकर्ता मूल्य के रूप में संग्रहीत की जाती है।</span><span class="sxs-lookup"><span data-stu-id="f1160-138">Usually, the price of subscription software is stored in the catalog as the price per user per month.</span></span> <span data-ttu-id="f1160-139">हालाँकि, आप इसके बजाय अन्य समय विवरण का उपयोग कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="f1160-139">However, you can use other time descriptions instead.</span></span> <span data-ttu-id="f1160-140">बिक्री प्रक्रिया के दौरान, उद्धरण पद्धति पर मूल्य आमतौर पर प्रति-उपयोगकर्ता, प्रति माह मूल्य होता है, जिस पर IT बिक्री एजेंट मोलभाव और छूट देता था।</span><span class="sxs-lookup"><span data-stu-id="f1160-140">During the sales process, the price on the quote line is usually the per-user, per-month price that was negotiated and discounted by the IT sales agent.</span></span> <span data-ttu-id="f1160-141">प्रत्येक सौदे में उपयोगकर्ताओं की एक अलग संख्या और सदस्यता महीनों की एक अलग संख्या होती है।</span><span class="sxs-lookup"><span data-stu-id="f1160-141">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="f1160-142">कोट पद्धति की मात्रा की गणना करने के लिए उपयोग की जाने वाली मात्रा, उपयोगकर्ताओं की संख्या और सदस्यता महीनों की संख्या का परिणाम है।</span><span class="sxs-lookup"><span data-stu-id="f1160-142">The quantity that is used to compute the amount of the quote line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="f1160-143">इस प्रकार की बिक्री का समर्थन करने के लिए, PSA ने मात्रा कारकों की अवधारणा पेश की।</span><span class="sxs-lookup"><span data-stu-id="f1160-143">To support this type of sale, PSA introduced the concept of quantity factors.</span></span> <span data-ttu-id="f1160-144">Dynamics 365 में, मात्रा कारक उत्पाद की विशेषताओं पर निर्भर करते हैं।</span><span class="sxs-lookup"><span data-stu-id="f1160-144">Quantity factors rely on the product attributes in Dynamics 365.</span></span> <span data-ttu-id="f1160-145">जब आप किसी उत्पाद के लिए विशिष्ट गुणों को कॉन्फ़िगर करते हैं, तो PSA आपको उन विशेषताओं के उपसमूह को या सभी विशेषताओं को मात्रा कारकों के रूप में चिह्नित करने देता है।</span><span class="sxs-lookup"><span data-stu-id="f1160-145">When you configure specific properties for a product, PSA lets you flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="f1160-146">PSA सत्यापित करता है कि केवल संख्यात्मक विशेषता या उत्पाद विशेषता, जिनमें एक संख्यात्मक डेटा प्रकार होता है, उन्हें मात्रा कारकों के रूप में चिह्नित किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="f1160-146">PSA validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="f1160-147">जब एक उत्पाद जिसमें मात्रा कारकों को कॉन्फिगर किया जाता है, को उद्धरण पद्धति में जोड़ा जाता है, तो **मात्रा** क्षेत्र उद्धरण पद्धति में केवल-पठन बन जाता है।</span><span class="sxs-lookup"><span data-stu-id="f1160-147">When a product that quantity factors are configured for is added to a quote line, the **Quantity** field on the quote line becomes a read-only field.</span></span> <span data-ttu-id="f1160-148">जब आप उत्पाद विशेषताओं के लिए मान दर्ज करते हैं, जो मात्रा कारक हैं, तो PSA उद्धरण पद्धति की मात्रा की गणना करता है।</span><span class="sxs-lookup"><span data-stu-id="f1160-148">After you enter values for product properties that are quantity factors, PSA computes the quantity of the quote line.</span></span>

<span data-ttu-id="f1160-149">उदाहरण के लिए, Dynamics 365 में निम्न गुण हो सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="f1160-149">For example, Dynamics 365 might have the following properties:</span></span> 

- <span data-ttu-id="f1160-150">**उपयोगकर्ता संख्या** - उपयोगकर्ताओं की संख्या</span><span class="sxs-lookup"><span data-stu-id="f1160-150">**No of users** - The number of users</span></span> 
- <span data-ttu-id="f1160-151">**महीनों की संख्या** - सदस्यता महीनों की संख्या</span><span class="sxs-lookup"><span data-stu-id="f1160-151">**No of Months** - The number of subscription months</span></span>
- <span data-ttu-id="f1160-152">**उत्पाद SKU**</span><span class="sxs-lookup"><span data-stu-id="f1160-152">**Product SKU**</span></span> 

<span data-ttu-id="f1160-153">उत्पाद पद्धति की विशेषताओं को संपादित करके **उपयोगकर्ताओं की संख्या** और **महीनों की संख्या** को मात्रा कारकों के रूप में चिह्नित किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="f1160-153">Tne **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span> 

> ![गुणवत्ता कारकों के रूप में उपयोगकर्ताओं की संख्या और महीनों की संख्या को चिह्नांकित करना](media/basic-guide-11.png)
 


[!INCLUDE[footer-include](../includes/footer-banner.md)]