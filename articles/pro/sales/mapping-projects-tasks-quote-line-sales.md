---
title: परियोजना-आधारित कोटेशन लाइन में परियोजनाओं और कार्यों का मानचित्रण करें
description: यह विषय जानकारी प्रदान करता है कि परियोजनाओं और कार्यों का परियोजना-आधारित कार्य लाइन में कैसे मानचित्रण करें.
author: rumant
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d714304f408050babae1a6ba74268979e0b6ea4b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5272750"
---
# <a name="map-projects-and-tasks-to-a-project-based-quote-line"></a><span data-ttu-id="60e59-103">परियोजना-आधारित कोटेशन लाइन में परियोजनाओं और कार्यों का मानचित्रण करें</span><span class="sxs-lookup"><span data-stu-id="60e59-103">Map projects and tasks to a project-based quote line</span></span>

<span data-ttu-id="60e59-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="60e59-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="60e59-105">परियोजना-आधारित कोटेशन लाइनों पर, आप एक परियोजना के विशिष्ट कार्यों का मानचित्रण कर सकते हैं जो पहले से ही एक कोटेशन लाइन से संबध्द है.</span><span class="sxs-lookup"><span data-stu-id="60e59-105">On project-based quote lines, you can map the specific tasks of a project that is already associated to a quote line.</span></span>

<span data-ttu-id="60e59-106">जब आप कार्यों का कोटेशन लाइन में मानचित्रण करते हैं, तो कोटेशन लाइन पर आपके द्वारा परिभाषित निम्नलिखित आइटम केवल उन कार्यों पर लागू होंगे:</span><span class="sxs-lookup"><span data-stu-id="60e59-106">When you map tasks to a quote line, the following items you defined on the quote line will only apply to those tasks:</span></span>

- <span data-ttu-id="60e59-107">बिलिंग विधि</span><span class="sxs-lookup"><span data-stu-id="60e59-107">Billing method</span></span>
- <span data-ttu-id="60e59-108">प्रभार्यता विकल्प</span><span class="sxs-lookup"><span data-stu-id="60e59-108">Chargeability options</span></span>
- <span data-ttu-id="60e59-109">सीमा से अधिक नहीं</span><span class="sxs-lookup"><span data-stu-id="60e59-109">Not-to-exceed limits</span></span>
- <span data-ttu-id="60e59-110">ग्राहक</span><span class="sxs-lookup"><span data-stu-id="60e59-110">Customers</span></span>

<span data-ttu-id="60e59-111">उदाहरणस्वरूप, आपके पास एक परियोजना हो सकती है जहां एक चरण की निर्धारित कीमत है और अन्य सभी चरण समय और सामग्री हैं.</span><span class="sxs-lookup"><span data-stu-id="60e59-111">For example, you might have a project where one phase is fixed price and all the other phases are time and materials.</span></span> <span data-ttu-id="60e59-112">इस मामले में, आप पहले चरण और उसके सभी छोटे कार्यों को एक निश्चित कीमत बिलिंग विधि के साथ उस चरण के लिए कोटेशन लाइन पर संबद्ध कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="60e59-112">In this case, you can associate the first phase, and all of its child tasks, to the quote line for that phase with a fixed price billing method.</span></span> <span data-ttu-id="60e59-113">फिर आप अन्य सभी चरणों को समय और सामग्री-आधारित कोटेशन लाइन से संबद्ध कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="60e59-113">You can then associate all the other phases to the time and materials-based quote line.</span></span>

## <a name="associate-tasks-to-project-based-quote-lines"></a><span data-ttu-id="60e59-114">परियोजना-आधारित कोटेशन लाइनों के साथ कार्य संबद्ध करें</span><span class="sxs-lookup"><span data-stu-id="60e59-114">Associate tasks to project-based quote lines</span></span>

<span data-ttu-id="60e59-115">आप निम्नलिखित स्थानों से कोटेशन लाइनों के साथ कार्यों को संबद्ध कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="60e59-115">You can associate tasks with quote lines from the following locations:</span></span>

- <span data-ttu-id="60e59-116">**परियोजना** पृष्ठ > **कार्य बिलिंग** टैब (इष्टतम)</span><span class="sxs-lookup"><span data-stu-id="60e59-116">**Project** page > **Task billing** tab (optimal)</span></span>
- <span data-ttu-id="60e59-117">**भाव रेखा** पृष्ठ>**देय योग्य कार्य** टैब</span><span class="sxs-lookup"><span data-stu-id="60e59-117">**Quote Line** page > **Chargeable tasks** tab</span></span> 

### <a name="from-the-project-page"></a><span data-ttu-id="60e59-118">परियोजना पृष्ठ से</span><span class="sxs-lookup"><span data-stu-id="60e59-118">From the Project page</span></span>

<span data-ttu-id="60e59-119">**परियोजना** पृष्ठ कोटेशन लाइनों से कार्यों को संबध्द करने के लिए इष्टतम अनुभव प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="60e59-119">The **Project** page provides the optimal experience for associating tasks to quote lines.</span></span> <span data-ttu-id="60e59-120">आप इस पृष्ठ का उपयोग कई कार्यों का चयन करने और उन सभी को साथ ही उनके छोटे कार्यों को चयनित कोटेशन लाइन से संबद्ध करने के लिए कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="60e59-120">You can use this page to select multiple tasks and associate all of them, plus their child tasks, to the selected quote line.</span></span>

1. <span data-ttu-id="60e59-121">परियोजना-आधारित कोटेशन लाइन के **सामान्य** टैब पर, सत्यापित करें कि **परियोजना** फ़ील्ड भर गया है.</span><span class="sxs-lookup"><span data-stu-id="60e59-121">On the **General** tab of a project–based quote line, verify the **Project** field is filled out.</span></span>
2. <span data-ttu-id="60e59-122">**शामिल किए गए कार्य** फ़ील्ड में, **केवल चयनित कार्य** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="60e59-122">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="60e59-123">परियोजना-आधारित कोटेशन लाइन को सहेजें.</span><span class="sxs-lookup"><span data-stu-id="60e59-123">Save the project-based quote line.</span></span> <span data-ttu-id="60e59-124">जब प्रपत्र रिफ़्रेश होता है, तो **देय योग्य कार्य** टैब प्रदर्शित होता है.</span><span class="sxs-lookup"><span data-stu-id="60e59-124">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="60e59-125">**सामान्य** टैब, पर **परियोजना** फ़ील्ड से परियोजना के लिए लिंक चुनें.</span><span class="sxs-lookup"><span data-stu-id="60e59-125">On the **General** tab, select the link for the project from the **Project** field.</span></span>
5. <span data-ttu-id="60e59-126">**परियोजना** पृष्ठ पर, **कार्य बिलिंग** टैब चुनें.</span><span class="sxs-lookup"><span data-stu-id="60e59-126">On the **Project** page, select the **Task billing** tab.</span></span>
6. <span data-ttu-id="60e59-127">दूसरे ग्रिड में, जो कार्य-विशिष्ट बिलिंग सेटअप पर लागू होता है, एक या अधिक कार्यों का चयन करें और फिर **कोटेशन लाइनों को संबध्द करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="60e59-127">In the second grid, which applies to task-specific billing setup, select one or more tasks and then select **Associate quote lines**.</span></span>
7. <span data-ttu-id="60e59-128">दिखाई देते संवाद पृष्ठ में, एक कोटेशन लाइन का चयन करें जो कोटेशन पर परियोजना-आधारित कोटेशन लाइनों को प्रदर्शित करता है.</span><span class="sxs-lookup"><span data-stu-id="60e59-128">In the dialog page that appears, select a quote line that displays project-based quote lines on the quote.</span></span>
8. <span data-ttu-id="60e59-129">**बिलिंग के प्रकार** फ़ील्ड में, इंगित करें कि ये कार्य देय योग्य हैं या आदेय हैं.</span><span class="sxs-lookup"><span data-stu-id="60e59-129">In the **Billing type** field, indicate if these tasks are chargeable or non-chargeable.</span></span>
9. <span data-ttu-id="60e59-130">यह इंगित करने के लिए चेक बॉक्स का चयन करें कि क्या संबंध को चयनित कार्यों के छोटे कार्यों को शामिल करना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="60e59-130">Select the check box to indicate if the association should include child tasks of the selected tasks.</span></span> <span data-ttu-id="60e59-131">बॉक्स की जांच चयनित कार्यों के छोटे कार्यों को कोटेशन लाइन से संबद्ध करेगी.</span><span class="sxs-lookup"><span data-stu-id="60e59-131">Checking the box will associate the child tasks of the selected tasks to the quote line.</span></span>
10. <span data-ttu-id="60e59-132">संवाद बंद करने के लिए **ठीक** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="60e59-132">Select **OK** to close the dialog.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="60e59-133">उद्धरण पंक्ति पृष्ठ से</span><span class="sxs-lookup"><span data-stu-id="60e59-133">From the Quote line page</span></span>

<span data-ttu-id="60e59-134">आप **कोटेशन लाइन** पृष्ठ पर **देय योग्य कार्य** टैब से कोटेशन लाइनों में परियोजना कार्यों को संबद्ध कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="60e59-134">You can associate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

>[!NOTE]
><span data-ttu-id="60e59-135">कोटेशन लाइनों से परियोजना कार्यों को संबद्ध करने का इष्टतम स्थान **परियोजना** पृष्ठ के **कार्य बिलिंग** टैब पर है.</span><span class="sxs-lookup"><span data-stu-id="60e59-135">The optimal place to associate project tasks to quote lines is on the **Task billing** tab on the **Project** page.</span></span> <span data-ttu-id="60e59-136">यदि आप **कोटेशन लाइन** पृष्ठ पर **देय योग्य कार्य** टैब से कार्यों को संबद्ध करते हैं, तो आपको प्रत्येक परियोजना को मैन्युअल रूप से संबद्ध करना होगा.</span><span class="sxs-lookup"><span data-stu-id="60e59-136">If you associate tasks from the **Chargeable tasks** tab on **Quote line** page, you must manually associate each project.</span></span>

1. <span data-ttu-id="60e59-137">एक परियोजना-आधारित कोटेशन लाइन के **सामान्य** टैब पर, सत्यापित करें कि **परियोजना** फ़ील्ड में चुनी गई एक परियोजना है.</span><span class="sxs-lookup"><span data-stu-id="60e59-137">On the **General** tab of a project–based quote line, verify that there is a project selected in the **Project** field.</span></span>
2. <span data-ttu-id="60e59-138">**शामिल किए गए कार्य** फ़ील्ड में, **केवल चयनित कार्य** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="60e59-138">In the **Included tasks** field, select **Selected tasks only**.</span></span>
3. <span data-ttu-id="60e59-139">परियोजना-आधारित कोटेशन लाइन को सहेजें.</span><span class="sxs-lookup"><span data-stu-id="60e59-139">Save the project-based quote line.</span></span> <span data-ttu-id="60e59-140">जब प्रपत्र रिफ़्रेश होता है, तो **देय योग्य कार्य** टैब प्रदर्शित होता है.</span><span class="sxs-lookup"><span data-stu-id="60e59-140">When the form refreshes, the **Chargeable tasks** tab displays.</span></span>
4. <span data-ttu-id="60e59-141">**देय योग्य टास्क** टैब पर, **एक कोटेशन लाइन कार्य जोड़ें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="60e59-141">On the **Chargeable tasks** tab, select **Add a quote line task**.</span></span>
5. <span data-ttu-id="60e59-142">**कोटेशन लाइन कार्य** पृष्ठ पर, **कार्य** फ़ील्ड में, कार्य का चयन करें और **बिलिंग के प्रकार** फ़ील्ड में, **सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="60e59-142">On the **Quote line task** page, in the **Tasks** field, select the task and in the **Billing type** field, select **Save**.</span></span> 
6. <span data-ttu-id="60e59-143">पृष्ठ बंद करें.</span><span class="sxs-lookup"><span data-stu-id="60e59-143">Close the page.</span></span> <span data-ttu-id="60e59-144">चयनित कार्य अब कोटेशन लाइन से संबध्द हो चुका है.</span><span class="sxs-lookup"><span data-stu-id="60e59-144">The selected task is now associated to the quote line.</span></span>

## <a name="disassociate-tasks-from-projectbased-quote-lines"></a><span data-ttu-id="60e59-145">परियोजना-आधारित कोटेशन लाइनों से कार्यों को असंबद्ध करें</span><span class="sxs-lookup"><span data-stu-id="60e59-145">Disassociate tasks from project–based quote lines</span></span>

### <a name="from-the-project-page"></a><span data-ttu-id="60e59-146">परियोजना पृष्ठ से</span><span class="sxs-lookup"><span data-stu-id="60e59-146">From the Project page</span></span>

<span data-ttu-id="60e59-147">यह विधि कोटेशन लाइनों से कार्यों को असंबद्ध करने का सबसे इष्टतम अनुभव प्रदान करती है.</span><span class="sxs-lookup"><span data-stu-id="60e59-147">This method provides the most optimal experience for disassociating tasks from quote lines.</span></span> <span data-ttu-id="60e59-148">आप कई कार्यों का चयन कर सकते हैं और चयनित कोटेशन लाइन से उन सभी को साथ ही उनके छोटे कार्यों को भी असंबद्ध कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="60e59-148">You can select multiple tasks and disassociate all of the them, plus their child tasks, from the selected quote line.</span></span>

1. <span data-ttu-id="60e59-149">**परियोजना** फ़ील्ड में परियोजना-आधारित कोटेशन लाइन के **सामान्य** टैब पर, परियोजना के लिंक का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="60e59-149">On the **General** tab of a project–based quote line, in the **Project** field, select the project link.</span></span>
2. <span data-ttu-id="60e59-150">**परियोजना** पृष्ठ पर, **कार्य बिलिंग** टैब चुनें.</span><span class="sxs-lookup"><span data-stu-id="60e59-150">On the **Project** page, select the **Task billing** tab.</span></span>
3. <span data-ttu-id="60e59-151">दूसरे ग्रिड में, जो कार्य-विशिष्ट बिलिंग सेटअप पर लागू होता है, एक या अधिक कार्यों का चयन करें और फिर **कोटेशन लाइनों को असंबद्ध करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="60e59-151">In the second grid, which applies to task-specific billing setup, select one or more tasks, and then select **Disassociate quote lines**.</span></span>
4. <span data-ttu-id="60e59-152">दिखाई देते संवाद पृष्ठ में, एक कोटेशन लाइन का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="60e59-152">In the dialog page that appears, select a quote line.</span></span>
5. <span data-ttu-id="60e59-153">चेक बॉक्स का चयन करें ताकि यह पता चल सके कि क्या संबंध को चयनित कार्यों के छोटे कार्यों से भी हटाया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="60e59-153">Select the check box to indicate whether the association should also be removed from child tasks of the selected tasks.</span></span> <span data-ttu-id="60e59-154">बॉक्स की जांच करने से चयनित कार्यों के छोटे कार्यों को कोटेशन लाइन से भी असंबद्ध किया जा सकेगा.</span><span class="sxs-lookup"><span data-stu-id="60e59-154">Checking the box will also disassociate the child tasks of the selected tasks to the quote line.</span></span>
6. <span data-ttu-id="60e59-155">**ठीक** चुनें।</span><span class="sxs-lookup"><span data-stu-id="60e59-155">Select **OK**.</span></span> <span data-ttu-id="60e59-156">एक चेतावनी संदेश आपको सूचित करता है कि यदि आप इस संबंध को हटा देते हैं, तो कार्य पर पहले से दर्ज किसी भी वास्तविक आँकड़ों को उलट दिया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="60e59-156">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
7. <span data-ttu-id="60e59-157">कार्य और परियोजना-आधारित कोटेशन लाइन के बीच सहयोग को जारी रखने और हटाने के लिए **ओके** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="60e59-157">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

### <a name="from-the-quote-line-page"></a><span data-ttu-id="60e59-158">उद्धरण पंक्ति पृष्ठ से</span><span class="sxs-lookup"><span data-stu-id="60e59-158">From the Quote line page</span></span>

<span data-ttu-id="60e59-159">आप **कोटेशन लाइन** पृष्ठ पर **देय योग्य कार्य** टैब द्वारा कोतेशन लाइन से परियोजना कार्यों को भी असंबद्ध कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="60e59-159">You can also disassociate project tasks to quote lines from the **Chargeable tasks** tab on **Quote line** page.</span></span>

1. <span data-ttu-id="60e59-160">पर **धर्मार्थ कार्य** टैब, चयन करें **एक उद्धरण पंक्ति कार्य हटाएँ**.</span><span class="sxs-lookup"><span data-stu-id="60e59-160">On the **Chargeable tasks** tab, select **Delete a quote line task**.</span></span>
2. <span data-ttu-id="60e59-161">**ठीक** चुनें।</span><span class="sxs-lookup"><span data-stu-id="60e59-161">Select **OK**.</span></span> <span data-ttu-id="60e59-162">एक चेतावनी संदेश आपको सूचित करता है कि यदि आप इस संबंध को हटा देते हैं, तो कार्य पर पहले से दर्ज किसी भी वास्तविक आँकड़ों को उलट दिया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="60e59-162">A warning message informs you that if you remove this association, any actuals previously recorded on the task could be reversed.</span></span> 
3. <span data-ttu-id="60e59-163">कार्य और परियोजना-आधारित कोटेशन लाइन के बीच सहयोग को जारी रखने और हटाने के लिए **ओके** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="60e59-163">Select **OK** to continue and remove the association between the task and the project-based quote line.</span></span>

>[!NOTE]
> <span data-ttu-id="60e59-164">यह प्रक्रिया परियोजना से कार्य को नहीं मिटाती है.</span><span class="sxs-lookup"><span data-stu-id="60e59-164">This procedure doesn't delete the task from the project.</span></span> <span data-ttu-id="60e59-165">यह केवल परियोजना-आधारित कोटेशन लाइन से कार्य संबंध को हटाता है.</span><span class="sxs-lookup"><span data-stu-id="60e59-165">It only removes the task association from the project-based quote line.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]