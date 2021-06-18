---
title: परियोजना विक्रय मूल्य सूचियाँ ओवरराइड करें
description: यह विषय कस्टम विक्रय मूल्य सूचियाँ बनाने के बारे में जानकारी प्रदान करता है.
author: rumant
ms.date: 10/22/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: db2ff6acaad6ab4cbcc98d3d5b06b36ed23b758f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5995083"
---
# <a name="override-project-sales-price-lists"></a><span data-ttu-id="a3d86-103">परियोजना विक्रय मूल्य सूचियाँ ओवरराइड करें</span><span class="sxs-lookup"><span data-stu-id="a3d86-103">Override project sales price lists</span></span>

<span data-ttu-id="a3d86-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="a3d86-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

## <a name="customer-specific-project-price-lists"></a><span data-ttu-id="a3d86-105">ग्राहक-विशिष्ट परियोजना मूल्य सूचियाँ</span><span class="sxs-lookup"><span data-stu-id="a3d86-105">Customer-specific project price lists</span></span>

<span data-ttu-id="a3d86-106">Dynamics 365 Project Operations में खाता-रिकॉर्ड पर ग्राहक-विशिष्ट मूल्य अनुबंधों को परियोजना मूल्य सूचियों के रूप में सेट किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="a3d86-106">Customer-specific price agreements can be set up as project price lists on an account record in Dynamics 365 Project Operations.</span></span>

<span data-ttu-id="a3d86-107">ग्राहक-विशिष्ट परियोजना मूल्य सूची सेट अप करने के लिए, **विक्रय** क्षेत्र में, खाता रिकॉर्ड पर नेविगेट करें.</span><span class="sxs-lookup"><span data-stu-id="a3d86-107">To set up a customer-specific project price list, in the **Sales** area, navigate to the account record.</span></span>

1. <span data-ttu-id="a3d86-108">**खाते** सूची पृष्ठ खोलें.</span><span class="sxs-lookup"><span data-stu-id="a3d86-108">Open the **Accounts** list page.</span></span>
2. <span data-ttu-id="a3d86-109">**खाता** विवरण पृष्ठ को खोलने के लिए ग्राहक रिकॉर्ड का पता लगाएँ और उस पर डबल-क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="a3d86-109">Locate and double-click a customer record to open the **Account** details page.</span></span>
3. <span data-ttu-id="a3d86-110">**परियोजना मूल्य सूची** टैब पर, **+ नई परियोजना मूल्य सूची** चुनें.</span><span class="sxs-lookup"><span data-stu-id="a3d86-110">On the **Project Price lists** tab, select **+ New Project Price List**.</span></span>
4. <span data-ttu-id="a3d86-111">**नई परियोजना मूल्य सूची** पृष्ठ पर, ड्रॉप-डाउन से मूल्य सूची चुनें.</span><span class="sxs-lookup"><span data-stu-id="a3d86-111">On the **New Project Price List** page, select a price list from the drop-down.</span></span> <span data-ttu-id="a3d86-112">केवल वे मूल्य सूचियाँ, जिनका संदर्भ **विक्रय** पर सेट है और जिनकी मुद्रा खाता मुद्रा से मेल खाती है, शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="a3d86-112">Only price lists that have the context set to **Sales** and whose currency matches the account currency are included.</span></span>
5. <span data-ttu-id="a3d86-113">संबद्धता को नाम दें और उसके बाद **सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="a3d86-113">Name the association, and then select **Save**.</span></span> <span data-ttu-id="a3d86-114">ग्राहक-विशिष्ट परियोजना मूल्य सूची बनाई जाती है.</span><span class="sxs-lookup"><span data-stu-id="a3d86-114">A customer-specific project price list is created.</span></span> <span data-ttu-id="a3d86-115">इस मूल्य सूची का उपयोग इस ग्राहक के लिए बनाए गए परियोजना कोट या अनुबंधों पर परियोजना मूल्यों को डिफ़ॉल्ट करने के लिए किया जाएगा, जहां कोट या परियोजना अनुबंध का निर्माण दिनांक मूल्य सूची के दिनांक प्रभावकारिता के भीतर आता है.</span><span class="sxs-lookup"><span data-stu-id="a3d86-115">This price list will be used to default project prices on project quotes or contracts created for this customer where the created date of the quote or project contract falls within the date effectivity of the price list.</span></span>

## <a name="custom-pricing-on-project-quotes"></a><span data-ttu-id="a3d86-116">परियोजना कोट पर कस्टम मूल्य निर्धारण</span><span class="sxs-lookup"><span data-stu-id="a3d86-116">Custom pricing on project quotes</span></span>

<span data-ttu-id="a3d86-117">परियोजना कोट पर, आपके पास ऐसा परियोजना मूल्य निर्धारण हो सकता है, जो डिफ़ॉल्ट मानक मूल्य सूची से शुरू होता है, जो ग्राहक से या परियोजना पैरामीटर से डिफ़ॉल्ट होता है.</span><span class="sxs-lookup"><span data-stu-id="a3d86-117">On project quotes, you can have project pricing that starts with a default standard price list that defaults from the customer or from the project parameters.</span></span>

<span data-ttu-id="a3d86-118">जब आपको किसी विशेष कोट पर परियोजना-संबंधित कार्य के लिए कस्टम मूल्य निर्धारण की आवश्यकता होती है, तो आप परियोजना मूल्य सूची संबद्ध निकाय से उसे प्राप्त कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a3d86-118">When you need custom pricing for project-related work on a particular quote, you can get that from the project price lists associated entity.</span></span>

<span data-ttu-id="a3d86-119">कोट-विशिष्ट परियोजना मूल्य निर्धारण सेट अप करने के लिए निम्न चरणों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="a3d86-119">Complete the following steps to set up quote-specific project pricing.</span></span>

1. <span data-ttu-id="a3d86-120">परियोजना कोट खोलें और **परियोजना मूल्य सूचियाँ** टैब चुनें.</span><span class="sxs-lookup"><span data-stu-id="a3d86-120">Open the project quote and select the **Project Price Lists** tab.</span></span>
2. <span data-ttu-id="a3d86-121">सब-ग्रिड में, **कस्टम मूल्य निर्धारण बनाएँ** चुनें.</span><span class="sxs-lookup"><span data-stu-id="a3d86-121">In the subgrid, select **Create custom pricing**.</span></span>

<span data-ttu-id="a3d86-122">कोट से संलग्न सभी परियोजना मूल्य सूचियाँ को नई मूल्य सूचियों पर कॉपी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="a3d86-122">All the project price lists that are attached to the quote are copied to new price lists.</span></span> <span data-ttu-id="a3d86-123">नई मूल्य सूचियों के नाम, इन मूल्य सूचियों के निर्माण के दिनांक-समय स्टैम्प के साथ कोट के नाम को दर्शाते हैं.</span><span class="sxs-lookup"><span data-stu-id="a3d86-123">The names of the new price lists reflect the name of quote with a date-time stamp for when these price lists were created.</span></span>

<span data-ttu-id="a3d86-124">आप उन मूल्य सूचियों में से प्रत्येक का उपयोग कर सकते हैं और लेबर (भूमिका मूल्य) और व्यय (श्रेणी मूल्य) मूल्य पर अद्यतन कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a3d86-124">You can use each of those price lists and make updates to labor (role price) and expense (category price) prices.</span></span> <span data-ttu-id="a3d86-125">ये मूल्य केवल इस परियोजना कोट पर लागू होंगे.</span><span class="sxs-lookup"><span data-stu-id="a3d86-125">These prices will only be applicable to this project quote.</span></span>

## <a name="price-lists-on-a-project-contract"></a><span data-ttu-id="a3d86-126">परियोजना अनुबंध पर मूल्य सूचियाँ</span><span class="sxs-lookup"><span data-stu-id="a3d86-126">Price lists on a project contract</span></span>

<span data-ttu-id="a3d86-127">परियोजना अनुबंध पर, परियोजना मूल्य निर्धारण हमेशा अनुबंध के नाम और नाम के साथ जोड़े गए निर्माण दिनांक समय स्टैम्प के साथ कस्टम मूल्य सूची के रूप में डिफ़ॉल्ट होते हैं.</span><span class="sxs-lookup"><span data-stu-id="a3d86-127">On a project contract, project pricing always defaults as a custom price list with the name of contract and the created date time stamp appended to the name.</span></span> <span data-ttu-id="a3d86-128">यह सही है चाहे तो अनुबंध को तब बनाया गया था, जब कोट को जीता गया था या अनुबंध को शुरुआत से बनाया गया था.</span><span class="sxs-lookup"><span data-stu-id="a3d86-128">This is true whether the contract was created when the quote was won or if the contract was created from scratch.</span></span> <span data-ttu-id="a3d86-129">यदि आवश्यक हो, तो आप कस्टम मूल्य सूची की संबद्धता को निकाल सकते हैं या इसके बजाए परियोजना अनुबंध से मानक मूल्य सूची संबद्ध कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a3d86-129">If needed, you can remove this association to the custom price list and associate a standard price list to the project contract instead.</span></span>

<span data-ttu-id="a3d86-130">जब आप मानक मूल्य सूची को कोट या अनुबंध पर परियोजना मूल्य सूचियों से संबद्ध करते हैं, तो मूल्य सूची के मूल्यों में किए गए कोई भी परिवर्तन उन सभी कोट और अनुबंधों को प्रभावित करेंगे, जो मूल्य सूची का उपयोग करते हैं.</span><span class="sxs-lookup"><span data-stu-id="a3d86-130">When you associate a standard price list to the project price lists on quote or contract, any changes made to the prices in the price list will impact all quotes and contracts that use the price list.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]