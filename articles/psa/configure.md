---
title: Project Service Automation कॉन्फ़िगर करें
description: Project Service को कॉन्फ़िगर करने के चरण
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: ef1724bb92e62ae21472e133fff0978c4faeeffa
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6002839"
---
# <a name="configure-project-service"></a><span data-ttu-id="8fcdc-103">Project Service कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="8fcdc-103">Configure Project Service</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="8fcdc-104">इससे पहले कि अपने खातों, परियोजनाओं और संसाधनों को प्रबंधित करने के लिए आप [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] में [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] स्वचालन क्षमताओं का उपयोग कर सकें, यह सुनिश्चित करने के लिए आपको कुछ कॉन्फ़िगरेशन चरण पूरे करने होंगे कि [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] समाधान आपके संगठन की आवश्यकताओं से मेल खाता है.</span><span class="sxs-lookup"><span data-stu-id="8fcdc-104">Before you can use the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] automation capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] to manage your accounts, projects, and resources, you need to complete a few configuration steps to ensure the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] solution matches your organization’s needs.</span></span> <span data-ttu-id="8fcdc-105">इन चरणों में शामिल हैं:</span><span class="sxs-lookup"><span data-stu-id="8fcdc-105">These steps include:</span></span>  
  
-   <span data-ttu-id="8fcdc-106">[समय इकाइयाँ सेट अप करें](../psa/set-up-time-units.md).</span><span class="sxs-lookup"><span data-stu-id="8fcdc-106">[Set up time units](../psa/set-up-time-units.md).</span></span> <span data-ttu-id="8fcdc-107">उत्पाद कैटलॉग में वे समय इकाइयाँ कॉन्फ़िगर करें, जिनका उपयोग आप अपनी परियोजनाओं को शेड्यूल और बिलिंग करने के आधार के रूप में करेंगे.</span><span class="sxs-lookup"><span data-stu-id="8fcdc-107">Configure the time units in the product catalog that you’ll use as a base for scheduling and billing your projects.</span></span>  
  
-   <span data-ttu-id="8fcdc-108">[मुद्रा और विनिमय दर सेट अप करें](../psa/set-up-currencies-exchange-rates.md).</span><span class="sxs-lookup"><span data-stu-id="8fcdc-108">[Set up currencies and exchange rates](../psa/set-up-currencies-exchange-rates.md).</span></span> <span data-ttu-id="8fcdc-109">अपनी परियोजनाओं में उपयोग की जाने वाली मुद्राएँ सेट करें.</span><span class="sxs-lookup"><span data-stu-id="8fcdc-109">Set up the currencies to use for your projects.</span></span>  
  
-   <span data-ttu-id="8fcdc-110">[संगठनात्मक इकाइयाँ बनाएँ](../psa/create-organizational-units.md).</span><span class="sxs-lookup"><span data-stu-id="8fcdc-110">[Create organizational units](../psa/create-organizational-units.md).</span></span> <span data-ttu-id="8fcdc-111">उन समूहों का सेट अप करें जिनका उपयोग आपकी कंपनी व्यवसाय को विभाजित करने के लिए करती है, चाहे भूगोल के आधार पर, व्यावसायिक फ़ंक्शन के आधार पर या अन्य तार्किक विभाग के आधार पर.</span><span class="sxs-lookup"><span data-stu-id="8fcdc-111">Set up the groups that your company uses to divide its business, whether by geography, business function, or other logical division.</span></span>  
  
-   <span data-ttu-id="8fcdc-112">[इनवॉइस आवृत्तियाँ सेट अप करें](../psa/set-up-invoice-frequencies.md).</span><span class="sxs-lookup"><span data-stu-id="8fcdc-112">[Set up invoice frequencies](../psa/set-up-invoice-frequencies.md).</span></span> <span data-ttu-id="8fcdc-113">वे समय अवधियाँ सेट करें जिनका उपयोग आप अपने ग्राहकों को बिल के लिए करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="8fcdc-113">Set up time periods that you want to use for billing your clients.</span></span>  
  
-   <span data-ttu-id="8fcdc-114">[लेनदेन श्रेणियाँ कॉन्फ़िगर करें](../psa/configure-transaction-categories.md).</span><span class="sxs-lookup"><span data-stu-id="8fcdc-114">[Configure transaction categories](../psa/configure-transaction-categories.md).</span></span> <span data-ttu-id="8fcdc-115">वे लेनदेने श्रेणियाँ सेट करें जिनमें आपके सलाहकार अपने बिल करने योग्य और बिना बिल करने योग्य व्यय चार्ज कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="8fcdc-115">Set up transaction categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="8fcdc-116">[व्यय श्रेणियाँ कॉन्फ़िगर करें](../psa/configure-expense-categories.md).</span><span class="sxs-lookup"><span data-stu-id="8fcdc-116">[Configure expense categories](../psa/configure-expense-categories.md).</span></span> <span data-ttu-id="8fcdc-117">वे श्रेणियाँ सेट करें जिनमें आपके सलाहकार अपने बिल करने योग्य और बिना बिल करने योग्य व्यय चार्ज कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="8fcdc-117">Set up the categories your consultants can charge their billable and unbillable expenses to.</span></span>  
  
-   <span data-ttu-id="8fcdc-118">[उत्पाद कैटलॉग आइटम बनाएँ](../psa/create-product-catalog-items.md).</span><span class="sxs-lookup"><span data-stu-id="8fcdc-118">[Create product catalog items](../psa/create-product-catalog-items.md).</span></span> <span data-ttu-id="8fcdc-119">जो उत्पाद आप बेचते हैं जैसे सॉफ़्टवेयर लायसेंस, उन्हें उत्पाद कैटलॉग में जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="8fcdc-119">Add the products you sell, such as software licenses, to the product catalog.</span></span>  
  
-   <span data-ttu-id="8fcdc-120">[एक मूल्य सूची बनाएँ](../psa/create-price-list.md).</span><span class="sxs-lookup"><span data-stu-id="8fcdc-120">[Create a price list](../psa/create-price-list.md).</span></span> <span data-ttu-id="8fcdc-121">इसके आधार पर कि आप अपने क्लायंट से उनकी परियोजना आवश्यकता के अनुसार प्रत्येक भूमिका के लिए उनसे कितना चार्ज करना चाहते हैं, विभिन्न मूल्य सूचियाँ कॉन्फ़िगर करें.</span><span class="sxs-lookup"><span data-stu-id="8fcdc-121">Configure different price lists, depending on how much you want to charge your clients for each role their project requires.</span></span>  
  
-   <span data-ttu-id="8fcdc-122">[संसाधन सेट अप करें](../psa/set-up-resources.md).</span><span class="sxs-lookup"><span data-stu-id="8fcdc-122">[Set up resources](../psa/set-up-resources.md).</span></span> <span data-ttu-id="8fcdc-123">अपनी परियोजनाओं के लिए जिन कौशल, दक्षता, संसाधन भूमिका और अन्य संसाधन जानकारी की आपको आवश्यकता होगी, उन्हें जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="8fcdc-123">Add the skills, proficiencies, resource roles, and other resource information that you’ll need for your projects.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="8fcdc-124">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="8fcdc-124">See Also</span></span>  
 <span data-ttu-id="8fcdc-125">[Project Service Automation का ओवरव्यू](../psa/overview.md) </span><span class="sxs-lookup"><span data-stu-id="8fcdc-125">[Overview of Project Service Automation](../psa/overview.md) </span></span>  
 <span data-ttu-id="8fcdc-126">[Project Service Automation कॉन्फ़िगर करें](../psa/configure.md) </span><span class="sxs-lookup"><span data-stu-id="8fcdc-126">[Configure Project Service Automation](../psa/configure.md) </span></span>  
 <span data-ttu-id="8fcdc-127">[खाता प्रबंधक मार्गदर्शिका](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="8fcdc-127">[Account Manager Guide](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="8fcdc-128">[परियोजना प्रबंधक मार्गदर्शिका](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="8fcdc-128">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 <span data-ttu-id="8fcdc-129">[संसाधन प्रबंधक मार्गदर्शिका](../psa/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="8fcdc-129">[Resource Manager Guide](../psa/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="8fcdc-130">समय, व्यय और सहयोग मार्गदर्शिका</span><span class="sxs-lookup"><span data-stu-id="8fcdc-130">Time, Expense, and Collaboration Guid</span></span>](../psa/time-expense-collaboration-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]