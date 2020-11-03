---
title: विक्रय मूल्य सूची सेटअप
description: यह विषय परियोजना के मूल्य निर्धारण के लिए बिक्री मूल्य सूचियों के बारे में जानकारी प्रदान करता है.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 1d2c797b72666123eb0a18d2d0c1df9fe3d207f7
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077755"
---
# <a name="sales-price-list-setup"></a><span data-ttu-id="f1691-103">विक्रय मूल्य सूची सेटअप</span><span class="sxs-lookup"><span data-stu-id="f1691-103">Sales price list setup</span></span>

<span data-ttu-id="f1691-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="f1691-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f1691-105">प्रोजेक्ट कोटेशन और अनुबंधों के लिए, एक प्रोजेक्ट मूल्य सूची में उत्पाद मूल्य सूची की तुलना में एक अलग मूल्य ओवरराइड पैटर्न होता है।</span><span class="sxs-lookup"><span data-stu-id="f1691-105">For project quotes and contracts, a project price list has a different price override pattern than a product price list.</span></span> <span data-ttu-id="f1691-106">उत्पाद सूची-आधारित कोटेशन लाइन पर, आप मूल्य और भूमिका श्रेणियों को सीधे कोटेशन लाइन पर ओवरराइड कर सकते हैं, क्योंकि प्रत्येक कोटेशन लाइन पूरी तरह से एक कैटलॉग आइटम की ओर इशारा करती है।</span><span class="sxs-lookup"><span data-stu-id="f1691-106">On a product catalog–based quote line, you can override the price to roles and categories directly on the quote line, because each quote line points to exactly one catalog item.</span></span> <span data-ttu-id="f1691-107">हालांकि, प्रोजेक्ट-आधारित कोटेशन लाइन पर, आप सीधे कोटेशन लाइन पर भूमिकाओं और श्रेणियों के लिए मूल्य को ओवरराइड नहीं कर सकते।</span><span class="sxs-lookup"><span data-stu-id="f1691-107">However, on a project-based quote line, you can't override the price to roles and categories directly on the quote line.</span></span> <span data-ttu-id="f1691-108">आप परियोजना मूल्य सूची का उपयोग दो अलग-अलग ओवरराइड पैटर्न के साथ काम करने के लिए कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="f1691-108">You can use the project price list to work with the two distinct override patterns.</span></span>

> [!NOTE]
> <span data-ttu-id="f1691-109">जब आप मूल्य निर्धारण को ओवरराइड करते हैं तो दोनों के बीच व्यवहार के अंतर के कारण, हम यह सिफारिश करते हैं कि आपके पास अपने प्रोजेक्ट संसाधनों और आपके पास कैटलॉग आइटम के लिए एक अलग मूल्य सूची हो।</span><span class="sxs-lookup"><span data-stu-id="f1691-109">We recommend that you have a separate price list for your project resources and your catalog items, because of the behavior differences between the two when you override pricing.</span></span>

<span data-ttu-id="f1691-110">निम्नलिखित इकाइयों में से हर एक में प्रोजेक्ट मूल्य निर्धारण के लिए एक या एक से अधिक बिक्री मूल्य सूची हो सकती है:</span><span class="sxs-lookup"><span data-stu-id="f1691-110">Each of the following entities can have one or more associated sales price lists for project pricing:</span></span>

- <span data-ttu-id="f1691-111">ग्राहक (खाता)</span><span class="sxs-lookup"><span data-stu-id="f1691-111">Customer (account)</span></span> 
- <span data-ttu-id="f1691-112">अवसर</span><span class="sxs-lookup"><span data-stu-id="f1691-112">Opportunity</span></span> 
- <span data-ttu-id="f1691-113">कोट</span><span class="sxs-lookup"><span data-stu-id="f1691-113">Quote</span></span> 
- <span data-ttu-id="f1691-114">प्रोजेक्ट अनुबंध</span><span class="sxs-lookup"><span data-stu-id="f1691-114">Project Contract</span></span>

<span data-ttu-id="f1691-115">मूल्य सूची के साथ इन इकाइयों का सहयोग प्रोजेक्ट मूल्य सूचियों द्वारा दर्शाया गया है।</span><span class="sxs-lookup"><span data-stu-id="f1691-115">The association of these entities with a price list is indicated by the project price lists.</span></span> <span data-ttu-id="f1691-116">आप ग्राहक, अवसर, कोटेशन और प्रोजेक्ट अनुबंध बिक्री इकाइयों के साथ एक या एक से अधिक मूल्य सूची जोड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="f1691-116">You can associate one or more price lists with the Customer, Opportunity, Quote, and Project Contract sales entities.</span></span>

<span data-ttu-id="f1691-117">एक डिफ़ॉल्ट प्रोजेक्ट मूल्य सूची स्वत: ग्राहक रिकॉर्ड पर दर्ज नहीं की जाती है।</span><span class="sxs-lookup"><span data-stu-id="f1691-117">A default project price list isn't automatically entered on a customer record.</span></span> <span data-ttu-id="f1691-118">हालांकि, आप ग्राहक रिकॉर्ड के लिए प्रोजेक्ट मूल्य सूची को मैनुअल रूप से जोड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="f1691-118">However, you can manually attach a project price list to the customer record.</span></span> <span data-ttu-id="f1691-119">फिर भी, आपको मैनुअल रूप से केवल तभी प्रोजेक्ट मूल्य सूची जोड़नी चाहिए जब आपके पास ग्राहक के साथ कस्टम मूल्य निर्धारण समझौता हो।</span><span class="sxs-lookup"><span data-stu-id="f1691-119">Nevertheless, you should manually attach a project price list only when you have a custom pricing agreement with the customer.</span></span> 

<span data-ttu-id="f1691-120">जब कोई परियोजना मूल्य सूची बिक्री निकाय से जुड़ी होती है, तो निम्नलिखित जानकारी मान्य है:</span><span class="sxs-lookup"><span data-stu-id="f1691-120">When a project price list is attached to a sales entity, the following information is validated:</span></span>

- <span data-ttu-id="f1691-121">मूल्य सूची में **विक्रय** का संदर्भ है.</span><span class="sxs-lookup"><span data-stu-id="f1691-121">The price list has a context of **Sales**.</span></span> 
- <span data-ttu-id="f1691-122">मूल्य सूची मुद्रा ग्राहक मुद्रा से मेल खाती है।</span><span class="sxs-lookup"><span data-stu-id="f1691-122">The price list currency matches the customer currency.</span></span> 

<span data-ttu-id="f1691-123">परियोजना अनुबंध पर, संबंधित परियोजना मूल्य सूचियों को स्वत: सेट करने के लिए पूर्ववर्ती क्रम का उपयोग किया जाता है:</span><span class="sxs-lookup"><span data-stu-id="f1691-123">On a project contract, the following order of precedence is used to automatically set related project price lists:</span></span>

1. <span data-ttu-id="f1691-124">भाव प्रस्ताव</span><span class="sxs-lookup"><span data-stu-id="f1691-124">Quote</span></span>
2. <span data-ttu-id="f1691-125">अवसर</span><span class="sxs-lookup"><span data-stu-id="f1691-125">Opportunity</span></span>
3. <span data-ttu-id="f1691-126">ग्राहक</span><span class="sxs-lookup"><span data-stu-id="f1691-126">Customer</span></span> 
4. <span data-ttu-id="f1691-127">ग्लोबल सेटिंग</span><span class="sxs-lookup"><span data-stu-id="f1691-127">Global settings</span></span> 

<span data-ttu-id="f1691-128">जब एक प्रोजेक्ट मूल्य सूची डिफ़ॉल्ट रूप से दर्ज की जाती है, तो सिस्टम पुष्टि करता है कि मुद्रा ग्राहक की मुद्रा से मेल खाती है, और जो डिफ़ॉल्ट मूल्य सूची दर्ज की गई है, उसका संदर्भ **विक्रय** है.</span><span class="sxs-lookup"><span data-stu-id="f1691-128">When a project price list is entered by default, the system validates that the currency matches the customer’s currency, and that the default price lists that have been entered have a context of **Sales**.</span></span>

<span data-ttu-id="f1691-129">आप ग्राहक, अवसर, कोटेशन और प्रोजेक्ट अनुबंध इकाइयों के साथ कई प्रोजेक्ट मूल्य सूचियां जोड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="f1691-129">You can associate multiple project price lists with the Customer, Opportunity, Quote, and Project Contract entities.</span></span> <span data-ttu-id="f1691-130">यह क्षमता लंबे समय से चल रहे उन प्रोजेक्ट अनुबंध के लिए दिनांक-विशिष्ट डिफ़ॉल्ट कीमतों का समर्थन करती है, जहां आपको मुद्रास्फीति के कारण होने वाले मूल्य अपडेट के लिए एक से अधिक मूल्य सूची की आवश्यकता हो सकती है।</span><span class="sxs-lookup"><span data-stu-id="f1691-130">This capability supports date-specific default prices for a long-running project contract, where you might require more than one price list to account for price updates that occur because of inflation.</span></span> <span data-ttu-id="f1691-131">हालांकि, यदि वह मूल्य सूची जिसे आप ग्राहक, अवसर, कोटेशन या प्रोजेक्ट अनुबंध इकाई के साथ जोड़ते हैं में ओवरलैपिंग की तिथि प्रभावी है, तो डिफ़ॉल्ट मूल्य गलत हो सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="f1691-131">However, if the price lists that you associate with the Customer, Opportunity, Quote, or Project Contract entity have overlapping date effectivity, the default prices might be incorrect.</span></span> <span data-ttu-id="f1691-132">इसलिए, आपको यह सुनिश्चित करना चाहिए कि ओवरलैपिंग तिथि प्रभावी वाली प्रोजेक्ट मूल्य सूचियां उन इकाइयों से संबद्ध नहीं हैं।</span><span class="sxs-lookup"><span data-stu-id="f1691-132">Therefore, you should make sure that project price lists that have overlapping date effectivity aren't associated with those entities.</span></span>
