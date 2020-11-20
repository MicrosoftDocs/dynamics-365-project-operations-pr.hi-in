---
title: मैं प्रोजेक्ट अवस्थाएँ व्यवसाय प्रोसेस फ़्लो कैसे अनुकूलित करूँ?
description: इस बात का अवलोकन कि प्रोजेक्ट स्टेज व्यावसायिक प्रक्रिया प्रवाह को कैसे अनुकूलित किया जाए।
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/11/2018
ms.topic: article
author: JohnPBurrows
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
ms.openlocfilehash: a999bbffff848db7a6349df380d9ed5e73c143ab
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4125043"
---
# <a name="how-do-i-customize-the-project-stages-business-process-flow"></a><span data-ttu-id="797d8-103">मैं प्रोजेक्ट अवस्थाएँ व्यवसाय प्रोसेस फ़्लो कैसे अनुकूलित करूँ?</span><span class="sxs-lookup"><span data-stu-id="797d8-103">How do I customize the Project Stages business process flow?</span></span>
[!INCLUDE[cc-applies-to-psa-app-2-4x-9-0-platform](../includes/cc-applies-to-psa-app-2-4x-9-0-platform.md)]
[!INCLUDE[cc-applies-to-psa-app-1x-8-2-platform](../includes/cc-applies-to-psa-app-1x-8-2-platform.md)]

<span data-ttu-id="797d8-104">Project Service अनुप्रयोग के पिछले संस्करणों में एक ज्ञात कमी है कि प्रोजेक्ट अवस्थाएँ व्यवसाय प्रोसेस फ़्लो में अवस्थाओं के नाम अनुमानित अंग्रेजी नामों (**Quote**, **Plan**, **Close**) से सटीक मेल खाने वाले होने चाहिए.</span><span class="sxs-lookup"><span data-stu-id="797d8-104">There's a known limitation in earlier versions of the Project Service application that the names of the stages in the Project Stages business process flow must exactly match the expected English names (**Quote**, **Plan**, **Close**).</span></span> <span data-ttu-id="797d8-105">अन्यथा, व्यवसाय तर्क, जो अंग्रेज़ी अवस्था नामों पर निर्भर करता है, अपेक्षा के अनुरूप कार्य नहीं करता.</span><span class="sxs-lookup"><span data-stu-id="797d8-105">Otherwise, the business logic, which relies on the English stage names, doesn't work as expected.</span></span> <span data-ttu-id="797d8-106">इसी कारण आपको प्रोजेक्ट प्रपत्र पर परिचित कार्रवाइयाँ, जैसे **प्रोसेस स्विच करें** या **प्रोसेस संपादित करें** उपलब्ध दिखाई नहीं देता, और व्यवसाय प्रोसेस फ़्लो को प्रोत्साहन नहीं मिलता.</span><span class="sxs-lookup"><span data-stu-id="797d8-106">That's why you don't see familiar actions such as **Switch Process** or **Edit Process** available on the project form, and customizing the business process flow isn't encouraged.</span></span> 

<span data-ttu-id="797d8-107">इस कमी को संस्करण 2.4.5.48 और इसके बाद वाले में ठीक कर लिया गया है.</span><span class="sxs-lookup"><span data-stu-id="797d8-107">This limitation has been addressed in version 2.4.5.48 and later.</span></span> <span data-ttu-id="797d8-108">यदि आपको डिफ़ॉल्ट व्यवसाय प्रोसेस फ़्लो को अनुकूलित करना है, तो यह आलेख कुछ वैकल्पिक समाधान सुझाता है.</span><span class="sxs-lookup"><span data-stu-id="797d8-108">This article provides suggested workarounds if you need to customize the default business process flow for earlier versions.</span></span>  

## <a name="business-logic-requires-an-exact-match-with-english-stage-names"></a><span data-ttu-id="797d8-109">व्यवसाय तर्क के लिए अंग्रेजी अवस्था नामों के साथ एक सटीक मिलान आवश्यक है</span><span class="sxs-lookup"><span data-stu-id="797d8-109">Business logic requires an exact match with English stage names</span></span>

<span data-ttu-id="797d8-110">प्रोजेक्ट अवस्थाएँ व्यवसाय प्रोसेस फ़्लो में व्यवसाय तर्क शामिल हैं, जो अनुप्रयोग में निम्न व्यवहार संचालित करते हैं:</span><span class="sxs-lookup"><span data-stu-id="797d8-110">The Project Stages business process flow includes business logic that drives the following behaviors in the app:</span></span>
- <span data-ttu-id="797d8-111">जब प्रोजेक्ट किसी कोट के साथ संबद्ध है, तो कोड व्यवसाय प्रोसेस फ़्लो को **Quote** अवस्था पर सेट करता है.</span><span class="sxs-lookup"><span data-stu-id="797d8-111">When the project is associated with a quote, the code sets the business process flow to the **Quote** stage.</span></span>
- <span data-ttu-id="797d8-112">जब प्रोजेक्ट किसी अनुबंध के साथ संबद्ध होता है, तो कोड व्यवसाय प्रोसेस फ़्लो को **Plan** अवस्था पर सेट करता है.</span><span class="sxs-lookup"><span data-stu-id="797d8-112">When the project is associated with a contract, the code sets the business process flow to the **Plan** stage.</span></span>
- <span data-ttu-id="797d8-113">जब व्यवसाय प्रोसेस फ़्लो **Close** अवस्था पर बढ़ता है, तो प्रोजेक्ट रिकॉर्ड निष्क्रिय हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="797d8-113">When the business process flow is advanced to the **Close** stage, the project record is deactivated.</span></span> <span data-ttu-id="797d8-114">जब प्रोजेक्ट निष्क्रिय हो जाता है, तो प्रोजेक्ट प्रपत्र और कार्य विश्लेषण संरचना (WBS) केवल पठन पर सेट हो जाते हैं, नामित संसाधन बुकिंग मुक्त हो जाते हैं, और कोई भी संबद्ध मूल्य सूची निष्क्रिय हो जाती है.</span><span class="sxs-lookup"><span data-stu-id="797d8-114">When the project is deactivated, the project form and work breakdown structure (WBS) are set to read-only, the named resource bookings are released, and any associated price lists are deactivated.</span></span>

<span data-ttu-id="797d8-115">यह व्यवसाय तर्क प्रोजेक्ट अवस्थाओं के लिए अंग्रेजी नामों पर निर्भर करता है.</span><span class="sxs-lookup"><span data-stu-id="797d8-115">This business logic relies on the English names for the project stages.</span></span> <span data-ttu-id="797d8-116">मुख्यतः अंग्रेजी अवस्था नामों पर इसी निर्भरता के कारण ही प्रोजेक्ट अवस्थाएँ व्यवसाय प्रोसेस फ़्लो के अनुकूलन को प्रोत्साहित नहीं किया जाता, साथ ही आपको प्रोजेक्ट निकाय पर सामान्य व्यवसाय प्रोसेस फ़्लो कार्रवाइयाँ, जैसे **प्रोसेस स्विच करें** या **प्रोसेस संपादित करें** दिखाई नहीं देते.</span><span class="sxs-lookup"><span data-stu-id="797d8-116">This dependency on the English stage names is the main reason why customization of the Project Stages business process flow isn't encouraged, as well as why you don’t see the common business process flow actions like **Switch Process** or **Edit Process** on the project entity.</span></span>

## <a name="what-happens-if-the-stage-names-dont-match-the-english-names"></a><span data-ttu-id="797d8-117">यदि अवस्थाओं के नाम अंग्रेजी नाम से मेल नहीं खाते तो क्या होगा?</span><span class="sxs-lookup"><span data-stu-id="797d8-117">What happens if the stage names don't match the English names?</span></span>

<span data-ttu-id="797d8-118">Project Service अनुप्रयोग संस्करण में 1.x में 8.2 प्लेटफ़ॉर्म पर, जब व्यवसाय प्रोसेस फ़्लो में अवस्था नाम अंग्रेज़ी अवस्था नामों से सटीक मेल नहीं खाते, तो कोट या अनुबंधों के लिए सही अवस्थाएँ सेट करने वाले, या प्रोजेक्ट बंद करने वाले व्यवसाय तर्क छोड़ दिए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="797d8-118">In the Project Service app version 1.x on the 8.2 platform, when the stage names in the business process flow don’t match the English stage names exactly, the business logic that sets the right stage for quotes or contracts, or that closes the project, is skipped.</span></span> <span data-ttu-id="797d8-119">कोई त्रुटि संदेश प्रदर्शित नहीं किया जाता.</span><span class="sxs-lookup"><span data-stu-id="797d8-119">No error messages are displayed.</span></span> <span data-ttu-id="797d8-120">इसलिए ऐसा लगता है कि आप प्रोजेक्ट अवस्थाएँ व्यवसाय प्रोसेस फ़्लो अनुकूलित करने में सक्षम हैं.</span><span class="sxs-lookup"><span data-stu-id="797d8-120">Therefore it appears that you are able to customize the Project Stages business process flow.</span></span> <span data-ttu-id="797d8-121">तथापि, आपको कोट, अनुबंधों या प्रोजेक्ट बंद करने के लिए कोई स्वचालित प्रोसेस दिखाई नहीं देगी.</span><span class="sxs-lookup"><span data-stu-id="797d8-121">However, you won’t see any of the automatic processes working for quotes, contracts, and project close.</span></span>

<span data-ttu-id="797d8-122">Project Service अनुप्रयोग संस्करण 2.4.4.30 या पिछले संस्करण में, 9.0 प्लेटफ़ॉर्म पर, व्यवसाय प्रोसेस फ़्लो पर एक महत्वपूर्ण संरचनात्मक परिवर्तन था, जिसमें व्यवसाय प्रोसेस फ़्लो व्यवसाय तर्क को पुनर्लेखित करना आवश्यक था.</span><span class="sxs-lookup"><span data-stu-id="797d8-122">In the Project Service app version 2.4.4.30 or earlier on the 9.0 platform, there was a significant architectural change to business process flows, which required a re-write of the business process flow business logic.</span></span> <span data-ttu-id="797d8-123">परिणामस्वरूप, यदि प्रोसेस अवस्था नाम अपेक्षित अंग्रेजी नाम से मेल नहीं खाते, तो आपको एक त्रुटि संदेश मिल जाता.</span><span class="sxs-lookup"><span data-stu-id="797d8-123">As a result, if the process stage names don’t match the expected English names, you do receive an error message.</span></span> 

<span data-ttu-id="797d8-124">इसलिए, यदि आप प्रोजेक्ट निकाय के लिए प्रोजेक्ट अवस्थाएँ व्यवसाय प्रोसेस फ़्लो अनुकूलित करना चाहते हैं, तो **Quote**, **Plan**, और **Close** को पूर्ववत रखते हुए प्रोजेक्ट निकाय के लिए डिफ़ॉल्ट व्यवसाय प्रोसेस फ़्लो पर केवल नई अवस्थाएँ जोड़ सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="797d8-124">Therefore, if you want to customize the Project Stages business process flow for the project entity, you can only add brand new stages to the default business process flow for the project entity, while keeping the **Quote**, **Plan**, and **Close** stages as-is.</span></span> <span data-ttu-id="797d8-125">यह प्रतिबंध सुनिश्चित करता है कि आपको उस व्यवसाय तर्क, जो व्यवसाय प्रोसेस फ़्लो में अंग्रेज़ी अवस्था नामों की अपेक्षा करता है, से त्रुटियाँ न मिलें.</span><span class="sxs-lookup"><span data-stu-id="797d8-125">This restriction ensures that you don’t get errors from the business logic that expects the English stage names in the business process flow.</span></span>

<span data-ttu-id="797d8-126">संस्करण 2.4.5.48 या इसके बाद वाले में, किसी प्रोजेक्ट निकाय के लिए डिफ़ॉल्ट व्यवसाय प्रोसेस फ़्लो से इस आलेख में वर्णित व्यवसाय तर्क निकाल दिए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="797d8-126">In version 2.4.5.48 or later, the business logic described in this article has been removed from the default business process flow for the project entity.</span></span> <span data-ttu-id="797d8-127">उस संस्करण या बाद के संस्करण में नवीनीकृत कर आप डिफ़ॉल्ट व्यवसाय प्रोसेस फ़्लो को अनुकूलित कर सकेंगे या इसे हमारे व्यवसाय प्रोसेस फ़्लो द्वारा प्रतिस्थापित कर सकेंगे.</span><span class="sxs-lookup"><span data-stu-id="797d8-127">Upgrading to that version or later will let you customize or replace the default business process flow with one of your own.</span></span> 

## <a name="workarounds-for-earlier-versions"></a><span data-ttu-id="797d8-128">पिछले संस्करणों के लिए वैकल्पिक समाधान</span><span class="sxs-lookup"><span data-stu-id="797d8-128">Workarounds for earlier versions</span></span>

<span data-ttu-id="797d8-129">यदि नवीनीकरण का विकल्प नहीं है, तो आप निम्न दो तरीकों में किसी एक से प्रोजेक्ट निकाय के लिए प्रोजेक्ट अवस्थाएँ व्यवसाय प्रोसेस फ़्लो अनुकूलित कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="797d8-129">If upgrading isn't an option, you can customize the Project Stages business process flow for the project entity in one of these two ways:</span></span>

1. <span data-ttu-id="797d8-130">डिफ़ॉल्ट कॉन्फ़िगरेशन पर अतिरिक्त अवस्थाएँ जोड़ें, साथ ही **Quote**, **Plan**, और **Close** के लिए अंग्रेज़ी अवस्था नाम कायम रखें.</span><span class="sxs-lookup"><span data-stu-id="797d8-130">Add additional stages to the default configuration, while retaining the English stage names for **Quote**, **Plan**, and **Close**.</span></span>


![डिफ़ॉल्ट कॉन्फ़िगरेशन पर अवस्थाएँ जोड़ने का स्क्रीनशॉट](media/FAQ-Customize-BPF-1.png)
 
2. <span data-ttu-id="797d8-132">स्वयं का व्यवसाय प्रोसेस फ़्लो बनाएँ और इसे प्रोजेक्ट निकाय के लिए प्राथमिक व्यवसाय प्रोसेस फ़्लो बनाएँ, जिससे आप मनचाहा नाम रख पाएंगे.</span><span class="sxs-lookup"><span data-stu-id="797d8-132">Create your own business process flow and make it the primary business process flow for the project entity, which lets you have any stage names you want.</span></span> <span data-ttu-id="797d8-133">तथापि, यदि आप उसी मानक प्रोजेक्ट अवस्थाओं **Quote**, **Plan**, और **Close** का उपयोग करना चाहते हैं, तो आपको कुछ अनुकूलन करने पड़ेंगे, जिनसे आपके कस्टम अवस्था नाम से छुटकारा मिल जाए.</span><span class="sxs-lookup"><span data-stu-id="797d8-133">However, if you want to use the same standard project stages **Quote**, **Plan**, and **Close**, you need to do some customizations that are driven off your custom stage names.</span></span> <span data-ttu-id="797d8-134">अधिक जटिल तर्क, प्रोजेक्ट बंद करने में लगता है, जिसे आप केवल प्रोजेक्ट रिकॉर्ड निष्क्रिय करके भी ट्रिगर कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="797d8-134">The more complex logic is in the closing of the project, which you can still trigger by just deactivating the project record.</span></span>

![BPF अनुकूलन](media/FAQ-Customize-BPF-2.png)

### <a name="additional-considerations-for-project-service-app-version-24430-or-earlier-on-platform-90"></a><span data-ttu-id="797d8-136">Project Service अनुप्रयोग संस्करण 2.4.4.30 या पिछला संस्करण, 9.0 प्लेटफ़ॉर्म पर, के लिए अतिरिक्त विचार</span><span class="sxs-lookup"><span data-stu-id="797d8-136">Additional considerations for Project Service app version 2.4.4.30 or earlier on platform 9.0</span></span>

<span data-ttu-id="797d8-137">Project Service 2.4.4.30 या पिछले संस्करण, प्लेटफ़ॉर्म 9.0 में, एक कस्टम व्यवसाय प्रोसेस फ़्लो से **अवस्था द्वारा प्रोजेक्ट** चार्ट द्वारा उपयोग में आने वाले प्रोजेक्ट निकाय पर **अवस्था नाम** फ़ील्ड और प्रोजेक्ट सूची दृश्य अद्यतन नहीं होते, क्योंकि यह डिफ़ॉल्ट प्रोजेक्ट अवस्थाएँ व्यवसाय प्रोसेस फ़्लो के साथ जुड़ा होता है.</span><span class="sxs-lookup"><span data-stu-id="797d8-137">In Project Service 2.4.4.30 or earlier on platform 9.0, with a custom business process flow the **Stage Name** field on the project entity used in the **Project By Stage** chart and project list views won’t update, because it’s coupled to the default Project Stages business process flow.</span></span> <span data-ttu-id="797d8-138">आप निम्‍नलिखित चरणों से इस समस्या का समाधान कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="797d8-138">You can address this issue with the following steps:</span></span>

- <span data-ttu-id="797d8-139">वर्तमान व्यवसाय प्रोसेस फ़्लो अवस्था कैप्चर करने के लिए एक कस्टम फ़ील्ड जोड़ें, जिसे उपयोगकर्ता के कस्टम व्यवसाय प्रोसेस फ़्लो से होकर आगे बढ़ने पर अद्यतन किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="797d8-139">Add a custom field to capture the current business process flow stage that is updated as the user advances through the custom business process flow.</span></span>

- <span data-ttu-id="797d8-140">डिफ़ॉल्ट कॉन्फ़िगरेशन के बजाय अपने कस्टम फ़ील्ड के साथ कार्य करने के लिए **अवस्था द्वारा प्रोजेक्ट** संशोधित करें.</span><span class="sxs-lookup"><span data-stu-id="797d8-140">Modify the **Project By Stage** chart to work with your custom field instead of the default configuration.</span></span>

### <a name="steps-to-create-your-own-business-process-flow-for-the-project-entity"></a><span data-ttu-id="797d8-141">प्रोजेक्ट निकाय के लिए अपने स्वयं के व्यवसाय प्रोसेस फ़्लो बनाने के चरण</span><span class="sxs-lookup"><span data-stu-id="797d8-141">Steps to create your own business process flow for the project entity</span></span>

<span data-ttu-id="797d8-142">प्रोजेक्ट निकाय के लिए अपने स्वयं के व्यवसाय प्रोसेस फ़्लो बनाने के लिए निम्न कार्य करें:</span><span class="sxs-lookup"><span data-stu-id="797d8-142">To create your own business process flow for the project entity do the following:</span></span>

1. <span data-ttu-id="797d8-143">**सेटिंग** > **प्रोसेस केंद्र** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="797d8-143">Go to **Settings** > **Process Center**.</span></span> <span data-ttu-id="797d8-144">प्रोजेक्ट अवस्थाएँ व्यवसाय प्रोसेस फ़्लो की प्रतिलिपि न बनाएँ क्योंकि इससे Project Service व्यवसाय तर्क की प्रतिलिपि भी बनती है.</span><span class="sxs-lookup"><span data-stu-id="797d8-144">Don’t copy the Project Stages business process flow because that also copies the Project Service business logic.</span></span>

  ![प्रक्रिया बनाएँ](media/FAQ-Customize-BPF-3.png)

2. <span data-ttu-id="797d8-146">वांछित अवस्था नाम बनाने के लिए प्रोसेस डिज़ाइनर का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="797d8-146">Use the Process Designer to create the stage names you want.</span></span> <span data-ttu-id="797d8-147">यदि आप **Quote**, **Plan**, और **Close** के लिए डिफ़ॉल्ट अवस्थाओं के समान कार्यक्षमता चाहते हैं, तो आपको यह अपने व्यवसाय प्रोसेस फ़्लो के अवस्था नामों के आधार पर बनाना पड़ेगा.</span><span class="sxs-lookup"><span data-stu-id="797d8-147">If you want the same functionality as the default stages for **Quote**, **Plan**, and **Close**, you’ll have to create that based on your custom business process flow’s stage names.</span></span>

   ![BPF अनुकूलित करने के लिए उपयोग में लाए गए प्रोसेस डिज़ाइनर का स्क्रीनशॉट](media/FAQ-Customize-BPF-4.png) 

3. <span data-ttu-id="797d8-149">प्रोसेस डिज़ाइनर में, **ऑर्डर प्रोसेस फ़्लो** क्लिक करें ताकि कस्टम व्यवसाय प्रोसेस फ़्लो को प्रोजेक्ट निकाय के लिए प्राथमिक व्यवसाय प्रोसेस फ़्लो बनाया जा सके, इसके लिए इसे सूची के शीर्ष पर प्रोजेक्ट अवस्थाएँ व्यवसाय प्रोसेस फ़्लो के ऊपर ले जाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="797d8-149">In the Process Designer, click **Order Process Flow** to make the custom business process flow the primary business process flow for the project entity by moving it above the Project Stages business process flow to the top of the list.</span></span>


   [<span data-ttu-id="797d8-150">ऑर्डर प्रोसेस फ़्लो का उपयोग करने का स्क्रीनशॉट</span><span class="sxs-lookup"><span data-stu-id="797d8-150">Screenshot of using Order Process Flow</span></span>](media/FAQ-Customize-BPF-5-720.png)

### <a name="the-following-steps-apply-to-project-service-app-24430-or-earlier-on-the-90-platform"></a><span data-ttu-id="797d8-151">निम्न चरण Project Service अनुप्रयोग 2.4.4.30 या पिछले संस्करण, 9.0 प्लेटफ़ॉर्म पर लागू होते हैं</span><span class="sxs-lookup"><span data-stu-id="797d8-151">The following steps apply to Project Service app 2.4.4.30 or earlier on the 9.0 platform</span></span>

4. <span data-ttu-id="797d8-152">प्रोजेक्ट निकाय पर एक कस्टम फ़ील्ड जोड़ें ताकि आपके कस्टम व्यवसाय प्रोसेस फ़्लो में कस्टम अवस्थाएँ कैप्चर की जा सके.</span><span class="sxs-lookup"><span data-stu-id="797d8-152">Add a new custom field to the project entity to capture the custom stages in your custom business process flow.</span></span> <span data-ttu-id="797d8-153">कस्टम व्यवसाय प्रोसेस फ़्लो पर अवस्था को अद्यतन करते समय आपको इस फ़ील्ड को अद्यतन करने के लिए व्यवसाय तर्क (प्लगइन/कार्यप्रवाह) जोड़ना पड़ेगा.</span><span class="sxs-lookup"><span data-stu-id="797d8-153">You’ll need to add business logic (plugin/workflow) to update this field when the stage on the custom business process flow is updated.</span></span>

   ![प्रोजेक्ट निकाय अनुकूलित करने का स्क्रीनशॉट](media/FAQ-Customize-BPF-6-720.png)

5. <span data-ttu-id="797d8-155">अवस्थाओं के लिए अपने नए कस्टम फ़ील्ड का उपयोग करने के लिए **अवस्था द्वारा प्रोजेक्ट** संशोधित करें.</span><span class="sxs-lookup"><span data-stu-id="797d8-155">Modify the **Project By Stage** chart to use your new custom field for stages.</span></span>

   ![अवस्था द्वारा प्रोजेक्ट चार्ट का उपयोग करने के स्क्रीनशॉट](media/FAQ-Customize-BPF-7-720.png)

6. <span data-ttu-id="797d8-157">प्रोजेक्ट निकाय के लिए किसी भी दृश्य को संशोधित करें ताकि अवस्थाओं के लिए आपका नया कस्टम फ़ील्ड शामिल किया जा सके.</span><span class="sxs-lookup"><span data-stu-id="797d8-157">Modify any views for the project entity to include your new custom field for stages.</span></span>

   ![प्रोजेक्ट निकाय पर दृश्यों को संशोधित करने का स्क्रीनशॉट](media/FAQ-Customize-BPF-8-720.png)

