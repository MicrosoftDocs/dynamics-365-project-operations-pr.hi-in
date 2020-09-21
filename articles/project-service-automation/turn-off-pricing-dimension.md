---
title: मूल्य निर्धारण आयाम बंद करें
description: इस टॉपिक में दिखाया गया है कि Project Service समाधान में प्राइस निर्धारण आयाम को कैसे सेट करें।
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/06/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 689e5a8d-e39a-471d-a6c4-7e2fc3bb5590
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 5cf2cd86fb1eba50c8e08b2bd624669ab0b1deb3
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3752054"
---
# <a name="turn-off-a-pricing-dimension"></a><span data-ttu-id="50dfd-103">मूल्य निर्धारण आयाम बंद करें</span><span class="sxs-lookup"><span data-stu-id="50dfd-103">Turn off a pricing dimension</span></span>

<span data-ttu-id="50dfd-104">आपको कुछेक वर्षों बाद अपनी प्राइस निर्धारण रणनीति की समीक्षा और इसे अपडेट करने की आवश्यकता हो सकती है।</span><span class="sxs-lookup"><span data-stu-id="50dfd-104">You may need to review and update your pricing strategy every few years.</span></span> <span data-ttu-id="50dfd-105">आपके द्वारा किए गए किसी भी अपडेट के लिए आपका किसी मौजूदा प्राइस निर्धारण आयाम को बंद कर नया आयाम बनाना आवश्यक हो सकता है।</span><span class="sxs-lookup"><span data-stu-id="50dfd-105">Any updates you make might require that you turn off an existing pricing dimension and create a new one.</span></span> <span data-ttu-id="50dfd-106">उदाहरण के लिए आपने पहले **भूमिका** के हिसाब से प्राइसिंग हो हो लेकिन अब आपने **कार्य अनुभव** के हिसाब से प्राइस तय करना है।</span><span class="sxs-lookup"><span data-stu-id="50dfd-106">For example, you may have previously priced by **Role**, but now you have decided to price by **Work Experience**.</span></span> <span data-ttu-id="50dfd-107">ऐसा करने के लिए आपको प्राइस निर्धारण आयाम के रूप में **रोल** को बंद कर **कार्य अनुभव** को नया प्राइस निर्धारण आयाम बनाना होगा।</span><span class="sxs-lookup"><span data-stu-id="50dfd-107">This may require you to turn off **Role** as a pricing dimension and create **Work Expereince** as a new pricing dimension.</span></span> 

<span data-ttu-id="50dfd-108">किसी प्राइस-निर्धारण आयाम को बंद करने हेतु, भले ही वह आउट-ऑफ-द-बॉक्स या कस्टम हो, प्राइस निर्धारण के **लागत पर लागू** और **बिक्री पर लागू** फ़ील्ड को **नहीं** पर सेट करें।</span><span class="sxs-lookup"><span data-stu-id="50dfd-108">Turning off a pricing dimension, regardless if it is out-of-the-box or custom, can be done by setting the **Applicable to Cost** and **Applicable to Sales** fields of the Pricing Dimension to **No**.</span></span>

<span data-ttu-id="50dfd-109">हालाँकि ऐसा करने पर आपको निम्न त्रुटि संदेश मिल सकता है।</span><span class="sxs-lookup"><span data-stu-id="50dfd-109">However, when you do this, you might receive the following error message.</span></span>

![प्राइस निर्धारण आयाम बंद करते समय बिज़नेस प्रोसेस में संभावित त्रुटि](media/Business-Process-Error.png)


<span data-ttu-id="50dfd-111">यह त्रुटि संदेश इंगित करता है कि जिस आयाम को बंद किया जा रहा है, उसके लिए पहले तय किये गए प्राइस रिकॉर्ड हैं।</span><span class="sxs-lookup"><span data-stu-id="50dfd-111">This error message indicates that there are price records that were previously set up for the dimension that is being turned off.</span></span> <span data-ttu-id="50dfd-112">किसी आयाम पर लागू होने की शर्त को **नहीं** पर सेट करने से पहले आयाम को दर्शाने वाले सभी **रोल प्राइस** और **रोल प्राइस मार्कअप** रिकॉर्ड को हटा दिया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="50dfd-112">All **Role Price** and **Role Price Markup** records that refer to a dimension must be deleted before the dimension’s applicability can be to set to **No**.</span></span> <span data-ttu-id="50dfd-113">यह नियम आउट-ऑफ-द-बॉक्स प्राइस निर्धारण आयामों और आपके द्वारा बनाए गए कस्टम प्राइस निर्धारण आयामों पर लागू होता है।</span><span class="sxs-lookup"><span data-stu-id="50dfd-113">This rule applies to both out-of-the-box pricing dimensions and any custom pricing dimensions that you may have created.</span></span> <span data-ttu-id="50dfd-114">इस सत्यापन का कारण Project Service में इस सीमा का होना है कि प्रत्येक **रोल प्राइस** रिकॉर्ड में आयामों का अनन्य संयोजन होना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="50dfd-114">The reason for this validation is because Project Service has a constraint that each **Role Price** record must have a unique combination of dimensions.</span></span> <span data-ttu-id="50dfd-115">उदाहरण के लिए किसी **US लागत रेट 2018** नामक प्राइस सूची में निम्न **रोल प्राइस** पंक्ति हैं।</span><span class="sxs-lookup"><span data-stu-id="50dfd-115">For example, on a price list called **US Cost Rates 2018**, you have the following **Role price** rows.</span></span> 

| <span data-ttu-id="50dfd-116">स्टेंडर्ड टाइटल</span><span class="sxs-lookup"><span data-stu-id="50dfd-116">Standard Title</span></span>         | <span data-ttu-id="50dfd-117">संगठन इकाई</span><span class="sxs-lookup"><span data-stu-id="50dfd-117">Org Unit</span></span>    |<span data-ttu-id="50dfd-118">इकाई</span><span class="sxs-lookup"><span data-stu-id="50dfd-118">Unit</span></span>   |<span data-ttu-id="50dfd-119">मूल्य</span><span class="sxs-lookup"><span data-stu-id="50dfd-119">Price</span></span>  |<span data-ttu-id="50dfd-120">मुद्रा</span><span class="sxs-lookup"><span data-stu-id="50dfd-120">Currency</span></span>  |
| -----------------------|-------------|-------|-------|----------|
| <span data-ttu-id="50dfd-121">सिस्ट्म्स इंजीनियर</span><span class="sxs-lookup"><span data-stu-id="50dfd-121">Systems Engineer</span></span>|<span data-ttu-id="50dfd-122">Contoso US</span><span class="sxs-lookup"><span data-stu-id="50dfd-122">Contoso US</span></span>|<span data-ttu-id="50dfd-123">Hour</span><span class="sxs-lookup"><span data-stu-id="50dfd-123">Hour</span></span>| <span data-ttu-id="50dfd-124">100</span><span class="sxs-lookup"><span data-stu-id="50dfd-124">100</span></span>|<span data-ttu-id="50dfd-125">USD</span><span class="sxs-lookup"><span data-stu-id="50dfd-125">USD</span></span>|
| <span data-ttu-id="50dfd-126">वरिष्ठ सिस्ट्म्स इंजीनियर</span><span class="sxs-lookup"><span data-stu-id="50dfd-126">Senior Systems Engineer</span></span>|<span data-ttu-id="50dfd-127">Contoso US</span><span class="sxs-lookup"><span data-stu-id="50dfd-127">Contoso US</span></span>|<span data-ttu-id="50dfd-128">Hour</span><span class="sxs-lookup"><span data-stu-id="50dfd-128">Hour</span></span>| <span data-ttu-id="50dfd-129">150</span><span class="sxs-lookup"><span data-stu-id="50dfd-129">150</span></span>| <span data-ttu-id="50dfd-130">USD</span><span class="sxs-lookup"><span data-stu-id="50dfd-130">USD</span></span>|


<span data-ttu-id="50dfd-131">जब आप प्राइस निर्धारण आयाम के तौर पर **स्टेंडर्ड टाइटल** को बंद कर देते हैं और Project Service मूल्य निर्धारण इंजन रोल के लिए प्राइस की खोज करता है, तो केवल इनपुट संदर्भ से **संगठनात्मक इकाई** मान का उपयोग करता है।</span><span class="sxs-lookup"><span data-stu-id="50dfd-131">When you turn off **Standard Title** as the pricing dimension, and the Project Service pricing engine searches for a price, it will only use the **Org Unit** value from the input context.</span></span> <span data-ttu-id="50dfd-132">यदि इनपुट संदर्भ की **संगठनात्मक इकाई** “Contoso US” है, तो कोई भी परिणाम नहीं निकल सकेंगे क्योंकि दोनों पंक्तियों का मिलान हो जाएगा।</span><span class="sxs-lookup"><span data-stu-id="50dfd-132">If the **Org Unit** of the input context is “Contoso US”, the result will be non-deterministic because both the rows will match.</span></span> <span data-ttu-id="50dfd-133">इससे बचने के लिए **भूमिका मू्ल्य** रिकॉर्ड बनाते समय Project Service पुष्टि करती है कि आयामों का संयोजन अनन्य है।</span><span class="sxs-lookup"><span data-stu-id="50dfd-133">To avoid this scenario, when you create **Role Price** records, Project Service validates that the combination of dimensions is unique.</span></span> <span data-ttu-id="50dfd-134">यदि **भूमिका मू्ल्य** रिकॉर्ड बनने के बाद आयाम बंद कर दिया जाता है, तो इस सीमा का उल्लंघन किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="50dfd-134">If the dimension is turned off after the **Role Price** records are created, this constraint can be violated.</span></span> <span data-ttu-id="50dfd-135">इसलिए आयाम बंद करने से पहले आवश्यक है कि आप सभी **भूमिका मू्ल्य** और **भूमिका मू्ल्य मार्कअप** पंक्तियों को हटा दें, जिनमें आयामों के मान दर्ज हैं।</span><span class="sxs-lookup"><span data-stu-id="50dfd-135">Therefore, it is required that before you turn off a dimension, you delete all **Role Price** and **Role Price Markup** rows that have that dimension value populated.</span></span>

