---
title: कस्टम फ़ील्ड और एंटिटी बनाएँ
description: यह विषय बताता है कि Power Apps प्लेटफ़ॉर्म में अपने स्वयं के समाधान में विकल्प सेट और इकाईयाँ कैसे बनाएं.
author: Rumant
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 3d838bde8a3d7cbc15e06fb3289924468c284a8a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998953"
---
# <a name="create-custom-fields-and-entities"></a><span data-ttu-id="dde42-103">कस्टम फ़ील्ड और एंटिटी बनाएँ</span><span class="sxs-lookup"><span data-stu-id="dde42-103">Create custom fields and entities</span></span> 

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="dde42-104">निम्नलिखित चरणों को किसी भी समय पूरा करें, जिनको आप Power Apps प्लेटफ़ॉर्म पर कस्टम विकल्प सेट या इकाई बनाना चाहते हैं।</span><span class="sxs-lookup"><span data-stu-id="dde42-104">Complete the following steps any time that you want to create a custom option set or entity on the Power Apps platform.</span></span>  
<span data-ttu-id="dde42-105">Project Service Automation (PSA) के वेब इंटरफेस का उपयोग करके इस विषय की प्रक्रियाओं को पूरा किया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="dde42-105">The procedures in this topic should be completed using the web interface of Project Service Automation (PSA).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="dde42-106">हम सिफारिश करते हैं कि आप एक अलग समाधान में सभी कस्टम मूल्य निर्धारण आयाम परिवर्तन करें।</span><span class="sxs-lookup"><span data-stu-id="dde42-106">We recommend that you make all custom pricing dimension changes in a separate solution.</span></span> <span data-ttu-id="dde42-107">यह महत्वपूर्ण सर्वोत्तम अभ्यास भविष्य में आवश्यकतानुसार परिवर्तन या अपडेट करने के लिए लचीलापन प्रदान करता है, आपके काम के पुन: उपयोग में मदद करेगा, और इन परिवर्तनों को दूसरे उदाहरण में पोर्ट करना आसान बनाता है।</span><span class="sxs-lookup"><span data-stu-id="dde42-107">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="dde42-108">आपके द्वारा सभी आवश्यक परिवर्तन किए जाने के बाद, इस समाधान को **प्रबंधित समाधान** के रूप में निर्यात करें और अपने मूल्य निर्धारण सेटअप का पुन: उपयोग करने के लिए इसे अन्य उदाहरणों में आयात करें।</span><span class="sxs-lookup"><span data-stu-id="dde42-108">After you have made all of the required changes, export this solution as a **Managed solution** and import it into other instances to reuse your pricing setup.</span></span>

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a><span data-ttu-id="dde42-109">मूल्य निर्धारण आयाम समाधान में कस्टम फ़ील्ड और विकल्प सेट बनाएं</span><span class="sxs-lookup"><span data-stu-id="dde42-109">Create custom fields and option sets in the pricing dimension solution</span></span>

<span data-ttu-id="dde42-110">एक मूल्य निर्धारण आयाम विकल्प सेट या इकाई हो सकता है।</span><span class="sxs-lookup"><span data-stu-id="dde42-110">A pricing dimension can be an option set or an entity.</span></span> <span data-ttu-id="dde42-111">दोनों को आपके मूल्य निर्धारण समाधान में बनाया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="dde42-111">Both must be created in your pricing solution.</span></span> <span data-ttu-id="dde42-112">इस प्रक्रिया के चरण बताते हैं कि इकाई-आधारित आयाम और विकल्प सेट-आधारित आयाम कैसे बनाएं।</span><span class="sxs-lookup"><span data-stu-id="dde42-112">The steps in this procedure explain how to create entity-based dimensions and option set-based dimensions.</span></span>

### <a name="entity-based-dimensions"></a><span data-ttu-id="dde42-113">इकाई-आधारित आयाम</span><span class="sxs-lookup"><span data-stu-id="dde42-113">Entity-based dimensions</span></span>

1. <span data-ttu-id="dde42-114">PSA में, **सेटिंग** > **समाधान** पर क्लिक करें, और उसके बाद **\<your organization name> के मूल्य निर्धारण आयाम पर डबल-क्लिक करें**.</span><span class="sxs-lookup"><span data-stu-id="dde42-114">In PSA, click **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span>
2. <span data-ttu-id="dde42-115">Solution Explorer में, बाएं नेविगेशन पैन पर, **इकाइयां** चुनें।</span><span class="sxs-lookup"><span data-stu-id="dde42-115">In Solution Explorer, on the left navigation pane, select **Entities**.</span></span>
3. <span data-ttu-id="dde42-116">**मानक शीर्षक** नामक एक नई इकाई बनाने के लिए **नया** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="dde42-116">Click **New** to create a new entity called **Standard Title**.</span></span> <span data-ttu-id="dde42-117">शेष आवश्यक जानकारी दर्ज करें और फिर **सहेजें** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="dde42-117">Enter the remaining required information, and then click **Save**.</span></span>

> ![मानक शीर्षक इकाई परिभाषा](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a><span data-ttu-id="dde42-119">विकल्प सेट-आधारित आयाम</span><span class="sxs-lookup"><span data-stu-id="dde42-119">Option set-based dimensions</span></span> 
<span data-ttu-id="dde42-120">आप दो विकल्प सेट-आधारित आयाम बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="dde42-120">You can create two option set-based dimensions.</span></span> <span data-ttu-id="dde42-121">**घर** कार्य स्थान और **ऑनसाइट** काम की कीमत को ट्रैक करने के लिए **संसाधन कार्य स्थान** का उपयोग करें और काम पूरा होने पर मार्कअप लागू करने के लिए **संसाधन कार्य के घंटे** को मूल्य **नियमित** और **ओवरटाइम** के साथ उपयोग करें।</span><span class="sxs-lookup"><span data-stu-id="dde42-121">Use **Resource Work Location** to track the price of **Home** location work and **Onsite** work and use **Resource Work hours** with values **Regular** and **Overtime** to apply a markup when work is completed.</span></span>


1. <span data-ttu-id="dde42-122">PSA में, **सेटिंग** > **समाधान** पर क्लिक करें, और उसके बाद **\<your organization name> के मूल्य निर्धारण आयाम पर डबल-क्लिक करें**.</span><span class="sxs-lookup"><span data-stu-id="dde42-122">In PSA, click **Settings** > **Solutions**, and then double-click  **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="dde42-123">समाधान एक्स्प्लोरर में, बाएं नेविगेशन पैन पर, **विकल्प सेट** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="dde42-123">In Solution Explorer, on the left navigation pane, select  **Option Sets**.</span></span> 
3. <span data-ttu-id="dde42-124">नया विकल्प सेट करने के लिए **नया** पर क्लिक करें, बाकी आवश्यक जानकारी दर्ज करें और फिर **सहेजें** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="dde42-124">Click **New** to create a new option set, enter the remaining required information, and then click **Save**.</span></span>

> ![<span data-ttu-id="dde42-125">विकल्प सेट आधारित मूल्य निर्धारण आयाम जिसे संसाधन कार्य स्थान कहा जाता है</span><span class="sxs-lookup"><span data-stu-id="dde42-125">Option set based pricing dimension called Resource Work Location</span></span> ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![<span data-ttu-id="dde42-126">विकल्प सेट आधारित मूल्य निर्धारण आयाम जिसे संसाधन कार्य घंटे कहा जाता है</span><span class="sxs-lookup"><span data-stu-id="dde42-126">Option set based pricing dimension called Resource Work Hours</span></span> ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a><span data-ttu-id="dde42-127">इकाई-आधारित आयामों के लिए डेटा बनाएं</span><span class="sxs-lookup"><span data-stu-id="dde42-127">Create data for entity-based dimensions</span></span>

<span data-ttu-id="dde42-128">आप इकाई-आधारित आयामों के लिए मैनुअल रूप से या Microsoft Excel आयात या सेवा कॉल का उपयोग करके डेटा बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="dde42-128">You can create data for entity-based dimensions manually, or by using Microsoft Excel import or service calls.</span></span> <span data-ttu-id="dde42-129">दो मानक शीर्षक बनाने के लिए इस प्रक्रिया में चरणों का उपयोग करें, इकाई-आधारित आयाम, **मानक शीर्षक** से **सिस्टम इंजीनियर** और **वरिष्ठ सिस्टम इंजीनियर**।</span><span class="sxs-lookup"><span data-stu-id="dde42-129">Use the steps in this procedure to create two standard titles, **Systems Engineer** and **Senior Systems Engineer** from the entity-based dimension, **Standard Title**.</span></span> <span data-ttu-id="dde42-130">यदि आप जो डेटा बनाना चाहते हैं वह छोटा है, तो निम्न उदाहरण में, आप एक मानक फॉर्म का उपयोग कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="dde42-130">If the data that you want to create is small, as in the following example, you can use a standard form.</span></span>

1. <span data-ttu-id="dde42-131">PSA में, **उन्नत खोज** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="dde42-131">In PSA, click **Advanced Find**.</span></span> <span data-ttu-id="dde42-132">इकाई **मानक शीर्षक** का चयन करें और फिर **नतीजे** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="dde42-132">Select the entity **Standard Title** and then click **Results**.</span></span> <span data-ttu-id="dde42-133">**मानक शीर्षक** इकाई में सभी पंक्तियों को दिखाया जाएगा।</span><span class="sxs-lookup"><span data-stu-id="dde42-133">All of the rows in the **Standard Title** entity will be shown.</span></span>
2. <span data-ttu-id="dde42-134">**नया** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="dde42-134">Click **New**.</span></span> <span data-ttu-id="dde42-135">**नाम** फ़ील्ड में, "सिस्टम इंजीनियर" दर्ज करें और फिर **सहेजें** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="dde42-135">In the **Name** field, enter "Systems Engineer" and then click **Save**.</span></span>
3. <span data-ttu-id="dde42-136">प्रपत्र बंद करें.</span><span class="sxs-lookup"><span data-stu-id="dde42-136">Close the form.</span></span> 
4. <span data-ttu-id="dde42-137">"सीनियर सिस्टम्स इंजीनियर" के लिए एक और मानक शीर्षक बनाने के लिए चरण 1 - 3 को दोहराएं।</span><span class="sxs-lookup"><span data-stu-id="dde42-137">Repeat steps 1 - 3 to create another standard title for "Senior Systems Engineer".</span></span>

> ![<span data-ttu-id="dde42-138">मानक शीर्षक इकाई के लिए नमूना डेटा</span><span class="sxs-lookup"><span data-stu-id="dde42-138">Sample Data for Standard Title entity</span></span> ](media/ST-data.png)




[!INCLUDE[footer-include](../includes/footer-banner.md)]