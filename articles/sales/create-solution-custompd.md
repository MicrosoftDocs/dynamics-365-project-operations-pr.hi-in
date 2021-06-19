---
title: कस्टम मूल्य निर्धारण आयामों के लिए एक समाधान बनाएँ
description: इस विषय में कस्टम मूल्य निर्धारण आयामों के लिए समाधान बनाने के तरीके के बारे में जानकारी प्रदान की गई है.
author: Rumant
ms.date: 11/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 86f4cd2c26ebfca621d1b226b571d220d3b2441e
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010338"
---
# <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="e456c-103">कस्टम मूल्य निर्धारण आयामों के लिए एक समाधान बनाएँ</span><span class="sxs-lookup"><span data-stu-id="e456c-103">Create a solution for custom pricing dimensions</span></span>

 <span data-ttu-id="e456c-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="e456c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span> 

>[!IMPORTANT]
><span data-ttu-id="e456c-105">सभी कस्टम मूल्य निर्धारण आयाम परिवर्तन एक अलग समाधान में होने चाहिए.</span><span class="sxs-lookup"><span data-stu-id="e456c-105">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="e456c-106">यह महत्वपूर्ण सर्वोत्तम व्यवहार आवश्यकतानुसार परिवर्तन अद्यतन करने या बदलने का लचीलापन प्रदान करता है, आपके कार्य का पुनः उपयोग करने में मदद करता और अन्य आवृत्तियों में बदलाव पोर्ट करना आसान बनाता है.</span><span class="sxs-lookup"><span data-stu-id="e456c-106">This important best practice allows the flexibility to update or remove changes as needed, helps with re-use of your work, and makes it easier to port changes to other instances.</span></span> <span data-ttu-id="e456c-107">आपके द्वारा आवश्यक परिवर्तन किए जाने के बाद, इस समाधान को **प्रबंधित** समाधान के रूप में निर्यात करें और उसके बाद पुनः उपयोग करने के लिए इसे अन्य आवृत्तियों में आयात करें.</span><span class="sxs-lookup"><span data-stu-id="e456c-107">After you make the required changes, export this solution as a **Managed** solution, and then import into other instances for reuse.</span></span>

## <a name="create-a-solution-for-custom-pricing-dimensions"></a><span data-ttu-id="e456c-108">कस्टम मूल्य निर्धारण आयामों के लिए एक समाधान बनाएँ</span><span class="sxs-lookup"><span data-stu-id="e456c-108">Create a solution for custom pricing dimensions</span></span>

1.  <span data-ttu-id="e456c-109">**सेटिंग** > **समाधान** चुने और फिर उसके बाद **नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="e456c-109">Select **Settings** > **Solutions**, and then select **New**.</span></span>
2.  <span data-ttu-id="e456c-110">समाधान को नाम दें, *<your organization name> मूल्य निर्धारण आयाम*.</span><span class="sxs-lookup"><span data-stu-id="e456c-110">Name the solution, *<your organization name> pricing dimensions*.</span></span>
3. <span data-ttu-id="e456c-111">शेष आवश्यक जानकारी दर्ज करें और फिर **सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="e456c-111">Enter the remaining required information, and then select **Save**.</span></span>

  ![कस्टम मूल्य निर्धारण आयाम समाधान का निर्माण](./media/Creation-of-custom-pricing-dimension-solution.png)
 
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="e456c-113">मूल्य निर्धारण आयाम समाधान के लिए सभी आवश्यक निकायों और संबंधित हिस्सों को जोड़ें</span><span class="sxs-lookup"><span data-stu-id="e456c-113">Add all required entities and related components to the Pricing dimension solution</span></span>

<span data-ttu-id="e456c-114">मूल्य निर्धारण समाधान में महत्वपूर्ण स्कीमा परिवर्तन करने के लिए अपने मूल्य निर्धारण समाधान में निम्नलिखित Project Service निकाय जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="e456c-114">Add the following Project Service entities to your pricing solution to make important schema changes in the pricing solution.</span></span> <span data-ttu-id="e456c-115">यह प्रक्रिया पूरी करने के बाद, निकाय नए मूल्य निर्धारण आयामों को पहचानेंगे.</span><span class="sxs-lookup"><span data-stu-id="e456c-115">After you have completed this procedure, the entities will recognize the new pricing dimensions.</span></span>

1.  <span data-ttu-id="e456c-116">**सेटिंग** > **समाधान** चुनें और उसके बाद **<*आपके संगठन का नाम*> मूल्य निर्धारण आयाम** पर डबल-क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="e456c-116">Select **Settings** > **Solutions**, and then double-click **<*your organization name*> pricing dimensions**.</span></span>
2.  <span data-ttu-id="e456c-117">समाधान एक्सप्लोरर में, बाएं नेविगेशन पैन पर, **मौजूदा जोड़ें** > **इकाइयां** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e456c-117">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3.  <span data-ttu-id="e456c-118">**समाधान हिस्से** संवाद बॉक्स में, निम्नलिखित इकाइयों का चयन करें:</span><span class="sxs-lookup"><span data-stu-id="e456c-118">In the **Solution Components** dialog box, select the following entities:</span></span>
 
   - <span data-ttu-id="e456c-119">**वास्तविक**</span><span class="sxs-lookup"><span data-stu-id="e456c-119">**Actual**</span></span>
   - <span data-ttu-id="e456c-120">**बुक करने योग्य संसाधन**</span><span class="sxs-lookup"><span data-stu-id="e456c-120">**Bookable Resource**</span></span>
   - <span data-ttu-id="e456c-121">**अनुमान पंक्ति**</span><span class="sxs-lookup"><span data-stu-id="e456c-121">**Estimate Line**</span></span>
   - <span data-ttu-id="e456c-122">**परियोजना कार्य**</span><span class="sxs-lookup"><span data-stu-id="e456c-122">**Project Task**</span></span>
   - <span data-ttu-id="e456c-123">**इनवॉइस पंक्ति विवरण**</span><span class="sxs-lookup"><span data-stu-id="e456c-123">**Invoice Line Detail**</span></span>
   - <span data-ttu-id="e456c-124">**जर्नल पंक्ति**</span><span class="sxs-lookup"><span data-stu-id="e456c-124">**Journal Line**</span></span>
   - <span data-ttu-id="e456c-125">**परियोजना अनुबंध पंक्ति विवरण**</span><span class="sxs-lookup"><span data-stu-id="e456c-125">**Project Contract Line Detail**</span></span>
   - <span data-ttu-id="e456c-126">**प्रोजेक्ट टीम सदस्य**</span><span class="sxs-lookup"><span data-stu-id="e456c-126">**Project Team Member**</span></span>
   - <span data-ttu-id="e456c-127">**कोट पंक्ति विवरण**</span><span class="sxs-lookup"><span data-stu-id="e456c-127">**Quote Line Detail**</span></span>
   - <span data-ttu-id="e456c-128">**भूमिका मू्ल्य मार्कअप**</span><span class="sxs-lookup"><span data-stu-id="e456c-128">**Role Price Markup**</span></span>
   - <span data-ttu-id="e456c-129">**भूमिका मू्ल्य**</span><span class="sxs-lookup"><span data-stu-id="e456c-129">**Role Price**</span></span>
   - <span data-ttu-id="e456c-130">**समय प्रविष्टि**</span><span class="sxs-lookup"><span data-stu-id="e456c-130">**Time Entry**</span></span>
 
   ![मौजूदा निकाय कस्टम मूल्य निर्धारण आयाम समाधान जोड़ें](./media/Existing-entities-to-PD-solution.png)
 
 4. <span data-ttu-id="e456c-132">प्रत्येक निकाय के लिए, जोड़े जा रहे घटकों और प्रत्येक निकाय के लिए निकाय परिसंपत्तियों की अंतिम सूची की समीक्षा करें.</span><span class="sxs-lookup"><span data-stu-id="e456c-132">For each entity, review the components being added and the final list of entity assets for each entity.</span></span> 

   >[!NOTE]
   > <span data-ttu-id="e456c-133">चयनित सभी निकायों के लिए सभी प्रपत्रों और दृश्यों को शामिल करें.</span><span class="sxs-lookup"><span data-stu-id="e456c-133">Include all forms and views for each of the selected entities.</span></span>

  ![निकाय जोड़े गए](./media/solution-component-selection.png)


5.  <span data-ttu-id="e456c-135">जब चयनित निकायों के लिए किसी भी निर्भर निकाय को शामिल करने के लिए कहा जाए, तो **नहीं, आवश्यक घटक शामिल न करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="e456c-135">When prompted to include any dependent entities for the selected entities, select **No, do not include required components.**</span></span>

    ![निर्भर निकायों को शामिल करना](./media/Do-not-include-required.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]