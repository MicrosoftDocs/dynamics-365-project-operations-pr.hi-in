---
title: मूल्य निर्धारण आयामों के रूप में कस्टम फ़ील्ड और निकाय बनाएँ
description: यह विषय कस्टम विकल्प सेट या निकाय बनाने के बारे में जानकारी देता है.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
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
ms.openlocfilehash: 616bcd5758b434b45bd06aa1a026f32efc8b7f99
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130895"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a><span data-ttu-id="04f58-103">मूल्य निर्धारण आयामों के रूप में कस्टम फ़ील्ड और निकाय बनाएँ</span><span class="sxs-lookup"><span data-stu-id="04f58-103">Create custom fields and entities as pricing dimensions</span></span>

<span data-ttu-id="04f58-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="04f58-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="04f58-105">निम्नलिखित चरणों को किसी भी समय पूरा करें, जिनको आप कस्टम विकल्प सेट या निकाय बनाना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="04f58-105">Complete the following steps any time that you want to create a custom option set or entity.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="04f58-106">हम सिफारिश करते हैं कि आप एक अलग समाधान में सभी कस्टम मूल्य निर्धारण आयाम परिवर्तन करें।</span><span class="sxs-lookup"><span data-stu-id="04f58-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="04f58-107">यह महत्वपूर्ण सर्वोत्तम अभ्यास भविष्य में आवश्यकतानुसार परिवर्तन या अपडेट करने के लिए लचीलापन प्रदान करता है, आपके काम के पुन: उपयोग में मदद करेगा, और इन परिवर्तनों को दूसरे उदाहरण में पोर्ट करना आसान बनाता है।</span><span class="sxs-lookup"><span data-stu-id="04f58-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="04f58-108">आपके द्वारा सभी आवश्यक परिवर्तन किए जाने के बाद, इस समाधान को **प्रबंधित समाधान** के रूप में निर्यात करें और अपने मूल्य निर्धारण सेटअप का पुन: उपयोग करने के लिए इसे अन्य उदाहरणों में आयात करें।</span><span class="sxs-lookup"><span data-stu-id="04f58-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="04f58-109">मूल्य निर्धारण आयामों के लिए एक कस्टम समाधान बनाएं</span><span class="sxs-lookup"><span data-stu-id="04f58-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="04f58-110">**सेटिंग्स** > **समाधान** पर जाएँ, और फिर नया समाधान बनाने के लिए **नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="04f58-110">Go to **Settings** > **Solutions**, and then select **New** to create a new solution.</span></span> 
2. <span data-ttu-id="04f58-111">समाधान का नाम दें, **\<your organization name> मूल्य निर्धारण के आयामों**, शेष आवश्यक जानकारी दर्ज करें और फिर **सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="04f58-111">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then select **Save**.</span></span>
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="04f58-112">मूल्य निर्धारण आयाम समाधान में कस्टम फ़ील्ड और विकल्प सेट बनाएं</span><span class="sxs-lookup"><span data-stu-id="04f58-112">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="04f58-113">एक मूल्य निर्धारण आयाम विकल्प सेट या इकाई हो सकता है।</span><span class="sxs-lookup"><span data-stu-id="04f58-113">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="04f58-114">दोनों को आपके मूल्य निर्धारण समाधान में बनाया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="04f58-114">Both must be created in your pricing solution.</span></span> <span data-ttu-id="04f58-115">इस प्रक्रिया के चरण बताते हैं कि इकाई-आधारित आयाम और विकल्प सेट-आधारित आयाम कैसे बनाएं।</span><span class="sxs-lookup"><span data-stu-id="04f58-115">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="04f58-116">इकाई-आधारित आयाम</span><span class="sxs-lookup"><span data-stu-id="04f58-116">Entity-based dimensions</span></span>

1. <span data-ttu-id="04f58-117">**समायोजन** > **समाधान** पर जाएँ, और तब डबल-क्लिक करें **\<your organization name> मूल्य निर्धारण के आयाम**.</span><span class="sxs-lookup"><span data-stu-id="04f58-117">Go to **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="04f58-118">Solution Explorer में, बाएं नेविगेशन पैन पर, **इकाइयां** चुनें।</span><span class="sxs-lookup"><span data-stu-id="04f58-118">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="04f58-119">मानक लीड सत्व **मानक शीर्षक** नामक एक नई निकाय बनाने के लिए **नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="04f58-119">Select **New** to create a new entity called **Standard Title**.</span></span> 
4. <span data-ttu-id="04f58-120">शेष आवश्यक जानकारी दर्ज करें और फिर **सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="04f58-120">Enter the remaining required information, and then select **Save**.</span></span>


### <a name="option-set-based-dimensions"></a><span data-ttu-id="04f58-121">विकल्प सेट-आधारित आयाम</span><span class="sxs-lookup"><span data-stu-id="04f58-121">Option set-based dimensions</span></span> 
<span data-ttu-id="04f58-122">आप दो विकल्प सेट-आधारित आयाम बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="04f58-122">You can create two option set-based dimensions.</span></span> <span data-ttu-id="04f58-123">**घर** कार्य स्थान और **ऑनसाइट** काम की कीमत को ट्रैक करने के लिए **संसाधन कार्य स्थान** का उपयोग करें और काम पूरा होने पर मार्कअप लागू करने के लिए **संसाधन कार्य के घंटे** को मूल्य **नियमित** और **ओवरटाइम** के साथ उपयोग करें।</span><span class="sxs-lookup"><span data-stu-id="04f58-123">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="04f58-124">**समायोजन** > **समाधान** पर जाएँ, और डबल-क्लिक करें  **\<your organization name> मूल्य निर्धारण के आयाम**.</span><span class="sxs-lookup"><span data-stu-id="04f58-124">Go to **Settings** > **Solutions**, and double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="04f58-125">समाधान एक्स्प्लोरर में, बाएं नेविगेशन पैन पर, **विकल्प सेट** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="04f58-125">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="04f58-126">नया विकल्प सेट करने के लिए **नया** चुनें, बाकी आवश्यक जानकारी दर्ज करें और फिर **सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="04f58-126">Select **New** to create a new option set, enter the remaining required information, and then select **Save**.</span></span>

## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="04f58-127">इकाई-आधारित आयामों के लिए डेटा बनाएं</span><span class="sxs-lookup"><span data-stu-id="04f58-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="04f58-128">आप इकाई-आधारित आयामों के लिए मैनुअल रूप से या Microsoft Excel आयात या सेवा कॉल का उपयोग करके डेटा बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="04f58-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="04f58-129">दो मानक शीर्षक बनाने के लिए इस प्रक्रिया में चरणों का उपयोग करें, इकाई-आधारित आयाम, **मानक शीर्षक** से **सिस्टम इंजीनियर** और **वरिष्ठ सिस्टम इंजीनियर**।</span><span class="sxs-lookup"><span data-stu-id="04f58-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="04f58-130">यदि आप जो डेटा बनाना चाहते हैं वह छोटा है, तो निम्न उदाहरण में, आप एक मानक फॉर्म का उपयोग कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="04f58-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="04f58-131">**उन्नत खोज** चुनें, निकाय **मानक शीर्षक** चुनें और फिर **परिणाम** चुनें.</span><span class="sxs-lookup"><span data-stu-id="04f58-131">Select **Advanced Find**, select the entity **Standard Title**, and then select **Results**.</span></span> <span data-ttu-id="04f58-132">**मानक शीर्षक** इकाई में सभी पंक्तियों को दिखाया जाएगा।</span><span class="sxs-lookup"><span data-stu-id="04f58-132">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="04f58-133">**नया** चुनें, और **नाम** फ़ील्ड में, "सिस्टम इंजीनियर" दर्ज करें और फिर **सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="04f58-133">Select **New**, and in the **Name** field, enter "Systems Engineer" and then select **Save**.</span></span>
3. <span data-ttu-id="04f58-134">प्रपत्र बंद करें.</span><span class="sxs-lookup"><span data-stu-id="04f58-134">Close the form.</span></span> 
4. <span data-ttu-id="04f58-135">"सीनियर सिस्टम्स इंजीनियर" के लिए एक और मानक शीर्षक बनाने के लिए चरण 1 - 3 को दोहराएं।</span><span class="sxs-lookup"><span data-stu-id="04f58-135">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="04f58-136">मूल्य निर्धारण आयाम समाधान के लिए सभी आवश्यक संस्थाओं और संबंधित हिस्सों को जोड़ें</span><span class="sxs-lookup"><span data-stu-id="04f58-136">Add all required entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="04f58-137">आपको अपने मूल्य निर्धारण समाधान में निम्नलिखित इकाइयों को जोड़ना होगा.</span><span class="sxs-lookup"><span data-stu-id="04f58-137">You will need to add the following entities to your pricing solution.</span></span> <span data-ttu-id="04f58-138">मूल्य निर्धारण समाधान में कुछ महत्वपूर्ण स्कीमा परिवर्तन करने के लिए इस प्रक्रिया में चरणों का उपयोग करें ताकि इकाइयां नए मूल्य निर्धारण आयामों से अवगत हो सकें।</span><span class="sxs-lookup"><span data-stu-id="04f58-138">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="04f58-139">**समायोजन** > **समाधान** चुनें, और डबल-क्लिक करें **\<your organization name> मूल्य निर्धारण के आयाम**.</span><span class="sxs-lookup"><span data-stu-id="04f58-139">Select **Settings** > **Solutions**, and double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="04f58-140">समाधान एक्सप्लोरर में, बाएं नेविगेशन पैन पर, **मौजूदा जोड़ें** > **इकाइयां** चुनें।</span><span class="sxs-lookup"><span data-stu-id="04f58-140">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="04f58-141">**समाधान हिस्से** संवाद बॉक्स में, निम्नलिखित इकाइयों का चयन करें:</span><span class="sxs-lookup"><span data-stu-id="04f58-141">In the **Solution Components** dialog box, select the following entities:</span></span>

  - <span data-ttu-id="04f58-142">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="04f58-142">Actual</span></span>
  - <span data-ttu-id="04f58-143">बुक करने योग्य संसाधन</span><span class="sxs-lookup"><span data-stu-id="04f58-143">Bookable Resource</span></span>
  - <span data-ttu-id="04f58-144">अनुमान पंक्ति</span><span class="sxs-lookup"><span data-stu-id="04f58-144">Estimate Line</span></span>
  - <span data-ttu-id="04f58-145">इनवॉइस पंक्ति विवरण</span><span class="sxs-lookup"><span data-stu-id="04f58-145">Invoice Line Detail</span></span>
  - <span data-ttu-id="04f58-146">जर्नल पंक्ति</span><span class="sxs-lookup"><span data-stu-id="04f58-146">Journal Line</span></span>
  - <span data-ttu-id="04f58-147">प्रोजेक्ट अनुबंध लाइन विवरण</span><span class="sxs-lookup"><span data-stu-id="04f58-147">Project Contract Line Detail</span></span>
  - <span data-ttu-id="04f58-148">परियोजना टीम सदस्य</span><span class="sxs-lookup"><span data-stu-id="04f58-148">Project Team Member</span></span>
  - <span data-ttu-id="04f58-149">कोट पंक्ति विवरण</span><span class="sxs-lookup"><span data-stu-id="04f58-149">Quote Line Detail</span></span>
  - <span data-ttu-id="04f58-150">भूमिका मू्ल्य मार्कअप</span><span class="sxs-lookup"><span data-stu-id="04f58-150">Role Price Markup</span></span>
  - <span data-ttu-id="04f58-151">भूमिका मू्ल्य</span><span class="sxs-lookup"><span data-stu-id="04f58-151">Role Price</span></span> 
  - <span data-ttu-id="04f58-152">समय प्रविष्टि</span><span class="sxs-lookup"><span data-stu-id="04f58-152">Time Entry</span></span> 


> [!NOTE]
> <span data-ttu-id="04f58-153">चयनित सभी संस्थाओं के लिए सभी फॉर्मों और दृश्य को शामिल करना सुनिश्चित करें।</span><span class="sxs-lookup"><span data-stu-id="04f58-153">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="04f58-154">जब ऊपर चयनित संस्थाओं के लिए किसी भी निर्भर संस्थाओं को शामिल करने के लिए कहा जाए, तो **नहीं** चुनें.</span><span class="sxs-lookup"><span data-stu-id="04f58-154">When prompted to include any dependent entities for the entities selected above, select **No**.</span></span>

