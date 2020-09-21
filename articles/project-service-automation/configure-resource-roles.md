---
title: संसाधन भूमिकाएँ कॉन्फ़िगर करें
description: Project Service में संसाधन भूमिकाओं को कॉन्फ़िगर करने का तरीका
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 0a180069-17d9-40fd-b4af-9b8d50f373ea
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 6a32ec4380e847b897931b6691fa8f9784d0cee7
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751980"
---
# <a name="configure-resource-roles-project-service"></a><span data-ttu-id="17c9d-103">संसाधन भूमिकाएँ कॉन्फ़िगर करना (Project Service)</span><span class="sxs-lookup"><span data-stu-id="17c9d-103">Configure resource roles (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="17c9d-104">भूमिकाएँ, परियोजना योजना में महत्वपूर्ण भूमिका निभाती हैं, जैसे संसाधन आवश्यकताओं या परियोजना की लागत निर्धारित करना.</span><span class="sxs-lookup"><span data-stu-id="17c9d-104">Roles play an important part in project planning, when determining resource requirements or costs of a project.</span></span> <span data-ttu-id="17c9d-105">अपनी परियोजनाओं के लिए आवश्यक प्रत्येक भूमिका के लिए, आपको संसाधन भूमिका बनाने और उस भूमिका से कौशल और दक्षताएँ को संबद्ध करने की आवश्यकता होती है.</span><span class="sxs-lookup"><span data-stu-id="17c9d-105">For each role your projects require, you need to create a resource role and associate skills and proficiencies to that role.</span></span> <span data-ttu-id="17c9d-106">उदाहरण के लिए, हो सकता है कि आप डेवलपर, परियोजना प्रबंधक या गेम टेस्टर के लिए भूमिकाएँ बनाना चाहें.</span><span class="sxs-lookup"><span data-stu-id="17c9d-106">For example, you might want to create roles for developer, project manager, or game tester.</span></span> <span data-ttu-id="17c9d-107">आप भूमिका के लिए कौशल और दक्षता स्तर को भी सेट करेंगे.</span><span class="sxs-lookup"><span data-stu-id="17c9d-107">You’ll also set the skills and proficiency levels required for the role.</span></span>  
  
 <span data-ttu-id="17c9d-108">अपने संगठन के लिए प्रभावी परियोजना आकलन सुनिश्चित करने हेतु संसाधन भूमिकाएँ कॉन्फ़िगर करें.</span><span class="sxs-lookup"><span data-stu-id="17c9d-108">Configure resource roles to ensure effective project estimation for your organization.</span></span>  <span data-ttu-id="17c9d-109">साथ ही सुनिश्चित करें कि आपने बिलिंग प्रकार को सटीक रूप से सेट किया है.</span><span class="sxs-lookup"><span data-stu-id="17c9d-109">Also make sure you accurately set the billing type.</span></span> <span data-ttu-id="17c9d-110">गैर-प्रभार्य बिलिंग प्रकार के साथ सेट किया गया आइटम, अनुबंध या कोट पंक्तियों पर दिखाया नहीं जाता है.</span><span class="sxs-lookup"><span data-stu-id="17c9d-110">An item set with a non-chargeable billing type doesn’t show up on contract or quote lines.</span></span>  
  
 <span data-ttu-id="17c9d-111">संसाधन भूमिकाएँ सेट करने के बाद, आप मूल्य सूची के साथ लागत और विक्रय मूल्य सेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="17c9d-111">Once you’ve set up resource roles, you can set up cost and sales prices with a price list.</span></span>  
  
 <span data-ttu-id="17c9d-112">जोड़ी जाने वाली प्रत्येक इच्छित भूमिका के लिए, निम्न करें:</span><span class="sxs-lookup"><span data-stu-id="17c9d-112">For each role you want to add, do the following:</span></span>  
  
1.  <span data-ttu-id="17c9d-113">**Project Service > संसाधन भूमिकाएँ** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="17c9d-113">Go to **Project Service > Resource Roles**.</span></span>  
  
2.  <span data-ttu-id="17c9d-114">**नया** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="17c9d-114">Click **New**.</span></span>  
  
3.  <span data-ttu-id="17c9d-115">**सामान्य** क्षेत्र में, **नाम** फ़ील्ड में भूमिका के लिए एक नाम दर्ज करें और उसके बाद आवश्यकतानुसार अन्य फ़ील्ड भरें.</span><span class="sxs-lookup"><span data-stu-id="17c9d-115">In the **General** area, enter a name for the role in **Name**, and then fill in the other fields as necessary.</span></span>  
  
4.  <span data-ttu-id="17c9d-116">रिकॉर्ड बनाने के लिए, **सहेजें** पर क्लिक करें ताकि आप उसको संपादित करना जारी रख सकें.</span><span class="sxs-lookup"><span data-stu-id="17c9d-116">Click **Save** to create the record so you can continue editing it.</span></span>  
  
5.  <span data-ttu-id="17c9d-117">**कौशल** क्षेत्र में, कौशल जोड़ने के लिए **+** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="17c9d-117">In the **Skills** area, click **+** to add a skill.</span></span>  
  
6.  <span data-ttu-id="17c9d-118">**भूमिका योग्यता आवश्यकता** फलक में, **कौशल** फ़ील्ड में क्लिक करें, **खोजें** बटन पर क्लिक करें और उसके बाद एक कौशल चुनें.</span><span class="sxs-lookup"><span data-stu-id="17c9d-118">In the **Role competency requirement** pane, click in the **Skill** field, click the **Search** button, and then select a skill.</span></span>  
  
7.  <span data-ttu-id="17c9d-119">उस कौशल के लिए दक्षता चुनें और उसके बाद **सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="17c9d-119">Select a proficiency for that skill, and then click **Save**.</span></span>  
  
8.  <span data-ttu-id="17c9d-120">आवश्यकतानुसार कौशल जोड़ना जारी रखें.</span><span class="sxs-lookup"><span data-stu-id="17c9d-120">Continue adding skills as necessary.</span></span> <span data-ttu-id="17c9d-121">काम पूरा होने पर, स्‍क्रीन के निचले दाएँ कोने में स्थित **सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="17c9d-121">When you’re done, click **Save** at the bottom right corner of the screen.</span></span>  
  
9. <span data-ttu-id="17c9d-122">इस संसाधन भूमिका को परियोजना के उपयोग के लिए उपलब्ध बनाने हेतु, **सक्रिय करें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="17c9d-122">To make this resource role available for projects to use, click **Activate**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="17c9d-123">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="17c9d-123">See Also</span></span>  
 [<span data-ttu-id="17c9d-124">संसाधन सेट अप करें</span><span class="sxs-lookup"><span data-stu-id="17c9d-124">Set up resources</span></span>](../project-service/set-up-resources.md)
