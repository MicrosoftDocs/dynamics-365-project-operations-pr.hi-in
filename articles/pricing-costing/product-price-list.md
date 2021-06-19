---
title: उत्पाद मूल्य सूचियाँ
description: यह विषय परियोजना कोटेशन और अनुबंधों में इस्तेमाल किए जाने वाले कैटलॉग मूल्य निर्धारण में मूल्य सूचियों के बारे में जानकारी देता है.
author: rumant
ms.date: 04/05/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 02d274725983e50adc35a4cae1ac60c35be346a4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004938"
---
# <a name="product-price-lists"></a><span data-ttu-id="c587a-103">उत्पाद मूल्य सूचियाँ</span><span class="sxs-lookup"><span data-stu-id="c587a-103">Product price lists</span></span>

<span data-ttu-id="c587a-104">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="c587a-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

 <span data-ttu-id="c587a-105">Project Operations में, **प्रोडक्ट प्राइस लिस्ट** और संबंधित प्राइस लिस्ट आइटम निकायें प्रोडक्ट-आधारित कोट और कॉन्ट्रैक्ट लाइन पर प्रोडक्टों के मूल्य निर्धारण के लिए कार्यक्षमता का समर्थन करती हैं.</span><span class="sxs-lookup"><span data-stu-id="c587a-105">In Project Operations, **Product price lists** and related price list item entities support functionality for pricing products on product-based quote and contract lines.</span></span> <span data-ttu-id="c587a-106">परियोजनाओं पर उपयोग किए जाने वाले प्रोडक्टों के लिए, परियोजना प्राइस लिस्टों के लिए प्राइस लिस्ट आइटम के रिकॉर्ड का उपयोग किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="c587a-106">For products used on projects, the price list item records for project price lists are used.</span></span> 

<span data-ttu-id="c587a-107">प्रॉडक्ट निर्धारित होने चाहिए ताकि प्रॉडक्ट कैटेलॉग में उनकी डिफाल्ट लागत और कीमत सूची हो।</span><span class="sxs-lookup"><span data-stu-id="c587a-107">Products should be set up so that they have default cost and price lists in the product catalog.</span></span> <span data-ttu-id="c587a-108">डिफ़ॉल्ट कीमत और सूची मूल्यों को कॉन्फ़िगर करने के लिए सूची मूल्य, मानक लागत और वर्तमान लागत का इस्तेमाल करें.</span><span class="sxs-lookup"><span data-stu-id="c587a-108">Use the list price, standard cost, and current cost to configure default cost and list prices.</span></span> <span data-ttu-id="c587a-109">इन डिफाल्ट सूची की कीमतों का इस्तेमाल केवल कोट लाइन या प्रोजेक्ट कांट्रेक्ट लाइन के लिए किया जाता है जब सिस्टम को किसी कोट या प्रोजेक्ट कांट्रेक्ट के लिए प्रॉडक्ट कीमत लाइन में उस प्रॉडक्ट की कीमत सूची लाइन नहीं मिल पाती है।</span><span class="sxs-lookup"><span data-stu-id="c587a-109">The default list prices are used on a quote line or a project contract line only when the system can't find a price list line for that product in the product price list for the quote or project contract.</span></span>

<span data-ttu-id="c587a-110">प्रॉडक्ट कैटेलॉग लाइनों की लागत कीमत को कोट के बीच परिवर्तित किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="c587a-110">The cost price of product catalog lines can be changed between quotes.</span></span> <span data-ttu-id="c587a-111">यह सक्षमता महत्वपूर्ण है क्योंकि यदि आप सटीक ढंग से लागतों का पता नहीं लगा सकते हैं तो आप प्रोजेक्ट के प्रचालनीय लाभ को भी निर्धारित नहीं कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="c587a-111">This capability is important, because if you don't accurately track costs, you can't determine operational profits on project engagements.</span></span> <span data-ttu-id="c587a-112">डिफ़ॉल्ट रूप से, उत्पाद की मानक लागत का इस्तेमाल लागत कीमत के रूप में किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="c587a-112">By default, the standard cost of the product is used as the cost price.</span></span> <span data-ttu-id="c587a-113">हालांकि, डिफाल्ट लागत कीमत को कोट लाइन पर अपडेट किया जा सकता है यदि उस कोट के लिए अलग लागत कीमत हो।</span><span class="sxs-lookup"><span data-stu-id="c587a-113">However, the default cost price can be updated on the quote line if there's a different cost price for that quote.</span></span>

## <a name="price-list-items"></a><span data-ttu-id="c587a-114">कीमत सूची के आइटम</span><span class="sxs-lookup"><span data-stu-id="c587a-114">Price list items</span></span>

<span data-ttu-id="c587a-115">आप एक प्रॉडक्ट कैटेलॉग से दूसरी कीमत सूचियों में उत्पाद जोड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="c587a-115">You can add products from a product catalog to different price lists.</span></span> <span data-ttu-id="c587a-116">प्रॉडक्ट की कीमत सूची लाइनें एक विशेष यूनिट को बताती हैं।</span><span class="sxs-lookup"><span data-stu-id="c587a-116">Price list lines for products always reference a specific unit.</span></span> <span data-ttu-id="c587a-117">कीमत सूची मदों पर प्रॉडक्ट के कीमत निर्धारण को मुद्रा की राशि के रूप में कॉन्फ़िगर किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="c587a-117">Pricing for a product on price list items can be configured as a currency amount.</span></span> <span data-ttu-id="c587a-118">वैकल्पिक रूप स, इसे कीमत सूची, चालू लागत या मानक लागत के कार्य के रूप में कॉन्फ़िगर किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="c587a-118">Alternatively, it can be configured as a function of the list price, current cost, or standard cost.</span></span>

<span data-ttu-id="c587a-119">जब उत्पाद मूल्य को कीमत सूची, मानक लागत या चालू लागत के कार्य के रूप में कन्फीगर किया जाता है तो मूल्य निर्धारण की कार्यक्षमता विभिन्न राउंडिंग विकल्पों का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="c587a-119">Pricing functionality supports various rounding options when product prices are configured as a function of the list price, standard cost, or current cost.</span></span> <span data-ttu-id="c587a-120">एक से अधिक कीमत निर्धारण विधियों और राउंडिंग विकल्पों का लाभ लेने के अलावा, आप डिस्काउंट सूची को कीमत सूची की मदों के साथ जोड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="c587a-120">In addition to taking advantage of multiple pricing methods and rounding options, you can associate discount lists with price list items.</span></span> 

 
## <a name="default-product-price-list"></a><span data-ttu-id="c587a-121">डिफाल्ट प्रॉडक्ट कीमत सूची</span><span class="sxs-lookup"><span data-stu-id="c587a-121">Default product price list</span></span>
<span data-ttu-id="c587a-122">प्रत्येक ग्राहक रिकार्ड में **डिफॉल्ट मूल्य लिस्ट** फील्ड होता है जहाँ आप ग्राहक की मुद्रा से मेल करने वाली कीमत सूची को निर्दिष्ट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="c587a-122">Each customer record has a **Default Price List** field, where you can specify a price list that matches the currency of the customer.</span></span> <span data-ttu-id="c587a-123">डिफाल्ट मूल्य इस फील्ड में अपने आप दर्ज नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="c587a-123">A default value isn't automatically entered in this field.</span></span> <span data-ttu-id="c587a-124">जब किसी विशेष ग्राहक के साथ कस्टम कीमत निर्धारण करार मौजूद होता है तो आप इस फील्ड का इस्तेमाल उस ग्राहक के साथ कीमत सूची से जोड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="c587a-124">When a custom pricing agreement with a specific customer exists, you can use this field to associate a price list with that customer.</span></span>

<span data-ttu-id="c587a-125">अवसर, कोट और प्रोजेक्ट कांट्रेक्ट एंटिटी डिफाल्ट प्रॉडक्ट कीमत सूचियों को दर्ज करने के लिए निम्नलिखित क्रम का इस्तेमाल करते हैं।</span><span class="sxs-lookup"><span data-stu-id="c587a-125">The Opportunity, Quote, and Project Contract entities use the following order to enter default product price lists.</span></span> <span data-ttu-id="c587a-126">इसी क्रम का इस्तेमाल प्रोजेक्ट कीमत सूचियों के लिए किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="c587a-126">The same order is used for project price lists.</span></span>

1.  <span data-ttu-id="c587a-127">भाव प्रस्ताव</span><span class="sxs-lookup"><span data-stu-id="c587a-127">Quote</span></span>
2.  <span data-ttu-id="c587a-128">अवसर</span><span class="sxs-lookup"><span data-stu-id="c587a-128">Opportunity</span></span>
3.  <span data-ttu-id="c587a-129">ग्राहक</span><span class="sxs-lookup"><span data-stu-id="c587a-129">Customer</span></span>
4.  <span data-ttu-id="c587a-130">ग्लोबल सेटिंग</span><span class="sxs-lookup"><span data-stu-id="c587a-130">Global settings</span></span> 

<span data-ttu-id="c587a-131">डिफाल्ट द्वारा, कोट लाइन पर **प्रॉडक्ट** फील्ड कोट की प्रॉडक्ट कीमत सूची में सभी सक्रिय प्रॉडक्ट की सूची बनाता है।</span><span class="sxs-lookup"><span data-stu-id="c587a-131">By default, the **Product** field on the quote line lists all the active products in the product price list of the quote.</span></span> <span data-ttu-id="c587a-132">यदि कोई प्रॉडक्ट निष्क्रिय किया गया हो यो यदि वह ड्राफ्ट प्रॉडक्ट हो तो कीमत की सूची में होने पर भी उसे सूचीबद्ध नहीं किया जाता।</span><span class="sxs-lookup"><span data-stu-id="c587a-132">If a product has been inactivated, or if it's a draft product, it isn't listed, even if it's in the price list.</span></span> 

<span data-ttu-id="c587a-133">प्रोजेक्ट कांट्रेक्ट के लिए बनाए गए पहले इनवॉइस पर इनवॉइस लाइनों के रूप में प्रॉडक्ट कैटेलॉग लाइनों को जोड़ा जाता है।</span><span class="sxs-lookup"><span data-stu-id="c587a-133">Product catalog lines are added as invoice lines on the first invoice that is created for a project contract.</span></span> <span data-ttu-id="c587a-134">ड्राफ्ट इनवॉइस में, ऐसी इनवॉइस लाइनों को हटाया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="c587a-134">On a draft invoice, those invoice lines can be deleted.</span></span> <span data-ttu-id="c587a-135">ऐसे मामले में, ये लाइनें इनवॉइस बनाए जाने तक या इनवॉइस ग्राहक को भेजे जाने तक, बाद की इनवॉइस में दिखता रहेगा।</span><span class="sxs-lookup"><span data-stu-id="c587a-135">In that case, the lines will appear on a subsequent invoice until they are invoiced, or until the invoice is sent to the customer.</span></span> <span data-ttu-id="c587a-136">आप प्रॉडक्ट इनवॉइस लाइन की आंशिक मात्रा का बीजक नहीं बना सकते.</span><span class="sxs-lookup"><span data-stu-id="c587a-136">You can't invoice a partial quantity of a product invoice line.</span></span> <span data-ttu-id="c587a-137">जब प्रोजेक्ट कांट्रेक्ट से प्रॉडक्ट लाइनों का इनवॉइस बनाया जाता है, तो वास्तविक इनवॉइस बनाया जाता है।</span><span class="sxs-lookup"><span data-stu-id="c587a-137">When the product lines from the project contract are invoiced, actuals are created.</span></span> <span data-ttu-id="c587a-138">हालांकि, ऐसे वास्तविक इनवॉइस संबंधित प्रोजेक्ट एंटिटी से जोड़े नहीं जाते।</span><span class="sxs-lookup"><span data-stu-id="c587a-138">However, those actuals aren't linked to the related project entity.</span></span> <span data-ttu-id="c587a-139">दूसरे शब्दों में, प्रॉडक्ट-आधारित प्रोजेक्ट कांट्रेक्ट लाइनें किसी प्रोजेक्ट-आधारित इस्तेमाल से स्वतंत्र होती हैं।</span><span class="sxs-lookup"><span data-stu-id="c587a-139">In other words, product-based project contract lines are independent of any project-based use.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]
