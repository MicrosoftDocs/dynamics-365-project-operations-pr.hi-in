---
title: जब कोई बुक करने योग्य संसाधन किसी परियोजना पर एकाधिक भूमिकाएँ भरता है, तो परियोजना की बिक्री और लागत का अनुमान लगाएँ
description: यह विषय उन मूल्य निर्धारण आयामों के बारे में जानकारी प्रदान करता है, जिन्हें किसी परियोजना पर एकाधिक भूमिकाएँ भरने वाले संसाधन के लिए मूल्य निर्धारण और लागत का समर्थन करने के लिए उपयोग किया जा सकता है.
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 8ddc827a4170c5576c0a4350b51e6a119094ac50
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077752"
---
# <a name="estimate-project-sales-and-costs-when-a-bookable-resource-fills-mulitple-roles-on-a-project"></a><span data-ttu-id="af46d-103">जब कोई बुक करने योग्य संसाधन किसी परियोजना पर एकाधिक भूमिकाएँ भरता है, तो परियोजना की बिक्री और लागत का अनुमान लगाएँ</span><span class="sxs-lookup"><span data-stu-id="af46d-103">Estimate project sales and costs when a bookable resource fills mulitple roles on a project</span></span> 

<span data-ttu-id="af46d-104">परियोजना-आधारित कंपनियों को अक्सर किसी न किसी परियोजना पर एकाधिक भूमिकाएँ निभाने के लिए एक संसाधन की आवश्यकता होती है.</span><span class="sxs-lookup"><span data-stu-id="af46d-104">Project-based companies often have the need for one resource to perform mulitple roles on a project.</span></span> <span data-ttu-id="af46d-105">इनमें से प्रत्येक भूमिका की कीमत और लागत अलग-अलग हो सकती है, जिसका मतलब है कि परियोजना पर एक ही संसाधन का समय प्रत्येक भूमिका के लिए बिल और लागत दरों के आधार पर एक अलग वित्तीय अनुमान हो सकता है.</span><span class="sxs-lookup"><span data-stu-id="af46d-105">Each of these roles could be priced and costed differently which means the same resource's time on the project could get a different financial estimate depending on the bill and cost rates for each of the roles.</span></span> <span data-ttu-id="af46d-106">Project Service Automation नामित संसाधन के लिए टीम के सदस्य रिकॉर्ड पर मूल्यों की स्थापना की अनुमति देता है और टीम के सदस्य को असाइन किए गए कार्यों में से प्रत्येक पर अलग-अलग ओवरराइड की अनुमति देता है.</span><span class="sxs-lookup"><span data-stu-id="af46d-106">Project Service Automation allows the setup of the values on the team member record for the named resource and allows for different overrides on each of the tasks that the team member is assigned to.</span></span>

<span data-ttu-id="af46d-107">निम्नलिखित उदाहरण समझता है कि कैसे इस मान का सरल ओवरराइड एक संसाधन को विभिन्न लागत और बिल दरों के साथ एक परियोजना में कई भूमिकाएँ निभाने की अनुमति देता है.</span><span class="sxs-lookup"><span data-stu-id="af46d-107">The following example  explains how the simple override of this value allows a resource to have multiple roles on a project with different cost and bill rates.</span></span>

## <a name="create-tasks"></a><span data-ttu-id="af46d-108">कार्य बनाएँ</span><span class="sxs-lookup"><span data-stu-id="af46d-108">Create tasks</span></span>
<span data-ttu-id="af46d-109">40 घंटे प्रत्येक के दो परियोजना कार्य बनाएँ, कार्य A और कार्य B. कार्य A को कार्य B के पूर्ववर्ती के रूप में चुनें.</span><span class="sxs-lookup"><span data-stu-id="af46d-109">Create two project tasks for 40 hours each, Task A and Task B. Select Task A as a predecessor to Task B.</span></span>

## <a name="set-up-role-and-organization-unit-for-a-generic-project-team-member"></a><span data-ttu-id="af46d-110">सामान्य परियोजना टीम के सदस्य के लिए भूमिका और संगठन इकाई स्थापित करें</span><span class="sxs-lookup"><span data-stu-id="af46d-110">Set up Role and Organization Unit for a generic project team member</span></span>

1. <span data-ttu-id="af46d-111">**शेड्यूल** पृष्ठ पर, कार्य A के लिए **कार्य** पंक्ति चुनें.</span><span class="sxs-lookup"><span data-stu-id="af46d-111">On the **Schedule** page, select the **Task** row for Task A.</span></span> 
2. <span data-ttu-id="af46d-112">**संसाधन** फ़ील्ड में, ड्रॉप-डाउन सूची से **बनाएँ** चुनें.</span><span class="sxs-lookup"><span data-stu-id="af46d-112">In the **Resources** field, select **Create** in the drop-down list.</span></span>
3. <span data-ttu-id="af46d-113">**टीम सदस्य त्वरित निर्माण** पृष्ठ पर, उस सामान्य टीम सदस्य के एट्रिब्यूट निर्दिष्ट करें, जो इस कार्य को कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="af46d-113">On the **Team Member Quick Create** page, specify the attributes of the generic team member who can perform this task.</span></span>
4. <span data-ttu-id="af46d-114">उपयुक्त भूमिका और संगठनात्मक इकाई चुने और फिर उसके बाद **सहेजें और बंद करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="af46d-114">Select the appropriate role and organizational unit, and then select **Save and Close**.</span></span> <span data-ttu-id="af46d-115">एक सामान्य टीम सदस्य बना दिया जाता है और यह कार्य असाइन किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="af46d-115">A generic team member is created and assigned to this task.</span></span> 

<span data-ttu-id="af46d-116">यही चरण कार्य B के लिए दोहराएँ और सुनिश्चित करें कि कार्य B के लिए बनाई गई सामान्य टीम के सदस्य की भूमिका और संगठनात्मक इकाई कार्य A से अलग है.</span><span class="sxs-lookup"><span data-stu-id="af46d-116">Repeat these steps for Task B and make sure that the role and organizational unit on the generic team member created for Task B is different than Task A.</span></span> 

## <a name="set-up-role-and-organization-unit-for-a-project-task"></a><span data-ttu-id="af46d-117">परियोजना कार्य के लिए भूमिका और संगठन इकाई स्थापित करें</span><span class="sxs-lookup"><span data-stu-id="af46d-117">Set up role and organization unit for a project task</span></span>

1. <span data-ttu-id="af46d-118">कार्य A बनाने के बाद, कार्य को चुनें और फिर उसके बाद **कार्य संपादित करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="af46d-118">After you create Task A, select the task, and then select **Edit task**.</span></span>
2. <span data-ttu-id="af46d-119">**कार्य विवरण** पृष्ठ पर, **भूमिका** और **संगठनात्मक इकाई** फ़ील्ड ढूंढें, वह मान जोड़ें जो उस संसाधन के लिए आवश्यक हैं, जो इस कार्य को करेगा.</span><span class="sxs-lookup"><span data-stu-id="af46d-119">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="af46d-120">यदि आप Project Service Automation डेमो डेटा का उपयोग करके इस परिदृश्य को पूरा कर रहे हैं, तो भूमिका के लिए **परामर्श लीड** और संगठनात्मक इकाई के रूप में **Fabrikam US** चुनें.</span><span class="sxs-lookup"><span data-stu-id="af46d-120">If you are completing this scenarios using Project Service Automation demo data, select **Consulting Lead** for the role, and **Fabrikam US** as the organizational unit.</span></span>

3. <span data-ttu-id="af46d-121">कार्य B चुने और फिर उसके बाद **कार्य संपादित करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="af46d-121">Select Task B and then select **Edit task**.</span></span>
4. <span data-ttu-id="af46d-122">**कार्य विवरण** पृष्ठ पर, **भूमिका** और **संगठनात्मक इकाई** फ़ील्ड ढूंढें, वह मान जोड़ें जो उस संसाधन के लिए आवश्यक हैं, जो इस कार्य को करेगा.</span><span class="sxs-lookup"><span data-stu-id="af46d-122">On the **Task Details** page, find the **Role** and **Organizational Unit** fields, add the values that are required of a resource that would perform this task.</span></span> <span data-ttu-id="af46d-123">सुनिश्चित करें कि **भूमिका** और **संगठनात्मक इकाई** में मान कार्य A के लिए अलग और कार्य B के लिए अलग हैं.</span><span class="sxs-lookup"><span data-stu-id="af46d-123">Make sure that the values in the **Role** and **Organizational Unit** fields are different for Task B from those for Task A.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="af46d-124">यदि आप Project Service Automation डेमो डेटा का उपयोग करके इस परिदृश्य को पूरा कर रहे हैं, तो भूमिका के लिए **नेटवर्क तकनीशियन** और संगठनात्मक इकाई के रूप में **Fabrikam US** चुनें.</span><span class="sxs-lookup"><span data-stu-id="af46d-124">If you are completing this scenarios using Project Service Automation demo data, select **Network Technician** for the role, and **Fabrikam US** as the organizational unit.</span></span>

5. <span data-ttu-id="af46d-125">**कार्य विवरण** पृष्ठ को सहेजें और बंद करें.</span><span class="sxs-lookup"><span data-stu-id="af46d-125">Save and close the **Task Details** page.</span></span> 

## <a name="team-member-and-estimates-behaviour"></a><span data-ttu-id="af46d-126">टीम के सदस्य और अनुमानित व्यवहार</span><span class="sxs-lookup"><span data-stu-id="af46d-126">Team member and estimates behaviour</span></span> 

1. <span data-ttu-id="af46d-127">**कार्य विवरण** पृष्ठ पर, **टीम के सदस्य** पर, दो सामान्य टीम के सदस्यों का चयन करें और फिर उसके बाद **आवश्यकताएं जनरेट करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="af46d-127">On the **Task Details** page, on the **Team Member** , select the two generic team Members and then select **Generate Requirements**.</span></span> <span data-ttu-id="af46d-128">इससे संसाधन आवश्यकताएँ जनरेट हो जाएँगी.</span><span class="sxs-lookup"><span data-stu-id="af46d-128">This will generate resource requirements.</span></span> 
2. <span data-ttu-id="af46d-129">**परामर्श लीड** के लिए टीम सदस्य पंक्ति चुनें और फिर उसके बाद **बुक करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="af46d-129">Select the team member row for **Consulting Lead** and then select **Book**.</span></span> <span data-ttu-id="af46d-130">शेड्यूल बोर्ड खुल जाता है और उस आवश्यकता के लिए संसाधन बुक करता है.</span><span class="sxs-lookup"><span data-stu-id="af46d-130">The schedule board opens and books a resource to that requirement.</span></span>
3. <span data-ttu-id="af46d-131">**नेटवर्क तकनीशियन** के लिए टीम सदस्य पंक्ति चुनें और फिर उसके बाद **बुक करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="af46d-131">Select the team member row for **Network Technician** and the select **Book**.</span></span> <span data-ttu-id="af46d-132">शेड्यूल बोर्ड खुल जाता है और उस आवश्यकता के लिए उसी संसाधन को बुक करता है.</span><span class="sxs-lookup"><span data-stu-id="af46d-132">The schedule board opens and books the same resource on that requirement.</span></span>

### <a name="team-member-grid"></a><span data-ttu-id="af46d-133">टीम सदस्य ग्रिड</span><span class="sxs-lookup"><span data-stu-id="af46d-133">Team Member grid</span></span> 
<span data-ttu-id="af46d-134">**टीम सदस्य** ग्रिड पर, ध्यान दें कि दो सामान्य टीम सदस्य रिकॉर्ड हटा दिए गए हैं और उन्हें एक संसाधन से बदल दिया गया है.</span><span class="sxs-lookup"><span data-stu-id="af46d-134">On the **Team Member** grid, notice that the two generic team member records are deleted and have been replaced one resource.</span></span> <span data-ttu-id="af46d-135">उस संसाधन के लिए मूल्यों का एक सेट है, जो **भूमिका** और **संगठनात्मक इकाई** के लिए मूल्यों का डिफ़ॉल्ट सेट दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="af46d-135">There is one set of values for that resource that shows a default set of values for **Role** and **Organizational Unit**.</span></span>
<span data-ttu-id="af46d-136">जब आप उस टीम सदस्य रिकॉर्ड की पंक्ति का विस्तार करते हैं, तो आप उन दोनों कार्यों के लिए टीम सदस्य रिकॉर्ड पर अलग-अलग असाइनमेंट देख सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="af46d-136">When you expand the row of that Team Member record, you can see distinct assignments on the team member record for both of those tasks.</span></span> <span data-ttu-id="af46d-137">प्रत्येक असाइनमेंट पंक्ति में **भूमिका** और **संगठनात्मक इकाई** के लिए कार्य विशिष्ट मान हैं.</span><span class="sxs-lookup"><span data-stu-id="af46d-137">Each assignment row has task specific values for **Role** and **Organizational Unit**.</span></span> 

### <a name="estimates-grid"></a><span data-ttu-id="af46d-138">अनुमान ग्रिड</span><span class="sxs-lookup"><span data-stu-id="af46d-138">Estimates grid</span></span> 
<span data-ttu-id="af46d-139">जब आप **अनुमान** ग्रिड पर नेविगेट करते हैं, आप देखेंगे कि एक ही संसाधन के लिए दोनों असाइनमेंट की कीमत अलग-अलग है.</span><span class="sxs-lookup"><span data-stu-id="af46d-139">When you navigate to the **Estimates** grid, you will notice that both assignments for the same resource are priced differently.</span></span>
<span data-ttu-id="af46d-140">कार्य A पर संसाधन की असाइनमेंट की कीमत का निर्धारण करने के लिए **परामर्श लीड** के **भूमिका** एट्रिब्यूट मान का उपयोग किया गया है.</span><span class="sxs-lookup"><span data-stu-id="af46d-140">The assignment for the resource on Task A is priced using the **Role** attribute value of **Consulting Lead**.</span></span> <span data-ttu-id="af46d-141">कार्य B पर उसी संसाधन की असाइनमेंट की कीमत का निर्धारण करने के लिए **नत्व्र्क तकनीशियन** के **भूमिका** एट्रिब्यूट मान का उपयोग किया गया है.</span><span class="sxs-lookup"><span data-stu-id="af46d-141">The assignment for the same resource on Task B is priced using the **Role** attribute value of **Network Technician**.</span></span>





