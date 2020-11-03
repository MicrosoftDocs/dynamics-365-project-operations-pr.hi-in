---
title: नई परियोजना बनाएँ
description: यह विषय एक नई प्रोजेक्ट बनाने के तरीके के बारे में जानकारी प्रदान करता है.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 727d287c571b2a64bf10b2393a87567093a420d2
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077835"
---
# <a name="create-a-new-project"></a><span data-ttu-id="17e8e-103">नई परियोजना बनाएँ</span><span class="sxs-lookup"><span data-stu-id="17e8e-103">Create a new project</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="17e8e-104">एक नई प्रोजेक्ट बनाने के लिए निम्नलिखित चरणों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-104">Complete the following steps to create a new project.</span></span>

1. <span data-ttu-id="17e8e-105">**परियोजना प्रबंधन** पृष्ठ पर, **नई परियोजना** का चयन करें, और निम्नलिखित मानों को दर्ज करें:</span><span class="sxs-lookup"><span data-stu-id="17e8e-105">On the **Project management** page, select **New project** , and enter the following values:</span></span>

    - <span data-ttu-id="17e8e-106">**प्रोजेक्ट का प्रकार:** समय और सामग्री</span><span class="sxs-lookup"><span data-stu-id="17e8e-106">**Project type:** Time and material</span></span>
    - <span data-ttu-id="17e8e-107">**प्रोजेक्ट का नाम:** XYZ अपग्रेड चरण 2</span><span class="sxs-lookup"><span data-stu-id="17e8e-107">**Project name:** XYZ Upgrade Phase 2</span></span>
    - <span data-ttu-id="17e8e-108">**प्रोजेक्ट समूह:** TM\_WIP</span><span class="sxs-lookup"><span data-stu-id="17e8e-108">**Project group:** TM\_WIP</span></span>
    - <span data-ttu-id="17e8e-109">**परियोजना अनुबंध ID** 00000002</span><span class="sxs-lookup"><span data-stu-id="17e8e-109">**Project contract ID:** 00000002</span></span>

2. <span data-ttu-id="17e8e-110">**परियोजना बनाएँ** चुनें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-110">Select **Create project**.</span></span>

## <a name="assign-a-resource-to-a-project"></a><span data-ttu-id="17e8e-111">किसी प्रोजेक्ट में एक संसाधन असाइन करें</span><span class="sxs-lookup"><span data-stu-id="17e8e-111">Assign a resource to a project</span></span>

1. <span data-ttu-id="17e8e-112">**श्रमिक** पृष्ठ पर, **श्रमिक** सूची में, उस श्रमिक के लिए रिकॉर्ड का चयन करें जिसे आप पूर्व में योग्यताओं के लिए सेट करते हैं, और श्रमिक रिकॉर्ड खोलें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-112">On the **Workers** page, in the **Workers** list, select the record for the worker that you previously set up competencies for, and open the worker record.</span></span>
2. <span data-ttu-id="17e8e-113">क्रियाकलाप फलक पर, **परियोजना** टैब पर, **सेटअप** समूह में, **परियोजना सौंपें**  का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-113">On the Action Pane, on the **Project** tab, in the **Setup** group, select **Assign projects**.</span></span>
3. <span data-ttu-id="17e8e-114">**संसाधन प्रमाणीकरण परियोजना कार्यभार** पृष्ठ पर **परियोजना** टैब पर, **चयनित परियोजनाओं से परियोजना जोड़ें** फील्ड में, **XYZ अपग्रेड चरण 2** परियोजना पर फ़िल्टर करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-114">On the **Resource validation project assignments** page, on the **Projects** tab, in the **Add the project to selected projects** field, filter on the **XYZ Upgrade Phase 2** project.</span></span>
4. <span data-ttu-id="17e8e-115">**शेष परियोजना** फलक में, एक परियोजना का चयन करें, और फिर इसे **चयनित परियोजना** फलक से जोड़ने के लिए तीर बटन का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-115">In the **Remaining projects** pane, select a project, and then select the arrow button to add it to the **Selected projects** pane.</span></span>

<span data-ttu-id="17e8e-116">आप अपनी आवश्यकतानुसार किसी संसाधन के लिए श्रेणियां भी नियत कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="17e8e-116">You can also assign categories for a resource as you require.</span></span> <span data-ttu-id="17e8e-117">श्रेणी प्रकार या तो **लागत** है या **राजस्व** है.</span><span class="sxs-lookup"><span data-stu-id="17e8e-117">The category type is either **Cost** or **Revenue**.</span></span> <span data-ttu-id="17e8e-118">श्रेणी प्रकार आपके संगठन द्वारा निर्धारित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="17e8e-118">The category type is determined by your organization.</span></span> <span data-ttu-id="17e8e-119">यदि संसाधन के लिए कोई श्रेणियां नियत नहीं की जाती हैं, तो फाइनैन्स लागत और राजस्व के लिए घंटे की कीमतों पर डिफ़ॉल्ट श्रेणी को खोजता है.</span><span class="sxs-lookup"><span data-stu-id="17e8e-119">If no categories are assigned for a resource, Finance looks up the default category on hour prices for cost and revenue.</span></span>

## <a name="set-up-project-resource-and-role-characteristics"></a><span data-ttu-id="17e8e-120">परियोजना संसाधन और भूमिका विशेषताओं को सेट करें</span><span class="sxs-lookup"><span data-stu-id="17e8e-120">Set up project resource and role characteristics</span></span>

<span data-ttu-id="17e8e-121">एक परियोजना प्रबंधक परियोजना के लिए आवश्यक भूमिकाओं को बनाने के लिए परियोजना रिसोर्सिंग कार्यक्षमता का उपयोग कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="17e8e-121">A project manager can use the project resourcing functionality to create the roles that are required for the project.</span></span> <span data-ttu-id="17e8e-122">यदि पुष्टि किए गए संसाधन अभी भी अज्ञात हैं जब संसाधन आरक्षित किए जा रहे हैं तो भूमिकाओं का उपयोग किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="17e8e-122">Roles can be used if confirmed resources are still unknown when resources are being reserved.</span></span> <span data-ttu-id="17e8e-123">भूमिकाओं को अस्थायी रूप से नियोजित संसाधनों के रूप में आरक्षित किया जा सकता है, ताकि आप परियोजना नियोजन के चरणों को जारी रख सकें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-123">Roles can be temporarily reserved as planned resources, so that you can continue the project planning stages.</span></span>

<span data-ttu-id="17e8e-124">[![एक भूमिका का उदाहरण](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg)</span><span class="sxs-lookup"><span data-stu-id="17e8e-124">[![Example of a role](./media/projectresourcing05.jpg)](./media/projectresourcing05.jpg)</span></span> 

<span data-ttu-id="17e8e-125">**परिदृश्य:** Contoso को एक समय और सामग्री परियोजना को पूरा करने के लिए काम पर रखा गया था जिसके पास एक अनुमोदित परियोजना चार्टर है.</span><span class="sxs-lookup"><span data-stu-id="17e8e-125">**Scenario:** Contoso was hired to complete a Time and material project that has an approved project charter.</span></span> <span data-ttu-id="17e8e-126">कनिष्ठ परियोजना प्रबंधक अभी भी परियोजना का दायरा पूरा कर रहा है.</span><span class="sxs-lookup"><span data-stu-id="17e8e-126">The junior project manager is still completing the scope of the project.</span></span> <span data-ttu-id="17e8e-127">संसाधन प्रबंधक वर्तमान में विशिष्ट संसाधनों की पहचान कर रहा है जो नई परियोजना पर काम करने के लिए आरक्षित होंगे.</span><span class="sxs-lookup"><span data-stu-id="17e8e-127">The resource manager is currently identifying specific resources that will be reserved to work on the new project.</span></span> <span data-ttu-id="17e8e-128">परियोजना की महत्वपूर्ण प्रकृति के कारण, परियोजना प्रायोजक ने वरिष्ठ परियोजना प्रबंधक से भूमिकाओं में से एक के रूप में अनुरोध किया.</span><span class="sxs-lookup"><span data-stu-id="17e8e-128">Because of the critical nature of the project, the project sponsor requested Senior project manager as one of the roles.</span></span> <span data-ttu-id="17e8e-129">यदि कनिष्ठ परियोजना प्रबंधक को परियोजना नियोजन के दौरान संसाधन जानकारी की आवश्यकता होती है तो संसाधन प्रबंधक को नए संसाधन प्राप्त करने चाहिए और सिस्टम में भूमिका को परिभाषित करना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="17e8e-129">The resource manager must acquire the new resource and define the role in the system in case the junior project manager requires the resource information during project planning.</span></span>

<span data-ttu-id="17e8e-130">निम्नलिखित चरणों से पता चलता है कि कैसे संसाधन प्रबंधक वरिष्ठ परियोजना प्रबंधक की भूमिका और इसके साथ सहयोगी संसाधन विशेषताओं को सेट कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="17e8e-130">The following steps show how the resource manager can set up the Senior project manager role and associate resource characteristics with it.</span></span> <span data-ttu-id="17e8e-131">बाद में, भूमिका का उपयोग आवश्यक संसाधन योग्यताओं से मेल खाने वाले उपलब्ध संसाधनों की खोज के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="17e8e-131">Later, the role can be used to search for available resources that match the required resource competencies.</span></span>

1. <span data-ttu-id="17e8e-132">**भूमिकाएं सेट करें** पृष्ठ पर, **नया** का चयन करें, और निम्नलिखित मानों को दर्ज करें:</span><span class="sxs-lookup"><span data-stu-id="17e8e-132">On the **Setup roles** page, select **New** , and enter the following values:</span></span>

    - <span data-ttu-id="17e8e-133">**भूमिका ID:** वरिष्ठ परियोजना प्रबंधक</span><span class="sxs-lookup"><span data-stu-id="17e8e-133">**Role ID:** Senior Project Manager</span></span>
    - <span data-ttu-id="17e8e-134">**वर्णन:** वरिष्ठ परियोजना प्रबंधक</span><span class="sxs-lookup"><span data-stu-id="17e8e-134">**Description:** Senior Project Manager</span></span>

2. <span data-ttu-id="17e8e-135">**बनाएँ** चुनें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-135">Select **Create**.</span></span>
3. <span data-ttu-id="17e8e-136">**वरिष्ठ परियोजना प्रबंधक** भूमिका का चयन करें, और फिर **विशेषताओं को कॉन्फ़िगर करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-136">Select the **Senior Project Manager** role, and then select **Configure characteristics**.</span></span>
4. <span data-ttu-id="17e8e-137">**विशेषताओं के प्रकार** फ़ील्ड में, **कौशल** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-137">In the **Characteristics type** field, select **Skill**.</span></span>
5. <span data-ttu-id="17e8e-138">**उपलब्ध विशेषताएं** फ़ील्ड में, खोजने के लिए कौशल दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-138">In the **Available characteristics** field, enter the skill to search for.</span></span>
6. <span data-ttu-id="17e8e-139">**विशेषताओं के प्रकार** फ़ील्ड में, **प्रमाण-पत्र** चुनें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-139">In the **Characteristic type** field, select **Certificate**.</span></span>
7. <span data-ttu-id="17e8e-140">**उपलब्ध विशेषताएं** फ़ील्ड में, खोजने के लिए प्रमाण-पत्र का प्रकार दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-140">In the **Available characteristics** field, enter the certificate type to search for.</span></span>

## <a name="assign-a-project-resource-to-a-project"></a><span data-ttu-id="17e8e-141">किसी प्रोजेक्ट के लिए प्रोजेक्ट संसाधन असाइन करें</span><span class="sxs-lookup"><span data-stu-id="17e8e-141">Assign a project resource to a project</span></span>

1. <span data-ttu-id="17e8e-142">**सभी परियोजना** पृष्ठ पर, **XYZ अपग्रेड चरण 2** परियोजना का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-142">On the **All projects** page, select the **XYZ Upgrade Phase 2** project.</span></span>
2. <span data-ttu-id="17e8e-143">**परियोजना दल और शेड्यूलिंग** टैब पर, **जोड़ें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-143">On the **Project team and scheduling** tab, select **Add**.</span></span>
3. <span data-ttu-id="17e8e-144">**भूमिका** फ़ील्ड में, **दल का सदस्य** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-144">In the **Role** field, select **Team member**.</span></span>
4. <span data-ttu-id="17e8e-145">**कैलेंडर से बुक करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-145">Select **Book from calendar**.</span></span>
5. <span data-ttu-id="17e8e-146">**संसाधन उपलब्धता** पृष्ठ पर, **दृश्य सेटिंग्स** चुनें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-146">On the **Resource availability** page, select **View settings**.</span></span>
6. <span data-ttu-id="17e8e-147">**दृश्य सेटिंग्स व्यवस्थित करें** पृष्ठ पर, निम्नलिखित मानों को दर्ज करें:</span><span class="sxs-lookup"><span data-stu-id="17e8e-147">On the **Adjust view settings** page, enter the following values:</span></span>

    - <span data-ttu-id="17e8e-148">**तारीख विस्तार दृश्य के लिए फॉर्मेट:** दिन</span><span class="sxs-lookup"><span data-stu-id="17e8e-148">**Format for date range view:** Day</span></span>
    - <span data-ttu-id="17e8e-149">**उपलब्धता विवरण प्रदर्शित करें:** हाँ</span><span class="sxs-lookup"><span data-stu-id="17e8e-149">**Display availability descriptions:** Yes</span></span>
    - <span data-ttu-id="17e8e-150">**शेष क्षमता प्रदर्शित करें:** हां</span><span class="sxs-lookup"><span data-stu-id="17e8e-150">**Display remaining capacity:** Yes</span></span>

7. <span data-ttu-id="17e8e-151">संसाधनों की सूची में, एक संसाधन का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-151">In the list of resources, select a resource.</span></span>
8. <span data-ttu-id="17e8e-152">**हार्ड बुक** और **पूरी क्षमता** चुनें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-152">Select **Hard book** and **Full capacity**.</span></span>

## <a name="assign-a-resource-to-a-default-role"></a><span data-ttu-id="17e8e-153">डिफ़ॉल्ट भूमिका के लिए संसाधन नियत करें</span><span class="sxs-lookup"><span data-stu-id="17e8e-153">Assign a resource to a default role</span></span>

<span data-ttu-id="17e8e-154">परियोजना या संसाधन प्रबंधकों को उन संसाधनों पर आगे ड्रिल कर सकने में मदद करने के लिए जिन्हें किसी परियोजना के लिए आरक्षित किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="17e8e-154">To help project or resource managers can drill down further on the resources that can be reserved for a project.</span></span> <span data-ttu-id="17e8e-155">आप एक मौजूदा संसाधन या एक नए अधिग्रहीत संसाधन के साथ एक डिफ़ॉल्ट भूमिका संबद्ध कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="17e8e-155">You can associate a default role with an existing resource or a newly acquired resource.</span></span> <span data-ttu-id="17e8e-156">उदाहरण के लिए, जब डैनियल को काम पर रखा गया था, तो उसके पास व्यापार विश्लेषक की भूमिका के लिए अनुभव और कौशल था.</span><span class="sxs-lookup"><span data-stu-id="17e8e-156">For example, when Daniel was hired, he had the experience and skills to fill the Business analyst role.</span></span> <span data-ttu-id="17e8e-157">संसाधन प्रबंधक ने डैनियल की डिफ़ॉल्ट भूमिका के रूप में इस भूमिका को नियत किया.</span><span class="sxs-lookup"><span data-stu-id="17e8e-157">The resource manager assigned this role as Daniel's default role.</span></span> <span data-ttu-id="17e8e-158">इसलिए, संसाधन प्रबंधक ने डैनियल को व्यापार विश्लेषकों के एक पूल से जोड़ा जो परियोजनाओं पर काम करने के लिए उपलब्ध हैं.</span><span class="sxs-lookup"><span data-stu-id="17e8e-158">Therefore, the resource manager added Daniel to a pool of business analysts who are available to work on projects.</span></span>

<span data-ttu-id="17e8e-159">संसाधन आरक्षण के दौरान, परियोजना प्रबंधक परियोजनाओं पर काम करने के लिए उपलब्ध भूमिका संसाधनों को फ़िल्टर कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="17e8e-159">During resource reservation, project managers can filter the role resources that are available to work on projects.</span></span> <span data-ttu-id="17e8e-160">वे इस जानकारी को एक मानदंड के रूप में उपयोग कर सकते हैं जब वे संसाधन पूर्ति के दौरान बहु-मानदंड निर्णय विश्लेषण करते हैं.</span><span class="sxs-lookup"><span data-stu-id="17e8e-160">They can use this information as one criterion when they perform multi-criteria decision analysis during resource fulfillment.</span></span> <span data-ttu-id="17e8e-161">वे किसी दिए गए परियोजना के लिए विशिष्ट कौशल, शिक्षा और अनुभव वाले संसाधनों की खोज करने के लिए फ़िल्टर में अन्य संसाधन विशेषताओं को भी जोड़ सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="17e8e-161">They can also add other resource characteristics to the filter to search for resources that have specific skills, education, and experience for a given project.</span></span>

<span data-ttu-id="17e8e-162">**परिदृश्य:** एक अनुमोदित परियोजना शुरू हो गई है, और परियोजना नियोजन के चरण के दौरान वरिष्ठ परियोजना प्रबंधक की भूमिका को एक नियोजित संसाधन के रूप में आरक्षित किया गया था.</span><span class="sxs-lookup"><span data-stu-id="17e8e-162">**Scenario:** An approved project has started, and the Senior project manager role was reserved as a planned resource during the project planning stage.</span></span> <span data-ttu-id="17e8e-163">संसाधन प्रबंधक ने अब वरिष्ठ परियोजना प्रबंधक की भूमिका को पूरा करने के लिए एक संसाधन प्राप्त कर लिया है.</span><span class="sxs-lookup"><span data-stu-id="17e8e-163">The resource manager has now acquired a resource to fulfill the Senior project manager role.</span></span>

1. <span data-ttu-id="17e8e-164">**संसाधन सूची** पृष्ठ पर, **Daniel Goldschmidt** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-164">On the **Resources list** page, select **Daniel Goldschmidt**.</span></span>
2. <span data-ttu-id="17e8e-165">**संसाधन भूमिका** पृष्ठ पर, **नया** चुनें, और निम्नलिखित मानों को दर्ज करें:</span><span class="sxs-lookup"><span data-stu-id="17e8e-165">On the **Resource role** page, select **New** , and enter the following values:</span></span>

    - <span data-ttu-id="17e8e-166">**प्रभावी:** वर्तमान तिथि दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-166">**Effective:** Enter the current date.</span></span>
    - <span data-ttu-id="17e8e-167">**समाप्ति:** **कभी नहीं** दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-167">**Expiration:** Enter **Never**.</span></span>
    - <span data-ttu-id="17e8e-168">**भूमिका:** **वरिष्ठ परियोजना प्रबंधक**  दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-168">**Role:** Enter **Senior Project Manager**.</span></span>

3. <span data-ttu-id="17e8e-169">**सहेजें** का चयन करें, और उसके बाद पृष्ठ बंद करें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-169">Select **Save** , and then close the page.</span></span>
4. <span data-ttu-id="17e8e-170">**योग्यता** टैब पर, **ProjectMgmt** कौशल और **PMP** प्रमाण-पत्र जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="17e8e-170">On the **Competencies** tab, add the **ProjectMgmt** skill and the **PMP** certificate.</span></span>
