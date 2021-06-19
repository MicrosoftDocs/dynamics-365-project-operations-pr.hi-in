---
title: मूल्य निर्धारण आयामों के लिए एक कस्टम समाधान बनाएँ
description: यह विषय कस्टम मूल्य निर्धारण आयाम बनाते समय कस्टम समाधान बनाने का तरीका समझाता है.
author: Rumant
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: ae7f22b9cb092e956d0f1eaf1f1997c8e97392f4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012318"
---
# <a name="create-custom-solutions-for-pricing-dimensions"></a><span data-ttu-id="b895d-103">मूल्य निर्धारण आयामों के लिए एक कस्टम समाधान बनाएँ</span><span class="sxs-lookup"><span data-stu-id="b895d-103">Create custom solutions for pricing dimensions</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

> [!IMPORTANT]
> <span data-ttu-id="b895d-104">सभी कस्टम मूल्य निर्धारण आयाम परिवर्तन एक अलग समाधान में होने चाहिए.</span><span class="sxs-lookup"><span data-stu-id="b895d-104">All custom pricing dimension changes should be in a separate solution.</span></span> <span data-ttu-id="b895d-105">यह महत्वपूर्ण सर्वोत्तम अभ्यास भविष्य में आवश्यकतानुसार परिवर्तन या अपडेट करने के लिए लचीलापन प्रदान करता है, आपके काम के पुन: उपयोग में मदद करेगा, और इन परिवर्तनों को दूसरे उदाहरण में पोर्ट करना आसान बनाता है।</span><span class="sxs-lookup"><span data-stu-id="b895d-105">This important best practice provides flexibility in the future to update or remove changes as needed, will help with re-use of your work, and makes it easier to port these changes to another instance.</span></span> <span data-ttu-id="b895d-106">सभी आवश्यक परिवर्तन कर लेने के बाद, इस समाधान को **प्रबंधित समाधान** के रूप में निर्यात करें और अपने मूल्य निर्धारण सेटअप का पुन: उपयोग करने के लिए इसे अन्य आवृत्तियों में आयात करें.</span><span class="sxs-lookup"><span data-stu-id="b895d-106">After you make the required changes, export this solution as a **Managed solution**, and import it into other instances to reuse your pricing setup.</span></span>

1. <span data-ttu-id="b895d-107">**सेटिंग** > **समाधान** चुने और फिर उसके बाद **नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="b895d-107">Select **Settings** > **Solutions**, and then select **New**.</span></span> 
2. <span data-ttu-id="b895d-108">समाधान का नाम दें, **\<your organization name> मूल्य निर्धारण के आयामों**, शेष आवश्यक जानकारी दर्ज करें और फिर **सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="b895d-108">Name the solution, **\<your organization name> pricing dimensions**, enter the remaining required information, and then select **Save**.</span></span>

> ![मूल्य निर्धारण आयामों के लिए एक कस्टम समाधान बनाना](media/Creation-of-custom-pricing-dimension-solution.PNG)
  
## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a><span data-ttu-id="b895d-110">मूल्य निर्धारण आयाम समाधान के लिए सभी आवश्यक निकायों और संबंधित हिस्सों को जोड़ें</span><span class="sxs-lookup"><span data-stu-id="b895d-110">Add all required entities and related components to the Pricing dimension solution</span></span>
<span data-ttu-id="b895d-111">आपको अपने मूल्य निर्धारण समाधान में निम्नलिखित Project Service इकाइयों को जोड़ना होगा।</span><span class="sxs-lookup"><span data-stu-id="b895d-111">You will need to add the following Project Service entities to your pricing solution.</span></span> <span data-ttu-id="b895d-112">मूल्य निर्धारण समाधान में कुछ महत्वपूर्ण स्कीमा परिवर्तन करने के लिए इस प्रक्रिया में चरणों को पूरा करें, ताकि निकाय नए मूल्य निर्धारण आयामों से अवगत हो सकें.</span><span class="sxs-lookup"><span data-stu-id="b895d-112">Complete the steps in this procedure to make some important schema changes in the pricing solution so that the entities become aware of the new pricing dimensions.</span></span>

1. <span data-ttu-id="b895d-113">**समायोजन** > **समाधान** चुनें, और तब डबल-क्लिक करें **\<your organization name> मूल्य निर्धारण के आयाम**.</span><span class="sxs-lookup"><span data-stu-id="b895d-113">Select **Settings** > **Solutions**, and then double-click **\<your organization name> pricing dimensions**.</span></span> 
2. <span data-ttu-id="b895d-114">समाधान एक्सप्लोरर में, बाएं नेविगेशन पैन पर, **मौजूदा जोड़ें** > **इकाइयां** चुनें।</span><span class="sxs-lookup"><span data-stu-id="b895d-114">In Solution Explorer, on the left navigation pane, select **Add Existing** > **Entities**.</span></span>
3. <span data-ttu-id="b895d-115">**समाधान हिस्से** संवाद बॉक्स में, निम्नलिखित इकाइयों का चयन करें:</span><span class="sxs-lookup"><span data-stu-id="b895d-115">In the **Solution Components** dialog box, select the following entities:</span></span>

- <span data-ttu-id="b895d-116">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="b895d-116">Actual</span></span>
- <span data-ttu-id="b895d-117">बुक करने योग्य संसाधन</span><span class="sxs-lookup"><span data-stu-id="b895d-117">Bookable Resource</span></span>
- <span data-ttu-id="b895d-118">अनुमान पंक्ति</span><span class="sxs-lookup"><span data-stu-id="b895d-118">Estimate Line</span></span>
- <span data-ttu-id="b895d-119">परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="b895d-119">Project Task</span></span>
- <span data-ttu-id="b895d-120">इनवॉइस पंक्ति विवरण</span><span class="sxs-lookup"><span data-stu-id="b895d-120">Invoice Line Detail</span></span>
- <span data-ttu-id="b895d-121">जर्नल पंक्ति</span><span class="sxs-lookup"><span data-stu-id="b895d-121">Journal Line</span></span>
- <span data-ttu-id="b895d-122">परियोजना अनुबंध पंक्ति विवरण</span><span class="sxs-lookup"><span data-stu-id="b895d-122">Project Contract Line Detail</span></span>
- <span data-ttu-id="b895d-123">प्रोजेक्ट टीम सदस्य</span><span class="sxs-lookup"><span data-stu-id="b895d-123">Project Team Member</span></span>
- <span data-ttu-id="b895d-124">कोट पंक्ति विवरण</span><span class="sxs-lookup"><span data-stu-id="b895d-124">Quote Line Detail</span></span>
- <span data-ttu-id="b895d-125">भूमिका मू्ल्य मार्कअप</span><span class="sxs-lookup"><span data-stu-id="b895d-125">Role Price Markup</span></span>
- <span data-ttu-id="b895d-126">भूमिका मू्ल्य</span><span class="sxs-lookup"><span data-stu-id="b895d-126">Role Price</span></span> 
- <span data-ttu-id="b895d-127">समय प्रविष्टि</span><span class="sxs-lookup"><span data-stu-id="b895d-127">Time Entry</span></span> 

> ![मूल्य निर्धारण आयाम समाधान में मौजूदा इकाइयां जोड़ें](media/Existing-entities-to-PD-solution.png)

> ![समाधान घटक चुनें](media/Dimension-Components.png)

> [!NOTE]
> <span data-ttu-id="b895d-130">चयनित सभी संस्थाओं के लिए सभी फॉर्मों और दृश्य को शामिल करना सुनिश्चित करें।</span><span class="sxs-lookup"><span data-stu-id="b895d-130">Make sure to include all forms and views for each of the entities selected.</span></span>

4. <span data-ttu-id="b895d-131">जब चयनित निकायों के लिए किसी भी निर्भर संस्थाओं को शामिल करने के लिए कहा जाए, तो **नहीं** चुनें.</span><span class="sxs-lookup"><span data-stu-id="b895d-131">When prompted to include any dependent entities for the selected entities, select **No**.</span></span>

> ![सभी संबंधित हिस्सों को शामिल न करें](media/Do-not-include-required.png)




[!INCLUDE[footer-include](../includes/footer-banner.md)]