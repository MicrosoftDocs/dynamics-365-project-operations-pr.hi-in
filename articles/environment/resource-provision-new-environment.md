---
title: नए परिवेश का प्रावधान
description: यह विषय एक नए परियोजना संचालन परिवेश का प्रावधान करने के बारे में जानकारी देता है।
author: sigitac
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 044a942a068b33318b98041cc94944d90c1d63c3
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121175"
---
# <a name="provision-a-new-environment"></a><span data-ttu-id="af30d-103">नए परिवेश का प्रावधान</span><span class="sxs-lookup"><span data-stu-id="af30d-103">Provision a new environment</span></span>

<span data-ttu-id="af30d-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="af30d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="af30d-105">यह विषय संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए नए Dynamics 365 परियोजना संचालन परिवेश का प्रावधान करने के बारे में जानकारी देता है।</span><span class="sxs-lookup"><span data-stu-id="af30d-105">This topic provides information about how to provision a new Dynamics 365 Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="enable-project-operations-automated-provisioning-in-an-lcs-project"></a><span data-ttu-id="af30d-106">LCS परियोजना में परियोजना संचालन स्वचालित प्रोविजनिंग सक्षम करें</span><span class="sxs-lookup"><span data-stu-id="af30d-106">Enable Project Operations automated provisioning in an LCS project</span></span>

<span data-ttu-id="af30d-107">अपनी LCS परियोजना के लिए परियोजना संचालन स्वचालित प्रोविजनिंग प्रवाह को सक्षम करने के लिए निम्न चरणों का उपयोग करें।</span><span class="sxs-lookup"><span data-stu-id="af30d-107">Use following steps to enable the Project Operations automated provisioning flow for your LCS project.</span></span>

1. <span data-ttu-id="af30d-108">[LCS](https://lcs.dynamics.com/v2) पर जाएं और **फ़ीचर प्रबंधन पूर्वावलोकन** टाइल चुनें।</span><span class="sxs-lookup"><span data-stu-id="af30d-108">Go to [LCS](https://lcs.dynamics.com/v2) and select the **Preview Feature management** tile.</span></span>
2. <span data-ttu-id="af30d-109">**प्रिव्यू विशेषता** सूची में, चुनिये **प्रकल्प परिचालन विशेषताएं**, और उसके बाद चुनिये **प्रिव्यू विशेषता सक्रिय** जिससे प्रकल्प परिचालन सक्रिय किया जा सके.</span><span class="sxs-lookup"><span data-stu-id="af30d-109">In the **Preview feature** list, select **Project Operations Feature**, and then select **Preview feature enabled** to enable Project Operations.</span></span>

> [!NOTE]
> <span data-ttu-id="af30d-110">यह चरण LCS परियोजना के अनुसार केवल एक बार किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="af30d-110">This step is performed only one time per LCS project.</span></span>

## <a name="provision-a-project-operations-environment"></a><span data-ttu-id="af30d-111">परियोजना संचालन परिवेश का प्रावधान</span><span class="sxs-lookup"><span data-stu-id="af30d-111">Provision a Project Operations environment</span></span>

1. <span data-ttu-id="af30d-112">नया Dynamics 365 Finance [डेमो परिवेश](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) या [sandbox/ production environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) परिनियोजन खोलें।</span><span class="sxs-lookup"><span data-stu-id="af30d-112">Open a new Dynamics 365 Finance [demo environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) or [sandbox/ production environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deployenvironment-newinfrastructure) deployment.</span></span> 
2. <span data-ttu-id="af30d-113">**परिवेश प्रोविजनिंग** विज़ार्ड में से निकलें।</span><span class="sxs-lookup"><span data-stu-id="af30d-113">Walk through the **Environment provisioning** wizard.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="af30d-114">सुनिश्चित करें कि चयनित एप्लिकेशन संस्करण 10.0.13 या उससे अधिक है।</span><span class="sxs-lookup"><span data-stu-id="af30d-114">Make sure selected application version is 10.0.13 or higher.</span></span>

3. <span data-ttu-id="af30d-115">**उन्नत सेटिंग्स** के तहत, परियोजना संचालन का प्रावधान करने के लिए, **Common Data Service** चुनें.</span><span class="sxs-lookup"><span data-stu-id="af30d-115">To provision Project Operations, under **Advance settings**, select **Common Data Service**.</span></span> 
4. <span data-ttu-id="af30d-116">**हां** चुनकर **Common Data Service सेटिंग** सक्षम करें और फिर आवश्यक फ़ील्ड में जानकारी दर्ज करें:</span><span class="sxs-lookup"><span data-stu-id="af30d-116">Enable the **Common Data Service Setting** by selecting **Yes** and then enter information in the required fields:</span></span>

  - <span data-ttu-id="af30d-117">नाम</span><span class="sxs-lookup"><span data-stu-id="af30d-117">Name</span></span>
  - <span data-ttu-id="af30d-118">क्षेत्र</span><span class="sxs-lookup"><span data-stu-id="af30d-118">Region</span></span>
  - <span data-ttu-id="af30d-119">भाषा</span><span class="sxs-lookup"><span data-stu-id="af30d-119">Language</span></span>
  - <span data-ttu-id="af30d-120">मुद्रा</span><span class="sxs-lookup"><span data-stu-id="af30d-120">Currency</span></span>
 
5. <span data-ttu-id="af30d-121">**Common Data Service खाका** फ़ील्ड में, **परियोजना संचालन** चुनें</span><span class="sxs-lookup"><span data-stu-id="af30d-121">In the **Common Data Service Template** field, select **Project Operations**</span></span> 

6. <span data-ttu-id="af30d-122">अपने परिनियोजन के लिए परिवेश प्रकार का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="af30d-122">Select the environment type for your deployment.</span></span> <span data-ttu-id="af30d-123">सदस्यता-आधारित परीक्षण आपको 30 दिनों के लिए CDS परिवेश परिनियोजित करने देगा।</span><span class="sxs-lookup"><span data-stu-id="af30d-123">A subscription-based trial will let you deploy a CDS environment for 30 days.</span></span> 

![परिनियोजन सेटिंग्स](./media/1DeploymentSettings.png)

> [!IMPORTANT]
> <span data-ttu-id="af30d-125">सेवा की शर्तों को स्वीकार करने के लिए **सहमत** चुनें और फिर परिनियोजन सेटिंग्स पर वापस जाने के लिए **पूर्ण** चुनें।</span><span class="sxs-lookup"><span data-stu-id="af30d-125">Select **Agree** to acknowledge the terms of service and then select **Done** to return to the deployment settings.</span></span>

![परिनियोजन सहमति](./media/2DeploymentConsent.png)

7. <span data-ttu-id="af30d-127">विज़ार्ड में बाकी आवश्यक फ़ील्ड को पूरा करें और परिनियोजन की पुष्टि करें।</span><span class="sxs-lookup"><span data-stu-id="af30d-127">Complete the remaining required fields in the wizard and confirm the deployment.</span></span> <span data-ttu-id="af30d-128">परिवेश के प्रकार के आधार पर परिवेश प्रोविजनिंग समय बदलता रहता है।</span><span class="sxs-lookup"><span data-stu-id="af30d-128">Environment provisioning time varies based on the environment type.</span></span> <span data-ttu-id="af30d-129">प्रोविजनिंग में छह घंटे तक लग सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="af30d-129">Provisioning might take up to six hours.</span></span>

  <span data-ttu-id="af30d-130">परिनियोजन सफलतापूर्वक पूरा होने के बाद, परिवेश **परिनियोजित** के रूप में दिखाएगा।</span><span class="sxs-lookup"><span data-stu-id="af30d-130">After the deployment completes successfully, the environment will show as **Deployed**.</span></span>

8. <span data-ttu-id="af30d-131">परिवेश सफलतापूर्वक परिनियोजित हुआ है या नहीं की पुष्टि करने के लिए, **लॉगिन** चुनें और पुष्टि करने के लिए परिवेश पर लॉग ऑन करें।</span><span class="sxs-lookup"><span data-stu-id="af30d-131">To confirm the environment has deployed successfully, select **Login** and log on to the environment to confirm.</span></span>

![परिवेश विवरण](./media/3EnvironmentDetails.png)

## <a name="apply-project-operations-finance-demo-data-optional-step"></a><span data-ttu-id="af30d-133">परियोजना संचालन वित्त डेमो डेटा लागू करें (वैकल्पिक चरण)</span><span class="sxs-lookup"><span data-stu-id="af30d-133">Apply Project Operations Finance demo data (optional step)</span></span>

<span data-ttu-id="af30d-134">10.0.13 सेवा रिलीज़ क्लाउड द्वारा होस्ट किए गए परिवेश पर परियोजना संचालन वित्त डेटा लागू करें जैसा कि [इस आलेख](resource-apply-finance-demo-data.md) में वर्णित है.</span><span class="sxs-lookup"><span data-stu-id="af30d-134">Apply Project Operations Finance demo data to 10.0.13 service release Cloud Hosted Environment as described in [this article](resource-apply-finance-demo-data.md).</span></span>

## <a name="apply-updates-to-the-finance-environment"></a><span data-ttu-id="af30d-135">वित्त परिवेश में अपडेट लागू करें</span><span class="sxs-lookup"><span data-stu-id="af30d-135">Apply updates to the Finance environment</span></span>

<span data-ttu-id="af30d-136">परियोजना संचालन के लिए एप्लिकेशन संस्करण **10.0.13 (10.0.569.20009)** या उच्चतर वाले वित्त परिवेश की आवश्यकता होती है।</span><span class="sxs-lookup"><span data-stu-id="af30d-136">Project Operations requires a Finance environment with application version **10.0.13 (10.0.569.20009)** or higher.</span></span>

<span data-ttu-id="af30d-137">इस संस्करण को पाने के लिए आपको अपने वित्त परिवेश में गुणवत्ता अपडेट लागू करने पड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="af30d-137">You might need to apply quality updates to your Finance environment to receive this version.</span></span>

1. <span data-ttu-id="af30d-138">LCS में, **परिवेश विवरण** पृष्ठ पर, **उपलब्ध अपडेट** अनुभाग में, **अपडेट देखें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="af30d-138">In LCS, on the **Environment details** page, in the **Available Updates** section, select **View Update**.</span></span>

![अपडेट देखें](./media/5ViewUpdates.png)

2. <span data-ttu-id="af30d-140">**बाइनरी अपडेट** पृष्ठ पर, **पैकेज सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="af30d-140">On the **Binary updates** page, select **Save package.**</span></span>

![पैकेज सहेजें](./media/6SavePackage.png)

3. <span data-ttu-id="af30d-142">**सभी चुनें** क्लिक करें और फिर **पैकेज सहेजें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="af30d-142">Click **Select all** and then select **Save package**.</span></span>

![अपडेट की समीक्षा करें और सहेजें](./media/7ReviewAndSaveUpdates.png)

4. <span data-ttu-id="af30d-144">पैकेज का नाम और विवरण दर्ज करें, और फिर **सहेजें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="af30d-144">Enter a name and a description of the package, and then select **Save**.</span></span> <span data-ttu-id="af30d-145">इंटरनेट कनेक्शन की गति के आधार पर, इस प्रक्रिया में कुछ समय लग सकता है।</span><span class="sxs-lookup"><span data-stu-id="af30d-145">Depending on the internet connection, this process might take some time.</span></span>

![परिसंपत्ति लाइब्रेरी में पैकेज अपलोड करें](./media/8UploadPackageToAssetsLibrary.png)

5. <span data-ttu-id="af30d-147">पैकेज सहेजे जाने के बाद **पूर्ण** चुनें और इस पैकेज को अपनी LCS परियोजना में परिसंपत्ति लाइब्रेरी में सहेजें।</span><span class="sxs-lookup"><span data-stu-id="af30d-147">After the package is saved, select **Done** and save this package to the Assets library in your LCS project.</span></span>

<span data-ttu-id="af30d-148">पैकेज को सहेजने और मान्य करने में ~15 मिनट लग सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="af30d-148">Saving and validating the package might take ~15 minutes.</span></span>

6. <span data-ttu-id="af30d-149">अपडेट लागू करने के लिए, LCS में **परिवेश विवरण** पृष्ठ पर जाएं और **बनाए रखें** > **अपडेट लागू करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="af30d-149">To apply the update, navigate to the **Environment details** page in LCS and select **Maintain** > **Apply updates**.</span></span>

![परिवेश बनाए रखें](./media/9MaintainEnvironment.png)

7. <span data-ttu-id="af30d-151">अपडेट सूची में, आपके द्वारा बनाया गया पैकेज चुनें और **लागू करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="af30d-151">In the updates list select the package you created, and select **Apply**.</span></span>

![अपडेट लागू करें](./media/10ApplyUpdates.png)

<span data-ttu-id="af30d-153">परिवेश की सर्विसिंग में कुछ समय लगेगा।</span><span class="sxs-lookup"><span data-stu-id="af30d-153">Environment servicing will take some time.</span></span> <span data-ttu-id="af30d-154">इसके पूरा होने के बाद, परिवेश परिनियोजित स्थिति में लौट आएगा।</span><span class="sxs-lookup"><span data-stu-id="af30d-154">After it is complete, the environment will return to a deployed state.</span></span>

![परिवेश नियोजित](./media/11EnvironmentDeployed.png)

## <a name="establish-a-dual-write-connection"></a><span data-ttu-id="af30d-156">एक ड्यूल राइट कनेक्शन स्थापित करें</span><span class="sxs-lookup"><span data-stu-id="af30d-156">Establish a Dual Write connection</span></span> 

1. <span data-ttu-id="af30d-157">अपनी LCS परियोजना में, **परिवेश विवरण** पृष्ठ पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="af30d-157">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="af30d-158">**Common Data Service परिवेश जानकारी** के तहत, **अनुप्रयोग के लिए CDS से लिंक करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="af30d-158">Under **Common Data Service Environment Information**, select **Link to CDS for Apps**.</span></span>
3. <span data-ttu-id="af30d-159">लिंक पूरा होने के बाद, फिर से **ऐप्स के लिए CDS से लिंक करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="af30d-159">After the link is complete, select **Link to CDS for Apps** again.</span></span> <span data-ttu-id="af30d-160">आपको वित्त में ड्यूल राइट पर रिडायरेक्ट किया जाएगा।</span><span class="sxs-lookup"><span data-stu-id="af30d-160">You will be redirected to Dual Write in Finance.</span></span>

![CDS से लिंक करें](./media/12LinktoCDS.png)

4. <span data-ttu-id="af30d-162">एकीकरण में मैप किए जाने वाले निकायों तक पहुंचने के लिए **समाधान लागू करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="af30d-162">Select **Apply Solution** to access the entities that will be mapped in the integration.</span></span>

![समाधान लागू करें](./media/13ApplySolutions.png)

5. <span data-ttu-id="af30d-164">दोनों समाधानों **Dynamics 365 Finance and Operations ड्यूल राइट निकाय मानचित्र** तथा **और Dynamics 365 परियोजना संचालन ड्यूल राइट निकाय मानचित्र**, को चुनें और फिर **लागू करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="af30d-164">Select both solutions, **Dynamics 365 Finance and Operations Dual Write Entity Map** and **Dynamics 365 Project Operations Dual Write Entity Maps**, and then select **Apply**.</span></span>

![समाधान की पुष्टि करें](./media/14ConfirmSolutions.png)

<span data-ttu-id="af30d-166">समाधान लागू किए जाने के बाद, ड्यूल राइट निकाय परिवेश पर लागू होती हैं।</span><span class="sxs-lookup"><span data-stu-id="af30d-166">After the solutions are applied, the Dual Write entities are applied to the environment.</span></span>

![समाधान लागू करना](./media/15ApplyingSolutions.png)

<span data-ttu-id="af30d-168">निकाय लागू किए जाने के बाद, सभी उपलब्ध मैपिंग परिवेश में सूचीबद्ध होती हैं।</span><span class="sxs-lookup"><span data-stu-id="af30d-168">After the entities are applied, all available mappings are listed in the environment.</span></span>

![ड्यूल राइट मानचित्र](./media/15DWMappings.png)

## <a name="refresh-the-data-entities-after-the-update"></a><span data-ttu-id="af30d-170">अपडेट के बाद डेटा निकायों को रिफ्रेश करें</span><span class="sxs-lookup"><span data-stu-id="af30d-170">Refresh the data entities after the update</span></span>

1. <span data-ttu-id="af30d-171">वित्त में, **डेटा प्रबंधन** कार्यक्षेत्र पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="af30d-171">In Finance, go to the **Data management** workspace.</span></span>

![डेटा प्रबंधन कार्यस्थान](./media/16DataManagement.png)

2. <span data-ttu-id="af30d-173">**फ्रेमवर्क मापदंड** शीर्षक चुनें।</span><span class="sxs-lookup"><span data-stu-id="af30d-173">Select the **Framework parameters** tile.</span></span>

![फ्रेमवर्क मापदंड](./media/17FrameworkParameters.png)

3. <span data-ttu-id="af30d-175">**निकाय सेटिंग्स** पृष्ठ पर, **निकाय सूची** चुनें।</span><span class="sxs-lookup"><span data-stu-id="af30d-175">On the **Entity settings** page, select **Refresh Entity list**.</span></span>

![निकाय सूची रिफ्रेश करें](./media/18RefreshEntityList.png)

<span data-ttu-id="af30d-177">रिफ्रेश में लगभग 20 मिनट लग सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="af30d-177">The refresh is going to take approximately 20 minutes.</span></span> <span data-ttu-id="af30d-178">पूर्ण होने पर आपको एक सूचना मिलेगी।</span><span class="sxs-lookup"><span data-stu-id="af30d-178">You will receive an alert when it is complete.</span></span>

![पुष्टिकरण रिफ्रेश](./media/19RefreshConfirmation.png)

## <a name="run-project-operations-dual-write-maps"></a><span data-ttu-id="af30d-180">परियोजना संचालन ड्यूल राइट मानचित्र चलाएं</span><span class="sxs-lookup"><span data-stu-id="af30d-180">Run Project Operations Dual Write maps</span></span>

1. <span data-ttu-id="af30d-181">अपनी LCS परियोजना में, **परिवेश विवरण** पृष्ठ पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="af30d-181">In your LCS project, go to the **Environment details** page.</span></span>
2. <span data-ttu-id="af30d-182">**Common Data Service परिवेश जानकारी** के तहत, **अनुप्रयोग के लिए CDS से लिंक करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="af30d-182">Under **Common Data Service Environment Information**, select **Link to CDS for Apps.**</span></span> <span data-ttu-id="af30d-183">आपके द्वारा लिंक चुनने के बाद, आप मैपिंग में निकायों की सूची पर रिडायरेक्ट हो जाएंगे।</span><span class="sxs-lookup"><span data-stu-id="af30d-183">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="af30d-184">निम्न तालिका में वर्णित के अनुसार मानचित्र शुरू करें।</span><span class="sxs-lookup"><span data-stu-id="af30d-184">Start the maps as described in the following table.</span></span> <span data-ttu-id="af30d-185">अनुक्रम का सूचीबद्ध के रूप में पालन करना सुनिश्चित करें।</span><span class="sxs-lookup"><span data-stu-id="af30d-185">Make sure to follow the sequence as listed.</span></span>

| <span data-ttu-id="af30d-186">**निकाय मानचित्र**</span><span class="sxs-lookup"><span data-stu-id="af30d-186">**Entity Map**</span></span> | <span data-ttu-id="af30d-187">**निकाय रिफ्रेश करें**</span><span class="sxs-lookup"><span data-stu-id="af30d-187">**Refresh entity**</span></span> | <span data-ttu-id="af30d-188">**प्रारंभिक सिंक**</span><span class="sxs-lookup"><span data-stu-id="af30d-188">**Initial sync**</span></span> | <span data-ttu-id="af30d-189">**प्रारंभिक सिंक के लिए मास्टर**</span><span class="sxs-lookup"><span data-stu-id="af30d-189">**Master for initial sync**</span></span> | <span data-ttu-id="af30d-190">**पूर्वापेक्षाएं चलाएं**</span><span class="sxs-lookup"><span data-stu-id="af30d-190">**Run prerequisites**</span></span> | <span data-ttu-id="af30d-191">**पूर्वापेक्षाएं प्रारंभिक सिंक**</span><span class="sxs-lookup"><span data-stu-id="af30d-191">**Prerequisites initial sync**</span></span> |
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="af30d-192">**सभी कंपनियों के लिए परियोजना संसाधन भूमिकाएं (bookableresourcecategories)**</span><span class="sxs-lookup"><span data-stu-id="af30d-192">**Project Resource Roles for All Companies (bookableresourcecategories)**</span></span> | <span data-ttu-id="af30d-193">No</span><span class="sxs-lookup"><span data-stu-id="af30d-193">No</span></span> | <span data-ttu-id="af30d-194">हाँ</span><span class="sxs-lookup"><span data-stu-id="af30d-194">Yes</span></span> | <span data-ttu-id="af30d-195">Common Data Service</span><span class="sxs-lookup"><span data-stu-id="af30d-195">Common Data Service</span></span> | <span data-ttu-id="af30d-196">No</span><span class="sxs-lookup"><span data-stu-id="af30d-196">No</span></span> | <span data-ttu-id="af30d-197">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-197">N\A</span></span> |
| <span data-ttu-id="af30d-198">**कानूनी निकाय (cdm\_companies)**</span><span class="sxs-lookup"><span data-stu-id="af30d-198">**Legal entities (cdm\_companies)**</span></span> | <span data-ttu-id="af30d-199">No</span><span class="sxs-lookup"><span data-stu-id="af30d-199">No</span></span> | <span data-ttu-id="af30d-200">हाँ</span><span class="sxs-lookup"><span data-stu-id="af30d-200">Yes</span></span> | <span data-ttu-id="af30d-201">Finance and Operations ऐप</span><span class="sxs-lookup"><span data-stu-id="af30d-201">Finance and Operations apps</span></span> | <span data-ttu-id="af30d-202">No</span><span class="sxs-lookup"><span data-stu-id="af30d-202">No</span></span> | <span data-ttu-id="af30d-203">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-203">N\A</span></span> |
| <span data-ttu-id="af30d-204">**परियोजना संचालन एकीकरण वास्तविक (msdyn\_actuals)**</span><span class="sxs-lookup"><span data-stu-id="af30d-204">**Project Operations integration actuals (msdyn\_actuals)**</span></span> | <span data-ttu-id="af30d-205">No</span><span class="sxs-lookup"><span data-stu-id="af30d-205">No</span></span> | <span data-ttu-id="af30d-206">No</span><span class="sxs-lookup"><span data-stu-id="af30d-206">No</span></span> | <span data-ttu-id="af30d-207">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-207">N\A</span></span> | <span data-ttu-id="af30d-208">हाँ</span><span class="sxs-lookup"><span data-stu-id="af30d-208">Yes</span></span> | <span data-ttu-id="af30d-209">No</span><span class="sxs-lookup"><span data-stu-id="af30d-209">No</span></span> |
| <span data-ttu-id="af30d-210">**परियोजना अनुबंध लाइन (salesorderdetails)**</span><span class="sxs-lookup"><span data-stu-id="af30d-210">**Project contract lines (salesorderdetails)**</span></span> | <span data-ttu-id="af30d-211">No</span><span class="sxs-lookup"><span data-stu-id="af30d-211">No</span></span> | <span data-ttu-id="af30d-212">No</span><span class="sxs-lookup"><span data-stu-id="af30d-212">No</span></span> | <span data-ttu-id="af30d-213">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-213">N\A</span></span> | <span data-ttu-id="af30d-214">No</span><span class="sxs-lookup"><span data-stu-id="af30d-214">No</span></span> | <span data-ttu-id="af30d-215">No</span><span class="sxs-lookup"><span data-stu-id="af30d-215">No</span></span> |
| <span data-ttu-id="af30d-216">**परियोजना लेनदेन संबंधों के लिए एकीकरण निकाय (msdyn\_transactionconnections)**</span><span class="sxs-lookup"><span data-stu-id="af30d-216">**Integration entity for project transaction relationships (msdyn\_transactionconnections)**</span></span> | <span data-ttu-id="af30d-217">No</span><span class="sxs-lookup"><span data-stu-id="af30d-217">No</span></span> | <span data-ttu-id="af30d-218">No</span><span class="sxs-lookup"><span data-stu-id="af30d-218">No</span></span> | <span data-ttu-id="af30d-219">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-219">N\A</span></span> | <span data-ttu-id="af30d-220">No</span><span class="sxs-lookup"><span data-stu-id="af30d-220">No</span></span> | <span data-ttu-id="af30d-221">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-221">N\A</span></span> |
| <span data-ttu-id="af30d-222">**परियोजना संचालन एकीकरण अनुबंध लाइन माइलस्टोन (msdyn\_contractlinesscheduleofvalues)**</span><span class="sxs-lookup"><span data-stu-id="af30d-222">**Project Operations integration contract line milestones (msdyn\_contractlinesscheduleofvalues)**</span></span> | <span data-ttu-id="af30d-223">No</span><span class="sxs-lookup"><span data-stu-id="af30d-223">No</span></span> | <span data-ttu-id="af30d-224">No</span><span class="sxs-lookup"><span data-stu-id="af30d-224">No</span></span> | <span data-ttu-id="af30d-225">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-225">N\A</span></span> | <span data-ttu-id="af30d-226">No</span><span class="sxs-lookup"><span data-stu-id="af30d-226">No</span></span> | <span data-ttu-id="af30d-227">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-227">N\A</span></span> |
| <span data-ttu-id="af30d-228">**व्यय अनुमानों के लिए परियोजना संचालन एकीकरण इकाई (msdyn\_estimateslines)**</span><span class="sxs-lookup"><span data-stu-id="af30d-228">**Project Operations integration entity for expense estimates (msdyn\_estimateslines)**</span></span> | <span data-ttu-id="af30d-229">No</span><span class="sxs-lookup"><span data-stu-id="af30d-229">No</span></span> | <span data-ttu-id="af30d-230">No</span><span class="sxs-lookup"><span data-stu-id="af30d-230">No</span></span> | <span data-ttu-id="af30d-231">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-231">N\A</span></span> | <span data-ttu-id="af30d-232">No</span><span class="sxs-lookup"><span data-stu-id="af30d-232">No</span></span> | <span data-ttu-id="af30d-233">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-233">N\A</span></span> |
| <span data-ttu-id="af30d-234">**प्रकल्प परिचालन एकीकरण प्रकल्प खर्च श्रेणी निर्यात निकाय (msdyn\_खर्च श्रेणी)**</span><span class="sxs-lookup"><span data-stu-id="af30d-234">**Project Operations integration project expense categories export entity (msdyn\_expensecategories)**</span></span> | <span data-ttu-id="af30d-235">No</span><span class="sxs-lookup"><span data-stu-id="af30d-235">No</span></span> | <span data-ttu-id="af30d-236">No</span><span class="sxs-lookup"><span data-stu-id="af30d-236">No</span></span> | <span data-ttu-id="af30d-237">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-237">N\A</span></span> | <span data-ttu-id="af30d-238">No</span><span class="sxs-lookup"><span data-stu-id="af30d-238">No</span></span> | <span data-ttu-id="af30d-239">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-239">N\A</span></span> |
| <span data-ttu-id="af30d-240">**परियोजना संचालन एकीकरण परियोजना व्यय निर्यात निकाय (msdyn\_expenses)**</span><span class="sxs-lookup"><span data-stu-id="af30d-240">**Project Operations integration project expenses export entity (msdyn\_expenses)**</span></span> | <span data-ttu-id="af30d-241">हाँ</span><span class="sxs-lookup"><span data-stu-id="af30d-241">Yes</span></span> | <span data-ttu-id="af30d-242">No</span><span class="sxs-lookup"><span data-stu-id="af30d-242">No</span></span> | <span data-ttu-id="af30d-243">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-243">N\A</span></span> | <span data-ttu-id="af30d-244">No</span><span class="sxs-lookup"><span data-stu-id="af30d-244">No</span></span> | <span data-ttu-id="af30d-245">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-245">N\A</span></span> |
| <span data-ttu-id="af30d-246">**घंटे के अनुमानों के लिए परियोजना संचालन एकीकरण निकाय (msdyn\_resourceassignments)**</span><span class="sxs-lookup"><span data-stu-id="af30d-246">**Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**</span></span> | <span data-ttu-id="af30d-247">हाँ</span><span class="sxs-lookup"><span data-stu-id="af30d-247">Yes</span></span> | <span data-ttu-id="af30d-248">No</span><span class="sxs-lookup"><span data-stu-id="af30d-248">No</span></span> | <span data-ttu-id="af30d-249">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-249">N\A</span></span> | <span data-ttu-id="af30d-250">No</span><span class="sxs-lookup"><span data-stu-id="af30d-250">No</span></span> | <span data-ttu-id="af30d-251">लागू नहीं है</span><span class="sxs-lookup"><span data-stu-id="af30d-251">N\A</span></span> |


4. <span data-ttu-id="af30d-252">निकाय को रिफ्रेश करने के लिए, मानचित्र नाम चुनें और उसके बाद **निकाय रिफ्रेश करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="af30d-252">To refresh the entity, select the map name, and then select **Refresh entities**.</span></span> 


![मानचित्र रिफ्रेश करें](./media/20RefreshMapping.png)

5. <span data-ttu-id="af30d-254">रिफ्रेश पूरा होते ही, मैप को रन करें.</span><span class="sxs-lookup"><span data-stu-id="af30d-254">After the refresh is complete, run the map.</span></span> <span data-ttu-id="af30d-255">इससे पहले कि आप अगला मानचित्र सक्षम करें, सत्यापित करें कि तालिका में मानचित्र **रनिंगहै** स्थिति में है।</span><span class="sxs-lookup"><span data-stu-id="af30d-255">Before you enable the next map, verify that the map in the table is in a state of **Running**.</span></span> <span data-ttu-id="af30d-256">बड़ी संख्या में पूर्वापेक्षाओं के साथ चल रहे मानचित्र में कुछ समय लग सकता है।</span><span class="sxs-lookup"><span data-stu-id="af30d-256">Running maps with a larger number of prerequisites might take some time.</span></span>

<span data-ttu-id="af30d-257">पूर्वापेक्षाओं के साथ एक मानचित्र चलाने के लिए, **संबंधित निकाय मानचित्र दिखाएं** टॉगल करें।</span><span class="sxs-lookup"><span data-stu-id="af30d-257">To run a map with prerequisites, enable the **Show related entity maps** toggle.</span></span> <span data-ttu-id="af30d-258">यदि तालिका दर्शाती है कि **पूर्वापेक्षा प्रारंभिक सिंक** है **नहीं** है, तो इसे चलाने से पहले सत्यापित करें कि सभी पूर्वापेक्षित मानचित्रों में **प्रारंभिक सिंक** फ्लैग **बंद** है।</span><span class="sxs-lookup"><span data-stu-id="af30d-258">If the table indicates **Prerequisite initial sync** is **No**, verify that the **Initial sync** flag is **Off** in all the prerequisite maps before you run it.</span></span>

![मानचित्र चलाएं](./media/21RunMap.png)

6. <span data-ttu-id="af30d-260">पुष्टि करें कि परियोजना से संबंधित सभी मानचित्र चालू स्थिति में हैं।</span><span class="sxs-lookup"><span data-stu-id="af30d-260">Validate all project related maps are in the running state.</span></span>

![सभी मानचित्र चलाए जा रहे हैं](./media/22AllMapsRunning.png)


## <a name="apply-configuration-data-in-cds-for-project-operations-optional"></a><span data-ttu-id="af30d-262">Project Operations के लिए CDS में कॉन्फ़िगरेशन डेटा लागू करें (वैकल्पिक)</span><span class="sxs-lookup"><span data-stu-id="af30d-262">Apply configuration data in CDS for Project Operations (optional)</span></span>

<span data-ttu-id="af30d-263">यदि आपने Finance परिवेश में डेमो डेटा लागू किया है, तो CDS परिवेश पर डेमो डेटा लागू करने के लिए [Project Operations के लिए Common Data Service में कॉन्फ़िगरेशन डेटा सेट अप करें और लागू करें](resource-apply-pro-setup-config-data.md) देखें.</span><span class="sxs-lookup"><span data-stu-id="af30d-263">If you have applied demo data to the Finance environment, see [Set up and apply configuration data in the Common Data Service for Project Operations](resource-apply-pro-setup-config-data.md) to apply demo data to CDS environment.</span></span>


<span data-ttu-id="af30d-264">आपका परियोजना संचालन परिवेश अब प्रोविजन और कॉन्फ़िगर किया गया है।</span><span class="sxs-lookup"><span data-stu-id="af30d-264">Your Project Operations environment is now provisioned and configured.</span></span> 
