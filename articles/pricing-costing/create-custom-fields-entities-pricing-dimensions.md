---
title: मूल्य निर्धारण आयामों के रूप में कस्टम फ़ील्ड और निकाय बनाएँ
description: यह विषय कस्टम विकल्प सेट या निकाय बनाने के बारे में जानकारी देता है.
author: rumant
manager: AnnBe
ms.date: 11/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: fc5917856b8f28d36dc55593a68eba7823a00b36
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642815"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="11e2b-103">मूल्य निर्धारण आयामों के रूप में कस्टम फ़ील्ड और निकाय बनाएँ</span><span class="sxs-lookup"><span data-stu-id="11e2b-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="11e2b-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="11e2b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="11e2b-105">जब आप कस्टम विकल्प सेट या निकाय बनाना चाहें, ताकि उसका उपयोग मूल्य निर्धारण आयाम के रूप में किया जा सके, तो निम्नलिखित चरणों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="11e2b-105">Complete the following steps when you want to create a custom option set or entity for using it as a pricing dimension.</span></span> <span data-ttu-id="11e2b-106">अधिक जानकारी के लिए, [मूल्य निर्धारण आयाम ओवरव्यू](pricing-dimensions-overview.md) देखें.</span><span class="sxs-lookup"><span data-stu-id="11e2b-106">For more information, see [Pricing dimensions overview](pricing-dimensions-overview.md).</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="11e2b-107">हम सिफारिश करते हैं कि आप एक अलग समाधान में सभी कस्टम मूल्य निर्धारण आयाम परिवर्तन करें।</span><span class="sxs-lookup"><span data-stu-id="11e2b-107">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="11e2b-108">यह महत्वपूर्ण सर्वोत्तम व्यवहार भविष्य में आवश्यकतानुसार परिवर्तन अद्यतन करने या निकालने के लिए लचीलापन प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="11e2b-108">This important best practice provides flexibility in the future to update or remove changes as needed.</span></span> <span data-ttu-id="11e2b-109">यह आपके कार्य का पुनः उपयोग करने में भी मदद करेगा और इन बदलावों को दूसरी आवृत्ति में पोर्ट करना आसान बना देगा. सभी आवश्यक परिवर्तन करने के बाद, इस समाधान को **प्रबंधित समाधान** के रूप में निर्यात करें और अपने मूल्य निर्धारण सेटअप का पुन: उपयोग करने के लिए इसे अन्य आवृत्तियों में आयात करें.</span><span class="sxs-lookup"><span data-stu-id="11e2b-109">This will also help with re-use of your work and make it easier to port these changes to another instance After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="11e2b-110">मूल्य निर्धारण आयाम समाधान में कस्टम फ़ील्ड और विकल्प सेट बनाएं</span><span class="sxs-lookup"><span data-stu-id="11e2b-110">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="11e2b-111">एक मूल्य निर्धारण आयाम विकल्प सेट या इकाई हो सकता है।</span><span class="sxs-lookup"><span data-stu-id="11e2b-111">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="11e2b-112">दोनों को आपके मूल्य निर्धारण समाधान में बनाया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="11e2b-112">Both must be created in your pricing solution.</span></span> <span data-ttu-id="11e2b-113">इस प्रक्रिया के चरण बताते हैं कि इकाई-आधारित आयाम और विकल्प सेट-आधारित आयाम कैसे बनाएं।</span><span class="sxs-lookup"><span data-stu-id="11e2b-113">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="11e2b-114">इकाई-आधारित आयाम</span><span class="sxs-lookup"><span data-stu-id="11e2b-114">Entity-based dimensions</span></span>
<span data-ttu-id="11e2b-115">निकाय-आधारित आयाम बनाने के लिए, इन चरणों का पालन करें:</span><span class="sxs-lookup"><span data-stu-id="11e2b-115">To create entity-based dimensions, follow these steps:</span></span>

1. <span data-ttu-id="11e2b-116">**समायोजन** > **समाधान** पर जाएँ, और तब डबल-क्लिक करें **\<your organization name> मूल्य निर्धारण के आयाम**.</span><span class="sxs-lookup"><span data-stu-id="11e2b-116">Go to **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="11e2b-117">समाधान एक्सप्लोरर में, बाएं नेविगेशन फलक में, **इकाइयाँ** चुनें.</span><span class="sxs-lookup"><span data-stu-id="11e2b-117">In Solution Explorer, in the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="11e2b-118">मानक लीड सत्व **मानक शीर्षक** नामक एक नई निकाय बनाने के लिए **नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="11e2b-118">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="11e2b-119">शेष आवश्यक जानकारी दर्ज करें और फिर **सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="11e2b-119">Enter the remaining required information, and then select **Save**.</span></span>

> ![मानक शीर्षक इकाई परिभाषा](media/Standard-Title-entity-definition.png)

### <a name="option-set-based-dimensions"></a><span data-ttu-id="11e2b-121">विकल्प सेट-आधारित आयाम</span><span class="sxs-lookup"><span data-stu-id="11e2b-121">Option set-based dimensions</span></span> 
<span data-ttu-id="11e2b-122">आप दो विकल्प सेट-आधारित आयाम बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="11e2b-122">You can create two option set-based dimensions.</span></span> 

- <span data-ttu-id="11e2b-123">**होम** स्थान कार्य और **ऑनसाइट** कार्य का मूल्य ट्रैक करने के लिए **संसाधन कार्य स्थान** का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="11e2b-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work.</span></span> 
- <span data-ttu-id="11e2b-124">कार्य पूर्ण होने पर मार्कअप लागू करने के लिए, **नियमित** और **ओवरटाइम** के साथ **संसाधन कार्य घंटों** का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="11e2b-124">Use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when the work is complete.</span></span>

<span data-ttu-id="11e2b-125">निम्नलिखित ग्राफ़िक **संसाधन कार्य स्थान** आयाम का एक दृश्य प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="11e2b-125">The following graphic provides a view of the **Resource Work Location** dimension.</span></span> 

> ![विकल्प सेट आधारित मूल्य निर्धारण आयाम जिसे संसाधन कार्य स्थान कहा जाता है](media/Option-set-PD-called-Resource-Work-Location.png)

<span data-ttu-id="11e2b-127">निम्नलिखित ग्राफ़िक **संसाधन कार्य घंटे** आयाम का एक दृश्य प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="11e2b-127">The following graphic provides a view of the **Resource Work Hours** dimension.</span></span> 

> ![विकल्प सेट आधारित मूल्य निर्धारण आयाम जिसे संसाधन कार्य घंटे कहा जाता है](media/Option-set-PD-called-Resource-Work-Hours.png)

1. <span data-ttu-id="11e2b-129">**समायोजन** > **समाधान** पर जाएँ, और डबल-क्लिक करें  **\<your organization name> मूल्य निर्धारण के आयाम**.</span><span class="sxs-lookup"><span data-stu-id="11e2b-129">Go to **Settings** > **Solutions**, and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="11e2b-130">समाधान एक्स्प्लोरर में, बाएं नेविगेशन फलक में, **विकल्प सेट** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="11e2b-130">In Solution Explorer, in the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="11e2b-131">नया विकल्प सेट करने के लिए **नया** चुनें, बाकी आवश्यक जानकारी दर्ज करें और फिर **सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="11e2b-131">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="11e2b-132">इकाई-आधारित आयामों के लिए डेटा बनाएं</span><span class="sxs-lookup"><span data-stu-id="11e2b-132">Create data for entity-based dimensions</span></span>

<span data-ttu-id="11e2b-133">आप इकाई-आधारित आयामों के लिए मैनुअल रूप से या Microsoft Excel आयात या सेवा कॉल का उपयोग करके डेटा बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="11e2b-133">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="11e2b-134">दो मानक शीर्षक बनाने के लिए इस प्रक्रिया में चरणों का उपयोग करें, इकाई-आधारित आयाम, **मानक शीर्षक** से **सिस्टम इंजीनियर** और **वरिष्ठ सिस्टम इंजीनियर**।</span><span class="sxs-lookup"><span data-stu-id="11e2b-134">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="11e2b-135">यदि आप जो डेटा बनाना चाहते हैं वह छोटा है, तो निम्न उदाहरण में, आप एक मानक फॉर्म का उपयोग कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="11e2b-135">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="11e2b-136">**उन्नत खोज** चुनें.</span><span class="sxs-lookup"><span data-stu-id="11e2b-136">Select **Advanced Find**.</span></span>
2. <span data-ttu-id="11e2b-137">निकाय **मानक शीर्षक** का चयन करें और उसके बाद **परिणाम** चुनें.</span><span class="sxs-lookup"><span data-stu-id="11e2b-137">Select the entity **Standard Title**, and then select **Results**.</span></span> <span data-ttu-id="11e2b-138">**मानक शीर्षक** इकाई में सभी पंक्तियों को दिखाया जाएगा।</span><span class="sxs-lookup"><span data-stu-id="11e2b-138">All of the rows in the **Standard Title** entity will be shown.</span></span>
3. <span data-ttu-id="11e2b-139">**नया** चुनें, और **नाम** फ़ील्ड में, "सिस्टम इंजीनियर" दर्ज करें और फिर **सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="11e2b-139">Select **New**, and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
4. <span data-ttu-id="11e2b-140">पृष्ठ बंद करें.</span><span class="sxs-lookup"><span data-stu-id="11e2b-140">Close the page.</span></span> 
5. <span data-ttu-id="11e2b-141">"सीनियर सिस्टम्स इंजीनियर" के लिए एक और मानक शीर्षक बनाने के लिए चरण 1 - 3 को दोहराएं।</span><span class="sxs-lookup"><span data-stu-id="11e2b-141">Repeat steps 1-3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![मानक शीर्षक निकाय के लिए नमूना डेटा](media/ST-data.png)
