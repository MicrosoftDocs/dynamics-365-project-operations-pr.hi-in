---
title: अपने वित्त परिवेश में Project Operations को अद्यतित करें
description: यह विषय आपके Dynamics 365 Finance परिवेश में Project Operations को अद्यतित करने के तरीके के बारे में जानकारी प्रदान करता है.
author: ruhercul
manager: tfehr
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 249b8dba17165da04596ec46a625131b9b4daeb5
ms.sourcegitcommit: f4fc6e3a81e8551da050e92f8fde85f8d7b52fbd
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 12/29/2020
ms.locfileid: "4816627"
---
# <a name="update-project-operations-in-your-finance-environment"></a><span data-ttu-id="2d1f1-103">अपने वित्त परिवेश में Project Operations को अद्यतित करें</span><span class="sxs-lookup"><span data-stu-id="2d1f1-103">Update Project Operations in your Finance environment</span></span>

<span data-ttu-id="2d1f1-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="2d1f1-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="2d1f1-105">यह विषय आपके Dynamics 365 Finance परिवेश में Dynamics 365 Project Operations को अद्यतित करने के तरीके के बारे में जानकारी प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-105">This topic provides information about how to update Dynamics 365 Project Operations in your Dynamics 365 Finance environment.</span></span> <span data-ttu-id="2d1f1-106">Project Operations को Update 5 (UR5) पर अद्यतित करने के लिए तीन प्रक्रियाएँ आवश्यक हैं:</span><span class="sxs-lookup"><span data-stu-id="2d1f1-106">There are three procedures that are required to update Project Operations to Update 5 (UR5):</span></span>

- [<span data-ttu-id="2d1f1-107">अपनी पूर्वावलोकन परियोजना में पैकेज आयात करें</span><span class="sxs-lookup"><span data-stu-id="2d1f1-107">Import the package into your preview project</span></span>](#import)
- [<span data-ttu-id="2d1f1-108"> अद्यतन लागू करें</span><span class="sxs-lookup"><span data-stu-id="2d1f1-108">Apply the update</span></span>](#apply)
- [<span data-ttu-id="2d1f1-109">अपना Dataverse परिवेश अद्यतित करें</span><span class="sxs-lookup"><span data-stu-id="2d1f1-109">Update your Dataverse environment</span></span>](#update)

## <a name="import-the-package-into-your-lcs-project"></a><a name="import"></a><span data-ttu-id="2d1f1-110">अपने पैकेज को LCS परियोजना में आयात करें</span><span class="sxs-lookup"><span data-stu-id="2d1f1-110">Import the package into your LCS project</span></span>

1. <span data-ttu-id="2d1f1-111">[Lifecycle Services (LCS)](https://lcs.dynamics.com/) में परियोजना स्वामी या परिवेश प्रबंधक के रूप में साइन इन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-111">Sign in to [Lifecycle Services (LCS)](https://lcs.dynamics.com/) as a Project Owner or Environment manager.</span></span>
2. <span data-ttu-id="2d1f1-112">परियोजनाओं की सूची से, अपनी LCS परियोजना का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-112">From the list of projects, select your LCS project.</span></span>
3. <span data-ttu-id="2d1f1-113">**परियोजना** पृष्ठ पर, **परिवेश** समूह में, उस परिवेश को खोलें जिसे आप अद्यतित करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-113">On the **Project** page, in the **Environments** group, open the environment that you want to update.</span></span>
4. <span data-ttu-id="2d1f1-114">सत्यापित करें कि परिवेश चल रहा है.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-114">Verify that the environment is running.</span></span> <span data-ttu-id="2d1f1-115">यदि यह शुरू नहीं हुआ है, तो परिवेश को प्रारंभ करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-115">If it isn't started, start the environment.</span></span>
5. <span data-ttu-id="2d1f1-116">**नया रिलीज़** सेक्शन में, **उपलब्ध अद्यतन** के तहत, 10.0.15 के लिए **अद्यतन देखें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-116">In the **New release** section under **Available updates**, select **View update** for 10.0.15.</span></span>

![अद्यतन देखें बटन](media/view-update.png)

6. <span data-ttu-id="2d1f1-118">**बाइनरी अद्यतन** पृष्ठ पर, **पैकेज सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-118">On the **Binary updates** page, select **Save package**.</span></span>
7. <span data-ttu-id="2d1f1-119">**अद्यतनों की समीक्षा करें और सहेजें** पृष्ठ पर, **पैकेज सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-119">On the **Review and save updates** page, select **Save package**.</span></span>
8. <span data-ttu-id="2d1f1-120">**परिसंपत्ति लाइब्रेरी में पैकेज सहेजें** फलक जो खुलता है, उस पर पैकेज नाम दर्ज करें और फिर **पैकेज सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-120">On the **Save package to asset library** pane that opens, enter the package name and then select **Save package**.</span></span>
9. <span data-ttu-id="2d1f1-121">LCS द्वारा पैकेज सहेजना समाप्त करने पर, **पूरा हुआ** बटन सक्षम हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-121">When LCS has finished saving the package, the **Done** button is enabled.</span></span> <span data-ttu-id="2d1f1-122">**पूर्ण** चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-122">Select **Done**.</span></span> <span data-ttu-id="2d1f1-123">LCS पैकेज को सत्यापित करेगा.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-123">LCS will verify the package.</span></span> <span data-ttu-id="2d1f1-124">सत्यापन में कुछ मिनट या एक घंटा तक लग सकता है.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-124">Verification can take a few minutes or up to one hour.</span></span>


## <a name="apply-the-package-update"></a><a name="apply"></a><span data-ttu-id="2d1f1-125">पैकेज अद्यतन लागू करें</span><span class="sxs-lookup"><span data-stu-id="2d1f1-125">Apply the package update</span></span>

1. <span data-ttu-id="2d1f1-126">LCS में, **परिवेश विवरण** पृष्ठ पर, **रखरखाव करें** > **अद्यतन लागू करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-126">In LCS, on the **Environment details** page, select **Maintain** > **Apply Updates**.</span></span>
2. <span data-ttu-id="2d1f1-127">सूची से, उस पैकेज का चयन करें जिसे आपने पहले सहेजा था, और फिर **लागू करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-127">From the list, select the package that you saved earlier, and then select **Apply**.</span></span>
3. <span data-ttu-id="2d1f1-128">आप पैकेज को परिनियोजित करना चाहते हैं, यह पुष्टि करने के लिए **हाँ** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-128">Select **Yes** to confirm that you want to deploy the package.</span></span>

![पैकेज परिनियोजन की पुष्टि करें संवाद बॉक्स](media/confirm-package-deployment.png)

4. <span data-ttu-id="2d1f1-130">आप ऐप्लिकेशन को अद्यतित करना चाहते हैं, यह पुष्टि करने के लिए **हाँ** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-130">Select **Yes** to confirm that you want to update the application.</span></span>

![ऐप्लिकेशन अद्यतन की पुष्टि करें संवाद बॉक्स](media/confirm-application-update.png)

<span data-ttu-id="2d1f1-132">परिनियोजन और ऐप्लिकेशन अद्यतन शुरू हो जाएगा.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-132">The deployment and application update will start.</span></span> 

<span data-ttu-id="2d1f1-133">**परिवेश विवरण** पृष्ठ पर, ऊपरी-दाएं कोने में, परिवेश की स्थिति **सेवा** पर अद्यतित हो जाएगी.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-133">On the **Environment details** page, in the top-right corner, the environment status will update to **Servicing**.</span></span> <span data-ttu-id="2d1f1-134">लगभग दो घंटे में, अद्यतन पूरा हो जाएगा.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-134">In approximately two hours, the update will be complete.</span></span> <span data-ttu-id="2d1f1-135">ऐप्लिकेशन रिलीज़ जानकारी **Microsoft Dynamics 365 for Finance and Operations 10.0.15)** पर अद्यतित हो जाएगी और परिवेश की स्थिति **परिनियोजित किया गया** पर अद्यतित हो जाएगी.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-135">The application release information will update to **Microsoft Dynamics 365 for Finance and Operations 10.0.15)** and the environment status will update to **Deployed**.</span></span>


## <a name="update-your-dataverse-environment"></a><a name="update"></a><span data-ttu-id="2d1f1-136">अपना Dataverse परिवेश अद्यतित करें</span><span class="sxs-lookup"><span data-stu-id="2d1f1-136">Update your Dataverse environment</span></span>

1. <span data-ttu-id="2d1f1-137">[Power Platform व्यवस्थापन केंद्र](https://admin.powerplatform.com/) में साइन इन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-137">Sign in to the [Power Platform admin center](https://admin.powerplatform.com/).</span></span>
2. <span data-ttu-id="2d1f1-138">सूची में, उस परिवेश को ढूंढें और खोलें जो आपने Project Operations को स्थापित करने के लिए उपयोग किया था.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-138">In the list, find and open the environment that you used to install Project Operations.</span></span>
3. <span data-ttu-id="2d1f1-139">**परिवेश** पृष्ठ पर, **संसाधन** > **Dynamics 365 ऐप्स** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-139">On the **Environments** page, select **Resource** > **Dynamics 365 apps**.</span></span>
4. <span data-ttu-id="2d1f1-140">सूची में, **Microsoft Dynamics 365 Project Operations** का पता लगाएं, और **स्थिति** स्तंभ में, **अद्यतन उपलब्ध है** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-140">In the list, locate **Microsoft Dynamics 365 Project Operations**, and in the **Status** column, select **Update Available**.</span></span>
5. <span data-ttu-id="2d1f1-141">**मैं सेवा की शर्तों से सहमत हूं** चेक बॉक्स चुनें, और फिर **अद्यतित करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-141">Select the **I agree to the terms of service** check box, and then select **Update**.</span></span> <span data-ttu-id="2d1f1-142">समाधान का नवीनतम संस्करण स्थापित किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-142">The latest version of the solution will be installed.</span></span>

<span data-ttu-id="2d1f1-143">स्थापना पूर्ण होने के बाद, आपके पास 4.5.0.134 संस्करण स्थापित होगा.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-143">After the installation is complete, you'll have version 4.5.0.134 installed.</span></span>

## <a name="configure-new-features"></a><span data-ttu-id="2d1f1-144">नई सुविधाएं कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="2d1f1-144">Configure new features</span></span>

### <a name="enable-dual-write-mapping"></a><span data-ttu-id="2d1f1-145">डुअल राइट मैपिंग को सक्षम करें</span><span class="sxs-lookup"><span data-stu-id="2d1f1-145">Enable dual-write mapping</span></span>

<span data-ttu-id="2d1f1-146">वित्त और Dataverse परिवेशों पर अद्यतन पूरा करने के बाद, आप आवश्यक डुअल राइट मैपिंग को सक्षम कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-146">After you complete the update on the Finance and Dataverse environments, you can enable the required dual-write mappings.</span></span> <span data-ttu-id="2d1f1-147">आप डुअल राइट मैपिंग को सक्षम करने के लिए निम्नलिखित प्रक्रियाओं को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-147">Complete the following procedures to enable dual-write mappings.</span></span>

- [<span data-ttu-id="2d1f1-148">सुरक्षा सेटिंग्स को Customer Engagement परिवेश पर अद्यतित करें</span><span class="sxs-lookup"><span data-stu-id="2d1f1-148">Update security settings on Customer Engagement environment</span></span>](#security)
- [<span data-ttu-id="2d1f1-149">डेटा इकाइयों को रीफ़्रेश करें</span><span class="sxs-lookup"><span data-stu-id="2d1f1-149">Refresh data entities</span></span>](#refresh)
- [<span data-ttu-id="2d1f1-150">अद्यतित करें और डुअल-राइट मैपिंग चलाएं</span><span class="sxs-lookup"><span data-stu-id="2d1f1-150">Update and run the dual-write mappings</span></span>](#run)

### <a name="update-security-settings-on-the-dataverse-environment"></a><a name="security"></a><span data-ttu-id="2d1f1-151">Dataverse परिवेश पर सुरक्षा सेटिंग्स को अद्यतित करें</span><span class="sxs-lookup"><span data-stu-id="2d1f1-151">Update security settings on the Dataverse environment</span></span>

<span data-ttu-id="2d1f1-152">निकायों के लिए सुरक्षा विशेषाधिकारों के लिए निम्न अद्यतन, UR5 में अद्यतन के भाग के रूप में आवश्यक हैं.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-152">The following updates to the security privileges for entities are required as part of the update to UR5.</span></span>

1. <span data-ttu-id="2d1f1-153">अपने Dataverse परिवेश में, **सेटिंग्स** में जाएं और **सिस्टम** समूह में, **सुरक्षा** चुनें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-153">In your Dataverse environment, go to **Settings**, and in the **System** group, select **Security**.</span></span>

![Dataverse परिवेश सेटिंग्स](media/Picture21.png)

2. <span data-ttu-id="2d1f1-155">**सुरक्षा भूमिकाएँ** चुनें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-155">Select **Security Roles**.</span></span>
3. <span data-ttu-id="2d1f1-156">भूमिकाओं की सूची से, **डुअल-राइट ऐप उपयोगकर्ता** चुनें और **कस्टम निकाय** टैब का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-156">From the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span> 
4. <span data-ttu-id="2d1f1-157">सत्यापित करें कि भूमिका में निम्न के लिए **पढ़ें** तथा**इसमें जोड़ें** अनुमतियां हैं:</span><span class="sxs-lookup"><span data-stu-id="2d1f1-157">Verify that the role has **Read** and **Append To** permissions for:</span></span>

      - <span data-ttu-id="2d1f1-158">**मुद्रा विनिमय दर प्रकार**</span><span class="sxs-lookup"><span data-stu-id="2d1f1-158">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="2d1f1-159">**खातों का चार्ट**</span><span class="sxs-lookup"><span data-stu-id="2d1f1-159">**Chart Of Accounts**</span></span> 
      - <span data-ttu-id="2d1f1-160">**वित्त कैलेंडर**</span><span class="sxs-lookup"><span data-stu-id="2d1f1-160">**Fiscal Calendar**</span></span> 
      - <span data-ttu-id="2d1f1-161">**लेजर**</span><span class="sxs-lookup"><span data-stu-id="2d1f1-161">**Ledger**</span></span>

5. <span data-ttu-id="2d1f1-162">सुरक्षा भूमिका अद्यतित करने के बाद, **सेटिंग्स** > **सुरक्षा** > **टीम** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-162">After the security role is updated, go to **Settings** > **Security** > **Teams**.</span></span> <span data-ttu-id="2d1f1-163">सत्यापित करें कि **डुअल-राइट ऐप उपयोगकर्ता** भूमिका को टीम के लिए लागू किया गया है.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-163">Verify that the **dual-write app user** role has been applied to the team.</span></span> 

### <a name="refresh-data-entities-from-the-update"></a><a name="refresh"></a><span data-ttu-id="2d1f1-164">अद्यतन से डेटा निकायों को रीफ़्रेश करें</span><span class="sxs-lookup"><span data-stu-id="2d1f1-164">Refresh data entities from the update</span></span>

1. <span data-ttu-id="2d1f1-165">आपके वित्त परिवेश में, **डेटा प्रबंधन** कार्यस्थान खोलें, और फिर **फ़्रेमवर्क मापदंड** पृष्ठ को खोलें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-165">In your Finance environment, open the **Data management** workspace, and then open the **Framework parameters** page.</span></span>
2. <span data-ttu-id="2d1f1-166">**निकाय सेटिंग्स** टैब पर, **निकाय सूची को रीफ़्रेश करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-166">On the **Entity settings** tab, select **Refresh entity list**.</span></span>
3. <span data-ttu-id="2d1f1-167">निकाय रीफ़्रेश होने की पुष्टि करने के लिए **बंद करे** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-167">Select **Close** to confirm the entity refresh.</span></span>

 > [!NOTE]
 > <span data-ttu-id="2d1f1-168">इस प्रक्रिया को पूरा होने में लगभग 20 मिनट का समय लग सकता है.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-168">This process will take approximately 20 minutes to complete.</span></span> <span data-ttu-id="2d1f1-169">रीफ़्रेश पूरा होने पर आपको सूचित किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-169">You will be notified when the refresh is complete.</span></span>

### <a name="update-dual-write-mappings"></a><a name="run"></a><span data-ttu-id="2d1f1-170">डुअल राइट मैपिंग को अद्यतित करें</span><span class="sxs-lookup"><span data-stu-id="2d1f1-170">Update dual-write mappings</span></span>

1. <span data-ttu-id="2d1f1-171">**डेटा प्रबंधन** कार्यस्थान में, **डुअल राइट** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-171">In the **Data management** workspace, select **Dual-write**.</span></span>
2. <span data-ttu-id="2d1f1-172">**समाधान लागू करें** का चयन करें, सूची में दोनों समाधान का चयन करें, और उसके बाद **लागू करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-172">Select **Apply solutions**, select both solutions in the list, and then select **Apply**.</span></span>
3. <span data-ttu-id="2d1f1-173">**डुअल राइट** पृष्ठ पर, निम्न तालिका मैप का चयन करें, और फिर **बंद करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-173">On the **Dual-write** page, select the following table maps, and then select **Stop**.</span></span>

    - <span data-ttu-id="2d1f1-174">**Project Operations एकीकरण वास्तविक (msdyn_actuals)**</span><span class="sxs-lookup"><span data-stu-id="2d1f1-174">**Project Operations integration actuals (msdyn_actuals)**</span></span>
    - <span data-ttu-id="2d1f1-175">**Project Operations एकीकरण परियोजना व्यय श्रेणियां (msdyn_expensecategories)**</span><span class="sxs-lookup"><span data-stu-id="2d1f1-175">**Project Operations integration project expense categories (msdyn_expensecategories)**</span></span>
    - <span data-ttu-id="2d1f1-176">**Project Operations एकीकरण वास्तविक परियोजना व्यय निर्यात श्रेणियां (msdyn_expenses)**</span><span class="sxs-lookup"><span data-stu-id="2d1f1-176">**Project Operations integration actuals project expenses export entity (msdyn_expenses)**</span></span>

4. <span data-ttu-id="2d1f1-177">**तालिका मैप संस्करण** पृष्ठ पर, मैप का एक नया संस्करण सभी तीन निकायों पर लागू करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-177">On the **Table map version** page, apply a new version of the map to each of the three entities.</span></span>
5. <span data-ttu-id="2d1f1-178">**डुअल राइट** पृष्ठ पर, मैप्स को पुनः आरंभ करने के लिए चलाएं का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-178">On the **Dual-write** page, select run to restart the maps.</span></span>
6. <span data-ttu-id="2d1f1-179">मैप्स की सूची से, सभी पूर्वावश्यकताओं वाले **लेजर (msdyn_ledgers)** मैप का चयन करें और **प्रारंभिक सिंक** चेक बॉक्स का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-179">From the list of maps, select the **Ledger (msdyn_ledgers)** map with all prerequisites and select the **Initial sync** check box.</span></span> 
7. <span data-ttu-id="2d1f1-180">**प्रारंभिक सिंक के लिए मास्टर** फ़ील्ड में, **Finance and Operations ऐप्स** का चयन करें और फिर **चलाएं** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="2d1f1-180">In the **Master for initial sync** field, select **Finance and Operations apps** and then select **Run**.</span></span>
 
 ![लेजर मैप सिंक्रोनाइज़ेशन](media/DW6.png)
 
