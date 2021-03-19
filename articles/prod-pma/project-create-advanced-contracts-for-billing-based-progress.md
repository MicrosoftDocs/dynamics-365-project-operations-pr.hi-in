---
title: प्रगति के आधार पर बिलिंग के लिए उन्नत अनुबंध बनाएं
description: यह विषय बताता है कि परियोजना अनुबंध कैसे बनाया जाए ताकि आप ग्राहकों के लिए पूर्ण कार्य के प्रतिशत के आधार पर इनवॉइस उत्पन्न कर सकें.
author: RadhikaRS
manager: AnnBe
ms.date: 03/26/2020
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
ms.openlocfilehash: b1de330df8cf85ed30c0ee4e4f2f2fe74d05dbff
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289506"
---
# <a name="create-advanced-contracts-for-billing-based-on-progress"></a><span data-ttu-id="3f50c-103">प्रगति के आधार पर बिलिंग के लिए उन्नत अनुबंध बनाएं</span><span class="sxs-lookup"><span data-stu-id="3f50c-103">Create advanced contracts for billing based on progress</span></span>
[!include [banner](../includes/banner.md)]

<span data-ttu-id="3f50c-104">यह विषय बताता है कि परियोजना अनुबंध कैसे बनाएं ताकि आप ग्राहकों के लिए पूर्ण कार्य के प्रतिशत के आधार पर इनवॉइस बना सकें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-104">This topic explains how to create project contracts so that you can create invoices for customers, based on a percentage of completed work.</span></span> <span data-ttu-id="3f50c-105">इनवॉइस राशि की गणना स्वचालित रूप से उस परियोजना की बजट श्रेणियों के लिए की जाती है, जिसे आप किसी परियोजना के लिए सेट करते हैं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-105">Invoice amounts are automatically calculated for the budget categories of work that you set up for a project.</span></span> <span data-ttu-id="3f50c-106">जब आप ग्राहक के साथ परियोजना अनुबंध पर बातचीत करते हैं, तो इनवॉइस समय सेट होता है.</span><span class="sxs-lookup"><span data-stu-id="3f50c-106">The invoice timing is set when you negotiate the project contract with the customer.</span></span>

<span data-ttu-id="3f50c-107">इस विषय में प्रक्रियाओं का इस्तेमाल अनुबंध, संबद्ध परियोजना, और बिलिंग नियमों को सेट करने के लिए करें जो आपके द्वारा परियोजना के लिए निर्धारित किए गए कार्य की बजट श्रेणियों के लिए इनवॉइस राशि की गणना करते हैं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-107">Use the procedures in this topic to set up a contract, an associated project, and the billing rules that calculate invoice amounts for the budget categories of work that you set up for the project.</span></span>

<span data-ttu-id="3f50c-108">आपके अनुबंध और परियोजना बनाने के बाद, आप परियोजना का विवरण सेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-108">After you've created the contract and the project, you can set up the details of the project.</span></span> <span data-ttu-id="3f50c-109">उदाहरण के लिए, आप गतिविधियों को स्पष्ट कर सकते हैं और श्रमिकों को परियोजना सौंप सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-109">For example, you can define activities and assign workers to the project.</span></span>

## <a name="example"></a><span data-ttu-id="3f50c-110">उदाहरण</span><span class="sxs-lookup"><span data-stu-id="3f50c-110">Example</span></span>

<span data-ttu-id="3f50c-111">आपका संगठन सॉफ्टवेयर डेवलपमेंट फ़र्म है.</span><span class="sxs-lookup"><span data-stu-id="3f50c-111">Your organization is a software development firm.</span></span> <span data-ttu-id="3f50c-112">आप 20,000 US डॉलर (USD) के कुल शुल्क के लिए ग्राहक के लिए पेरोल लेखांकन पैकेज विकसित करने के लिए सहमत हैं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-112">You agree to develop a payroll accounting package for a customer for a total fee of 20,000 US dollars (USD).</span></span> <span data-ttu-id="3f50c-113">जब आप परियोजना के विशिष्ट प्रतिशत को पूरा करते हैं, तो आपका संगठन ग्राहक को इनवॉइस करने के लिए सहमत होता है.</span><span class="sxs-lookup"><span data-stu-id="3f50c-113">Your organization agrees to invoice the customer as you complete specific percentages of the project.</span></span> <span data-ttu-id="3f50c-114">आप कार्य के लिए निम्नांकित परियोजना श्रेणियां सेट करते हैं, ताकि आप उन्हें बिलिंग प्रक्रिया में इस्तेमाल कर सकें:</span><span class="sxs-lookup"><span data-stu-id="3f50c-114">You set up the following project categories for the work, so that you can use them in the billing process:</span></span>

- <span data-ttu-id="3f50c-115">परामर्शी</span><span class="sxs-lookup"><span data-stu-id="3f50c-115">Consulting</span></span>
- <span data-ttu-id="3f50c-116">डिज़ाइन</span><span class="sxs-lookup"><span data-stu-id="3f50c-116">Design</span></span>
- <span data-ttu-id="3f50c-117">स्थापना</span><span class="sxs-lookup"><span data-stu-id="3f50c-117">Installation</span></span>

<span data-ttu-id="3f50c-118">आप बिलिंग नियम भी सेट करते हैं, जो प्रत्येक श्रेणी में पूरा होने वाले परियोजना कार्य के प्रतिशत के लिए स्वचालित रूप से इनवॉइस राशि की गणना करता है.</span><span class="sxs-lookup"><span data-stu-id="3f50c-118">You also set up billing rules that automatically calculate the invoice amounts for the percentage of project work that is completed in each category.</span></span>

<span data-ttu-id="3f50c-119">बजट प्रबंधक परियोजना श्रेणियों के लिए बजट बनाता है.</span><span class="sxs-lookup"><span data-stu-id="3f50c-119">The budget manager creates a budget for the project categories.</span></span> <span data-ttu-id="3f50c-120">पूर्ण कार्य की राशि की गणना स्वचालित रूप से बजटीय राशियों की तुलना में वास्तविक कार्य के प्रतिशत के रूप में की जाती है.</span><span class="sxs-lookup"><span data-stu-id="3f50c-120">The amount of completed work is automatically calculated as a percentage of actual work in comparison to the budgeted amounts.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f50c-121">पूर्वावश्यकताएँ</span><span class="sxs-lookup"><span data-stu-id="3f50c-121">Prerequisites</span></span>

<span data-ttu-id="3f50c-122">इससे पहले कि आप परियोजना बनाएं जो बिलिंग नियमों का उपयोग करती है, आपको बिलिंग नियमों के लिए संख्या अनुक्रम और शुल्क रोज़नामचा सेट करना होगा जो प्रगति बिलिंग दर्ज करने के लिए इस्तेमाल होता है.</span><span class="sxs-lookup"><span data-stu-id="3f50c-122">Before you create a project that uses billing rules, you must set up the number sequences for billing rules and a fee journal that is used to post progress billings.</span></span>

1. <span data-ttu-id="3f50c-123">**परियोजना प्रबंधन और लेखांकन** \> **सेट अप** \> **परियोजना प्रबंधन और लेखांकन मानकों** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-123">Go to **Project management and accounting** \> **Setup** \> **Project management and accounting parameters**.</span></span>
2. <span data-ttu-id="3f50c-124">**परियोजना प्रबंधन और लेखांकन मापदंड** पृष्ठ पर, **संख्या अनुक्रम** टैब पर, संख्या अनुक्रम सेट करें जिसे आप बिलिंग नियम बनाते समय इस्तेमाल करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-124">On the **Project management and accounting parameters** page, on the **Number sequences** tab, set up the number sequence that you want to use when billing rules are created.</span></span>
3. <span data-ttu-id="3f50c-125">**परियोजना प्रबंधन और लेखांकन** \> **रोज़नामचा** \> **शुल्क** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-125">Go to **Project management and accounting** \> **Journals** \> **Fee**.</span></span>
4. <span data-ttu-id="3f50c-126">**शुल्क रोज़नामचा** पृष्ठ पर, **नया** चुनें, और रोज़नामचा का नाम दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-126">On the **Fee journal** page, select **New**, and enter the journal name.</span></span>

## <a name="create-a-contract-for-progress-billings"></a><span data-ttu-id="3f50c-127">प्रगति बिलिंग के लिए अनुबंध बनाएं</span><span class="sxs-lookup"><span data-stu-id="3f50c-127">Create a contract for progress billings</span></span>

<span data-ttu-id="3f50c-128">निश्चित मूल्य परियोजना के लिए परियोजना अनुबंध बनाने के लिए इस प्रक्रिया को इस्तेमाल करें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-128">Use this procedure to create a project contract for a fixed-price project.</span></span> <span data-ttu-id="3f50c-129">आप परियोजना इनवॉइस तब बनाते हैं, जब परियोजना पर पूरा किया गया कार्य निर्दिष्ट प्रतिशत तक पहुंच जाता है.</span><span class="sxs-lookup"><span data-stu-id="3f50c-129">You create a project invoice when the work that is completed on the project reaches a specified percentage.</span></span>

1. <span data-ttu-id="3f50c-130">**परियोजना प्रबंधन और लेखांकन** \> **परियोजना** \> **परियोजना अनुबंध** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-130">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="3f50c-131">**परियोजना अनुबंध** पृष्ठ पर, **नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-131">On the **Project contracts** page, select **New**.</span></span>
3. <span data-ttu-id="3f50c-132">**नया परियोजना अनुबंध** संवाद बॉक्स में, निम्नांकित फ़ील्ड सेट करें:</span><span class="sxs-lookup"><span data-stu-id="3f50c-132">In the **New project contract** dialog box, set the following fields:</span></span>

    - <span data-ttu-id="3f50c-133">**नाम**</span><span class="sxs-lookup"><span data-stu-id="3f50c-133">**Name**</span></span>
    - <span data-ttu-id="3f50c-134">**निधीयन प्रकार**</span><span class="sxs-lookup"><span data-stu-id="3f50c-134">**Funding type**</span></span>
    - <span data-ttu-id="3f50c-135">**वित्तपोषण का स्रोत**</span><span class="sxs-lookup"><span data-stu-id="3f50c-135">**Funding source**</span></span>
    - <span data-ttu-id="3f50c-136">**बिक्री मुद्रा** - डिफ़ॉल्ट रूप से, इस मुद्रा का इस्तेमाल उन ग्राहक इनवॉइस के लिए किया जाता है, जो परियोजना अनुबंध से जुड़ी होती हैं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-136">**Sales currency** – By default, this currency is used for customer invoices that are associated with the project contract.</span></span> <span data-ttu-id="3f50c-137">हालांकि, आप किसी विशिष्ट ग्राहक इनवॉइस पर बिक्री मुद्रा बदल सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-137">However, you can change the sales currency on a specific customer invoice.</span></span>

4. <span data-ttu-id="3f50c-138">**ठीक** चुनें।</span><span class="sxs-lookup"><span data-stu-id="3f50c-138">Select **OK**.</span></span> <span data-ttu-id="3f50c-139">जानकारी को **परियोजना अनुबंध** पृष्ठ के हेडर में कॉपी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="3f50c-139">The information is copied to the header of the **Project contracts** page.</span></span>
5. <span data-ttu-id="3f50c-140">**परियोजना अनुबंध** पृष्ठ पर, परियोजना के लिए आवश्यक जानकारी का शेष भाग भरें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-140">On the **Project contracts** page, fill in the rest of the required information for the project.</span></span>

## <a name="create-a-project-for-progress-billings"></a><span data-ttu-id="3f50c-141">प्रगति बिलिंग के लिए परियोजना बनाएं</span><span class="sxs-lookup"><span data-stu-id="3f50c-141">Create a project for progress billings</span></span>

<span data-ttu-id="3f50c-142">परियोजना और परियोजना अनुबंध के साथ जुड़ी किसी भी उपपरियोजना को बनाने के लिए इन चरणों का पालन करें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-142">Follow these steps to create a project and any subprojects that are associated with a project contract.</span></span>

1. <span data-ttu-id="3f50c-143">**परियोजना प्रबंधन और खाता** \> **परियोजना** \> **सभी परियोजना** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-143">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="3f50c-144">**सभी परियोजनाओं** पृष्ठ पर, **नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-144">On the **All projects** page, select **New**.</span></span>
3. <span data-ttu-id="3f50c-145">**नई परियोजना** संवाद बॉक्स में, **परियोजना प्रकार** फ़ील्ड में, **समय और सामग्री** चुनें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-145">In the **New project** dialog box, in the **Project type** field, select **Time and material**.</span></span>
4. <span data-ttu-id="3f50c-146">परियोजना समूह चुनें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-146">Select a project group.</span></span> <span data-ttu-id="3f50c-147">परियोजना समूह उन परियोजनाओं के लिए दर्ज जानकारी को स्पष्ट करता है, जिन्हें समूह को सौंपा गया है.</span><span class="sxs-lookup"><span data-stu-id="3f50c-147">A project group defines the posting information for the projects that are assigned to the group.</span></span>
5. <span data-ttu-id="3f50c-148">**परियोजना बनाएँ** चुनें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-148">Select **Create project**.</span></span>
6. <span data-ttu-id="3f50c-149">परियोजना बनने के बाद परियोजना चरण को **संसाधित किया जा रहा है** पर सेट करें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-149">After the project is created, set the project stage to **In process**.</span></span>

## <a name="create-a-budget-for-a-project"></a><span data-ttu-id="3f50c-150">परियोजना के लिए बजट बनाएं</span><span class="sxs-lookup"><span data-stu-id="3f50c-150">Create a budget for a project</span></span>

<span data-ttu-id="3f50c-151">बजट श्रेणियों का उपयोग प्रत्येक श्रेणी के लिए काम के प्रतिशत के लिए इनवॉइस राशि की गणना करने के लिए स्वचालित रूप से किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="3f50c-151">Budget categories are used to automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="3f50c-152">अनुमानित लागतों के लिए बजट श्रेणियां बनाने के लिए इन चरणों का पालन करें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-152">Follow these steps to create budget categories for the estimated costs.</span></span>

1. <span data-ttu-id="3f50c-153">**परियोजना प्रबंधन और खाता** \> **परियोजना** \> **सभी परियोजना** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-153">Go to **Project management and accounting** \> **Projects** \> **All projects**.</span></span>
2. <span data-ttu-id="3f50c-154">**सभी परियोजना** पृष्ठ पर, उस परियोजना को चुनें और खोलें, जिसे आप चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-154">On the **All projects** page, select and open the project that you want.</span></span>
3. <span data-ttu-id="3f50c-155">**परियोजना** पृष्ठ पर, प्रक्रिया फलक पर, **योजना** टैब पर, **बजट** समूह में, **परियोजना बजट** चुनें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-155">On the **Projects** page, on the Action Pane, on the **Plan** tab, in the **Budget** group, select **Project budget**.</span></span>
4. <span data-ttu-id="3f50c-156">**परियोजना बजट** पृष्ठ पर, परियोजना में प्रत्येक श्रेणी के लिए अनुमानित लागत दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-156">On the **Project budget** page, enter an estimated cost for each category in the project.</span></span>

## <a name="create-billing-rules-for-progress-billings"></a><span data-ttu-id="3f50c-157">प्रगति बिलिंग के लिए बिलिंग नियम बनाएं</span><span class="sxs-lookup"><span data-stu-id="3f50c-157">Create billing rules for progress billings</span></span>

1. <span data-ttu-id="3f50c-158">**परियोजना प्रबंधन और लेखांकन** \> **परियोजना** \> **परियोजना अनुबंध** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-158">Go to **Project management and accounting** \> **Projects** \> **Project contracts**.</span></span>
2. <span data-ttu-id="3f50c-159">**परियोजना अनुबंध** पृष्ठ पर, परियोजना अनुबंध चुनें और खोलें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-159">On the **Project contracts** page, select and open a project contract.</span></span>
3. <span data-ttu-id="3f50c-160">परियोजना अनुबंध पृष्ठ पर, **बिलिंग नियम** FastTab पर, **जोड़ें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-160">On the project contract page, on the **Billing rules** FastTab, select **Add**.</span></span>
4. <span data-ttu-id="3f50c-161">**बिलिंग नियम** पृष्ठ पर, **पंक्ति प्रकार** फ़ील्ड में **प्रगति** चुनें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-161">On the **Billing rule** page, in the **Line type** field, select **Progress**.</span></span>
5. <span data-ttu-id="3f50c-162">**बिलिंग नियम पंक्ति विवरण** FastTab पर, **अनुबंध मान** फ़ील्ड में, अनुबंध का कुल मान दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-162">On the **Billing rule line details** FastTab, in the **Contract value** field, enter the total value of the contract.</span></span>
6. <span data-ttu-id="3f50c-163">**श्रेणी** फ़ील्ड में, शुल्क लेन-देन दर्ज करने के लिए श्रेणी चुनें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-163">In the **Category** field, select the category to post the fee transaction to.</span></span>
7. <span data-ttu-id="3f50c-164">**परियोजना** फ़ील्ड में, इस बिलिंग नियम को इस्तेमाल करने वाली परियोजना चुनें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-164">In the **Project** field, select the project that uses this billing rule.</span></span>
8. <span data-ttu-id="3f50c-165">वैकल्पिक: अतिरिक्त परियोजनाओं के लिए बिलिंग नियम निर्धारित करें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-165">Optional: Assign the billing rule to additional projects.</span></span> <span data-ttu-id="3f50c-166">**परियोजना** FastTab पर, **उपलब्ध परियोजना** अनुभाग में, परियोजना चुनें और फिर **चुनी गयी परियोजना** अनुभाग में परियोजना जोड़ने के लिए दायां एरो बटन चुनें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-166">On the **Project** FastTab, in the **Available projects** section, select a project, and then select the right arrow button to add the project to the **Selected projects** section.</span></span>
9. <span data-ttu-id="3f50c-167">वैकल्पिक: उस प्रतिशत राशि की गणना करता है, जिसे ग्राहक इनवॉइस का भुगतान करते समय रोकता है.</span><span class="sxs-lookup"><span data-stu-id="3f50c-167">Optional: Calculate the percentage amount that the customer withholds from payments on an invoice.</span></span> <span data-ttu-id="3f50c-168">**भुगतान अवधारण शर्तें** FastTab पर, धन स्रोत चुनें, और फिर, **अवधारण प्रतिशत** फ़ील्ड में, अवधारण प्रतिशत लिखें.</span><span class="sxs-lookup"><span data-stu-id="3f50c-168">On the **Payment retention terms** FastTab, select the funding source, and then, in the **Retention percentage** field, enter the retention percentage.</span></span>
10. <span data-ttu-id="3f50c-169">परियोजना अनुबंध के लिए अतिरिक्त बिलिंग नियम बनाने के लिए इन चरणों को दोहराएं.</span><span class="sxs-lookup"><span data-stu-id="3f50c-169">Repeat these steps to create additional billing rules for the project contract.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]