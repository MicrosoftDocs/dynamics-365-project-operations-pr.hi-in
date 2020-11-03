---
title: संसाधनों की ज़रूरतों में से नामित संसाधनों को बुक करें
description: यह विषय सामान्य संसाधन आवश्यकता के लिए नामित संसाधनों की बुकिंग के बारे में जानकारी प्रदान करता है।
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 12/11/2018
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
ms.openlocfilehash: 20e3a904bc33360b194c0c53e58430c80d1ff55f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077905"
---
# <a name="book-named-resources-from-resource-requirements"></a><span data-ttu-id="e4e9e-103">संसाधनों की ज़रूरतों में से नामित संसाधनों को बुक करें</span><span class="sxs-lookup"><span data-stu-id="e4e9e-103">Book named resources from resource requirements</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="e4e9e-104">आप सामान्य संसाधन को बदलने के लिए ऐसा नामित संसाधन बुक कर सकते हैं जिसके पास संसाधन की आवश्यकता है।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-104">You can book a named resource to replace generic resource that has a resource requirement.</span></span>

1. <span data-ttu-id="e4e9e-105">Project Service Automation (PSA) में, **प्रोजेक्ट्स** पृष्ठ पर, **टीम** टैब पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-105">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab.</span></span>
2. <span data-ttu-id="e4e9e-106">सूची से संसाधन की आवश्यकता वाले सामान्य संसाधन का चयन करें और फिर **बुक** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-106">Select the generic resource that has a resource requirement from the list and then click **Book**.</span></span> <span data-ttu-id="e4e9e-107">या, संसाधन आवश्यकता खोलें और फिर **बुक** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-107">Or, open the resource requirement and then click **Book**.</span></span>


![एक सामान्य टीम के सदस्य की बुकिंग](media/RM-how-to-14.png)


3. <span data-ttu-id="e4e9e-109">**शेड्यूल सहायक** पृष्ठ पर, अपनी प्रोजेक्ट टीम पर बुक करने के लिए एक नामित संसाधन का चयन करें और फिर **बुक** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-109">On the **Schedule Assistant** page, select a named resource to book onto your project team and then click **Book**.</span></span>

![शेड्यूल सहायक का उपयोग कर एक सामान्य टीम के सदस्य को बुक करना](media/RM-how-to-15.png)

<span data-ttu-id="e4e9e-111">जब नामांकित संसाधन द्वारा बुकिंग पूरी और संतुष्ट हो जाती है, तो सामान्य संसाधन को नामित संसाधन से बदल दिया जाता है।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-111">When the booking is complete and fulfilled by a named resource, the generic resource is replaced with the named resource.</span></span>

![नामित टीम सदस्य एक सामान्य टीम के सदस्य की जगह](media/RM-how-to-16.png)

<span data-ttu-id="e4e9e-113">शेड्यूल पर असाइनमेंट नामित संसाधन के साथ भी अपडेट किए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-113">The assignments on the schedule are updated with the named resource as well.</span></span>

![नामित टीम सदस्य को प्रोजेक्ट कार्यों के लिए सौंपा गया](media/RM-how-to-17.png)

## <a name="fulfill-a-generic-resource-with-multiple-named-resources"></a><span data-ttu-id="e4e9e-115">कई नामित संसाधनों के साथ एक सामान्य संसाधन को पूरा करें</span><span class="sxs-lookup"><span data-stu-id="e4e9e-115">Fulfill a generic resource with multiple named resources</span></span>
<span data-ttu-id="e4e9e-116">कई नामित संसाधनों के साथ एक सामान्य संसाधन के लिए एक आवश्यकता को पूरा करना एक एकल नामित संसाधन को असाइन करने के समान है।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-116">Fulfilling a requirement for a generic resource with multiple named resources is similar to assigning a single named resource.</span></span> <span data-ttu-id="e4e9e-117">उदाहरण के लिए, पांच दिनों की अवधि और 120 घंटे के प्रयास के साथ एक कार्य है।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-117">For example, there is a task with a duration of five days and 120 hours of effort.</span></span> <span data-ttu-id="e4e9e-118">यह कार्य एक संसाधन द्वारा पूरा नहीं किया जा सकता है जो पांच दिन के सप्ताह में आठ घंटे तक कार्य करता है।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-118">This task can't be completed by one resource that works a typical eight-hour day over a five day week.</span></span> 

![एक कार्य जिसमें पांच दिनों में 120 घंटे के प्रयास की आवश्यकता होती है](media/RM-how-to-21.png)

<span data-ttu-id="e4e9e-120">आवश्यकता पांच दिनों में 120 घंटे की रोबोटिक्स इंजीनियरिंग की है, जो प्रति दिन 24 घंटे है।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-120">The requirement is for 120 hours of robotics engineering over five days, which is 24 hours per day.</span></span>

![प्रति दिन की आवश्यकता](media/RM-how-to-22.png)

<span data-ttu-id="e4e9e-122">यह एक उदाहरण है जब सामान्य संसाधन अनुरोध को पूरा करने के लिए कई नामित संसाधनों की आवश्यकता होती है।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-122">This is an example of when multiple named resources are needed to fulfill a generic resource request.</span></span> <span data-ttu-id="e4e9e-123">आवश्यकता को पूरा करने के लिए आपको कई संसाधन बुक करने होंगे।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-123">You will need to book multiple resources to fulfill the requirement.</span></span>

![आवश्यकता को पूरा करने के लिए कई संसाधनों की बुकिंग](media/RM-how-to-23.png)

<span data-ttu-id="e4e9e-125">इस परिदृश्य में मुख्य अंतर यह है कि कार्य करने के लिए सौंपी गई टीम पर सामान्य संसाधन रहता है और बुक किए गए संसाधन टीम के सदस्यों को पद के हिस्से के रूप में असाइन नहीं किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-125">The main difference in this scenario is that the generic resource remains on the team assigned to the task, and the booked named resource team members are not assigned as part of the position.</span></span> <span data-ttu-id="e4e9e-126">प्रोजेक्ट मैनेजर नामांकित संसाधनों के लिए उपयुक्त कार्य को असाइन कर सकता है।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-126">The project manager can assign the work as appropriate to the named resources.</span></span> <span data-ttu-id="e4e9e-127">**रीकॉन्सीलेशन** दृश्य कार्य असाइनमेंट को कार्य करने के लिए कई संसाधनों में बुकिंग को तोड़ने में एक प्रोजेक्ट प्रबंधक की सहायता कर सकता है।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-127">The **Reconciliation** view can assist a project manager in breaking up the bookings across multiple resources to task assignments.</span></span> <span data-ttu-id="e4e9e-128">यह स्वचालित रूप से नहीं किया जाता है क्योंकि यह किसी भी परिदृश्य में ऊपर दिए गए सरल उदाहरण की तुलना में अधिक जटिल है, जैसे कि आपके पास आवश्यकता को पूरा करने वाले कार्यों का एक बंडल है, प्रोजेक्ट प्रबंधक कैसे असाइन करना चाहता है, इस इरादे को सिस्टम द्वारा ग्रहण किए जाने की आवश्यकता है।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-128">This is not done automatically because in any scenario more complicated than the simple example above, such as where you have a bundle of tasks making up the requirement, the intent of how the project manager wants to assign, needs to be assumed by the system.</span></span> <span data-ttu-id="e4e9e-129">क्योंकि सिस्टम इरादे को समझ नहीं सकता है, संभावना है कि धारणाएं इरादे से अलग होंगी और एक गलत या अप्रत्याशित परिणाम होगा।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-129">Because the system can't understand intent, chances are that the assumptions will be different than intended and an incorrect or unpredictable result will happen.</span></span> <span data-ttu-id="e4e9e-130">अनुमानित परिणाम यह है कि सामान्य संसाधन तब तक असाइन रहता है जब तक कि प्रोजेक्ट मैनेजर जानबूझकर **रीकॉन्सीलेशन** की सहायता से असाइनमेंट नहीं बनाता है।</span><span class="sxs-lookup"><span data-stu-id="e4e9e-130">The predictable outcome is that the generic resource remains assigned until the project manager deliberately creates assignments, with the assistance of the **Reconciliation** view.</span></span>


