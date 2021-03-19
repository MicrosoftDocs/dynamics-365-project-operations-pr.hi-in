---
title: नए परिवेश का प्रावधान
description: यह विषय एक नए परियोजना संचालन परिवेश का प्रावधान करने के बारे में जानकारी देता है।
author: sigitac
manager: Annbe
ms.date: 12/11/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 50e623d3716c9dd03ce34ec293ba57b5d966d39e
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276890"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="9a0cd-103">नए परिवेश का प्रावधान</span><span class="sxs-lookup"><span data-stu-id="9a0cd-103">Provision a new environment</span></span>

<span data-ttu-id="9a0cd-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="9a0cd-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="9a0cd-105">यह विषय संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए नए Dynamics 365 Project Operations परिवेश को प्रोविज़न करने के तरीके के बारे में जानकारी प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="9a0cd-106">LCS परियोजना में परियोजना संचालन स्वचालित प्रोविजनिंग सक्षम करें</span><span class="sxs-lookup"><span data-stu-id="9a0cd-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="9a0cd-107">अपनी LCS परियोजना के लिए परियोजना संचालन स्वचालित प्रोविजनिंग प्रवाह को सक्षम करने के लिए निम्न चरणों का उपयोग करें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="9a0cd-108">[LCS](https://lcs.dynamics.com/v2) पर जाएं और **फ़ीचर प्रबंधन पूर्वावलोकन** टाइल चुनें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="9a0cd-109">**प्रिव्यू विशेषता** सूची में, चुनिये **प्रकल्प परिचालन विशेषताएं**, और उसके बाद चुनिये **प्रिव्यू विशेषता सक्रिय** जिससे प्रकल्प परिचालन सक्रिय किया जा सके.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-109">In the **Preview feature** list, select **Project Operations Feature**, and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="9a0cd-110">यह चरण LCS परियोजना के अनुसार केवल एक बार किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="9a0cd-111">परियोजना संचालन परिवेश का प्रावधान</span><span class="sxs-lookup"><span data-stu-id="9a0cd-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="9a0cd-112">नया Dynamics 365 Finance [डेमो परिवेश](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) या [sandbox/ production environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) परिनियोजन खोलें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-112">Open a new Dynamics 365 Finance [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="9a0cd-113">**परिवेश प्रोविजनिंग** विज़ार्ड में से निकलें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="9a0cd-114">सुनिश्चित करें कि चयनित एप्लिकेशन संस्करण 10.0.13 या उससे अधिक है।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="9a0cd-115">**उन्नत सेटिंग्स** के तहत, परियोजना संचालन का प्रावधान करने के लिए, **Common Data Service** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="9a0cd-116">**हां** चुनकर **Common Data Service सेटिंग** सक्षम करें और फिर आवश्यक फ़ील्ड में जानकारी दर्ज करें:</span><span class="sxs-lookup"><span data-stu-id="9a0cd-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="9a0cd-117">नाम</span><span class="sxs-lookup"><span data-stu-id="9a0cd-117">Name</span></span>
  - <span data-ttu-id="9a0cd-118">क्षेत्र</span><span class="sxs-lookup"><span data-stu-id="9a0cd-118">Region</span></span>
  - <span data-ttu-id="9a0cd-119">भाषा</span><span class="sxs-lookup"><span data-stu-id="9a0cd-119">Language</span></span>
  - <span data-ttu-id="9a0cd-120">मुद्रा</span><span class="sxs-lookup"><span data-stu-id="9a0cd-120">Currency</span></span>
 
5. <span data-ttu-id="9a0cd-121">**Common Data Service खाका** फ़ील्ड में, **परियोजना संचालन** चुनें</span><span class="sxs-lookup"><span data-stu-id="9a0cd-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="9a0cd-122">अपने परिनियोजन के लिए परिवेश प्रकार का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="9a0cd-123">सदस्यता-आधारित परीक्षण आपको 30 दिनों के लिए CDS परिवेश परिनियोजित करने देगा।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![परिनियोजन सेटिंग्स](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="9a0cd-125">सेवा की शर्तों को स्वीकार करने के लिए **सहमत** चुनें और फिर परिनियोजन सेटिंग्स पर वापस जाने के लिए **पूर्ण** चुनें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![परिनियोजन सहमति](./media/2DeploymentConsent.png)

7. <span data-ttu-id="9a0cd-127">वैकल्पिक - परिवेश पर डेमो डेटा लागू करें.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-127">Optional - Apply demo data to the environment.</span></span> <span data-ttu-id="9a0cd-128">**उन्नत सेटिंग** पर जाएँ, **SQL डेटाबेस कॉन्फ़िगरेशन अनुकूलित करें** चुनें और **एप्लिकेशन डेटाबेस के लिए एक डेटाबेस निर्दिष्ट करें** को **डेमो** पर सेट करें.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-128">Go to **Advanced settings**, select **Customize SQL Database Configuration**, and set **Specify a dataset for Application database** to **Demo**.</span></span>

8. <span data-ttu-id="9a0cd-129">विज़ार्ड में बाकी आवश्यक फ़ील्ड को पूरा करें और परिनियोजन की पुष्टि करें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-129">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="9a0cd-130">परिवेश को प्रोविज़न करने का समय, परिवेश प्रकार के आधार पर अलग-अलग होता है.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-130">The time to provision the environment varies based on the environment type.</span></span> <span data-ttu-id="9a0cd-131">प्रोविजनिंग में छह घंटे तक लग सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-131">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="9a0cd-132">परिनियोजन सफलतापूर्वक पूरा होने के बाद, परिवेश **परिनियोजित** के रूप में दिखाएगा।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-132">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

9. <span data-ttu-id="9a0cd-133">यह पुष्टि करने के लिए कि परिवेश को सफलतापूर्वक परिनियोजित कर दिया गया है, **लॉगिन** चुनें और पुष्टि करने के लिए परिवेश पर लॉग ऑन करें.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-133">To confirm that the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![परिवेश विवरण](./media/3EnvironmentDetails.png)

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="9a0cd-135">वित्त परिवेश में अपडेट लागू करें</span><span class="sxs-lookup"><span data-stu-id="9a0cd-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="9a0cd-136">परियोजना संचालन के लिए एप्लिकेशन संस्करण **10.0.13 (10.0.569.20009)** या उच्चतर वाले वित्त परिवेश की आवश्यकता होती है।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="9a0cd-137">इस संस्करण को पाने के लिए आपको अपने वित्त परिवेश में गुणवत्ता अपडेट लागू करने पड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="9a0cd-138">LCS में, **परिवेश विवरण** पृष्ठ पर, **उपलब्ध अपडेट** अनुभाग में, **अपडेट देखें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![अपडेट देखें](./media/5ViewUpdates.png)

2. <span data-ttu-id="9a0cd-140">**बाइनरी अपडेट** पृष्ठ पर, **पैकेज सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-140">On the **Binary updates** page, select **Save package.**</span></span>

![पैकेज सहेजें](./media/6SavePackage.png)

3. <span data-ttu-id="9a0cd-142">**सभी चुनें** क्लिक करें और फिर **पैकेज सहेजें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-142">Click **Select all** and then select **Save package**.</span></span>

![अपडेट की समीक्षा करें और सहेजें](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="9a0cd-144">पैकेज का नाम और विवरण दर्ज करें, और फिर **सहेजें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="9a0cd-145">इंटरनेट कनेक्शन की गति के आधार पर, इस प्रक्रिया में कुछ समय लग सकता है।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-145">Depending on the internet connection, this process might take some time.</span></span>

![परिसंपत्ति लाइब्रेरी में पैकेज अपलोड करें](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="9a0cd-147">पैकेज सहेजे जाने के बाद **पूर्ण** चुनें और इस पैकेज को अपनी LCS परियोजना में परिसंपत्ति लाइब्रेरी में सहेजें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="9a0cd-148">पैकेज को सहेजने और मान्य करने में ~15 मिनट लग सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="9a0cd-149">अपडेट लागू करने के लिए, LCS में **परिवेश विवरण** पृष्ठ पर जाएं और **बनाए रखें** > **अपडेट लागू करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![परिवेश बनाए रखें](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="9a0cd-151">अपडेट सूची में, आपके द्वारा बनाया गया पैकेज चुनें और **लागू करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-151">In the updates list select the package you created, and select **Apply**.</span></span>

![अपडेट लागू करें](./media/10ApplyUpdates.png)

<span data-ttu-id="9a0cd-153">परिवेश की सर्विसिंग में कुछ समय लगेगा।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-153">Environment servicing will take some time.</span></span> <span data-ttu-id="9a0cd-154">इसके पूरा होने के बाद, परिवेश परिनियोजित स्थिति में लौट आएगा।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-154">After it is complete, the environment will return to a deployed state.</span></span>

![परिवेश नियोजित](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="9a0cd-156">एक ड्यूल राइट कनेक्शन स्थापित करें</span><span class="sxs-lookup"><span data-stu-id="9a0cd-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="9a0cd-157">अपनी LCS परियोजना में, **परिवेश विवरण** पृष्ठ पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="9a0cd-158">**Common Data Service परिवेश जानकारी** के तहत, **अनुप्रयोग के लिए CDS से लिंक करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="9a0cd-159">लिंक पूरा होने के बाद, फिर से **ऐप्स के लिए CDS से लिंक करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="9a0cd-160">आपको वित्त में ड्यूल राइट पर रिडायरेक्ट किया जाएगा।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-160">You will be redirected to Dual Write in Finance.</span></span>

![CDS से लिंक करें](./media/12LinktoCDS.png)

4. <span data-ttu-id="9a0cd-162">एकीकरण में मैप किए जाने वाले निकायों तक पहुंचने के लिए **समाधान लागू करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![समाधान लागू करें](./media/13ApplySolutions.png)

5. <span data-ttu-id="9a0cd-164">दोनों समाधान चुनें, **Dynamics 365 Finance and Operations डुअल लेखन निकाय मैप** और **Dynamics 365 Project Operations डुअल लेखन निकाय मैप** और उसके बाद **लागू करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![समाधान की पुष्टि करें](./media/14ConfirmSolutions.png)

<span data-ttu-id="9a0cd-166">समाधान लागू किए जाने के बाद, ड्यूल राइट निकाय परिवेश पर लागू होती हैं।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![समाधान लागू करना](./media/15ApplyingSolutions.png)

<span data-ttu-id="9a0cd-168">निकाय लागू किए जाने के बाद, सभी उपलब्ध मैपिंग परिवेश में सूचीबद्ध होती हैं।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![ड्यूल राइट मानचित्र](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="9a0cd-170">अपडेट के बाद डेटा निकायों को रिफ्रेश करें</span><span class="sxs-lookup"><span data-stu-id="9a0cd-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="9a0cd-171">वित्त में, **डेटा प्रबंधन** कार्यक्षेत्र पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-171">In Finance, go to the **Data management** workspace.</span></span>

![डेटा प्रबंधन कार्यस्थान](./media/16DataManagement.png)

2. <span data-ttu-id="9a0cd-173">**फ्रेमवर्क मापदंड** शीर्षक चुनें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-173">Select the **Framework parameters** tile.</span></span>

![फ्रेमवर्क मापदंड](./media/17FrameworkParameters.png)

3. <span data-ttu-id="9a0cd-175">**निकाय सेटिंग्स** पृष्ठ पर, **निकाय सूची** चुनें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![निकाय सूची रिफ्रेश करें](./media/18RefreshEntityList.png)

<span data-ttu-id="9a0cd-177">रिफ्रेश में लगभग 20 मिनट लग सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="9a0cd-178">पूर्ण होने पर आपको एक सूचना मिलेगी।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-178">You will receive an alert when it is complete.</span></span>

![पुष्टिकरण रिफ्रेश](./media/19RefreshConfirmation.png)

## <a name="update-security-settings-on-project-operations-on-dataverse"></a><span data-ttu-id="9a0cd-180">Dataverse पर Project Operations पर सुरक्षा सेटिंग अद्यतन करें</span><span class="sxs-lookup"><span data-stu-id="9a0cd-180">Update security settings on Project Operations on Dataverse</span></span>

1. <span data-ttu-id="9a0cd-181">अपने Dataverse परिवेश में Project Operations पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-181">Go to Project Operations on your Dataverse environment.</span></span> 
2. <span data-ttu-id="9a0cd-182">**सेटिंग** > **सुरक्षा** > **सुरक्षा भूमिकाएँ** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-182">Go to **Settings** > **Security** > **Security roles**.</span></span> 
3. <span data-ttu-id="9a0cd-183">**सुरक्षा भूमिकाएँ** पृष्ठ पर, भूमिकाओं की सूची में, **डुअल-राइट ऐप उपयोगकर्ता** चुनें और **कस्टम निकाय** टैब चुनें.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-183">On the **Security roles** page, in the list of roles, select **dual-write app user** and select the **Custom Entities** tab.</span></span>  
4. <span data-ttu-id="9a0cd-184">सत्यापित करें भूमिका के पास निम्न के लिए **पठन** और **जोड़ें** अनुमतियाँ हैं:</span><span class="sxs-lookup"><span data-stu-id="9a0cd-184">Verify that the role has **Read** and **Append To** permissions for the:</span></span>
      
      - <span data-ttu-id="9a0cd-185">**मुद्रा विनिमय दर प्रकार**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-185">**Currency Exchange Rate Type**</span></span>
      - <span data-ttu-id="9a0cd-186">**खातों का चार्ट**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-186">**Chart Of Accounts**</span></span>
      - <span data-ttu-id="9a0cd-187">**वित्त कैलेंडर**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-187">**Fiscal Calendar**</span></span>
      - <span data-ttu-id="9a0cd-188">**लेजर**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-188">**Ledger**</span></span>

5. <span data-ttu-id="9a0cd-189">सुरक्षा भूमिका अद्यतन होने के बाद, **सेटिंग** > **सुरक्षा** > **टीम** पर जाएँ और **स्थानीय व्यवसाय स्वामी** टीम दृश्य में डिफ़ॉल्ट टीम चुनें.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-189">After the security role is updated, go to **Settings** > **Security** > **Teams**, and select the default team in the **Local Business Owner** team view.</span></span>
6. <span data-ttu-id="9a0cd-190">**भूमिकाएं प्रबंधित करें** चुनें और सत्यापित करें कि इस टीम पर **डुअल-राइट ऐप उपयोगकर्ता** सुरक्षा विशेषाधिकार लागू किया गया है.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-190">Select **Manage Roles** and verify that the **dual-write app user** security privilege is applied to this team.</span></span>

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="9a0cd-191">परियोजना संचालन ड्यूल राइट मानचित्र चलाएं</span><span class="sxs-lookup"><span data-stu-id="9a0cd-191">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="9a0cd-192">अपनी LCS परियोजना में, **परिवेश विवरण** पृष्ठ पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-192">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="9a0cd-193">**Common Data Service परिवेश जानकारी** के तहत, **अनुप्रयोग के लिए CDS से लिंक करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-193">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="9a0cd-194">आपके द्वारा लिंक चुनने के बाद, आप मैपिंग में निकायों की सूची पर रिडायरेक्ट हो जाएंगे।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-194">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="9a0cd-195">निम्न तालिका में वर्णित के अनुसार मानचित्र शुरू करें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-195">Start the maps as described in the following table.</span></span> <span data-ttu-id="9a0cd-196">अनुक्रम का सूचीबद्ध के रूप में पालन करना सुनिश्चित करें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-196">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="9a0cd-197">**निकाय मानचित्र**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-197">**Entity Map**</span></span> | <span data-ttu-id="9a0cd-198">**निकाय रिफ्रेश करें**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-198">**Refresh entity**</span></span> | <span data-ttu-id="9a0cd-199">**प्रारंभिक सिंक**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-199">**Initial sync**</span></span> | <span data-ttu-id="9a0cd-200">**प्रारंभिक सिंक के लिए मास्टर**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-200">**Master for initial sync**</span></span> | <span data-ttu-id="9a0cd-201">**पूर्वापेक्षाएं चलाएं**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-201">**Run prerequisites**</span></span> | <span data-ttu-id="9a0cd-202">**पूर्वापेक्षाएं प्रारंभिक सिंक**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-202">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="9a0cd-203">**सभी कंपनियों के लिए परियोजना संसाधन भूमिकाएं (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-203">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="9a0cd-204">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-204">No</span></span> | <span data-ttu-id="9a0cd-205">हाँ</span><span class="sxs-lookup"><span data-stu-id="9a0cd-205">Yes</span></span> | <span data-ttu-id="9a0cd-206">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="9a0cd-206">Common Data Service</span></span> | <span data-ttu-id="9a0cd-207">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-207">No</span></span> | <span data-ttu-id="9a0cd-208">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-208">N\A</span></span> |
| <span data-ttu-id="9a0cd-209">**कानूनी निकाय (cdm\_companies)**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-209">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="9a0cd-210">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-210">No</span></span> | <span data-ttu-id="9a0cd-211">हाँ</span><span class="sxs-lookup"><span data-stu-id="9a0cd-211">Yes</span></span> | <span data-ttu-id="9a0cd-212">Finance and Operations ऐप</span><span class="sxs-lookup"><span data-stu-id="9a0cd-212">Finance and Operations apps</span></span> | <span data-ttu-id="9a0cd-213">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-213">No</span></span> | <span data-ttu-id="9a0cd-214">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-214">N\A</span></span> |
| <span data-ttu-id="9a0cd-215">**लेज़र (msdyn_ledgers)**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-215">**Ledger (msdyn_ledgers)**</span></span> | <span data-ttu-id="9a0cd-216">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-216">No</span></span> | <span data-ttu-id="9a0cd-217">हाँ</span><span class="sxs-lookup"><span data-stu-id="9a0cd-217">Yes</span></span> | <span data-ttu-id="9a0cd-218">Finance and Operations ऐप</span><span class="sxs-lookup"><span data-stu-id="9a0cd-218">Finance and Operations apps</span></span> | <span data-ttu-id="9a0cd-219">हाँ</span><span class="sxs-lookup"><span data-stu-id="9a0cd-219">Yes</span></span> | <span data-ttu-id="9a0cd-220">हाँ, Finance and Operations ऐप</span><span class="sxs-lookup"><span data-stu-id="9a0cd-220">Yes, Finance and Operations apps</span></span> |
| <span data-ttu-id="9a0cd-221">**परियोजना संचालन एकीकरण वास्तविक (msdyn\_actuals)**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-221">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="9a0cd-222">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-222">No</span></span> | <span data-ttu-id="9a0cd-223">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-223">No</span></span> | <span data-ttu-id="9a0cd-224">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-224">N\A</span></span> | <span data-ttu-id="9a0cd-225">हाँ</span><span class="sxs-lookup"><span data-stu-id="9a0cd-225">Yes</span></span> | <span data-ttu-id="9a0cd-226">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-226">No</span></span> |
| <span data-ttu-id="9a0cd-227">**परियोजना अनुबंध लाइन (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-227">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="9a0cd-228">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-228">No</span></span> | <span data-ttu-id="9a0cd-229">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-229">No</span></span> | <span data-ttu-id="9a0cd-230">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-230">N\A</span></span> | <span data-ttu-id="9a0cd-231">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-231">No</span></span> | <span data-ttu-id="9a0cd-232">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-232">No</span></span> |
| <span data-ttu-id="9a0cd-233">**परियोजना लेनदेन संबंधों के लिए एकीकरण निकाय (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-233">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="9a0cd-234">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-234">No</span></span> | <span data-ttu-id="9a0cd-235">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-235">No</span></span> | <span data-ttu-id="9a0cd-236">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-236">N\A</span></span> | <span data-ttu-id="9a0cd-237">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-237">No</span></span> | <span data-ttu-id="9a0cd-238">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-238">N\A</span></span> |
| <span data-ttu-id="9a0cd-239">**परियोजना संचालन एकीकरण अनुबंध लाइन माइलस्टोन (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-239">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="9a0cd-240">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-240">No</span></span> | <span data-ttu-id="9a0cd-241">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-241">No</span></span> | <span data-ttu-id="9a0cd-242">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-242">N\A</span></span> | <span data-ttu-id="9a0cd-243">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-243">No</span></span> | <span data-ttu-id="9a0cd-244">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-244">N\A</span></span> |
| <span data-ttu-id="9a0cd-245">**व्यय अनुमानों के लिए परियोजना संचालन एकीकरण इकाई (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-245">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="9a0cd-246">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-246">No</span></span> | <span data-ttu-id="9a0cd-247">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-247">No</span></span> | <span data-ttu-id="9a0cd-248">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-248">N\A</span></span> | <span data-ttu-id="9a0cd-249">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-249">No</span></span> | <span data-ttu-id="9a0cd-250">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-250">N\A</span></span> |
| <span data-ttu-id="9a0cd-251">**प्रकल्प परिचालन एकीकरण प्रकल्प खर्च श्रेणी निर्यात निकाय (msdyn\_खर्च श्रेणी)**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-251">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="9a0cd-252">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-252">No</span></span> | <span data-ttu-id="9a0cd-253">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-253">No</span></span> | <span data-ttu-id="9a0cd-254">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-254">N\A</span></span> | <span data-ttu-id="9a0cd-255">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-255">No</span></span> | <span data-ttu-id="9a0cd-256">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-256">N\A</span></span> |
| <span data-ttu-id="9a0cd-257">**परियोजना संचालन एकीकरण परियोजना व्यय निर्यात निकाय (msdyn\_expenses)**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-257">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="9a0cd-258">हाँ</span><span class="sxs-lookup"><span data-stu-id="9a0cd-258">Yes</span></span> | <span data-ttu-id="9a0cd-259">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-259">No</span></span> | <span data-ttu-id="9a0cd-260">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-260">N\A</span></span> | <span data-ttu-id="9a0cd-261">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-261">No</span></span> | <span data-ttu-id="9a0cd-262">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-262">N\A</span></span> |
| <span data-ttu-id="9a0cd-263">**घंटे के अनुमानों के लिए परियोजना संचालन एकीकरण निकाय (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="9a0cd-263">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="9a0cd-264">हाँ</span><span class="sxs-lookup"><span data-stu-id="9a0cd-264">Yes</span></span> | <span data-ttu-id="9a0cd-265">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-265">No</span></span> | <span data-ttu-id="9a0cd-266">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-266">N\A</span></span> | <span data-ttu-id="9a0cd-267">No</span><span class="sxs-lookup"><span data-stu-id="9a0cd-267">No</span></span> | <span data-ttu-id="9a0cd-268">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="9a0cd-268">N\A</span></span> |


4. <span data-ttu-id="9a0cd-269">निकाय को रिफ्रेश करने के लिए, मानचित्र नाम चुनें और उसके बाद **निकाय रिफ्रेश करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-269">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![मानचित्र रिफ्रेश करें](./media/20RefreshMapping.png)

5. <span data-ttu-id="9a0cd-271">रिफ्रेश पूरा होते ही, मैप को रन करें.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-271">After the refresh is complete, run the map.</span></span> <span data-ttu-id="9a0cd-272">इससे पहले कि आप अगला मानचित्र सक्षम करें, सत्यापित करें कि तालिका में मानचित्र **रनिंगहै** स्थिति में है।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-272">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="9a0cd-273">बड़ी संख्या में पूर्वापेक्षाओं के साथ चल रहे मानचित्र में कुछ समय लग सकता है।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-273">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="9a0cd-274">पूर्वापेक्षाओं के साथ एक मानचित्र चलाने के लिए, **संबंधित निकाय मानचित्र दिखाएं** टॉगल करें।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-274">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="9a0cd-275">यदि तालिका दर्शाती है कि **पूर्वापेक्षा प्रारंभिक सिंक** है **नहीं** है, तो इसे चलाने से पहले सत्यापित करें कि सभी पूर्वापेक्षित मानचित्रों में **प्रारंभिक सिंक** फ्लैग **बंद** है।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-275">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![मानचित्र चलाएं](./media/21RunMap.png)

6. <span data-ttu-id="9a0cd-277">पुष्टि करें कि परियोजना से संबंधित सभी मानचित्र चालू स्थिति में हैं।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-277">Validate all project related maps are in the running state.</span></span>

![सभी मानचित्र चलाए जा रहे हैं](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a><span data-ttu-id="9a0cd-279">Project Operations के लिए CDS में कॉन्फ़िगरेशन डेटा लागू करें (वैकल्पिक)</span><span class="sxs-lookup"><span data-stu-id="9a0cd-279">Apply configuration data in CDS for Project Operations (optional)</span></span>

<span data-ttu-id="9a0cd-280">यदि आपने Finance परिवेश में डेमो डेटा लागू किया है, तो CDS परिवेश पर डेमो डेटा लागू करने के लिए [Project Operations के लिए Common Data Service में कॉन्फ़िगरेशन डेटा सेट अप करें और लागू करें](resource-apply-pro-setup-config-data.md) देखें.</span><span class="sxs-lookup"><span data-stu-id="9a0cd-280">If you have applied demo data to the Finance environment, see [Set up and apply configuration data in the Common Data Service for Project Operations](resource-apply-pro-setup-config-data.md) to apply demo data to CDS environment.</span></span>


<span data-ttu-id="9a0cd-281">आपका परियोजना संचालन परिवेश अब प्रोविजन और कॉन्फ़िगर किया गया है।</span><span class="sxs-lookup"><span data-stu-id="9a0cd-281">Your Project Operations environment is now provisioned and configured.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]