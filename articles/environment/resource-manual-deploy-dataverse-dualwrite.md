---
title: Project Operations Dataverse अनुप्रयोग को डुअल-राइट समर्थन के साथ मैन्युअल रूप से परिनियोजित करना
description: यह विषय बताता है कि Project Operations Dataverse अनुप्रयोग को मैन्युअल रूप से कैसे परिनियोजित किया जाए, ताकि यह डुअल-राइट का समर्थन करे.
author: stsporen
ms.date: 06/18/2021
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 2ad147da542fc9e7a2705da7a834d1a6512907e5
ms.sourcegitcommit: 205a94ab4168de25b102f31d00a691c8205ba63e
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/18/2021
ms.locfileid: "6274010"
---
# <a name="manually-deploy-the-project-operations-dataverse-app-with-dual-write-support"></a><span data-ttu-id="c6c06-103">Project Operations Dataverse अनुप्रयोग को डुअल-राइट समर्थन के साथ मैन्युअल रूप से परिनियोजित करना</span><span class="sxs-lookup"><span data-stu-id="c6c06-103">Manually deploy the Project Operations Dataverse app with dual-write support</span></span>

<span data-ttu-id="c6c06-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations_</span><span class="sxs-lookup"><span data-stu-id="c6c06-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="c6c06-105">यह विषय बताता है कि Microsoft Dataverse में Microsoft Dynamics 365 Project Operations को मैन्युअल रूप से कैसे परिनियोजित किया जाए, ताकि यह डुअल-राइट का समर्थन करे.</span><span class="sxs-lookup"><span data-stu-id="c6c06-105">This topic explains how to manually deploy Microsoft Dynamics 365 Project Operations in Microsoft Dataverse so that it supports dual-write.</span></span> <span data-ttu-id="c6c06-106">Project Operations परिवेश के कॉन्फ़िगरेशन का पता लगाता है और यदि पूर्वापेक्षाएँ पूरी होती हैं, तो डुअल-राइट के लिए अतिरिक्त समर्थन जोड़ता है.</span><span class="sxs-lookup"><span data-stu-id="c6c06-106">Project Operations detects the environment's configuration and adds additional support for dual-write if the prerequisites are met.</span></span>

<span data-ttu-id="c6c06-107">Microsoft Dynamics Lifecycle Services (LCS) के माध्यम से परिनियोजन के दौरान, यदि आपने इस विषय में दिए गए निर्देशों का पालन किया है, तो आप Microsoft Power Platform एकीकरण (जिसे पहले Common Data Service परिवेश के रूप में जाना जाता था) के परिनियोजन को छोड़ सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="c6c06-107">During deployment through Microsoft Dynamics Lifecycle Services (LCS), if you've followed the instructions in this topic, you can skip the deployment of the Microsoft Power Platform integration (previously known as the Common Data Service environment).</span></span>

<span data-ttu-id="c6c06-108">Dataverse में Project Operations परिनियोजित करने की प्रक्रिया ताकि यह डुअल-राइट का समर्थन करता है, इसके चार मुख्य चरण हैं:</span><span class="sxs-lookup"><span data-stu-id="c6c06-108">The process of deploying Project Operations in Dataverse so that it supports dual-write has four main steps:</span></span>

1. <span data-ttu-id="c6c06-109">[Dataverse मेंनया परिवेश बनाएं, जो डुअल-राइट का समर्थन करता है](#create).</span><span class="sxs-lookup"><span data-stu-id="c6c06-109">[Create a new environment in Dataverse that supports dual-write](#create).</span></span>
2. <span data-ttu-id="c6c06-110">[परिवेश में डुअल-राइट पूर्वापेक्षाएँ जोड़ें](#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="c6c06-110">[Add dual-write prerequisites to the environment](#prerequisites).</span></span>
3. <span data-ttu-id="c6c06-111">[Project Operations Dataverse अनुप्रयोग जोड़ें](#dataverse).</span><span class="sxs-lookup"><span data-stu-id="c6c06-111">[Add the Project Operations Dataverse app](#dataverse).</span></span>
4. <span data-ttu-id="c6c06-112">[अपने परिवेश लिंक करें](#link).</span><span class="sxs-lookup"><span data-stu-id="c6c06-112">[Link your environments](#link).</span></span>

## <a name="create-a-new-environment-in-dataverse-that-supports-dual-write"></a><a name="create"></a><span data-ttu-id="c6c06-113">Dataverse में नया परिवेश बनाएं, जो डुअल-राइट का समर्थन करता है</span><span class="sxs-lookup"><span data-stu-id="c6c06-113">Create a new environment in Dataverse that supports dual-write</span></span>

<span data-ttu-id="c6c06-114">इस प्रक्रिया को पूरा करने के लिए, आपको एक व्यवस्थापक के रूप में लॉग इन करना होगा.</span><span class="sxs-lookup"><span data-stu-id="c6c06-114">To complete this procedure, you must sign in as an administrator.</span></span>

1. <span data-ttu-id="c6c06-115">[Power Platform व्यवस्थापक केंद्र](https://admin.powerplatform.com) खोलें और एक व्यवस्थापक के रूप में लॉग इन करें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-115">Open the [Power Platform admin center](https://admin.powerplatform.com), and sign in as an administrator.</span></span>
2. <span data-ttu-id="c6c06-116">नया परिवेश बनाएं और उसे नाम दें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-116">Create a new environment, and name it.</span></span>
3. <span data-ttu-id="c6c06-117">परिवेश प्रकार चुनें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-117">Select the environment type.</span></span> <span data-ttu-id="c6c06-118">यदि आपने परीक्षण ऑफ़र के लिए साइन अप किया है, तो **ट्रायल (सदस्यता-आधारित)** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-118">If you signed up for the trial offer, select **Trial (subscription-based)**.</span></span>
4. <span data-ttu-id="c6c06-119">परिनियोजन क्षेत्र की पुष्टि करें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-119">Confirm the deployment region.</span></span>
5. <span data-ttu-id="c6c06-120">**इस परिवेश के लिए डेटाबेस बनाएँ** विकल्प सक्षम करें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-120">Enable the **Create a database for this environment** option.</span></span> 
6. <span data-ttu-id="c6c06-121">भाषा की पुष्टि करें और फिर पुष्टि करें कि मुद्रा आपके Finance and Operations अनुप्रयोग के लिए मुद्रा से मेल खाती है.</span><span class="sxs-lookup"><span data-stu-id="c6c06-121">Confirm the language, and then confirm that the currency matches the currency for your Finance and Operations apps.</span></span>
7. <span data-ttu-id="c6c06-122">**Dynamics 365 अनुप्रयोग** विकल्प सक्षम करें और पुष्टि करें कि **इन अनुप्रयोग को स्वचालित रूप से परिनियोजित करें** फ़ील्ड **कोई नहीं** पर सेट है.</span><span class="sxs-lookup"><span data-stu-id="c6c06-122">Enable the **Dynamics 365 apps** option, and confirm that the **Automatically deploy these apps** field is set to **None**.</span></span>
8. <span data-ttu-id="c6c06-123">यदि सुरक्षा समूह की आवश्यकता है, तो सुरक्षा समूह जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-123">Add a security group, if a security group is required.</span></span>
9. <span data-ttu-id="c6c06-124">परिवेश बनाने के लिए **सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-124">Select **Save** to create the environment.</span></span>
10. <span data-ttu-id="c6c06-125">परिनियोजन पूरा होने और परिवेश के **तैयार** स्थिति तक पहुंच जाने तक प्रतीक्षा करें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-125">Wait until the deployment is completed and the environment reaches the **Ready** state.</span></span>

## <a name="add-dual-write-prerequisites-to-the-environment"></a><a name="prerequisites"></a><span data-ttu-id="c6c06-126">परिवेश में डुअल-राइट पूर्वापेक्षाएँ जोड़ें</span><span class="sxs-lookup"><span data-stu-id="c6c06-126">Add dual-write prerequisites to the environment</span></span>

<span data-ttu-id="c6c06-127">डुअल-राइट समर्थन में अतिरिक्त फ़ील्ड शामिल हैं जो प्रमुख निकायों में जोड़े जाते हैं, जैसे कि **कंपनी** निकाय.</span><span class="sxs-lookup"><span data-stu-id="c6c06-127">Dual-write support includes additional fields that are added to key entities, such as the **Company** entity.</span></span> <span data-ttu-id="c6c06-128">यदि आप किसी मौजूदा परिवेश में दोहरा-लेखन समर्थन जोड़ रहे हैं, तो आपको समर्थन को सक्षम करने के लिए डेटा को अद्यतित करना पड़ सकता है.</span><span class="sxs-lookup"><span data-stu-id="c6c06-128">If you're adding dual-write support to an existing environment, you might have to update the data to enable the support.</span></span> <span data-ttu-id="c6c06-129">डेटा को बूटस्ट्रैप करने के तरीके के बारे में जानकारी के लिए, [बूटस्ट्रैप कंपनी डेटा](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data) देखें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-129">For information about how to bootstrap the data, see [Bootstrap company data](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/bootstrap-company-data).</span></span> <span data-ttu-id="c6c06-130">डुअल-राइट के बारे में अधिक जानकारी के लिए, [डुअल-राइट सिस्टम आवश्यकताएँ](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req) देखें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-130">For more information about dual-write, see [Dual-write system requirements](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-system-req).</span></span>

<span data-ttu-id="c6c06-131">अपने परिवेश में डुअल-राइट पूर्वापेक्षाएँ जोड़ने के लिए यह प्रक्रिया पूरी करें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-131">Complete this procedure to add the dual-write prerequisites to your environment.</span></span>

1. <span data-ttu-id="c6c06-132">आपके द्वारा अभी-अभी बनाया गया परिवेश खोलें, और फिर **संसाधन** \> **Dynamics 365 अनुप्रयोग** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="c6c06-132">Open the environment that you just created, and then go to **Resource** \> **Dynamics 365 apps**.</span></span>
2. <span data-ttu-id="c6c06-133">अनुप्रयोग सूची में **डुअल-राइट कोर समाधान** चुनें और उसे इंस्टॉल करें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-133">Select **Dual-write core solution** in the app list, and install it.</span></span>
3. <span data-ttu-id="c6c06-134">इंस्टॉलेशन पूर्ण होने तक प्रतीक्षा करें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-134">Wait until the installation is completed.</span></span> <span data-ttu-id="c6c06-135">फिर अनुप्रयोग सूची में **डुअल-राइट अनुप्रयोग ऑर्केस्ट्रेशन समाधान** चुनें और उसे इंस्टॉल करें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-135">Then select **Dual-write application orchestration solution** in the app list, and install it.</span></span>

## <a name="add-the-project-operations-dataverse-app"></a><a name="dataverse"></a><span data-ttu-id="c6c06-136">Project Operations Dataverse अनुप्रयोग जोड़ें</span><span class="sxs-lookup"><span data-stu-id="c6c06-136">Add the Project Operations Dataverse app</span></span>

<span data-ttu-id="c6c06-137">आप इस प्रक्रिया को तभी पूरा कर सकते हैं, जब आपने Project Operations इंस्टॉल करने से पहले पिछली प्रक्रियाओं को पूरा किया हो.</span><span class="sxs-lookup"><span data-stu-id="c6c06-137">You can complete this procedure only if you completed the previous procedures before you installed Project Operations.</span></span> <span data-ttu-id="c6c06-138">इंस्टॉल करने के दौरान, सिस्टम परिवेश कॉन्फ़िगरेशन का विश्लेषण करता है और यदि आवश्यक हो तो डुअल-राइट के लिए समर्थन जोड़ता है.</span><span class="sxs-lookup"><span data-stu-id="c6c06-138">During installation, the system analyzes the environment configuration and adds support for dual-write if it's required.</span></span>

1. <span data-ttu-id="c6c06-139">आपके द्वारा पहले बनाया गया परिवेश खोलें और फिर **संसाधन** \> **Dynamics 365 अनुप्रयोग** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="c6c06-139">Open the environment that you created earlier, and then go to **Resource** \> **Dynamics 365 apps**.</span></span>
2. <span data-ttu-id="c6c06-140">अनुप्रयोग सूची में **Microsoft Dynamics 365 Project Operations** चुनें और उसे इंस्टॉल करें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-140">Select **Microsoft Dynamics 365 Project Operations** in the app list, and install it.</span></span>

## <a name="link-your-environments"></a><a name="link"></a><span data-ttu-id="c6c06-141">अपने परिवेश लिंक करें</span><span class="sxs-lookup"><span data-stu-id="c6c06-141">Link your environments</span></span>

<span data-ttu-id="c6c06-142">Dataverse परिवेश परिनियोजित होने के बाद, आप अपने Finance and Operations अनुप्रयोग में लिंक सेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="c6c06-142">After the Dataverse environment is deployed, you can set up the link in your Finance and Operations apps.</span></span> <span data-ttu-id="c6c06-143">[अपने परिवेश को जोड़ने के लिए डुअल-राइट विज़ार्ड का उपयोग करें](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment) में चरणों का पालन करें.</span><span class="sxs-lookup"><span data-stu-id="c6c06-143">Follow the steps in [Use the dual-write wizard to link your environments](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/link-your-environment).</span></span>
