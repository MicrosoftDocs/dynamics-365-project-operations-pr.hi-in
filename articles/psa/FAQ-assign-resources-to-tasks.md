---
title: किसी कार्य के लिए कोई संसाधन असाइन करें
description: यह विषय संसाधनों को कार्य करने के तरीके के बारे में जानकारी प्रदान करता है।
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 9/27/2019
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
ms.openlocfilehash: 77f13d1e96b76dfea241fbf7a67d5676582f0235
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077889"
---
# <a name="assign-a-resource-to-a-task"></a><span data-ttu-id="cb9dd-103">किसी कार्य के लिए कोई संसाधन असाइन करें</span><span class="sxs-lookup"><span data-stu-id="cb9dd-103">Assign a resource to a task</span></span>

<span data-ttu-id="cb9dd-104">Microsoft Dynamics 365 Project Service Automation में किसी कार्य पर एक संसाधन असाइन करने के तीन तरीके हैं.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-104">There are three ways to assign a resource to a task in Microsoft Dynamics 365 Project Service Automation.</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="cb9dd-105">संसाधन को टीम के एक सदस्य के रूप में बुक करें, और फिर संसाधन को कार्य पर असाइन करें</span><span class="sxs-lookup"><span data-stu-id="cb9dd-105">Book a resource as a team member, and then assign the resource to a task</span></span>

<span data-ttu-id="cb9dd-106">आप प्रोजेक्ट टीम में एक संसाधन जोड़ सकते हैं, और फिर प्रोजेक्ट शेड्यूल में कार्यों के लिए संसाधन असाइन कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-106">You can add a resource to the project team, and then assign the resource to tasks in the project schedule.</span></span>

1. <span data-ttu-id="cb9dd-107">**टीम सदस्य** टैब पर, **नया** चयन कर एक नया टीम सदस्य जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-107">On the **Team Member** tab, add a new team member by selecting **New**.</span></span> 

2. <span data-ttu-id="cb9dd-108">**टीम सदस्य त्वरित बनाएँ** पैनल खोलता है, जहाँ आप बुक करने योग्य संसाधन का नाम चुन सकते हैं और एक भूमिका सेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-108">The **Team Member Quick Create** panel opens, where you can select the bookable resource name and set a role.</span></span> 

    <span data-ttu-id="cb9dd-109">संसाधन की बुकिंग के लिए निम्न आबंटन विधियों से एक विधि का चयन करें:</span><span class="sxs-lookup"><span data-stu-id="cb9dd-109">Select one of the following allocation methods for the resource’s booking:</span></span>

    - <span data-ttu-id="cb9dd-110">**पूर्ण क्षमता** निर्दिष्ट प्रारंभ से लेकर समाप्ति दिनांकों के लिए संसाधन की पूर्ण क्षमता बुक करता है.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-110">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="cb9dd-111">**प्रतिशत क्षमता** निर्दिष्ट प्रारंभ से लेकर समाप्ति दिनांकों के लिए संसाधन की किसी प्रतिशत क्षमता के लिए संसाधन बुक करता है.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-111">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="cb9dd-112">**समान रूप से वितरित घंटों द्वारा** निर्दिष्ट प्रारंभ और समाप्ति दिनांकों तक प्रतिदिन घंटों को समान रूप से वितरित करते हुए निर्दिष्ट घंटों के लिए संसाधन बुक करती है.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-112">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing them evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="cb9dd-113">**फ़्रंट लोड घंटों द्वारा** निर्दिष्ट प्रारंभ से लेकर समाप्ति दिनांकों तक प्रतिदिन फ़्रंट लोडिंग करते हुए निर्दिष्ट घंटों के लिए संसाधन बुक करता है.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-113">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>
    - <span data-ttu-id="cb9dd-114">**कोई नहीं** विधि टीम में संसाधन जोड़ती तो है लेकिन कोई ऐसी बुकिंग नहीं बनाती जो उसकी क्षमता को शामिल करती है.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-114">**None** adds the resource to the team but doesn’t create any bookings that absorb their capacity.</span></span>

3. <span data-ttu-id="cb9dd-115">किसी कार्य के लिए **शेड्यूल** ग्रिड पर, संसाधन सेल में **संसाधन** आइकन का चयन करें और फिर **टीम के सदस्यों** के तहत, आपके द्वारा जोड़े गए टीम के सदस्य का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="cb9dd-115">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell, and then under **Team Members** , select the team member you just added.</span></span> 

> [!NOTE]
> <span data-ttu-id="cb9dd-116">**टीम सदस्य** और **समन्वय** टैब पर, संसाधन बुक किए गए और असाइन किए गए घंटे दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-116">On the **Team Member** and **Reconciliation** tabs, the resource shows booked and assigned hours.</span></span> <span data-ttu-id="cb9dd-117">घंटे समान होने चाहिए, लेकिन इसकी आवश्यकता नहीं है क्योंकि बुकिंग और असाइनमेंट अच्छी तरह से जोड़े नहीं जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="cb9dd-117">The hours should be the same, but it isn't required as bookings and assignments are not tightly coupled.</span></span> <span data-ttu-id="cb9dd-118">**समन्वय** टैब आपको इसका विवरण प्रदान करती है कि वे कब भिन्न होते हैं, जैसे जब आप किसी संसाधन को उससे अधिक घंटे असाइन करते हैं जितने आपने बुक किए हैं.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-118">The **Reconciliation** tab gives you details when they are different, such as when you assign a resource more hours than you have booked.</span></span> <span data-ttu-id="cb9dd-119">यदि आवश्यक हो, तो आप संसाधन की बुकिंग को बढ़ाकर या असाइनमेंट को बदलकर जानकारी को सही कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="cb9dd-119">If needed, you can correct the information by extending the resource's bookings or changing the assignment.</span></span>

## <a name="create-a-generic-team-member-through-task-assignment"></a><span data-ttu-id="cb9dd-120">कार्य असाइनमेंट के माध्यम से एक जेनेरिक टीम सदस्य बनाएँ</span><span class="sxs-lookup"><span data-stu-id="cb9dd-120">Create a generic team member through task assignment</span></span>

<span data-ttu-id="cb9dd-121">जब आप कार्य असाइनमेंट के माध्यम से एक जेनेरिक टीम सदस्य बनाते हैं, आप एक कार्यों पर ऐसा प्लेसहोल्डर या जेनेरिक संसाधन बनाते हैं, जो उन नामित संसाधन के गुणों का वर्णन करता है, जिसे आप उस कार्य पर लगाना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-121">When you create a generic team member through task assignment, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks.</span></span> <span data-ttu-id="cb9dd-122">फिर आप एक आवश्यकता जनरेट करते हैं (या आवश्यकता का उपयोग करके एक अनुरोध सबमिट करते हैं) जिसका उपयोग नामित संसाधन को खोजने और बुक करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-122">You then generate a requirement (or submit a request using the requirement) that is used to search for and book the named resource.</span></span>

1. <span data-ttu-id="cb9dd-123">किसी कार्य के लिए **शेड्यूल** ग्रिड पर, संसाधन कक्ष में **संसाधन** चिह्न का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-123">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="cb9dd-124">प्लेसहोल्डर संसाधन के नाम के रूप में काम करने के लिए कोई नाम टाइप करें.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-124">Type a name to serve as the placeholder resource’s name.</span></span> <span data-ttu-id="cb9dd-125">उदाहरण के लिए, प्रोग्राम प्रबंधक.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-125">For example, Program Manager.</span></span>

3. <span data-ttu-id="cb9dd-126">**बनाएं** का चयन करें और **प्रोजेक्ट टीम के सदस्य त्वरित बनाएं** फ़ील्ड में, सामान्य संसाधन के लिए भूमिका निर्धारित करें।</span><span class="sxs-lookup"><span data-stu-id="cb9dd-126">Select **Create** , and in the **Quick Create Project Team Member** field, set the role for the generic resource.</span></span>

4. <span data-ttu-id="cb9dd-127">आप कार्य के लिए **संसाधन चयनकर्ता** पर संसाधन का चयन करके इस प्लेसहोल्डर संसाधन के लिए कार्य असाइन करना जारी रख सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-127">You can continue to assign tasks to this placeholder resource by selecting the resource on the **Resource Selector** for the task.</span></span> <span data-ttu-id="cb9dd-128">वे **टीम के सदस्य** के अंतर्गत सूचीबद्ध हैं.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-128">They’re listed under **Team Members**.</span></span>

5. <span data-ttu-id="cb9dd-129">जेनेरिक संसाधन असाइन करना पूरा करने के बाद, **टीम** टैब में जेनेरिक संसाधन का चयन करें, और फिर जेनेरिक संसाधन के लिए संसाधन आवश्यकता बनाने के लिए **आवश्यकता जनरेट करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-129">When you’re done assigning the generic resource, select the generic resource on the **Team** tab, and then select **Generate Requirement** to create a resource requirement for the generic resource.</span></span>

6. <span data-ttu-id="cb9dd-130">जेनेरिक संसाधन के लिए **बुक करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-130">Select **Book** for the generic resource.</span></span> <span data-ttu-id="cb9dd-131">फिर आप किसी वास्तविक संसाधन को ढूँढकर उसे बुक करने के लिए शेड्यूल बोर्ड का उपयोग कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-131">You can then use the Schedule board to find and book a real resource.</span></span> <span data-ttu-id="cb9dd-132">आप संसाधन प्रबंधक द्वारा पूरी की जाने वाली आवश्यकता भी सबमिट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-132">You can also submit the requirement for fulfillment by a resource manager.</span></span>

7. <span data-ttu-id="cb9dd-133">जब जेनेरिक संसाधन किसी नामित संसाधन द्वारा पूर्ण कर लिया जाता है, तो जेनेरिक संसाधन को टीम से निकाल दिया जाता है और जेनेरिक संसाधन के लिए कार्य असाइनमेंट उस नामित संसाधन को असाइन कर दिए जाते हैं, जिसने जेनेरिक संसाधन की संसाधन आवश्यकता को पूर्ण किया था.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-133">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>

## <a name="assign-a-named-resource-from-the-list-of-all-bookable-resources"></a><span data-ttu-id="cb9dd-134">सभी बुक करने योग्य संसाधनों की सूची से नामित संसाधन असाइन करें</span><span class="sxs-lookup"><span data-stu-id="cb9dd-134">Assign a named resource from the list of all bookable resources</span></span>

<span data-ttu-id="cb9dd-135">आप सभी बुक करने योग्य संसाधन खोजने के लिए **संसाधन चयनकर्ता** में खोज बॉक्स का उपयोग कर सकते हैं और उन्हें कार्य के लिए असाइन कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-135">You can use the search box in the **Resource Selector** to search all bookable resources and assign them to a task.</span></span>

<span data-ttu-id="cb9dd-136">इस तरह से सौंपे गए संसाधनों को बिना किसी बुकिंग के टीम में जोड़ा जाता है।</span><span class="sxs-lookup"><span data-stu-id="cb9dd-136">Resources assigned this way are added to the team without any bookings.</span></span> <span data-ttu-id="cb9dd-137">यह टीम के सदस्य को जोड़ने और आवंटन विधि के रूप में किसी को भी नहीं चुनने के समान है।</span><span class="sxs-lookup"><span data-stu-id="cb9dd-137">This is similar to adding a team member and selecting None as the allocation method.</span></span> <span data-ttu-id="cb9dd-138">संसाधन को केवल टीम असाइनमेंट और बुकिंग में कमी वाले संसाधनों के रूप में **टीम** और **रीकॉन्सीलेशन** टैब में प्रदर्शित किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="cb9dd-138">The resource is displayed in the **Team** and **Reconciliation** tabs as resources with only assignments and a booking deficit.</span></span> <span data-ttu-id="cb9dd-139">यदि आप उनकी उपलब्धता का उपयोग करना चाहते हैं तो उन्हें बुक करें.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-139">Book them if you want to use their availability.</span></span>

1. <span data-ttu-id="cb9dd-140">किसी कार्य के लिए **शेड्यूल** ग्रिड पर, संसाधन कक्ष में **संसाधन** चिह्न का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-140">On the **Schedule** grid for a task, select the **Resource** icon in the resource cell.</span></span>

2. <span data-ttu-id="cb9dd-141">नाम टाइप करना प्रारंभ करें.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-141">Start typing a name.</span></span> <span data-ttu-id="cb9dd-142">**अन्य संसाधन** के अंतर्गत **संसाधन चयनकर्ता** में नाम के लिए खोज परिणाम प्रदर्शित किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-142">The search results for the name are displayed in the **Resource Selector** under **Other Resources**.</span></span>

3. <span data-ttu-id="cb9dd-143">कार्य को जो संसाधन आप असाइन करना चाहते हैं उन्हें चुनें.</span><span class="sxs-lookup"><span data-stu-id="cb9dd-143">Select the resource that you want to assign to the task.</span></span>

