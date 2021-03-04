---
title: स्वीकृत समय और व्यय प्रविष्टियों द्वारा बनाए गए वास्तविक सुधार
description: यह विषय बताता है कि यदि बिलिंग पूरी नहीं होती है तो कोई व्यवस्थापक पहले स्वीकृत समय या व्यय प्रविष्टियों के लिए एकल या थोक सुधार कैसे कर सकता है.
author: rumant
manager: AnnBe
ms.date: 04/02/2020
ms.topic: article
ms.service: dynamics-ax-applications
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
search.app:
- ProjectOperations
ms.openlocfilehash: 063c4d017f5904f09c3c239bfa432a128872e4d7
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144955"
---
# <a name="bulk-corrections-of-actuals-created-by-approved-time-and-expense-entries"></a><span data-ttu-id="89d41-103">स्वीकृत समय और व्यय प्रविष्टियों द्वारा बनाए गए वास्तविक सुधार</span><span class="sxs-lookup"><span data-stu-id="89d41-103">Bulk corrections of actuals created by approved time and expense entries</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="89d41-104">कभी-कभी गलत तरीके से समय या व्यय प्रविष्टि दर्ज की जा सकती है.</span><span class="sxs-lookup"><span data-stu-id="89d41-104">Occasionally a time or expense entry may be entered incorrectly.</span></span> <span data-ttu-id="89d41-105">उदाहरण के लिए, एक सलाहकार कोई समय प्रविष्टि बनाते समय गलत दिनांक का चयन कर सकता है या वह एक व्यय दर्ज करते समय संख्याओं को स्थानांतरित कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="89d41-105">For example, a consultant might select the wrong date when creating a time entry or they might transpose the numbers when entering an expense.</span></span> <span data-ttu-id="89d41-106">यदि कोई सलाहकार सबमिट की गई प्रविष्टियों में अपडेट नहीं कर सकता है, तो एक व्यवस्थापक सीधे एक परियोजना के लिए प्रविष्टि को सही कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="89d41-106">If a consultant can’t make the updates to the submitted entries, an administrator can directly correct the entry for a project.</span></span>

<span data-ttu-id="89d41-107">इस विषय में कार्यविधियों को पूरा करने के लिए, आपको व्यवस्थापक की अनुमति की आवश्यकता होगी.</span><span class="sxs-lookup"><span data-stu-id="89d41-107">To complete the procedures in this topic, you will need Administrator permissions.</span></span>

## <a name="correct-approved-time-entries"></a><span data-ttu-id="89d41-108">स्वीकृत समय प्रविष्टियों को सही करें</span><span class="sxs-lookup"><span data-stu-id="89d41-108">Correct approved time entries</span></span>     

<span data-ttu-id="89d41-109">किसी परियोजना के लिए एकल या एकाधिक समय प्रविष्टियों को सही करने के लिए निम्न चरणों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-109">Complete the following steps to correct single or multiple time entries for a project.</span></span>

1. <span data-ttu-id="89d41-110">**विक्रय** क्षेत्र में, **लेन-देन** का चयन करें और फिर **स्वीकृत समय** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-110">In the **Sales** area, select **Transactions**, and then select **Approved Time**.</span></span> 

2. <span data-ttu-id="89d41-111">**स्वीकृत समय** सूची में, सही करने के लिए एक या अधिक स्वीकृत समय प्रविष्टियों का पता लगाएँ और उनका चयन करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-111">In the **Approved Time** list, locate and select one or more approved time entries to correct.</span></span> <span data-ttu-id="89d41-112">आप संबंधित प्रविष्टियों का पता लगाने के लिए फ़िल्टर का उपयोग कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="89d41-112">You can use the filter to locate related entries.</span></span> <span data-ttu-id="89d41-113">उदाहरण के लिए, आप किसी परियोजना ID पर फ़िल्टर कर सकते हैं, और उस परियोजना ID के साथ सभी स्वीकृत समय प्रविष्टियों का चयन कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="89d41-113">For example, you might filter on a Project ID, and select all approved time entries with that Project ID.</span></span>

3. <span data-ttu-id="89d41-114">**सही प्रविष्टियों** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-114">Select **Correct entries**.</span></span> <span data-ttu-id="89d41-115">एक नया सुधार जर्नल, असाइन किए गए प्रकार **समय का सुधार** के साथ स्वचालित रूप से बनाया गया है.</span><span class="sxs-lookup"><span data-stu-id="89d41-115">A new correction journal is automatically created, with the assigned type **Time correction**.</span></span> <span data-ttu-id="89d41-116">आपके द्वारा चुनी गई प्रविष्टियों को जर्नल में जोड़ा जाता है.</span><span class="sxs-lookup"><span data-stu-id="89d41-116">The entries you selected are added to the journal.</span></span> 

4. <span data-ttu-id="89d41-117">**नया जर्नल** पृष्ठ पर, अपने सुधार जर्नल के लिए कोई **वर्णन** दर्ज करें और फिर **समय प्रविष्टि सुधार** टैब का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-117">On the **New Journal** page, enter a **Description** for your correction journal, and then select the **Time Entry Corrections** tab.</span></span>  
5. <span data-ttu-id="89d41-118">**समय प्रविष्टियों के लिए नए मान** सेक्शन में, आवश्यकतानुसार सही जानकारी के साथ फ़ील्ड को अपडेट करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-118">In the **New Values for Time Entries** section, update the fields with the correct information as necessary.</span></span> <span data-ttu-id="89d41-119">उदाहरण के लिए, आप असाइन की गई परियोजना या बुक करने योग्य संसाधन को बदल सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="89d41-119">For example, you can change the assigned project or the bookable resource.</span></span>

6. <span data-ttu-id="89d41-120">**पूर्वावलोकन**.</span><span class="sxs-lookup"><span data-stu-id="89d41-120">Select **Preview**.</span></span> <span data-ttu-id="89d41-121">संवाद बॉक्स में **ठीक** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-121">In the dialog box, select **OK**.</span></span> <span data-ttu-id="89d41-122">**जर्नल पंक्तियों** टैब पर, आप मूल वास्तविक की एक सूची देख सकते हैं जो चयनित समय प्रविष्टियों से संबंधित हैं जिन्हें विपरीत किया गया है और बनाई गई सही पंक्तियों को सही किया गया है.</span><span class="sxs-lookup"><span data-stu-id="89d41-122">On the **Journal lines** tab, you can view a list of the original actuals that are related to the selected time entries that have been reversed and the corrected corresponding lines that have been created.</span></span> <span data-ttu-id="89d41-123">यदि अतिरिक्त सुधार किए जाने की आवश्यकता है, तो चरण 5 और 6 दोहराएँ.</span><span class="sxs-lookup"><span data-stu-id="89d41-123">If additional corrections need to be made, repeat steps 5 and 6.</span></span> 

> [!NOTE]
> <span data-ttu-id="89d41-124">सभी सही किए गए वास्तविक लोगों के पास वही मान होंगे जिन्हें आपने **समय प्रविष्टियों के लिए नए मान** सेक्शन में चयनित किया है.</span><span class="sxs-lookup"><span data-stu-id="89d41-124">All the corrected actuals will have the same values that you selected in the **New values for Time Entries** section.</span></span>

7. <span data-ttu-id="89d41-125">यदि अपेक्षा के अनुसार सुधार दिखाई देते हैं, तो **पुष्टि करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-125">If the corrections appear as expected, select **Confirm**.</span></span> <span data-ttu-id="89d41-126">संवाद बॉक्स में **ठीक** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-126">In the dialog box, select **OK**.</span></span>

8. <span data-ttu-id="89d41-127">**विक्रय** क्षेत्र में वापस जाएँ, **परियोजनाओं** का चयन करें और फिर उस परियोजना को खोलें जिसके लिए आपने अभी-अभी समय प्रविष्टियों को अपडेट किया है.</span><span class="sxs-lookup"><span data-stu-id="89d41-127">Return to the **Sales** area, select **Projects**, and then open the project for which you just updated the time entries.</span></span> 

9. <span data-ttu-id="89d41-128">**परियोजनाओं** पृष्ठ पर, **वास्तविक** टैब पर, आपके द्वारा किए गए परिवर्तनों को देखें.</span><span class="sxs-lookup"><span data-stu-id="89d41-128">On the **Projects** page, on the **Actuals** tab, view the changes that you made.</span></span> 

> [!NOTE]
> <span data-ttu-id="89d41-129">यदि **वास्तविक** टैब दिखाई नहीं देता है, तो **संबंधित** > **वास्तविक** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-129">If the **Actuals** tab is not visible, select **Related** > **Actuals**.</span></span>  

10. <span data-ttu-id="89d41-130">**वास्तविक संबद्ध दृश्य** सूची में, आप देख सकते हैं कि मूल समय प्रविष्टियाँ जो विपरीत हो गई हैं और वे अभी भी सूचीबद्ध हैं, जैसा कि संबंधित सही समय प्रविष्टियाँ हैं.</span><span class="sxs-lookup"><span data-stu-id="89d41-130">In the **Actual Associated View** list, you can see that the original time entries that have been reversed are still listed, as are the corresponding corrected time entries.</span></span> 

<span data-ttu-id="89d41-131">उदाहरण के लिए, निम्नलिखित ग्राफ़िक में, 8.00 की मात्रा के साथ दो पंक्ति वस्तुएँ होती हैं जिनके पास राशि कॉलम में सूचीबद्ध डेबिट होते हैं.</span><span class="sxs-lookup"><span data-stu-id="89d41-131">For example, in the following graphic, there are two line items with a quantity of 8.00 that have debits listed in the Amount column.</span></span> <span data-ttu-id="89d41-132">इसके अतिरिक्त, -8.00 की मात्रा के साथ दो पंक्ति वस्तुएँ हैं जो राशि कॉलम में जमा राशि दिखाती हैं.</span><span class="sxs-lookup"><span data-stu-id="89d41-132">Additionally, there are two line items with a quantity of -8.00 that show credited amounts in the Amount column.</span></span> <span data-ttu-id="89d41-133">ये सुधार मात्रा को शून्य तक लाते हैं.</span><span class="sxs-lookup"><span data-stu-id="89d41-133">These corrections bring the quantity to zero.</span></span>

![वास्तविक संबद्ध दृश्य सूची](https://github.com/MicrosoftDocs/dynamics-365-customer-engagement-pr/blob/bulk-corrections-actuals-created-by-approved-time-expense-entries.md/time-actuals.png)
 
## <a name="correct-approved-expense-entries"></a><span data-ttu-id="89d41-135">स्वीकृत व्यय प्रविष्टियों को सही करें</span><span class="sxs-lookup"><span data-stu-id="89d41-135">Correct approved expense entries</span></span>

<span data-ttu-id="89d41-136">एक या अधिक व्यय प्रविष्टियों को सही करने के लिए निम्नलिखित चरणों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-136">Complete the following steps to correct one or more expense entries.</span></span> 

1. <span data-ttu-id="89d41-137">**विक्रय** क्षेत्र में, बाएँ नेविगेशन फलक में, **लेन-देन** के अंतर्गत, **स्वीकृत व्यय** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-137">In the **Sales** area, in the left navigation pane, under **Transactions**, select **Approved Expenses**.</span></span>

2. <span data-ttu-id="89d41-138">**स्वीकृत व्यय** सूची में, उस परियोजना का चयन करें जिसे आप सही करना चाहते हैं और फिर **सही प्रविष्टियाँ** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-138">In the **Approved Expenses** list, select the project that you want to correct, and then select **Correct entries**.</span></span> <span data-ttu-id="89d41-139">एक नया सुधार जर्नल, असाइन किए गए **व्यय का सुधार** प्रकार के साथ स्वचालित रूप से बनाया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="89d41-139">A new correction journal will be created automatically with the assigned type of **Expense correction**.</span></span> 

3. <span data-ttu-id="89d41-140">**नए जर्नल** पृष्ठ पर, सुधार के लिए कोई **वर्णन** दर्ज करें और **व्यय सुधार** टैब पर **व्यय के नए मान** सेक्शन में, उन डेटा फ़ील्ड का चयन करें जिन्हें आप चयनित व्यय पंक्तियों के लिए सही करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="89d41-140">On the **New Journal** page, enter a **Description** for the correction, and on the **Expense Correction** tab, in the **New Values for Expenses** section, select the data fields that you want to correct for the selected expense lines.</span></span> <span data-ttu-id="89d41-141">उदाहरण के लिए, आप दूसरे **परियोजना** को व्यय असाइन कर सकते हैं, या **व्यय की श्रेणी**, **व्यय दिनांक** या **बुक करने योग्य संसाधन** सही कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="89d41-141">For example, you can assign the expense to another **Project**, or correct the **Expense Category**, **Expense Date**, or **Bookable Resource**.</span></span>

4. <span data-ttu-id="89d41-142">**पूर्वावलोकन**.</span><span class="sxs-lookup"><span data-stu-id="89d41-142">Select **Preview**.</span></span> <span data-ttu-id="89d41-143">संवाद बॉक्स में **ठीक** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-143">In the dialog box, select **OK**.</span></span> 

5. <span data-ttu-id="89d41-144">**जर्नल पंक्तियों** टैब पर सुधारों को सत्यापित करें. आप मूल वास्तविक की एक सूची देख सकते हैं जो चयनित व्यय प्रविष्टियों से संबंधित हैं जिन्हें विपरीत किया गया है और बनाई गई सही पंक्तियों को सही किया गया है.</span><span class="sxs-lookup"><span data-stu-id="89d41-144">Verify the corrections on the **Journal lines** tab. You can view a list of the original actuals that are related to the selected expense entries that have been reversed and the corrected corresponding lines that have been created.</span></span>

6. <span data-ttu-id="89d41-145">यदि सुधार किए गए मान अपेक्षा के अनुसार होते हैं, तो **पुष्टि करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-145">If the corrected values are as expected, select **Confirm**.</span></span> <span data-ttu-id="89d41-146">संवाद बॉक्स में, **ठीक** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-146">In the dialog box, select **OK.**</span></span> <span data-ttu-id="89d41-147">यदि मान अपेक्षा के अनुरूप नहीं दिखाई दे रहे हैं, तो **स्वीकृत व्यय** सूची पर वापस लौटने के लिए **रद्द करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-147">If the values are not showing as expected, select **Cancel** to return to the **Approved Expenses** list.</span></span> <span data-ttu-id="89d41-148">चरण 2 से 5 तक दोहराएँ.</span><span class="sxs-lookup"><span data-stu-id="89d41-148">Repeat steps 2 through 5.</span></span> 

> [!NOTE]
> <span data-ttu-id="89d41-149">सभी सही किए गए वास्तविक लोगों के पास वही मान होंगे जिन्हें आपने **व्यय के लिए नए मान** सेक्शन में चयनित किया है.</span><span class="sxs-lookup"><span data-stu-id="89d41-149">The corrected actuals will have the same values that you selected in the **New values for Expenses** section.</span></span>

7. <span data-ttu-id="89d41-150">आपके द्वारा सुधार जर्नल की पुष्टि करने के बाद, अपने परिवर्तनों को देखने के लिए उस परियोजना या परियोजनाओं पर वापस नेविगेट करें, जिसे आपके द्वारा अपडेट किया गया था.</span><span class="sxs-lookup"><span data-stu-id="89d41-150">After you confirm the correction journal, navigate back to the project or projects that you updated, to view your changes.</span></span>  

8. <span data-ttu-id="89d41-151">परियोजना पृष्ठ में, **वास्तविक** टैब पर, **वास्तविक संबद्ध दृश्य** की समीक्षा करें.</span><span class="sxs-lookup"><span data-stu-id="89d41-151">In the project page, on the **Actuals** tab, review the **Actual Associated View**.</span></span> <span data-ttu-id="89d41-152">मूल प्रविष्टियाँ और सही प्रविष्टियाँ सूचीबद्ध हैं.</span><span class="sxs-lookup"><span data-stu-id="89d41-152">The original entries and the corrected entries are listed.</span></span> <span data-ttu-id="89d41-153">निम्नलिखित ग्राफ़िक, मूल व्यय प्रविष्टि और संबंधित सही व्यय प्रविष्टि राशियाँ दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="89d41-153">The following graphic shows original expense entry amounts and the corresponding corrected expense entry amounts.</span></span> 

![Expense_actuals](https://user-images.githubusercontent.com/60806505/77122219-4cd52900-69fa-11ea-8349-ccd2ffebf640.png)
