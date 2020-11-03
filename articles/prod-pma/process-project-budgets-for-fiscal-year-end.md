---
title: वित्तीय वर्ष की समाप्ति पर परियोजना बजट स्थानांतरित करें
description: यह लेख भविष्य के वर्षों के लिए शेष बजट राशियों को स्थानांतरित करने और बजट लेखा विवरण बनाने के बारे में जानकारी देता है.
author: Yowelle
manager: AnnBe
ms.date: 03/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 26e013ab99e9a0aeafe25916715ce0ee024df3f7
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077833"
---
# <a name="transfer-project-budgets-at-fiscal-year-end"></a><span data-ttu-id="f651e-103">वित्तीय वर्ष की समाप्ति पर परियोजना बजट स्थानांतरित करें</span><span class="sxs-lookup"><span data-stu-id="f651e-103">Transfer project budgets at fiscal year end</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="f651e-104">बहु-वर्षीय परियोजना पर काम करते समय, आपके पास वित्तीय वर्ष की समाप्ति पर बजट बाकी हो सकता है.</span><span class="sxs-lookup"><span data-stu-id="f651e-104">When working on a multi-year project, you might have remaining budget at the end of the fiscal year.</span></span> <span data-ttu-id="f651e-105">आप शेष बजट राशियों को भविष्य के वर्ष में स्थानांतरित कर सकते हैं और संबद्ध प्रधान खाता-बही में राशि के लिए बजट लेखा विवरण बनाएं.</span><span class="sxs-lookup"><span data-stu-id="f651e-105">You can transfer the remaining budget amounts to a future year, and create budget register details for the amounts in the associated general ledger accounts.</span></span> <span data-ttu-id="f651e-106">शेष राशियों को आगे स्थानांतरित करने से पहले, शेष बजट राशियों की समीक्षा और विश्लेषण करें.</span><span class="sxs-lookup"><span data-stu-id="f651e-106">Before you carry forward the remaining amounts, review and analyze the remaining budget amounts.</span></span>

## <a name="review-and-analyze-remaining-budget-amounts"></a><span data-ttu-id="f651e-107">शेष बजट राशियों की समीक्षा और विश्लेषण करें</span><span class="sxs-lookup"><span data-stu-id="f651e-107">Review and analyze remaining budget amounts</span></span>

<span data-ttu-id="f651e-108">परियोजनाओं के लिए वर्ष की समाप्ति पर बजट राशियों की समीक्षा करने के लिए निम्नलिखित चरण पूरे करें, लेकिन राशियों को आगे स्थानांतरित न करें.</span><span class="sxs-lookup"><span data-stu-id="f651e-108">Complete the following steps to review the year-end budget amounts for projects, but not carry the amounts forward.</span></span>

1. <span data-ttu-id="f651e-109">**परियोजना प्रबंधन और लेखा** > **आवधिक** >  **बजट** > **बजट स्थानांतरित करें** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="f651e-109">Go to **Project management and accounting** > **Periodic** > **Budgets** > **Carry forward budgets**.</span></span> 
2. <span data-ttu-id="f651e-110">**प्रोजेक्ट बजट को आगे स्थानांतरित करने की प्रक्रिया** \* पृष्ठ में, **वर्ष समाप्ति विकल्प** टैब पर, सत्यापित करें कि **शेष परियोजना बजट राशियों को आगे स्थानांतरित करें** सक्रिय नहीं है.</span><span class="sxs-lookup"><span data-stu-id="f651e-110">On the **Project budget carry-forward process** page, on the **Year-end options** tab, verify that **Carry forward remaining project budget amounts** is not enabled.</span></span>
3. <span data-ttu-id="f651e-111">**मापदंड** टैब पर, **परियोजना बजट वर्ष** फ़ील्ड में, वह वित्तीय वर्ष चुनें जिसकी आप शेष बजट राशि देखना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="f651e-111">On the **Parameters** tab, in the **Project budget year** field, select the fiscal year for which you want to view the remaining budget amount.</span></span> 
4. <span data-ttu-id="f651e-112">**वित्तीय वर्ष प्रारंभ** फ़ील्ड में, वह वित्तीय वर्ष चुनें जिसकी आप शेष बजट राशि देखना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="f651e-112">In the **Opening fiscal year** field, select the fiscal year for which you want to view the remaining budget amount.</span></span> 
5. <span data-ttu-id="f651e-113">**पूर्वानुमान मॉडल से** फ़ील्ड में, **शेष बजट** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f651e-113">In the **From forecast model** field, select **Remaining budget**.</span></span> 
6. <span data-ttu-id="f651e-114">उन परियोजनाओं को शामिल करने के लिए जो आपके चुनें गए मानदंडों को पूरा करती हैं और जिनमे कोई शेष बजट नहीं है, **शेष शून्य दिखाएं** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f651e-114">To include projects that meet your selected criteria and have no remaining budget, select **Show zero remaining**.</span></span>  
7. <span data-ttu-id="f651e-115">**बजट चुनें** टैब पर, अपने चुनें गए मानदंडों से मेल खाने वाले सभी बजट लोड करने के लिए **सभी बजट पुन: प्राप्‍त करें** चुनें, और फिर **प्रक्रिया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f651e-115">On the **Select Budgets** tab, select **Retrieve all budgets** to load all budgets that match your selected criteria, and then select **Process**.</span></span> 
8. <span data-ttu-id="f651e-116">डेटाबेस में विशिष्ट सेट लोड करने वाली डेटाबेस क्वेरी को डिज़ाइन करने के लिए, **चुने गए बजट को पुन: प्राप्‍त करें**.</span><span class="sxs-lookup"><span data-stu-id="f651e-116">To design a database query that loads a specific set of budgets into the pane, select **Retrieve selected budgets**.</span></span>

<span data-ttu-id="f651e-117">फलक में किसी विशिष्ट पंक्ति के बारे में अधिक जानकारी के लिए, लाइन चुनें, और फिर **बजट विवरण देखें** या **खाता देखें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f651e-117">For more information about a specific line in the pane, select the line, and then select **View budget details** or **View accounts**.</span></span>

## <a name="carry-forward-remaining-budget-amounts"></a><span data-ttu-id="f651e-118">शेष बजट राशियां स्थानांतरित करें</span><span class="sxs-lookup"><span data-stu-id="f651e-118">Carry forward remaining budget amounts</span></span> 

<span data-ttu-id="f651e-119">जब आप शेष बजट राशि संसाधित करते हैं, तो आप स्थानांतरित की गई राशि के लिए प्रधान खाता-बही में लेन-देन बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="f651e-119">When you process remaining budget amounts, you can create transactions in the general ledger for the amounts that you are carrying forward.</span></span> <span data-ttu-id="f651e-120">सामान्य खाता बही लेनदेन बनाने के लिए, अनुभाग [बजट राशि स्थानांतरित करें और प्रधान खाता-बही लेन-देन बनाएं](#carry-forward) में दिए गए चरणों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="f651e-120">To create general ledger transactions, complete the steps in the section, [Carry forward budget amounts and create general ledger transactions](#carry-forward).</span></span> 

> [!NOTE]
> <span data-ttu-id="f651e-121">बजट राशियां जो पूर्वानुमान मॉडल में आगे स्थानांतरित की गई हैं जिनको आगे स्थानांतरित पूर्वानुमान मॉडल के रूप में **पूर्वानुमान मॉडल** पृष्ठ में चुना गया है.</span><span class="sxs-lookup"><span data-stu-id="f651e-121">Budget amounts that are carried forward are transferred to the forecast model that is selected in the **Forecast models** page as the carry-forward forecast model.</span></span>  

## <a name="carry-forward-budget-amounts-and-create-general-ledger-transactions"></a><a name="carry-forward"></a><span data-ttu-id="f651e-122">बजट राशियां आगे स्थानांतरित करें और प्रधान खाता-बही लेन-देन बनाएं</span><span class="sxs-lookup"><span data-stu-id="f651e-122">Carry forward budget amounts and create general ledger transactions</span></span>

1.  <span data-ttu-id="f651e-123">**परियोजना प्रबंधन और लेखा** > **आवधिक** > **बजट** > **बजट आगे स्थानांतरित करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f651e-123">Select **Project management and accounting** > **Periodic** > **Budgets** > **Carry forward budgets**.</span></span> 
2. <span data-ttu-id="f651e-124">**परियोजना प्रबंधन आगे स्थानांतरित करने की प्रक्रिया** पेज पर **समाप्ति वर्ष** चुनें और फिर **शेष बजट राशियों को आगे स्थानांतरित करें** और **प्रधान खाता-बही में बजट खाता प्रविष्टियां बनाएं** को सक्रिय करें.</span><span class="sxs-lookup"><span data-stu-id="f651e-124">On the **Project budget carry-forward process** page, select **Year-end** , and then enable **Carry forward remaining project budget amounts** and **Create budget register entries in general ledger**.</span></span> 
3. <span data-ttu-id="f651e-125">**मापदंड** टैब पर, **परियोजना मापदंड** फ़ील्ड समूह में, निम्न को चुनें:</span><span class="sxs-lookup"><span data-stu-id="f651e-125">On the **Parameters** tab, in the **Project parameters** field group, select the following:</span></span>

   - <span data-ttu-id="f651e-126">**परियोजना बजट वर्ष** : उस वित्तीय वर्ष की शुरुआत चुनें जिसकी आप शेष बजट राशियां देखना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="f651e-126">**Project budget year** : Select the beginning of the fiscal year for which you want to view the remaining budget amounts.</span></span> 
   - <span data-ttu-id="f651e-127">**लाभ और हानि** : प्रधान खाता-बही में लाभ और हानि लेन-देन बनाएं.</span><span class="sxs-lookup"><span data-stu-id="f651e-127">**Profit and loss** : Create profit and loss transactions in the general ledger.</span></span> 
   -  <span data-ttu-id="f651e-128">**WIP** : प्रधान खाता-बही में कार्य प्रगति पर (WIP) लेन-देन बनाएं.</span><span class="sxs-lookup"><span data-stu-id="f651e-128">**WIP** : Create Work in Progress (WIP) transactions in the general ledger.</span></span>
   -  <span data-ttu-id="f651e-129">**पेरोल** : प्रधान खाता-बही में पेरोल आवंटन लेन-देन बनाएं.</span><span class="sxs-lookup"><span data-stu-id="f651e-129">**Payroll** : Create payroll allocation transactions in the general ledger.</span></span> 

5. <span data-ttu-id="f651e-130">**सामान्य बहीखाता** फ़ील्ड समूह में, निम्न जानकारी प्रदान करें:</span><span class="sxs-lookup"><span data-stu-id="f651e-130">In the **General ledger** field group, provide the following information:</span></span> 

   - <span data-ttu-id="f651e-131">**वित्तीय वर्ष प्रारंभ** फ़ील्ड में, वह वित्तीय वर्ष चुनें जिसमें आप परियोजनाओं के लिए शेष बजट राशियों को स्थानांतरित करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="f651e-131">In the **Opening fiscal year** field, select the fiscal year that you want to transfer remaining budget amounts to for the projects.</span></span> <span data-ttu-id="f651e-132">**परियोजना बजट वर्ष** फ़ील्ड में मान के एक वर्ष बाद डिफ़ॉल्ट मान है.</span><span class="sxs-lookup"><span data-stu-id="f651e-132">The default value is one year after the value in the **Project budget year** field.</span></span>
   -  <span data-ttu-id="f651e-133">**आगे स्थानांतरित अवधि** फ़ील्ड में, वह अवधि चुनें जिसको आप प्रधान खाता-बही में बजट लेखा विवरण बनाना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="f651e-133">In the **Carry-forward period** field, select the period that you want to create the budget register details for in the general ledger.</span></span> <span data-ttu-id="f651e-134">यह आमतौर पर शुरुआती वित्तीय वर्ष में पहली अवधि होती है.</span><span class="sxs-lookup"><span data-stu-id="f651e-134">This is typically the first period in the opening fiscal year.</span></span>

6. <span data-ttu-id="f651e-135">**से /में कॉपी करें** फ़ील्ड समूह में, निम्नांकित जानकारी दें:</span><span class="sxs-lookup"><span data-stu-id="f651e-135">In the **Copy from/to** field group, provide the following information:</span></span>

   - <span data-ttu-id="f651e-136">**पूर्वानुमान मॉडल से** फ़ील्ड में, वह परियोजना बजट पूर्वानुमान मॉडल चुनें, जो उन शेष बजट राशियों से जुड़े हैं, जिनको आप परियोजना के लिए स्थानांतरित करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="f651e-136">In the **From forecast model** field, select the project budget forecast model associated with the remaining budget amounts you want to transfer for the projects.</span></span> 
   - <span data-ttu-id="f651e-137">**खाता-बही बजट मॉडल में** फ़ील्ड में, प्रधान खाता-बही में स्थानांतरित करने के लिए इच्छित बजट राशि से संबंधित खाता बजट मॉडल चुनें.</span><span class="sxs-lookup"><span data-stu-id="f651e-137">In the **To ledger budget model** field, select the ledger budget model associated with the budget amounts you want to transfer to the general ledger.</span></span> 
   -  <span data-ttu-id="f651e-138">परियोजना के लिए बजट राशियों को स्थानांतरित करते समय बनाए जाने वाले प्रधान खाता-बही के लिए परियोजना की बिक्री मुद्रा को इस्तेमाल करने के लिए **बिक्री मुद्रा स्थानांतरित करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f651e-138">Select **Transfer sales currency** to use the project's sales currency for the general ledger transactions that are created when you transfer the budget amounts for the projects.</span></span> <span data-ttu-id="f651e-139">जब विकल्प को नहीं चुना जाता है, तो लेन-देन लेखांकन मुद्रा इस्तेमाल करते हैं.</span><span class="sxs-lookup"><span data-stu-id="f651e-139">When the option is not selected, the transactions use the accounting currency.</span></span> 
   -  <span data-ttu-id="f651e-140">उन परियोजनाओं को शामिल करने के लिए जिनमें बजट की शेष राशि नहीं है **शेष शून्य दिखाएं** चुनें लेकिन अन्य मानदंड पूरे करें, जिनको आप नीचे फलक में प्रदर्शित परियोजनाओं में चुनते हैं.</span><span class="sxs-lookup"><span data-stu-id="f651e-140">Select **Show zero remaining** to include projects that have no remaining budget amounts, but meet the other criteria that you select in the projects displayed in the bottom pane.</span></span>

7. <span data-ttu-id="f651e-141">**बजट चुनें** टैब पर, उन सभी बजटों को लोड करने के लिए **सभी बजटों चुनें** जो आपके चुने गए मानदंड से मेल खाते हैं.</span><span class="sxs-lookup"><span data-stu-id="f651e-141">On the **Select Budgets** tab, select **Retrieve all budgets** to load all budgets that match the criteria you selected.</span></span> <span data-ttu-id="f651e-142">अगर आप ऐसी डेटाबेस क्वेरी डिज़ाइन करना चाहते हैं जो परियोजना बजट के विशिष्ट सेट को फलक में लोड करती है, तो **चुने गए बजट को पुन प्राप्त करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f651e-142">If you prefer to design a database query that loads a specific set of project budgets into the pane, select **Retrieve selected budgets**.</span></span>
8. <span data-ttu-id="f651e-143">प्रत्येक उस परियोजना के लिए जिसे आप संसाधित करना चाहते हैं, परियोजना के लिए लाइन की शुरुआत में विकल्प चुनें.</span><span class="sxs-lookup"><span data-stu-id="f651e-143">For each project that you want to process, select the option at the beginning of the line for the project.</span></span>

    > [!TIP]
    > <span data-ttu-id="f651e-144">सभी या अधिकांश परियोजनाओं को चुनने के लिए, ऊपरी ऊपरी-बायें कोने में चेक मार्क चुनें.</span><span class="sxs-lookup"><span data-stu-id="f651e-144">To select all or most of the projects, select the check mark in the top upper-left corner.</span></span> <span data-ttu-id="f651e-145">किसी परियोजना को संसाधित करने के लिए, उस परियाजना के लिए चेक मार्क को हटाएं.</span><span class="sxs-lookup"><span data-stu-id="f651e-145">To exclude processing any project, clear the check mark for that project.</span></span>

9. <span data-ttu-id="f651e-146">चुनी गयी परियोजनाओं के लिए शेष बजट राशि को चुने गए वित्तीय वर्ष में स्थानांतरित करने और प्रधान खाता-बही में बजट लेखा विवरण बनाने के लिए, **संसाधित करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f651e-146">To transfer the remaining budget amounts for the selected projects to the selected fiscal year and create budget register details in the general ledger, select **Process**.</span></span>

## <a name="carry-forward-budget-amounts-without-creating-general-ledger-transactions"></a><span data-ttu-id="f651e-147">प्रधान खाता-बही लेन-देन बनाए बिना बजट की राशियों को आगे स्थानांतरित करें</span><span class="sxs-lookup"><span data-stu-id="f651e-147">Carry forward budget amounts without creating general ledger transactions</span></span>

1. <span data-ttu-id="f651e-148">**परियोजना प्रबंधन और लेखा** > **आवधिक** >  **बजट** > **बजट स्थानांतरित करें** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="f651e-148">Go to **Project management and accounting** > **Periodic** > **Budgets** > **Carry forward budgets**.</span></span>
2. <span data-ttu-id="f651e-149">**परियोजना बजट आगे स्थानांतरित करें प्रक्रिया** पेज पर, **समाप्ति वर्ष विकल्प** फील्ड में, **शेष परियोजना बजट राशियों को आगे स्थानांतरित करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f651e-149">On the **Project budget carry-forward process** page, in the **Year-end options** field, select **Carry forward remaining project budget amounts**.</span></span>
3. <span data-ttu-id="f651e-150">**मापदंड** समूह में, **परियोजना बजट वर्ष** फ़ील्ड में, वह वित्तीय वर्ष चुनें जिसके लिए आप शेष बजट राशियां देखना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="f651e-150">In the **Parameters** group, in the **Project budget year** field, select the fiscal year for which you want to view the remaining budget amounts.</span></span>
4. <span data-ttu-id="f651e-151">**से/ में कॉपी करें** समूह में, निम्नांकित जानकारी दें:</span><span class="sxs-lookup"><span data-stu-id="f651e-151">In the **Copy from/to** group, provide the following information:</span></span>

   - <span data-ttu-id="f651e-152">**पूर्वानुमान मॉडल से** फ़ील्ड में, वह परियोजना बजट पूर्वानुमान मॉडल चुनें जो शेष बजट राशियों से जुड़ा है और जिसको आप परियोजनाओं के लिए स्थानांतरित करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="f651e-152">In the **From forecast model** field, select the project budget forecast model that is associated with the remaining budget amounts that you want to transfer for the projects.</span></span> 
   - <span data-ttu-id="f651e-153">उन परियोजनाओं को शामिल करने के लिए **शेष शून्य दिखाएं** चुनें, जिनकी कोई शेष बजट राशियां नहीं है, लेकिन जो आपके चुने गए अन्य मानदंडों को पूरा करती हैं.</span><span class="sxs-lookup"><span data-stu-id="f651e-153">Select **Show zero remaining** to include projects that have no remaining budget amounts, but that meet the other criteria you selected.</span></span>
   - <span data-ttu-id="f651e-154">**बजट चुनें** समूह में, उन सभी बजटों को लोड करने के लिए **सभी बजटों चुनें** जो आपके चुने गए मानदंडों से मेल खाते हैं.</span><span class="sxs-lookup"><span data-stu-id="f651e-154">In the **Select Budgets** group, select **Retrieve all budgets** to load all budgets that match the criteria that you selected.</span></span> <span data-ttu-id="f651e-155">फलक में परियोजना बजट के विशेष सेट को लोड करने वाली डेटाबेस क्वेरी को डिज़ाइन करने के लिए **चुने गए बजट पुन: प्राप्त करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f651e-155">To design a database query that loads a specific set of project budgets into the pane, select **Retrieve selected budgets**.</span></span>

5. <span data-ttu-id="f651e-156">प्रत्येक उस परियोजना के लिए जिसे आप संसाधित करना चाहते हैं, परियोजना के लिए लाइन की शुरुआत में विकल्प चुनें.</span><span class="sxs-lookup"><span data-stu-id="f651e-156">For each project that you want to process, select the option at the beginning of the line for the project.</span></span> 
6. <span data-ttu-id="f651e-157">चुनी गयी परियोजनाओं के लिए शेष बजट राशियों को चुने गए वित्तीय वर्ष में स्थानांतरित करने के लिए **संसाधित करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f651e-157">Select **Process** to transfer the remaining budget amounts for the selected projects to the selected fiscal year.</span></span>

