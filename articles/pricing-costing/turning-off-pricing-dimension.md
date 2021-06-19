---
title: मूल्य निर्धारण आयाम बंद करना
description: यह विषय मूल्य निर्धारण पैमानों को बंद करने के बारे में जानकारी देता है.
author: rumant
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 7b7c1d1b3363c0d158fcf6fda532822354b852a3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004533"
---
# <a name="turning-off-a-pricing-dimension"></a><span data-ttu-id="e57f9-103">मूल्य निर्धारण आयाम बंद करना</span><span class="sxs-lookup"><span data-stu-id="e57f9-103">Turning off a pricing dimension</span></span>

<span data-ttu-id="e57f9-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="e57f9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e57f9-105">आपको कुछेक वर्षों बाद अपनी प्राइस निर्धारण रणनीति की समीक्षा और इसे अपडेट करने की आवश्यकता हो सकती है।</span><span class="sxs-lookup"><span data-stu-id="e57f9-105">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="e57f9-106">आपके द्वारा किए गए किसी भी अपडेट के लिए आपका किसी मौजूदा प्राइस निर्धारण आयाम को बंद कर नया आयाम बनाना आवश्यक हो सकता है।</span><span class="sxs-lookup"><span data-stu-id="e57f9-106">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="e57f9-107">उदाहरण के लिए आपने पहले **भूमिका** के हिसाब से प्राइसिंग हो हो लेकिन अब आपने **कार्य अनुभव** के हिसाब से प्राइस तय करना है।</span><span class="sxs-lookup"><span data-stu-id="e57f9-107">For example, you may have previously priced by **Role**, but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="e57f9-108">ऐसा करने के लिए आपको मूल्य निर्धारण पैमानों के रूप में **रोल** को बंद करके **कार्य अनुभव** को नया मूल्य निर्धारण पैमाना बनाना होगा.</span><span class="sxs-lookup"><span data-stu-id="e57f9-108">This may require you to turn off **Role** as a pricing dimension and create **Work Experience** as a new pricing dimension.</span></span> 

<span data-ttu-id="e57f9-109">किसी प्राइस-निर्धारण आयाम को बंद करने हेतु, भले ही वह आउट-ऑफ-द-बॉक्स या कस्टम हो, प्राइस निर्धारण के **लागत पर लागू** और **बिक्री पर लागू** फ़ील्ड को **नहीं** पर सेट करें।</span><span class="sxs-lookup"><span data-stu-id="e57f9-109">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="e57f9-110">यद्यपि, जब आप ऐसा करते हैं तो आपको त्रुटि संदेश प्राप्त हो सकता है, **यदि संबंधित मूल्य रिकॉर्ड हैं, तो मूल्य निर्धारण पैमाना को अद्यतन या मिटाया नहीं जा सकता है.**</span><span class="sxs-lookup"><span data-stu-id="e57f9-110">However, when you do this, you might receive the error message, **Pricing dimension cannot be updated or deleted if there are associated price records.**</span></span>

![प्राइस निर्धारण आयाम बंद करते समय बिज़नेस प्रोसेस में संभावित त्रुटि](media/Business-Process-Error.png)

<span data-ttu-id="e57f9-112">यह त्रुटि संदेश इंगित करता है कि जिस आयाम को बंद किया जा रहा है, उसके लिए पहले तय किये गए प्राइस रिकॉर्ड हैं।</span><span class="sxs-lookup"><span data-stu-id="e57f9-112">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="e57f9-113">किसी आयाम पर लागू होने की शर्त को **नहीं** पर सेट करने से पहले आयाम को दर्शाने वाले सभी **रोल प्राइस** और **रोल प्राइस मार्कअप** रिकॉर्ड को हटा दिया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="e57f9-113">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="e57f9-114">यह नियम आउट-ऑफ-द-बॉक्स प्राइस निर्धारण आयामों और आपके द्वारा बनाए गए कस्टम प्राइस निर्धारण आयामों पर लागू होता है।</span><span class="sxs-lookup"><span data-stu-id="e57f9-114">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="e57f9-115">इस सत्यापन का कारण यह है कि प्रत्येक **रोल प्राइस** रिकॉर्ड में पैमानों का विशिष्ट संयोजन होना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="e57f9-115">The reason for this validation is because each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="e57f9-116">उदाहरण के लिए किसी **US लागत रेट 2018** नामक प्राइस सूची में निम्न **रोल प्राइस** पंक्ति हैं।</span><span class="sxs-lookup"><span data-stu-id="e57f9-116">For example, on a price list called **US Cost Rates 2018**, you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="e57f9-117">स्टेंडर्ड टाइटल</span><span class="sxs-lookup"><span data-stu-id="e57f9-117">Standard Title</span></span>         | <span data-ttu-id="e57f9-118">संगठन इकाई</span><span class="sxs-lookup"><span data-stu-id="e57f9-118">Org Unit</span></span>    |<span data-ttu-id="e57f9-119">इकाई</span><span class="sxs-lookup"><span data-stu-id="e57f9-119">Unit</span></span>   |<span data-ttu-id="e57f9-120">कीमत</span><span class="sxs-lookup"><span data-stu-id="e57f9-120">Price</span></span>  |<span data-ttu-id="e57f9-121">मुद्रा</span><span class="sxs-lookup"><span data-stu-id="e57f9-121">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="e57f9-122">सिस्ट्म्स इंजीनियर</span><span class="sxs-lookup"><span data-stu-id="e57f9-122">Systems Engineer</span></span>|<span data-ttu-id="e57f9-123">Contoso अमेरिका</span><span class="sxs-lookup"><span data-stu-id="e57f9-123">Contoso US</span></span>|<span data-ttu-id="e57f9-124">घंटा</span><span class="sxs-lookup"><span data-stu-id="e57f9-124">Hour</span></span>| <span data-ttu-id="e57f9-125">100</span><span class="sxs-lookup"><span data-stu-id="e57f9-125">100</span></span>|<span data-ttu-id="e57f9-126">USD</span><span class="sxs-lookup"><span data-stu-id="e57f9-126">USD</span></span>|
| <span data-ttu-id="e57f9-127">वरिष्ठ सिस्ट्म्स इंजीनियर</span><span class="sxs-lookup"><span data-stu-id="e57f9-127">Senior Systems Engineer</span></span>|<span data-ttu-id="e57f9-128">Contoso अमेरिका</span><span class="sxs-lookup"><span data-stu-id="e57f9-128">Contoso US</span></span>|<span data-ttu-id="e57f9-129">घंटा</span><span class="sxs-lookup"><span data-stu-id="e57f9-129">Hour</span></span>| <span data-ttu-id="e57f9-130">150</span><span class="sxs-lookup"><span data-stu-id="e57f9-130">150</span></span>| <span data-ttu-id="e57f9-131">USD</span><span class="sxs-lookup"><span data-stu-id="e57f9-131">USD</span></span>|


<span data-ttu-id="e57f9-132">जब आप मूल्य निर्धारण पैमानों के तौर पर **मानक शीर्षक** को बंद कर देते हैं और मूल्य निर्धारण इंजन रोल के लिए मूल्य की खोज करता है, तो केवल इनपुट संदर्भ से **संगठन इकाई** मान का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="e57f9-132">When you turn off **Standard Title** as the pricing dimension, and the pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="e57f9-133">अगर इनपुट संदर्भ की **संगठन इकाई** "Contoso US" है, तो परिणाम गैर-नियतात्मक होगा क्योंकि दोनों पंक्तियों का मिलान किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="e57f9-133">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="e57f9-134">इस परिदृश्य से बचने के लिए, जब आप **रोल प्राइस** रिकॉर्ड बनाते हैं, तो सिस्टम यह पुष्टि करता है कि पैमानों का संयोजन विशिष्ट है.</span><span class="sxs-lookup"><span data-stu-id="e57f9-134">To avoid this scenario, when you create **Role Price** records, the system validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="e57f9-135">यदि **भूमिका मू्ल्य** रिकॉर्ड बनने के बाद आयाम बंद कर दिया जाता है, तो इस सीमा का उल्लंघन किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="e57f9-135">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="e57f9-136">इसलिए आयाम बंद करने से पहले आवश्यक है कि आप सभी **भूमिका मू्ल्य** और **भूमिका मू्ल्य मार्कअप** पंक्तियों को हटा दें, जिनमें आयामों के मान दर्ज हैं।</span><span class="sxs-lookup"><span data-stu-id="e57f9-136">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]