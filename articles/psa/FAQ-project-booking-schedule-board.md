---
title: शेड्यूल बोर्ड से एक प्रोजेक्ट बुकिंग बनाएँ
description: यह विषय आपको जानकारी प्रदान करता है कि शेड्यूल बोर्ड से प्रोजेक्ट बुकिंग कैसे बनाते हैं।
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
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
ms.openlocfilehash: d33786a5d0a2485a06d174eb7afcbaaa2f337cf6
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5992968"
---
# <a name="create-a-project-booking-from-the-schedule-board"></a><span data-ttu-id="bf842-103">शेड्यूल बोर्ड से एक प्रोजेक्ट बुकिंग बनाएँ</span><span class="sxs-lookup"><span data-stu-id="bf842-103">Create a project booking from the Schedule board</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="bf842-104">आप सीधे प्रोजेक्ट की **टीम** टैब से या जेनेरिक टीम सदस्य असाइनमेंट से संसाधन की आवश्यकता जनरेट करके और फिर प्रोजेक्ट टीम के सदस्य के साथ, जनरेट की गई आवश्यकता की पूर्ति करके प्रोजेक्ट में संसाधन बुक कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="bf842-104">You can book a resource onto a project directly from the **Team** tab of the project or by generating a resource requirement from a generic team member assignment and then fulfilling the generated requirement with a project team member.</span></span>

<span data-ttu-id="bf842-105">आप सीधे शेड्यूल बोर्ड से भी प्रोजेक्ट में कोई संसाधन बुक कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="bf842-105">You can also book a resource onto a project directly from the Schedule board.</span></span> <span data-ttu-id="bf842-106">इसे करने के तीन मार्ग हैं:</span><span class="sxs-lookup"><span data-stu-id="bf842-106">There are three ways to do this:</span></span>

- <span data-ttu-id="bf842-107">**जनरेट की गई संसाधन आवश्यकता से बुक करें:** आप जेनेरिक संसाधन बनाने और किसी ऐसे प्रोजेक्ट में कार्य असाइन करने के बाद एक संसाधन आवश्यकता जनरेट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="bf842-107">**Book from a generated resource requirement:** You can generate a resource requirement after you create a generic resource and assign tasks within a project.</span></span>

- <span data-ttu-id="bf842-108">**प्राथमिक आवश्यकता से बुक:** प्राथमिक आवश्यकताएं **प्रोजेक्ट** टैब पर शेड्यूल बोर्ड पर दिखाई देती हैं।</span><span class="sxs-lookup"><span data-stu-id="bf842-108">**Book from the primary requirement:** The primary requirements show up on the Schedule board on the **Project** tab.</span></span> 

- <span data-ttu-id="bf842-109">**नई संसाधन आवश्यकता से बुक करें** आप शुरू से संसाधन आवश्यकता बना सकते हैं और उसे किसी प्रोजेक्ट के साथ संबद्ध कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="bf842-109">**Book from a new resource requirement:** You can create a resource requirement from scratch and associate it with a project.</span></span> <span data-ttu-id="bf842-110">शेड्यूल बोर्ड पर, संसाधन आवश्यकता **खुली आवश्यकताएँ** टैब में दिखाई देती है।</span><span class="sxs-lookup"><span data-stu-id="bf842-110">On the Schedule board, the resource requirement shows up on the **Open Requirements** tab.</span></span>

## <a name="book-from-a-generated-resource-requirement"></a><span data-ttu-id="bf842-111">जनरेट की गई संसाधन आवश्यकता से बुक करें</span><span class="sxs-lookup"><span data-stu-id="bf842-111">Book from a generated resource requirement</span></span>

<span data-ttu-id="bf842-112">आप एक जेनेरिक संसाधन बना सकते हैं और उसे एक कार्य या किसी प्रोजेक्ट में एकाधिक कार्य असाइन कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="bf842-112">You can create a generic resource and assign it one or more tasks within a project.</span></span> <span data-ttu-id="bf842-113">फिर आप जेनेरिक टीम सदस्य से एक संसाधन आवश्यकता जनरेट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="bf842-113">Then you can generate a resource requirement from the generic team member.</span></span> 

1.  <span data-ttu-id="bf842-114">शेड्यूल बोर्ड पर, यह संसाधन **खुली आवश्यकताएँ** टैब में दिखाई देगा। यदि आपके पास कई खुली आवश्यकताएँ हैं तो आपको ग्रिड पर स्तंभ फ़िल्टर्स का उपयोग करने की आवश्यकता हो सकती है।</span><span class="sxs-lookup"><span data-stu-id="bf842-114">On the Schedule board, this resource will show up on the **Open Requirements** tab. You might need to use column filters on the grid if you have many open requirements.</span></span> 

    <span data-ttu-id="bf842-115">![शेड्यूल बोर्ड पर आवश्यकता टैब खोलें](media/FAQ-Project-Booking-Schedule-Board-1.png "बुकिंग और असाइनमेंट तालिका का स्क्रीनशॉट")</span><span class="sxs-lookup"><span data-stu-id="bf842-115">![Open Requirements tab on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-1.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="bf842-116">आवश्यकता का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="bf842-116">Select the requirement.</span></span> <span data-ttu-id="bf842-117">**उपलब्धता ढूँढें** टैब चयनित पंक्ति के शीर्ष पर प्रदर्शित होंगे।</span><span class="sxs-lookup"><span data-stu-id="bf842-117">The **Find Availability** tab will appear at the top of the selected row.</span></span>
 
3. <span data-ttu-id="bf842-118">जब आप टैब चुनते हैं, शेड्यूल बोर्ड का शेड्यूल असिस्टेंट मोड खुलता है और फिर उन उपलब्ध संसाधनों को फ़िल्टर करता है जो संसाधन की आवश्यकता को पूरा करते हैं।</span><span class="sxs-lookup"><span data-stu-id="bf842-118">When you select the tab, the Schedule Assistant mode of the Schedule board opens and then filters the available resources that meet the resource requirement.</span></span> <span data-ttu-id="bf842-119">उसके बाद, आप एक संसाधन बुक कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="bf842-119">After that, you can book a resource.</span></span>

4. <span data-ttu-id="bf842-120">आप चयनित पंक्ति को शेड्यूल बोर्ड के निचले भाग से खींचकर उसे ऊपर मौजूद ग्रिड में संसाधन कक्ष तक छोड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="bf842-120">You can also drag and drop the selected row from the bottom of the Schedule board to a resource cell in the grid above.</span></span> <span data-ttu-id="bf842-121">जब आप उसे छोड़ते हैं, तो वह दाईं ओर **संसाधन बुकिंग बनाएँ** पैनल को खोलता है.</span><span class="sxs-lookup"><span data-stu-id="bf842-121">When you drop it, it opens the **Create Resource Booking** panel on the right.</span></span>

    <span data-ttu-id="bf842-122">**बुक करें** का चयन करना प्रोजेक्ट टीम में संसाधन को बुक करता है.</span><span class="sxs-lookup"><span data-stu-id="bf842-122">Selecting **Book** books the resource onto the project team.</span></span>

![संसाधन बुकिंग पैनल बनाएँ](media/FAQ-Project-Booking-Schedule-Board-6.png "")
 

## <a name="book-from-the-primary-requirement"></a><span data-ttu-id="bf842-124">प्राथमिक आवश्यकता से बुक करें</span><span class="sxs-lookup"><span data-stu-id="bf842-124">Book from the Primary Requirement</span></span>

<span data-ttu-id="bf842-125">Project Service में प्रोजेक्ट बनाना स्वचालित रूप से एक संसाधन आवश्यकता बनाता है जिसे प्राथमिक आवश्यकता कहा जाता है.</span><span class="sxs-lookup"><span data-stu-id="bf842-125">Creating a project in Project Service automatically creates a resource requirement called the Primary Requirement.</span></span> <span data-ttu-id="bf842-126">यह एक रिक्त आवश्यकता है, कोई आवश्यकता जनरेट किए बिना या शुरू से आवश्यकता बनाए बिना शेड्यूल बोर्ड के साथ संसाधन को बुक करने के लिए जिसका उपयोग किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="bf842-126">This is an empty requirement that is used to quickly book a resource with the Schedule board without generating a requirement or creating one from scratch.</span></span> <span data-ttu-id="bf842-127">क्योंकि आवश्यकता रिक्त है, इसलिए आपको दिनांकों के साथ-साथ आबंटन विधि और घंटे, यदि लागू हों, निर्दिष्ट करने होंगे।</span><span class="sxs-lookup"><span data-stu-id="bf842-127">Because the requirement is empty, you’ll need to specify dates as well as the allocation method and hours, if applicable.</span></span> 

1. <span data-ttu-id="bf842-128">प्राथमिक आवश्यकता के साथ किसी संसाधन को बुक करने के लिए, शेड्यूल बोर्ड पर, **प्रोजेक्ट** टैब का चयन करें। यदि आपके पास कई प्रोजेक्ट्स हैं तो आपको **प्रोजेक्ट** स्तंभ पर स्तंभ फ़िल्टर का उपयोग करने की आवश्‍यकता पड़ सकती है।</span><span class="sxs-lookup"><span data-stu-id="bf842-128">To book a resource with the Primary Requirement, on the Schedule board, select the **Project** tab. You might need to use the column filter on the **Project** column if you have many projects.</span></span>

   <span data-ttu-id="bf842-129">![शेड्यूल बोर्ड पर कॉलम फिल्टर](media/FAQ-Project-Booking-Schedule-Board-2.png "बुकिंग और असाइनमेंट तालिका का स्क्रीनशॉट")</span><span class="sxs-lookup"><span data-stu-id="bf842-129">![Column filters on the Schedule board](media/FAQ-Project-Booking-Schedule-Board-2.png "Screenshot of bookings and assignments table")</span></span>

2. <span data-ttu-id="bf842-130">ऐसी आवश्यकता का चयन करें केवल जिसका नाम प्रोजेक्ट के नाम के समान है और अवधि शून्य 0 है।</span><span class="sxs-lookup"><span data-stu-id="bf842-130">Select the requirement that only has the project name as its name and has a duration of zero (0).</span></span>

3. <span data-ttu-id="bf842-131">पंक्ति में प्रकट होने वाली **उपलब्धता ढूँढें** टैब का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="bf842-131">Select the **Find Availability** tab that appears on the row.</span></span> <span data-ttu-id="bf842-132">यह शेड्यूल बोर्ड को शेड्यूल सहायक मोड में डालता है और उपलब्ध संसाधन दिखाता है जिन्हें प्रोजेक्ट पर बुक किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="bf842-132">This puts the Schedule board in Schedule Assistant mode and shows the available resources that can be booked onto the project.</span></span>

4. <span data-ttu-id="bf842-133">क्योंकि **प्राथमिक आवश्यकता** शून्य (0) अवधि के साथ एक रिक्त आवश्यकता है, इसलिए आपको किसी संसाधन का चयन और उसे बुक करते समय **संसाधन बुकिंग बनाएँ** पैनल पर अवधि सेट करनी होगी।</span><span class="sxs-lookup"><span data-stu-id="bf842-133">Because a **Primary Requirement** is an empty requirement with zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when selecting and booking a resource.</span></span>

5. <span data-ttu-id="bf842-134">आप शेड्यूल बोर्ड के निचले भाग में **प्रोजेक्ट प्राथमिक आवश्यकता** का चयन भी कर सकते हैं और खींचें और उसे बुक करने के लिए उसे किसी संसाधन पर खींचकर छोड़ें।</span><span class="sxs-lookup"><span data-stu-id="bf842-134">You can also select the **Project Primary Requirement** at the bottom of the Schedule board and drag and drop it on a resource to book it.</span></span>
 
    <span data-ttu-id="bf842-135">क्योंकि **प्राथमिक आवश्यकता** एक रिक्त आवश्यकता है जिसकी शून्य (0) अवधि है, इसलिए आपको किसी संसाधन का चयन और उसे बुक करते समय **संसाधन बुकिंग बनाएँ** पैनल पर अवधि सेट करनी होगी।</span><span class="sxs-lookup"><span data-stu-id="bf842-135">Because the **Primary Requirement** is an empty requirement that has zero (0) duration, you’ll need to set the duration on the **Create Resource Booking** panel when you select and book a resource.</span></span>
 
    <span data-ttu-id="bf842-136">जब आप शेड्यूल बोर्ड पर **प्राथमिक आवश्यकता** के माध्यम से किसी संसाधन को बुक करते हैं, तो आप किसी भी असाइनमेंट के बिना उसे प्रोजेक्ट टीम में जोड़ते हैं।</span><span class="sxs-lookup"><span data-stu-id="bf842-136">When you book a resource through the **Primary Requirement** on the Schedule board, you add it to the project team without any assignments.</span></span>
 
## <a name="book-from-a-new-resource-requirement"></a><span data-ttu-id="bf842-137">नई संसाधन आवश्यकता से बुक करें</span><span class="sxs-lookup"><span data-stu-id="bf842-137">Book from a new resource requirement</span></span>
<span data-ttu-id="bf842-138">नई संसाधन आवश्यकता से बुकिंग करने के लिए निम्नलिखित चरणों को पूरा करें।</span><span class="sxs-lookup"><span data-stu-id="bf842-138">Complete the following steps to book from a new resource requirement.</span></span> 

1. <span data-ttu-id="bf842-139">**संसाधन आवश्यकताएँ** पर जाएँ, और फिर एक नई संसाधन आवश्यकता बनाने के लिए **नई** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="bf842-139">Go to **Resource Requirements**, and then select **New** to create a new resource requirement.</span></span>

2. <span data-ttu-id="bf842-140">**प्रोजेक्ट** टैब पर, प्रोजेक्ट की आवश्यकता को संबद्ध करने के लिए प्रोजेक्ट का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="bf842-140">On the **Project** tab, select a project to associate the requirement to the project.</span></span>
 
    <span data-ttu-id="bf842-141">शेड्यूल बोर्ड पर, यह नई आवश्यकता **खुली आवश्यकता** के रूप में दिखाई देती है, जिसे आप पूरा कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="bf842-141">On the Schedule board, this new requirement shows as an **Open Requirement** that you can fulfill.</span></span>

3. <span data-ttu-id="bf842-142">प्रोजेक्ट टीम में जोड़ने के लिए संसाधन बुक करें।</span><span class="sxs-lookup"><span data-stu-id="bf842-142">Book the resource to add it to the project team.</span></span>

4. <span data-ttu-id="bf842-143">अब जब संसाधन बुक किया हुआ है, आपको मैन्युअल रूप से कार्य असाइन करने होंगे।</span><span class="sxs-lookup"><span data-stu-id="bf842-143">Now that the resource is booked, you must assign tasks manually.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]