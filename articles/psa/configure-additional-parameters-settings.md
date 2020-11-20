---
title: अतिरिक्त मापदंड सेटिंग्स कॉन्फ़िगर करें
description: Project Service में अतिरिक्त पैरामीटर सेटिंग कॉन्फ़िगर करने का तरीका
author: JohnPBurrows
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: 5ce7ffd635b10689c8295d9349966450f11282d1
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4129365"
---
# <a name="configure-additional-parameter-settings-project-service"></a><span data-ttu-id="6a9be-103">अतिरिक्त पैरामीटर सेटिंग कॉन्फ़िगर करना (Project Service)</span><span class="sxs-lookup"><span data-stu-id="6a9be-103">Configure additional parameter settings (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="6a9be-104">जब आपने पिछले विषयों में आइटम कॉन्फ़िगर कर लिए हैं, तो आपको अपनी परियोजनाओं के लिए उपयोग करने के लिए अतिरिक्त परियोजना पैरामीटर सेट करना पड़ेगा.</span><span class="sxs-lookup"><span data-stu-id="6a9be-104">Once you’ve configured the items in previous topics, you need to set additional project parameters to use for your projects.</span></span> <span data-ttu-id="6a9be-105">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] को पहली बार स्‍थापित करने पर, आपने एक पैरामीटर सेटिंग बनाई थी, ताकि [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] के कार्य करने के लिए पहले सभी आवश्यक रिकॉर्ड्स बनाए जा सकें.</span><span class="sxs-lookup"><span data-stu-id="6a9be-105">When you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you created a parameters setting to first create all the records required for [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] to work.</span></span> <span data-ttu-id="6a9be-106">अब समय है कि वापस जाएँ और इन सेटिंग्स के लिए अतिरिक्त फ़ील्ड्स कॉन्फ़िगर करें.</span><span class="sxs-lookup"><span data-stu-id="6a9be-106">Now it’s time to go back and configure additional fields for these settings.</span></span>  
  
 <span data-ttu-id="6a9be-107">आपको निम्न सेटिंग्स कॉन्फ़िगर करने की आवश्यकता होगी:</span><span class="sxs-lookup"><span data-stu-id="6a9be-107">You’ll need to have configured the following settings:</span></span>  
  
-   <span data-ttu-id="6a9be-108">संगठनात्मक इकाई</span><span class="sxs-lookup"><span data-stu-id="6a9be-108">Organizational unit</span></span>  
  
-   <span data-ttu-id="6a9be-109">इनवॉइस आवृत्ति</span><span class="sxs-lookup"><span data-stu-id="6a9be-109">Invoice frequency</span></span>  
  
-   <span data-ttu-id="6a9be-110">कार्य घंटे टेम्पलेट</span><span class="sxs-lookup"><span data-stu-id="6a9be-110">Work hours template</span></span>  
  
-   <span data-ttu-id="6a9be-111">मूल्य सूची</span><span class="sxs-lookup"><span data-stu-id="6a9be-111">Price list</span></span>  
 
<span data-ttu-id="6a9be-112">इस चरण में, आप यह भी संकेत देंगे कि आपको किस प्रकार का संसाधन आवंटन चाहिए:</span><span class="sxs-lookup"><span data-stu-id="6a9be-112">In this step, you’ll also indicate what type of resource allocation you want:</span></span>  
  
- <span data-ttu-id="6a9be-113">**केंद्रीय**.</span><span class="sxs-lookup"><span data-stu-id="6a9be-113">**Central**.</span></span> <span data-ttu-id="6a9be-114">केवल संसाधन प्रबंधक परियोजनाओं के लिए संसाधनों को आबंटित कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="6a9be-114">Only resource managers can allocate resources to projects.</span></span>  
  
- <span data-ttu-id="6a9be-115">**हाइब्रिड**.</span><span class="sxs-lookup"><span data-stu-id="6a9be-115">**Hybrid**.</span></span> <span data-ttu-id="6a9be-116">संसाधन प्रबंधक, परियोजना प्रबंधक और खाता प्रबंधक, परियोजनाओं के लिए संसाधनों को आबंटित कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="6a9be-116">Resource managers, project managers, and account managers can allocate resources to projects.</span></span>  
  
 
<span data-ttu-id="6a9be-117">परियोजना पैरामीटर्स सेट करने के लिए:</span><span class="sxs-lookup"><span data-stu-id="6a9be-117">To set project parameters:</span></span>  
  
1. <span data-ttu-id="6a9be-118">**Project Service > पैरामीटर्स** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="6a9be-118">Go to **Project Service > Parameters**.</span></span>  
  
2. <span data-ttu-id="6a9be-119">उस पैरामीटर्स सेटिंग पर क्लिक करें, जिसे आप कॉन्फ़िगर करना चाहते हैं (जिसे आपने [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] को पहली बार स्‍थापित करते समय बनाया था) या नई बनाने के लिए **नया** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="6a9be-119">Click the parameters setting you want to configure (the one you created when you first installed [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)]), or click **New** to create a new one.</span></span>  
  
3. <span data-ttu-id="6a9be-120">**सामान्य** क्षेत्र में, अपने सभी परियोजना पैरामीटर्स के लिए सभी विकल्प सेट करें.</span><span class="sxs-lookup"><span data-stu-id="6a9be-120">In the **General** area, set all the options for your project parameters.</span></span>  
  
4. <span data-ttu-id="6a9be-121">**मूल्य सूची** क्षेत्र में, मूल्‍य सूची जोड़ने के लिए **+** पर क्लिक करें, **परियोजना पैरामीटर मूल्य सूची** ड्रॉप-डाउन सूची में एक मूल्‍य सूची चुनें और उसके बाद **सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="6a9be-121">In the **Price List** area, click **+** to add a price list, select a price list in the **Project Parameter Price List** drop-down list, and then click **Save**.</span></span>  
  
5. <span data-ttu-id="6a9be-122">स्‍क्रीन के निचले दाएँ कोने में दिए गए **सहेजें** बटन पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="6a9be-122">Click the **Save** button in the bottom right corner of the screen.</span></span>  

> [!NOTE]
> <span data-ttu-id="6a9be-123">Project Service के सही ढंग से काम करने के लिए परियोजना पैरामीटर रिकॉर्ड बनाए रखा जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="6a9be-123">The project parameter record must be maintained for Project Service to function correcly.</span></span> <span data-ttu-id="6a9be-124">इस रिकॉर्ड को हटाया नहीं जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="6a9be-124">This record should not be deleted.</span></span>

### <a name="see-also"></a><span data-ttu-id="6a9be-125">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="6a9be-125">See Also</span></span>  
 [<span data-ttu-id="6a9be-126">संसाधन सेट अप करें</span><span class="sxs-lookup"><span data-stu-id="6a9be-126">Set up resources</span></span>](../psa/set-up-resources.md)
