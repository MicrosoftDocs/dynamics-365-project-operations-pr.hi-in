---
title: एक मूल्य सूची बनाएँ
description: Project Service में मूल्य सूची बनाने का तरीका
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 08d93ad86d782922df6b22370749628ddbdc0718
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122030"
---
# <a name="create-a-price-list-project-service"></a><span data-ttu-id="314ac-103">मूल्‍य सूची बनाना (Project Service)</span><span class="sxs-lookup"><span data-stu-id="314ac-103">Create a price list (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="314ac-104">मूल्‍य सूचियाँ एक ऐसा टेम्पलेट बनाती हैं, जिनका उपयोग आपके खाता प्रबंधक, कोट और परियोजनाएँ बनाने, और परियोजना की लागत स्‍थापित करने के लिए कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="314ac-104">Price lists provide a template your account managers can use for creating quotes and projects, and for establishing the costs of a project.</span></span> <span data-ttu-id="314ac-105">वे भूमिकाओं और व्‍यय, और प्रत्‍येक के लिए आपके द्वारा लिए जाने वाले मूल्‍य की एक पंक्ति आइटम सूची प्रदान करते हैं.</span><span class="sxs-lookup"><span data-stu-id="314ac-105">They provide a line item list of roles and expenses, and the price you will charge for each.</span></span> <span data-ttu-id="314ac-106">आप एकाधिक मूल्य सूचियाँ बना सकते हैं, ताकि आप भिन्न-भिन्न क्षेत्रों के लिए, जहाँ आप विक्रय करते हैं या भिन्न-भिन्न विक्रय चैनल के लिए, अलग-अलग मूल्य संरचनाओं को बनाए रख सकें.</span><span class="sxs-lookup"><span data-stu-id="314ac-106">You can create multiple price lists so that you can maintain separate price structures for different regions you sell your products in or for different sales channels.</span></span> <span data-ttu-id="314ac-107">आप अपने ग्राहकों से जिन मुद्राओं में बिल करने की योजना बनाते हैं, उनमें प्रत्‍येक मुद्रा के लिए कम से कम एक मूल्‍य सूची बनाना एक अच्छा विचार है.</span><span class="sxs-lookup"><span data-stu-id="314ac-107">It’s a good idea to create at least one price list for every currency you plan to bill your customers in.</span></span>  
  
<span data-ttu-id="314ac-108">डिलीवर किए जाने वाले कार्यों के लिए वित्तीय अनुमान बनाने के लिए, सुनिश्चित करें कि प्रत्येक परियोजना के पास एक बैकिंग लागत और विक्रय मूल्‍य सूची मौजूद है.</span><span class="sxs-lookup"><span data-stu-id="314ac-108">To create financial estimates for the work to be delivered, make sure every project has a backing cost and sales price list.</span></span> <span data-ttu-id="314ac-109">एक डिफ़ॉल्ट लागत और विक्रय मूल्य सूची सेट अप करें, जो आपके संगठन में बनाई गई सभी परियोजनाओं पर लागू होती है.</span><span class="sxs-lookup"><span data-stu-id="314ac-109">Set up a default cost and sales pricelist that applies to all projects created in your organization.</span></span>  
  
<span data-ttu-id="314ac-110">मूल्य सूचियाँ, भूमिकाओं और व्यय श्रेणियों पर निर्भर करती हैं, अतः आप एक मूल्य सूची बनाने से पहले, सुनिश्चित कर लें कि आपने पहले ही भूमिकाएँ और व्‍यय श्रेणियाँ कॉन्फ़िगर कर ली हैं जिनका उपयोग आप मूल्य सूची बनाते समय करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="314ac-110">Price lists rely on roles and expense categories, so before you create a price list, make sure you’ve already configured the roles and expense categories you want to use while creating the price list.</span></span>  
  
1.  <span data-ttu-id="314ac-111">**Project Service > मूल्‍य सूचियाँ** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="314ac-111">Go to **Project Service > Price Lists**.</span></span>  
  
2.  <span data-ttu-id="314ac-112">**नया** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="314ac-112">Click **New**.</span></span>  
  
3.  <span data-ttu-id="314ac-113">**संदर्भ** में, यह चयन करें कि यह मूल्‍य सूची **लागत**, **क्रय** या **विक्रय** के लिए है.</span><span class="sxs-lookup"><span data-stu-id="314ac-113">In **Context**, select whether this price list is for **Cost**, **Purchase**, or **Sales**.</span></span>  
  
4.  <span data-ttu-id="314ac-114">**नाम** में, मूल्य सूची के लिए एक नाम दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="314ac-114">In **Name**, enter a name for the price list.</span></span>  
  
5.  <span data-ttu-id="314ac-115">**मुद्रा** में, वह मुद्रा चुनें, जिसका उपयोग आप लागत या बिलिंग के लिए करने जा रहे हैं.</span><span class="sxs-lookup"><span data-stu-id="314ac-115">In **Currency**, select the currency you’re going to use for billing or costing.</span></span>  
  
6.  <span data-ttu-id="314ac-116">**समय इकाई** में, वह समय अवधि निर्दिष्ट करें, जिस पर मूल्य लागू होते हैं, जैसे दिन या घंटा.</span><span class="sxs-lookup"><span data-stu-id="314ac-116">In **Time Unit**, specify the period of time the price applies to, such as day or hour.</span></span>  
  
7.  <span data-ttu-id="314ac-117">आवश्‍यकतानुसार **प्रारंभ दिनांक**, **समाप्ति दिनांक** और **वर्णन** भरें.</span><span class="sxs-lookup"><span data-stu-id="314ac-117">Fill in the **Start Date**, **End Date**, and **Description** as needed.</span></span>  
  
8.  <span data-ttu-id="314ac-118">रिकॉर्ड बनाने के लिए, **सहेजें** पर क्लिक करें ताकि आप उसको संपादित करना जारी रख सकें.</span><span class="sxs-lookup"><span data-stu-id="314ac-118">Click **Save** to create the record so you can continue editing it.</span></span>  
  
9. <span data-ttu-id="314ac-119">मूल्य सूची पर एक भूमिका मूल्य जोड़ने के लिए, **भूमिका मूल्‍यों** के अंतर्गत **+** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="314ac-119">To add a role price to the price list, click **+** under **Role prices**.</span></span>  
  
10. <span data-ttu-id="314ac-120">**भूमिका मूल्‍य** फलक में, विवरण भरें और उसके बाद **सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="314ac-120">In the **Role Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="314ac-121">आवश्यकतानुसार भूमिका मूल्‍य जोड़ना जारी रखें.</span><span class="sxs-lookup"><span data-stu-id="314ac-121">Continue adding role prices as necessary.</span></span> <span data-ttu-id="314ac-122">काम पूरा होने पर, स्‍क्रीन के निचले दाएँ कोने में स्थित **सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="314ac-122">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
11. <span data-ttu-id="314ac-123">मूल्य सूची पर एक व्‍यय श्रेणी मूल्य जोड़ने के लिए, **श्रेणी मूल्‍य** के अंतर्गत **+** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="314ac-123">To add an expense category price to the price list, click **+** under **Category prices**.</span></span>  
  
12. <span data-ttu-id="314ac-124">**हस्‍तांतरण श्रेणी मूल्‍य** फलक में, विवरण भरें और उसके बाद **सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="314ac-124">In the **Transaction Category Price** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="314ac-125">आवश्यकतानुसार श्रेणी मूल्‍य जोड़ना जारी रखें.</span><span class="sxs-lookup"><span data-stu-id="314ac-125">Continue adding category prices as necessary.</span></span> <span data-ttu-id="314ac-126">काम पूरा होने पर, स्‍क्रीन के निचले दाएँ कोने में स्थित **सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="314ac-126">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
13. <span data-ttu-id="314ac-127">मूल्य सूची में मूल्य सूची आइटम जोड़ने के लिए, **मूल्‍य सूची आइटम** के अंतर्गत **+** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="314ac-127">To add price list items to the price list, click **+** under **Price List Items**.</span></span>  
  
14. <span data-ttu-id="314ac-128">**मूल्‍य सूची आइटम** फलक में, विवरण भरें और उसके बाद **सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="314ac-128">In the **Price List Item** pane, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="314ac-129">आवश्यकतानुसार मूल्‍य सूची आइटम जोड़ना जारी रखें.</span><span class="sxs-lookup"><span data-stu-id="314ac-129">Continue adding price list items as necessary.</span></span> <span data-ttu-id="314ac-130">काम पूरा होने पर, स्‍क्रीन के निचले दाएँ कोने में स्थित **सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="314ac-130">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
15. <span data-ttu-id="314ac-131">मूल्‍य सूची में क्षेत्र संबंध जोड़ने के लिए, **क्षेत्र संबंध** के अंतर्गत **+** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="314ac-131">To add territory relationships to the price list, click **+** under **Territory Relationships**.</span></span>  
  
16. <span data-ttu-id="314ac-132">**नए कनेक्‍शन** विंडो में, विवरण भरें और उसके बाद **सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="314ac-132">In the **New Connection** window, fill in the details, and then click **Save**.</span></span> <span data-ttu-id="314ac-133">आवश्‍यकतानुसार क्षेत्र संबंध जोड़ना जारी रखें.</span><span class="sxs-lookup"><span data-stu-id="314ac-133">Continue adding territory relationships as necessary.</span></span> <span data-ttu-id="314ac-134">काम पूरा होने पर, स्‍क्रीन के निचले दाएँ कोने में स्थित **सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="314ac-134">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="314ac-135">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="314ac-135">See Also</span></span>  
 [<span data-ttu-id="314ac-136">Project Service Automation कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="314ac-136">Configure Project Service Automation</span></span>](../psa/configure.md)
