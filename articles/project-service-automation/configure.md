---
title: Project Service Automation कॉन्फ़िगर करें
description: Project Service को कॉन्फ़िगर करने के चरण
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 56ba0b8d-808c-48d6-965f-abd74b49c2b4
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 52be4705e6ef983dcf421df5d1bfb5c6de8e9a30
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751999"
---
# <a name="configure-project-service"></a><span data-ttu-id="0529c-103">Project Service कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="0529c-103">Configure Project Service</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="0529c-104">इससे पहले कि अपने खातों, परियोजनाओं और संसाधनों को प्रबंधित करने के लिए आप [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] में [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] स्वचालन क्षमताओं का उपयोग कर सकें, यह सुनिश्चित करने के लिए आपको कुछ कॉन्फ़िगरेशन चरण पूरे करने होंगे कि [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] समाधान आपके संगठन की आवश्यकताओं से मेल खाता है.</span><span class="sxs-lookup"><span data-stu-id="0529c-104">Before you can use the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] automation capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] to manage your accounts, projects, and resources, you need to complete a few configuration steps to ensure the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] solution matches your organization’s needs.</span></span> <span data-ttu-id="0529c-105">इन चरणों में शामिल हैं:</span><span class="sxs-lookup"><span data-stu-id="0529c-105">These steps include:</span></span>  
  
-   <span data-ttu-id="0529c-106">[समय इकाइयाँ सेट अप करें](../project-service/set-up-time-units.md).</span><span class="sxs-lookup"><span data-stu-id="0529c-106">[Set up time units](../project-service/set-up-time-units.md).</span></span> <span data-ttu-id="0529c-107">उत्पाद कैटलॉग में वे समय इकाइयाँ कॉन्फ़िगर करें, जिनका उपयोग आप अपनी परियोजनाओं को शेड्यूल और बिलिंग करने के आधार के रूप में करेंगे.</span><span class="sxs-lookup"><span data-stu-id="0529c-107">Configure the time units in the product catalog that you’ll use as a base for scheduling and billing your projects.</span></span>  
  
-   <span data-ttu-id="0529c-108">[मुद्रा और विनिमय दर सेट अप करें](../project-service/set-up-currencies-exchange-rates.md).</span><span class="sxs-lookup"><span data-stu-id="0529c-108">[Set up currencies and exchange rates](../project-service/set-up-currencies-exchange-rates.md).</span></span> <span data-ttu-id="0529c-109">अपनी परियोजनाओं में उपयोग की जाने वाली मुद्राएँ सेट करें.</span><span class="sxs-lookup"><span data-stu-id="0529c-109">Set up the currencies to use for your projects.</span></span>  
  
-   <span data-ttu-id="0529c-110">[संगठनात्मक इकाइयाँ बनाएँ](../project-service/create-organizational-units.md).</span><span class="sxs-lookup"><span data-stu-id="0529c-110">[Create organizational units](../project-service/create-organizational-units.md).</span></span> <span data-ttu-id="0529c-111">उन समूहों का सेट अप करें जिनका उपयोग आपकी कंपनी व्यवसाय को विभाजित करने के लिए करती है, चाहे भूगोल के आधार पर, व्यावसायिक फ़ंक्शन के आधार पर या अन्य तार्किक विभाग के आधार पर.</span><span class="sxs-lookup"><span data-stu-id="0529c-111">Set up the groups that your company uses to divide its business, whether by geography, business function, or other logical division.</span></span>  
  
-   <span data-ttu-id="0529c-112">[इनवॉइस आवृत्तियाँ सेट अप करें](../project-service/set-up-invoice-frequencies.md).</span><span class="sxs-lookup"><span data-stu-id="0529c-112">[Set up invoice frequencies](../project-service/set-up-invoice-frequencies.md).</span></span> <span data-ttu-id="0529c-113">वे समय अवधियाँ सेट करें जिनका उपयोग आप अपने ग्राहकों को बिल के लिए करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="0529c-113">Set up time periods that you want to use for billing your clients.</span></span>  
  
-   <span data-ttu-id="0529c-114">[लेनदेन श्रेणियाँ कॉन्फ़िगर करें](../project-service/configure-transaction-categories.md).</span><span class="sxs-lookup"><span data-stu-id="0529c-114">[Configure transaction categories](../project-service/configure-transaction-categories.md).</span></span> <span data-ttu-id="0529c-115">वे लेनदेने श्रेणियाँ सेट करें जिनमें आपके सलाहकार अपने बिल करने योग्य और बिना बिल करने योग्य व्यय चार्ज कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="0529c-115">Set up transaction categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="0529c-116">[व्यय श्रेणियाँ कॉन्फ़िगर करें](../project-service/configure-expense-categories.md).</span><span class="sxs-lookup"><span data-stu-id="0529c-116">[Configure expense categories](../project-service/configure-expense-categories.md).</span></span> <span data-ttu-id="0529c-117">वे श्रेणियाँ सेट करें जिनमें आपके सलाहकार अपने बिल करने योग्य और बिना बिल करने योग्य व्यय चार्ज कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="0529c-117">Set up the categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="0529c-118">[उत्पाद कैटलॉग आइटम बनाएँ](../project-service/create-product-catalog-items.md).</span><span class="sxs-lookup"><span data-stu-id="0529c-118">[Create product catalog items](../project-service/create-product-catalog-items.md).</span></span> <span data-ttu-id="0529c-119">जो उत्पाद आप बेचते हैं जैसे सॉफ़्टवेयर लायसेंस, उन्हें उत्पाद कैटलॉग में जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="0529c-119">Add the products you sell, such as software licenses, to the product catalog.</span></span>  
  
-   <span data-ttu-id="0529c-120">[एक मूल्य सूची बनाएँ](../project-service/create-price-list.md).</span><span class="sxs-lookup"><span data-stu-id="0529c-120">[Create a price list](../project-service/create-price-list.md).</span></span> <span data-ttu-id="0529c-121">इसके आधार पर कि आप अपने क्लायंट से उनकी परियोजना आवश्यकता के अनुसार प्रत्येक भूमिका के लिए उनसे कितना चार्ज करना चाहते हैं, विभिन्न मूल्य सूचियाँ कॉन्फ़िगर करें.</span><span class="sxs-lookup"><span data-stu-id="0529c-121">Configure different price lists, depending on how much you want to charge your clients for each role their project requires.</span></span>  
  
-   <span data-ttu-id="0529c-122">[संसाधन सेट अप करें](../project-service/set-up-resources.md).</span><span class="sxs-lookup"><span data-stu-id="0529c-122">[Set up resources](../project-service/set-up-resources.md).</span></span> <span data-ttu-id="0529c-123">अपनी परियोजनाओं के लिए जिन कौशल, दक्षता, संसाधन भूमिका और अन्य संसाधन जानकारी की आपको आवश्यकता होगी, उन्हें जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="0529c-123">Add the skills, proficiencies, resource roles, and other resource information that you’ll need for your projects.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="0529c-124">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="0529c-124">See Also</span></span>  
 <span data-ttu-id="0529c-125">[Project Service Automation का ओवरव्यू](../project-service/overview.md) </span><span class="sxs-lookup"><span data-stu-id="0529c-125">[Overview of Project Service Automation](../project-service/overview.md) </span></span>  
 <span data-ttu-id="0529c-126">[Project Service Automation कॉन्फ़िगर करें](../project-service/configure.md) </span><span class="sxs-lookup"><span data-stu-id="0529c-126">[Configure Project Service Automation](../project-service/configure.md) </span></span>  
 <span data-ttu-id="0529c-127">[खाता प्रबंधक मार्गदर्शिका](../project-service/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="0529c-127">[Account Manager Guide](../project-service/account-manager-guide.md) </span></span>  
 <span data-ttu-id="0529c-128">[परियोजना प्रबंधक मार्गदर्शिका](../project-service/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="0529c-128">[Project Manager Guide](../project-service/project-manager-guide.md) </span></span>  
 <span data-ttu-id="0529c-129">[संसाधन प्रबंधक मार्गदर्शिका](../project-service/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="0529c-129">[Resource Manager Guide](../project-service/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="0529c-130">समय, व्यय और सहयोग मार्गदर्शिका</span><span class="sxs-lookup"><span data-stu-id="0529c-130">Time, Expense, and Collaboration Guid</span></span>](../project-service/time-expense-collaboration-guide.md)
