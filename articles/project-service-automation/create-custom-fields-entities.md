---
title: कस्टम फ़ील्ड और एंटिटी बनाएँ
description: यह विषय बताता है कि Power Apps प्लेटफ़ॉर्म में अपने स्वयं के समाधान में विकल्प सेट और इकाईयाँ कैसे बनाएं.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/26/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: fb160bfd-e037-4a21-a968-3ff2e6e16481
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 7ee30e3bb6b8034ef226e2e9181195685355011f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3752081"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="e2cfd-103">कस्टम फ़ील्ड और एंटिटी बनाएँ</span><span class="sxs-lookup"><span data-stu-id="e2cfd-103">Create custom fields and entities</span></span> 

<span data-ttu-id="e2cfd-104">निम्नलिखित चरणों को किसी भी समय पूरा करें, जिनको आप Power Apps प्लेटफ़ॉर्म पर कस्टम विकल्प सेट या इकाई बनाना चाहते हैं।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="e2cfd-105">Project Service Automation (PSA) के वेब इंटरफेस का उपयोग करके इस विषय की प्रक्रियाओं को पूरा किया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e2cfd-106">हम सिफारिश करते हैं कि आप एक अलग समाधान में सभी कस्टम मूल्य निर्धारण आयाम परिवर्तन करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="e2cfd-107">यह महत्वपूर्ण सर्वोत्तम अभ्यास भविष्य में आवश्यकतानुसार परिवर्तन या अपडेट करने के लिए लचीलापन प्रदान करता है, आपके काम के पुन: उपयोग में मदद करेगा, और इन परिवर्तनों को दूसरे उदाहरण में पोर्ट करना आसान बनाता है।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="e2cfd-108">आपके द्वारा सभी आवश्यक परिवर्तन किए जाने के बाद, इस समाधान को **प्रबंधित समाधान** के रूप में निर्यात करें और अपने मूल्य निर्धारण सेटअप का पुन: उपयोग करने के लिए इसे अन्य उदाहरणों में आयात करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>


## <a name="create-a-custom-solution-for-pricing-dimensions"></a><span data-ttu-id="e2cfd-109">मूल्य निर्धारण आयामों के लिए एक कस्टम समाधान बनाएं</span><span class="sxs-lookup"><span data-stu-id="e2cfd-109">Create a custom solution for pricing dimensions</span></span>
1. <span data-ttu-id="e2cfd-110">PSA में, **सेटिंग्स** > **समाधान** पर क्लिक करें और फिर नया समाधान बनाने के लिए **नया** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-110">In PSA, click **Settings** > **Solutions**, and then click **New** to create a new solution.</span></span> 
2. <span data-ttu-id="e2cfd-111">समाधान का नाम दें, **\<आपके संगठन का नाम> मूल्य निर्धारण के आयामों**, शेष आवश्यक जानकारी दर्ज करें और फिर **सहेजें** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-111">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then click **Save**.</span></span>

> ![मूल्य निर्धारण आयामों के लिए एक कस्टम समाधान बनाना](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="e2cfd-113">मूल्य निर्धारण आयाम समाधान में कस्टम फ़ील्ड और विकल्प सेट बनाएं</span><span class="sxs-lookup"><span data-stu-id="e2cfd-113">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="e2cfd-114">एक मूल्य निर्धारण आयाम विकल्प सेट या इकाई हो सकता है।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-114">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="e2cfd-115">दोनों को आपके मूल्य निर्धारण समाधान में बनाया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-115">Both must be created in your pricing solution.</span></span> <span data-ttu-id="e2cfd-116">इस प्रक्रिया के चरण बताते हैं कि इकाई-आधारित आयाम और विकल्प सेट-आधारित आयाम कैसे बनाएं।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-116">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="e2cfd-117">इकाई-आधारित आयाम</span><span class="sxs-lookup"><span data-stu-id="e2cfd-117">Entity-based dimensions</span></span>

1. <span data-ttu-id="e2cfd-118">PSA में, **सेटिंग्स** > **समाधान** पर क्लिक करें और फिर **\<आपके संगठन का नाम> मूल्य निर्धारण आयामों** पर डबल-क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-118">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="e2cfd-119">Solution Explorer में, बाएं नेविगेशन पैन पर, **इकाइयां** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-119">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="e2cfd-120">**मानक शीर्षक** नामक एक नई इकाई बनाने के लिए **नया** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-120">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="e2cfd-121">शेष आवश्यक जानकारी दर्ज करें और फिर **सहेजें** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-121">Enter the remaining required information, and then click **Save**.</span></span>

> ![मानक शीर्षक इकाई परिभाषा](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="e2cfd-123">विकल्प सेट-आधारित आयाम</span><span class="sxs-lookup"><span data-stu-id="e2cfd-123">Option set-based dimensions</span></span> 
<span data-ttu-id="e2cfd-124">आप दो विकल्प सेट-आधारित आयाम बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-124">You can create two option set-based dimensions.</span></span> <span data-ttu-id="e2cfd-125">**घर** कार्य स्थान और **ऑनसाइट** काम की कीमत को ट्रैक करने के लिए **संसाधन कार्य स्थान** का उपयोग करें और काम पूरा होने पर मार्कअप लागू करने के लिए **संसाधन कार्य के घंटे** को मूल्य **नियमित** और **ओवरटाइम** के साथ उपयोग करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-125">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="e2cfd-126">PSA में, **सेटिंग्स** > **समाधान** पर क्लिक करें और फिर **\<आपके संगठन का नाम> मूल्य निर्धारण आयामों** पर डबल-क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-126">In PSA, click **Settings** > **Solutions**, and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="e2cfd-127">समाधान एक्स्प्लोरर में, बाएं नेविगेशन पैन पर, **विकल्प सेट** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-127">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="e2cfd-128">नया विकल्प सेट करने के लिए **नया** पर क्लिक करें, बाकी आवश्यक जानकारी दर्ज करें और फिर **सहेजें** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-128">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="e2cfd-129">विकल्प सेट आधारित मूल्य निर्धारण आयाम जिसे संसाधन कार्य स्थान कहा जाता है</span><span class="sxs-lookup"><span data-stu-id="e2cfd-129">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="e2cfd-130">विकल्प सेट आधारित मूल्य निर्धारण आयाम जिसे संसाधन कार्य घंटे कहा जाता है</span><span class="sxs-lookup"><span data-stu-id="e2cfd-130">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="e2cfd-131">इकाई-आधारित आयामों के लिए डेटा बनाएं</span><span class="sxs-lookup"><span data-stu-id="e2cfd-131">Create data for entity-based dimensions</span></span>

<span data-ttu-id="e2cfd-132">आप इकाई-आधारित आयामों के लिए मैनुअल रूप से या Microsoft Excel आयात या सेवा कॉल का उपयोग करके डेटा बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-132">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="e2cfd-133">दो मानक शीर्षक बनाने के लिए इस प्रक्रिया में चरणों का उपयोग करें, इकाई-आधारित आयाम, **मानक शीर्षक** से **सिस्टम इंजीनियर** और **वरिष्ठ सिस्टम इंजीनियर**।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-133">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="e2cfd-134">यदि आप जो डेटा बनाना चाहते हैं वह छोटा है, तो निम्न उदाहरण में, आप एक मानक फॉर्म का उपयोग कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-134">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="e2cfd-135">PSA में, **उन्नत खोज** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-135">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="e2cfd-136">इकाई **मानक शीर्षक** का चयन करें और फिर **नतीजे** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-136">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="e2cfd-137">**मानक शीर्षक** इकाई में सभी पंक्तियों को दिखाया जाएगा।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-137">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="e2cfd-138">**नया** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-138">Click **New**.</span></span> <span data-ttu-id="e2cfd-139">**नाम** फ़ील्ड में, "सिस्टम इंजीनियर" दर्ज करें और फिर **सहेजें** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-139">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="e2cfd-140">प्रपत्र बंद करें.</span><span class="sxs-lookup"><span data-stu-id="e2cfd-140">Close the form.</span></span> 
4. <span data-ttu-id="e2cfd-141">"सीनियर सिस्टम्स इंजीनियर" के लिए एक और मानक शीर्षक बनाने के लिए चरण 1 - 3 को दोहराएं।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-141">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="e2cfd-142">मानक शीर्षक इकाई के लिए नमूना डेटा</span><span class="sxs-lookup"><span data-stu-id="e2cfd-142">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)

## <a name="add-all-required-psa-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="e2cfd-143">मूल्य निर्धारण आयाम समाधान के लिए सभी आवश्यक PSA संस्थाओं और संबंधित हिस्सों को जोड़ें</span><span class="sxs-lookup"><span data-stu-id="e2cfd-143">Add all required PSA entities and related components to the Pricing Dimension Solution</span></span>
<span data-ttu-id="e2cfd-144">आपको अपने मूल्य निर्धारण समाधान में निम्नलिखित Project Service इकाइयों को जोड़ना होगा।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-144">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="e2cfd-145">मूल्य निर्धारण समाधान में कुछ महत्वपूर्ण स्कीमा परिवर्तन करने के लिए इस प्रक्रिया में चरणों का उपयोग करें ताकि इकाइयां नए मूल्य निर्धारण आयामों से अवगत हो सकें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-145">Use the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="e2cfd-146">PSA में, **सेटिंग्स** > **समाधान** पर क्लिक करें और फिर **\<आपके संगठन का नाम> मूल्य निर्धारण आयामों** पर डबल-क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-146">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="e2cfd-147">समाधान एक्सप्लोरर में, बाएं नेविगेशन पैन पर, **मौजूदा जोड़ें** > **इकाइयां** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-147">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="e2cfd-148">**समाधान हिस्से** संवाद बॉक्स में, निम्नलिखित इकाइयों का चयन करें:</span><span class="sxs-lookup"><span data-stu-id="e2cfd-148">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="e2cfd-149">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="e2cfd-149">Actual</span></span>
- <span data-ttu-id="e2cfd-150">बुक करने योग्य संसाधन</span><span class="sxs-lookup"><span data-stu-id="e2cfd-150">Bookable Resource</span></span>
- <span data-ttu-id="e2cfd-151">अनुमान पंक्ति</span><span class="sxs-lookup"><span data-stu-id="e2cfd-151">Estimate Line</span></span>
- <span data-ttu-id="e2cfd-152">इनवॉइस पंक्ति विवरण</span><span class="sxs-lookup"><span data-stu-id="e2cfd-152">Invoice Line Detail</span></span>
- <span data-ttu-id="e2cfd-153">जर्नल पंक्ति</span><span class="sxs-lookup"><span data-stu-id="e2cfd-153">Journal Line</span></span>
- <span data-ttu-id="e2cfd-154">प्रोजेक्ट अनुबंध लाइन विवरण</span><span class="sxs-lookup"><span data-stu-id="e2cfd-154">Project Contract Line Detail</span></span>
- <span data-ttu-id="e2cfd-155">प्रोजेक्ट टीम सदस्य</span><span class="sxs-lookup"><span data-stu-id="e2cfd-155">Project Team Member</span></span>
- <span data-ttu-id="e2cfd-156">कोट पंक्ति विवरण</span><span class="sxs-lookup"><span data-stu-id="e2cfd-156">Quote Line Detail</span></span>
- <span data-ttu-id="e2cfd-157">भूमिका मू्ल्य मार्कअप</span><span class="sxs-lookup"><span data-stu-id="e2cfd-157">Role Price Markup</span></span>
- <span data-ttu-id="e2cfd-158">भूमिका मू्ल्य</span><span class="sxs-lookup"><span data-stu-id="e2cfd-158">Role Price</span></span> 
- <span data-ttu-id="e2cfd-159">समय प्रविष्टि</span><span class="sxs-lookup"><span data-stu-id="e2cfd-159">Time Entry</span></span> 

> ![मूल्य निर्धारण आयाम समाधान में मौजूदा इकाइयां जोड़ें](media/Existing-entities-to-PD-solution.png)

> ![समाधान घटक चुनें](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="e2cfd-162">चयनित सभी संस्थाओं के लिए सभी फॉर्मों और दृश्य को शामिल करना सुनिश्चित करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-162">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="e2cfd-163">जब ऊपर चयनित संस्थाओं के लिए किसी भी निर्भर संस्थाओं को शामिल करने के लिए कहा जाए, तो **नहीं** क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e2cfd-163">When prompted to include any dependent entities for the entities selected above, click **No**.</span></span>

> ![सभी संबंधित हिस्सों को शामिल न करें](media/Do-not-include-required.png)


