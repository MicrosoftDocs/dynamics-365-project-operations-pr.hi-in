---
title: समय क्षेत्र का प्रबंधन करें
description: जब कोई परियोजना बनाई जाती है, तो उसका समय क्षेत्र लागू हुए कार्य घंटे के टेम्पलेट में परिभाषित समय क्षेत्र पर आधारित होता है.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 278b226c88c2f441262eb5be0504f34a1964848c
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4119825"
---
# <a name="manage-time-zones"></a><span data-ttu-id="f5a58-103">समय क्षेत्र का प्रबंधन करें</span><span class="sxs-lookup"><span data-stu-id="f5a58-103">Manage time zones</span></span>

<span data-ttu-id="f5a58-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="f5a58-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


## <a name="projects"></a><span data-ttu-id="f5a58-105">प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="f5a58-105">Projects</span></span>

<span data-ttu-id="f5a58-106">जब कोई परियोजना बनाई जाती है, तो समय क्षेत्र लागू हुए कार्य घंटे टेम्पलेट में परिभाषित समय क्षेत्र पर आधारित होता है.</span><span class="sxs-lookup"><span data-stu-id="f5a58-106">When a project is created, the time zone is based on the time zone defined in the applied work hour template.</span></span> <span data-ttu-id="f5a58-107">**परियोजना** के लिए, तिथियां हमेशा उपयोगकर्ता के समय क्षेत्र के सापेक्ष होती हैं, जो **कार्य** टैब को छोड़कर प्रत्येक टैब पर लॉग इन किया जाता है. जब आप कार्य विभाजन संरचना को देखते हैं, तो तिथियां हमेशा परियोजना के समय क्षेत्र में प्रदर्शित की जाएंगी.</span><span class="sxs-lookup"><span data-stu-id="f5a58-107">On the **Project** for, the dates are always relative to the time zone of the user that is logged in on each tab, except the **Task** tab. When you view the work breakdown structure, the dates will always be displayed in the project’s time zone.</span></span>

## <a name="tasks"></a><span data-ttu-id="f5a58-108">कार्य</span><span class="sxs-lookup"><span data-stu-id="f5a58-108">Tasks</span></span>

<span data-ttu-id="f5a58-109">जब कोई कार्य बनाया जाता है, तो परियोजना के कार्य घंटों द्वारा शुरू होने वाला समय, खत्म होने का समय और घंटे/दिन नियंत्रित होता है.</span><span class="sxs-lookup"><span data-stu-id="f5a58-109">When a task is created, the start time, end time, and hours/day is controlled by the working hours of the project.</span></span> <span data-ttu-id="f5a58-110">उदाहरण के लिए, यदि कोई कार्य ऐसी परियोजना के साथ बनाया जाता है जिसका समय क्षेत्र -8 PST है और इसमें निम्नलिखित कार्य घंटे हैं: सुबह 9:00 बजे से शाम 5:00 बजे तक सोमवार से शुक्रवार तक, तो किसी असाइनमेंट के बिना बनाया गया कोई भी कार्य परियोजना कैलेंडर के शुरू होने वाले समय और खत्म होने के समय का संदर्भ रखेगा.</span><span class="sxs-lookup"><span data-stu-id="f5a58-110">For example, if a task is created with a project whose time zone is -8 PST and has the following working hours: 9:00 AM to 5:00 PM Monday to Friday, any task created without an assignment will respect the start time and end time of the project calendar.</span></span>

## <a name="manage-resources-with-time-zones"></a><span data-ttu-id="f5a58-111">समय क्षेत्र के साथ संसाधनों का प्रबंधन</span><span class="sxs-lookup"><span data-stu-id="f5a58-111">Manage resources with time zones</span></span>

<span data-ttu-id="f5a58-112">**बुकिंग का विस्तार करें**, का उपयोग करते समय सटीक और अनुमानित परिणामों के लिए, दो प्रमुख आवश्यकताएं हैं जिन्हें पूरा किया जाना चाहिए:</span><span class="sxs-lookup"><span data-stu-id="f5a58-112">For accurate and predictable results when using **Extend Booking**, there are two key prerequisites that must be met:</span></span>  

- <span data-ttu-id="f5a58-113">उपयोगकर्ता को सिस्टम के **निजीकरण सेटिंग्सस** में परिभाषित समय क्षेत्र से मेल खाने के लिए अपने डिवाइस के समय क्षेत्र को कॉन्फ़िगर करना होगा.</span><span class="sxs-lookup"><span data-stu-id="f5a58-113">The user must configure their device's time zone to match the time zone defined in the system's **Personalization Settings**.</span></span>
 
  ![Windows 10 में समय क्षेत्र सेटिंग](media/reconcile-assignments-03.png)

  ![वैयक्तिकरण सेटिंग में समय क्षेत्र सेटिंग](media/reconcile-assignments-04.png)
 
- <span data-ttu-id="f5a58-116">बुक करने योग्य संसाधन में कम से कम एक मिनट का काम करने का समय होना चाहिए जो अनुरोध किए गए विस्तार को परिभाषित करने के लिए उपयोग की जाने वाली रूपरेखा के साथ ओवरलैप होता है.</span><span class="sxs-lookup"><span data-stu-id="f5a58-116">The bookable resource must have at least one minute of working time that overlaps with the contours that are used to define the requested extension.</span></span> <span data-ttu-id="f5a58-117">उदाहरण के लिए, सुबह 9:00 बजे और शाम 7:00 बजे के बीच पड़ने वाले काम के घंटों के साथ निम्नलिखित संसाधन.</span><span class="sxs-lookup"><span data-stu-id="f5a58-117">For example, the following resources with working hours that fall between 9:00 AM and 7:00 PM.</span></span> 

  ![संसाधन कोंटूरों की तुलना](media/reconcile-assignments-05.png)

<span data-ttu-id="f5a58-119">निम्न तालिका दर्शाती है:</span><span class="sxs-lookup"><span data-stu-id="f5a58-119">The following table shows:</span></span>

- <span data-ttu-id="f5a58-120">एक परियोजना कैलेंडर टेम्पलेट</span><span class="sxs-lookup"><span data-stu-id="f5a58-120">A project calendar template</span></span>
- <span data-ttu-id="f5a58-121">संसाधन A: इस संसाधन का कैलेंडर और समय क्षेत्र परियोजना के समान ही है.</span><span class="sxs-lookup"><span data-stu-id="f5a58-121">Resource A: This resource has the same calendar and is in the same time zone as the project.</span></span> <span data-ttu-id="f5a58-122">बुकिंग शुरू होने का समय सुबह 9:00 बजे होगा.</span><span class="sxs-lookup"><span data-stu-id="f5a58-122">The start time of the bookings will be 9:00 AM.</span></span>
- <span data-ttu-id="f5a58-123">संसाधन बी: यह संसाधन परियोजना की तुलना में एक अलग समय क्षेत्र में स्थित है और अपने समय क्षेत्र में सुबह 7:00 बजे शुरू होता है.</span><span class="sxs-lookup"><span data-stu-id="f5a58-123">Resource B: This resource is located in a different time zone than the project and starts at 7:00 AM in their time zone.</span></span> <span data-ttu-id="f5a58-124">हालाँकि, बुकिंग सुबह 9:00 बजे से शुरू होगी, क्योंकि यह असाइनमेंट कोंटूर का सबसे प्रारंभिक शुरुआती समय है.</span><span class="sxs-lookup"><span data-stu-id="f5a58-124">However, the bookings will begin at 9:00 AM as that is the earliest start time of the assignment contour.</span></span>
- <span data-ttu-id="f5a58-125">संसाधन सी और डी: संसाधन अलग-अलग समय क्षेत्रों में स्थित हैं, दोनों एक दूसरे से और परियोजना से अलग हैं, और उनकी बुकिंग उनके अपने उपलब्ध शुरू करने के समय से पहले शुरू नहीं होती है.</span><span class="sxs-lookup"><span data-stu-id="f5a58-125">Resources C and D: The resources are located in different time zones, both different from each other and the project, and their bookings start no earlier than their respective available start times.</span></span>

|<span data-ttu-id="f5a58-126">निकाय</span><span class="sxs-lookup"><span data-stu-id="f5a58-126">Entity</span></span>  |<span data-ttu-id="f5a58-127">कैलेंडर</span><span class="sxs-lookup"><span data-stu-id="f5a58-127">Calendar</span></span>  |
|-|-|
|<span data-ttu-id="f5a58-128">परियोजना कैलेंडर टेम्पलेट</span><span class="sxs-lookup"><span data-stu-id="f5a58-128">Project calendar template</span></span>   | ![परियोजना कैलेंडर](media/reconcile-assignments-06.png) |
|<span data-ttu-id="f5a58-130">संसाधन A</span><span class="sxs-lookup"><span data-stu-id="f5a58-130">Resource A</span></span>  | ![संसाधन A कैलेंडर](media/reconcile-assignments-06.png) |
|<span data-ttu-id="f5a58-132">संसाधन B</span><span class="sxs-lookup"><span data-stu-id="f5a58-132">Resource B</span></span>  |  ![संसाधन B कैलेंडर](media/reconcile-assignments-07.png) |
|<span data-ttu-id="f5a58-134">संसाधन C</span><span class="sxs-lookup"><span data-stu-id="f5a58-134">Resource C</span></span>  |  ![संसाधन C कैलेंडर](media/reconcile-assignments-08.png) |
|<span data-ttu-id="f5a58-136">संसाधन D</span><span class="sxs-lookup"><span data-stu-id="f5a58-136">Resource D</span></span>  | ![संसाधन D कैलेंडर](media/reconcile-assignments-09.png)  |
 
<span data-ttu-id="f5a58-138">जब आप **मेल** दृश्य पर नेविगेट करते हैं, तो संसाधन निर्धारण और संबंधित बुकिंग की कमी प्रदर्शित होती है.</span><span class="sxs-lookup"><span data-stu-id="f5a58-138">When you navigate to the **Reconciliation** view, the resource assignments and the associated booking shortages are displayed.</span></span>

![विस्तार से पहले समायोजन दृश्य](media/reconcile-assignments-10.png)

<span data-ttu-id="f5a58-140">प्रत्येक संसाधन के लिए बढ़ाये गये बुकिंग कार्यक्षमता का उपयोग कर लेने के बाद, प्रत्येक संसाधन के लिए बुकिंग सफलतापूर्वक बढ़ा दी जाती है क्योंकि प्रत्येक संसाधन के काम के घंटे कमी की रूपरेखा के साथ ओवरलैप कर जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="f5a58-140">After the extend booking functionality has been used for each resource, bookings are successfully extended for each resource because each resource’s working hours overlapped with the contours of the shortage.</span></span>

![बुकिंग विस्तार के बाद समायोजन दृश्य](media/reconcile-assignments-11.png) 

<span data-ttu-id="f5a58-142">ध्यान दें कि बुकिंग के विवरण पर करीब से नजर डालने से बुकिंग के शुरुआती समय में अंतर दिखाई देता है।</span><span class="sxs-lookup"><span data-stu-id="f5a58-142">Notice that a closer look at the details of the bookings shows differences in the start time of the bookings.</span></span> <span data-ttu-id="f5a58-143">बुकिंग, असाइनमेंट की रूपरेखा के शुरु होने के समय से पहले और संसाधन के लिए शुरू होने के उपलब्ध समय से पहले शुरू नहीं होती है.</span><span class="sxs-lookup"><span data-stu-id="f5a58-143">The bookings start no earlier than the start time of the assignment contour and no earlier than the available start time of the resource.</span></span>

![शेड्यूल बोर्ड में संसाधनों की नई बुकिंग](media/reconcile-assignments-12.png)
