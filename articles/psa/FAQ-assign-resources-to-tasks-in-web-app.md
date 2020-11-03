---
title: मैं वेब ऐप में किसी कार्य को एक बुक करने योग्य संसाधन कैसे असाइन करूं
description: उन तरीकों का अवलोकन जिनसे आप बुक करने योग्य संसाधनों को असाइन कर सकते हैं।
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
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
ms.openlocfilehash: 7b95eff52351904f97c62b3806f17b02db47860b
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077888"
---
# <a name="how-do-i-assign-a-bookable-resource-to-a-task-in-the-web-app-project-service-app-v2x"></a><span data-ttu-id="34bbc-103">मैं वेब अनुप्रयोग (Project Service अनुप्रयोग v2.x) में एक बुक करने योग्य संसाधन को किसी कार्य पर कैसे असाइन करूँ?</span><span class="sxs-lookup"><span data-stu-id="34bbc-103">How do I assign a bookable resource to a task in the web app (Project Service app v2.x)?</span></span>

[!INCLUDE[cc-applies-to-psa-app-1.x-2.x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="34bbc-104">Project Service में किसी कार्य पर एक संसाधन असाइन करने के दो तरीके हैं.</span><span class="sxs-lookup"><span data-stu-id="34bbc-104">There are two ways to assign a resource to a task in Project Service.</span></span> <span data-ttu-id="34bbc-105">आप संसाधन को टीम के एक सदस्य के रूप में बुक कर सकते हैं और फिर उसे कार्य पर असाइन कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="34bbc-105">You can book a resource as a team member and then assign it to a task.</span></span> <span data-ttu-id="34bbc-106">या, आप कार्यों पर भूमिका असाइनमेंट के माध्यम से एक जेनेरिक टीम सदस्य बना सकते हैं, एक टीम उत्पन्न कर सकते हैं, और उसके बाद एक नामित संसाधन के साथ बैकिंग आवश्यकताएँ पूरी कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="34bbc-106">Or, you can create a generic team member through role assignment on tasks, generate a team, and then fulfill the backing requirements with a named resource.</span></span>

<span data-ttu-id="34bbc-107">ध्यान दें कि यदि आप किसी कार्य पर एक बुक करने योग्य संसाधन असाइन करना चाहते हैं, तो बुक करने योग्य संसाधन टीम सदस्य के पास पर्याप्त बुकिंग उपलब्ध होनी चाहिए.</span><span class="sxs-lookup"><span data-stu-id="34bbc-107">Note that if you’d like to assign a bookable resource to a task, the bookable resource team member must have enough available bookings.</span></span> <span data-ttu-id="34bbc-108">बुकिंग की स्थिति कमिट प्रकार हार्ड बुक और स्थिति कमिटेड होनी चाहिए.</span><span class="sxs-lookup"><span data-stu-id="34bbc-108">The status of the booking must be Commit Type Hard Book and Status Committed.</span></span> <span data-ttu-id="34bbc-109">यदि संसाधन के लिए पर्याप्त बुकिंग नहीं हैं, तो Project Service असाइनमेंट निकाल देता है और निम्न त्रुटि संदेश प्रदर्शित करता है:</span><span class="sxs-lookup"><span data-stu-id="34bbc-109">If there aren’t enough bookings for the resource, Project Service removes the assignment and displays the following error message:</span></span>

<span data-ttu-id="34bbc-110">*कार्य पर संसाधन असाइन करने में असमर्थ - निम्न संसाधन (संसाधनों) के पास प्रोजेक्ट से समक्ष बुक किए गए पर्याप्त घंटे मौजूद नहीं हैं*</span><span class="sxs-lookup"><span data-stu-id="34bbc-110">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project*</span></span>

## <a name="book-a-resource-as-a-team-member-and-then-assign-the-resource-to-a-task"></a><span data-ttu-id="34bbc-111">संसाधन को टीम के एक सदस्य के रूप में बुक करें और फिर संसाधन को कार्य पर असाइन करें</span><span class="sxs-lookup"><span data-stu-id="34bbc-111">Book a resource as a team member and then assign the resource to a task</span></span>

<span data-ttu-id="34bbc-112">इस विधि से आप प्रोजेक्ट टीम पर एक संसाधन जोड़ते हैं और उसके बाद प्रोजेक्ट शेड्यूल में संसाधन पर कार्य असाइन करते हैं.</span><span class="sxs-lookup"><span data-stu-id="34bbc-112">With this method you add a resource to the project team and then assign tasks to the resource in the project schedule.</span></span> <span data-ttu-id="34bbc-113">यह आप निम्न तरीके से करते हैं:</span><span class="sxs-lookup"><span data-stu-id="34bbc-113">Here’s how you do this:</span></span>
1.  <span data-ttu-id="34bbc-114">टीम सदस्य ग्रिड पर, **नया** चयन कर एक नया टीम सदस्य जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="34bbc-114">On the team member grid, add a new team member by selecting **New**.</span></span>
2.  <span data-ttu-id="34bbc-115">टीम सदस्य त्वरित बनाएँ स्क्रीन पर, बुक करने योग्य संसाधन नाम का चयन करें और एक भूमिका सेट करें.</span><span class="sxs-lookup"><span data-stu-id="34bbc-115">On the Team Member Quick Create screen, select the bookable resource name and set a role.</span></span>
3.  <span data-ttu-id="34bbc-116">**प्रारंभ दिनांक** और **समाप्ति दिनांक** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="34bbc-116">Select the **From** and **To** dates.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="34bbc-117">![टीम सदस्य जोड़ने का स्क्रीनशॉट](media/FAQ-Resources-to-Tasks2-1.png "टीम सदस्य जोड़ने का स्क्रीनशॉट")</span><span class="sxs-lookup"><span data-stu-id="34bbc-117">![Screenshot of adding team member](media/FAQ-Resources-to-Tasks2-1.png "Screenshot of adding team member")</span></span>
 
4.  <span data-ttu-id="34bbc-118">संसाधन बुक करने के लिए निम्न आबंटन विधियों से एक विधि का चयन करें:</span><span class="sxs-lookup"><span data-stu-id="34bbc-118">Select one of the following allocation methods for booking the resource:</span></span>
    - <span data-ttu-id="34bbc-119">**पूर्ण क्षमता** निर्दिष्ट प्रारंभ से लेकर समाप्ति दिनांकों के लिए संसाधन की पूर्ण क्षमता बुक करता है.</span><span class="sxs-lookup"><span data-stu-id="34bbc-119">**Full Capacity** books the resource’s full capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="34bbc-120">**प्रतिशत क्षमता** निर्दिष्ट प्रारंभ से लेकर समाप्ति दिनांकों के लिए संसाधन की किसी प्रतिशत क्षमता के लिए संसाधन बुक करता है.</span><span class="sxs-lookup"><span data-stu-id="34bbc-120">**Percentage Capacity** books the resource for a percentage of the resource's capacity for the specified from and to dates.</span></span>
    - <span data-ttu-id="34bbc-121">**समान रूप से वितरित घंटों द्वारा** निर्दिष्ट प्रारंभ से लेकर समाप्ति दिनांकों तक प्रतिदिन घंटों को समान रूप से वितरित करते हुए निर्दिष्ट घंटों के लिए संसाधन बुक करता है.</span><span class="sxs-lookup"><span data-stu-id="34bbc-121">**By Hours Distribute Evenly** books the resource for a specified number of hours, distributing it evenly per day over the specified from and to dates.</span></span>
    - <span data-ttu-id="34bbc-122">**फ़्रंट लोड घंटों द्वारा** निर्दिष्ट प्रारंभ से लेकर समाप्ति दिनांकों तक प्रतिदिन फ़्रंट लोडिंग करते हुए निर्दिष्ट घंटों के लिए संसाधन बुक करता है.</span><span class="sxs-lookup"><span data-stu-id="34bbc-122">**By Hours Front Load** books the resource for a specified number of hours, front-loading the per-day hours over the specified from and to dates.</span></span>

    <span data-ttu-id="34bbc-123">**कोई नहीं** का चयन न करें क्योंकि यह टीम पर संसाधन जोड़ता तो है, पर कोई ऐसी बुकिंग नहीं बनाता जो संसाधन की क्षमता को अपनाती है.</span><span class="sxs-lookup"><span data-stu-id="34bbc-123">Don’t select **None** because it adds the resource to the team but doesn’t create any bookings that absorb the resource's capacity.</span></span>
5.  <span data-ttu-id="34bbc-124">**सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="34bbc-124">Select **Save**.</span></span>

    <span data-ttu-id="34bbc-125">ध्यान दें कि बुकिंग के घंटे पर्याप्त होने चाहिए जो आपके द्वारा संसाधन को असाइन किए गए कार्य के प्रयास घंटे और दिनांकों की सीमाओं को कवर कर सके.</span><span class="sxs-lookup"><span data-stu-id="34bbc-125">Note that the hours of the booking must be enough to cover the effort hours and date ranges of the tasks that you assign this resource to.</span></span> <span data-ttu-id="34bbc-126">यदि आप संरेखण में नहीं है, तो आप कार्य पर संसाधन असाइन नहीं कर सकते.</span><span class="sxs-lookup"><span data-stu-id="34bbc-126">If they aren’t in alignment, you can’t assign the resource to the task.</span></span>

6.  <span data-ttu-id="34bbc-127">कार्य के लिए कार्य विश्लेषण संरचना (WBS) पर, संसाधन कक्ष ड्रॉपडाउन क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="34bbc-127">On the work breakdown structure (WBS) for the task, click the resource cell dropdown.</span></span> <span data-ttu-id="34bbc-128">फिर:</span><span class="sxs-lookup"><span data-stu-id="34bbc-128">Then:</span></span> 

    1. <span data-ttu-id="34bbc-129">**जोड़ें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="34bbc-129">Select **Add**.</span></span>
    2. <span data-ttu-id="34bbc-130">**संसाधन** के अंतर्गत ड्रॉपडाउन का चयन करें और उसके बाद स्वयं द्वारा ऊपर जोड़े गए टीम सदस्य का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="34bbc-130">Select the dropdown under **Resources** and select the team member you added above.</span></span>
    3. <span data-ttu-id="34bbc-131">**ठीक** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="34bbc-131">Select **OK**.</span></span> <span data-ttu-id="34bbc-132">अब टीम सदस्य कार्य पर असाइन हो गया है.</span><span class="sxs-lookup"><span data-stu-id="34bbc-132">The team member is now assigned to the task.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="34bbc-133">![WBS से संसाधन जोड़ने का स्क्रीनशॉट](media/FAQ-Resources-to-Tasks2-2.png "WBS से संसाधन जोड़ने का स्क्रीनशॉट")</span><span class="sxs-lookup"><span data-stu-id="34bbc-133">![Screenshot of adding resources with WBS](media/FAQ-Resources-to-Tasks2-2.png "Screenshot of adding resources with WBS")</span></span>
 
<span data-ttu-id="34bbc-134">टीम सदस्य ग्रिड पर, आपको असाइन घंटों के अंतर्गत संसाधन के असाइन किए गए कुल घंटे दिखाई देंगे.</span><span class="sxs-lookup"><span data-stu-id="34bbc-134">On the team member grid, you’ll see the aggregate of the resource’s assigned hours under Assigned Hours.</span></span> <span data-ttu-id="34bbc-135">यह संसाधन के लिए बुक किए गए घंटों से कम या बराबर होंगे.</span><span class="sxs-lookup"><span data-stu-id="34bbc-135">It will be less than or equal to the booked hours for the resource.</span></span> 

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="34bbc-136">![एक संसाधन के लिए निर्धारित घंटों का स्क्रीनशॉट](media/FAQ-Resources-to-Tasks2-3.png "एक संसाधन के लिए निर्धारित घंटों का स्क्रीनशॉट")</span><span class="sxs-lookup"><span data-stu-id="34bbc-136">![Screenshot of assigned hours for a resource](media/FAQ-Resources-to-Tasks2-3.png "Screenshot of assigned hours for a resource")</span></span>
 
<span data-ttu-id="34bbc-137">यदि आप संसाधन पर जिस कार्य को असाइन करने का प्रयास कर रहे हैं, वह संसाधन बुकिंग की समाप्ति दिनांक के बाद प्रारंभ होता है, तो संसाधन ड्रॉपडाउन में दिखाई नहीं देगा.</span><span class="sxs-lookup"><span data-stu-id="34bbc-137">If the task you’re attempting to assign to the resource starts after the end date of the resources bookings, the resource won’t appear in the dropdown.</span></span>

<span data-ttu-id="34bbc-138">ध्यान दें कि यदि संसाधन के पास कुछ अनअसाइन क्षमता शेष है, तो आप संसाधन को बुक किए गए घंटों की तुलना में अधिक घंटे असाइन कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="34bbc-138">Note that you can assign a resource to more hours than their booked hours if the resource has some remaining unassigned capacity.</span></span> <span data-ttu-id="34bbc-139">इस मामले में संसाधन केवल आंशिक रूप से अपनी बुकिंग तक असाइन किए जाएँगे.</span><span class="sxs-lookup"><span data-stu-id="34bbc-139">In this case the resource will only be partially assigned up to their bookings.</span></span> <span data-ttu-id="34bbc-140">आप कार्य विश्लेषण संरचना पर अनस्टाफ़ घंटे वाला स्तंभ जोड़कर इन शेष अनअसाइन कार्य घंटों को देख सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="34bbc-140">You can see these remaining unassigned task hours by adding the Unstaffed Hours column to the work breakdown structure.</span></span>

<span data-ttu-id="34bbc-141">यदि संसाधन उनके बुक किए गए घंटों पर असाइन किए गए जाते हैं (उनके बुक किए गए घंटे उनके असाइन किए गए घंटों के बराबर हैं), तो उन्हें अधिक कार्य असाइन करने का प्रयास करने पर आपको निम्न त्रुटि संदेश दिखाई देगा:</span><span class="sxs-lookup"><span data-stu-id="34bbc-141">If resources are assigned to their booked hours (their booked hours equals their assigned hours), you’ll see the following error message when you attempt to assign them further tasks:</span></span>

<span data-ttu-id="34bbc-142">*कार्य पर संसाधन असाइन करने में असमर्थ - निम्न संसाधन (संसाधनों) के पास प्रोजेक्ट से समक्ष बुक किए गए पर्याप्त घंटे मौजूद नहीं हैं.*</span><span class="sxs-lookup"><span data-stu-id="34bbc-142">*Unable to assign resource to task - Following resource(s) do not have sufficient hours booked against project.*</span></span>

<span data-ttu-id="34bbc-143">इसके अतिरिक्त, आपके द्वारा प्रोजेक्ट बनाते समय टीम पर जोड़ा गया डिफ़ॉल्ट प्रोजेक्ट प्रबंधक टीम सदस्य बिना किसी भी बुकिंग के जुड़ जाता है और उसे किसी कार्य पर असाइन नहीं किया जा सकता.</span><span class="sxs-lookup"><span data-stu-id="34bbc-143">Additionally, the default project manager team member that is added to the team when you create the project is added without any bookings and can’t be assigned to any task.</span></span> <span data-ttu-id="34bbc-144">वे कार्यों के लिए संसाधन ड्रॉपडाउन में दिखाई नहीं देंगे.</span><span class="sxs-lookup"><span data-stu-id="34bbc-144">They won’t show up in the resource dropdown for tasks.</span></span>

<span data-ttu-id="34bbc-145">यदि आप यह संसाधन असाइन करना चाहते हैं, तो आपको उन्हें टीम से निकालना होगा और फिर उन्हें कुछ नहीं के अलावा अन्य आबंटन विधि के साथ पुनः जोड़ना होगा.</span><span class="sxs-lookup"><span data-stu-id="34bbc-145">If you want to assign this resource, you need to remove them from the team and then re-add them with an allocation method other than None.</span></span> <span data-ttu-id="34bbc-146">प्रोजेक्ट बनाते समय इन्हें जोड़े जाने का कारण यह है कि प्रोजेक्ट के पास डिफ़ॉल्ट रूप से कम से कम एक प्रोजेक्ट अनुमोदक रहे.</span><span class="sxs-lookup"><span data-stu-id="34bbc-146">The reason they’re added to the team when the project is created is so that a project has at least one project approver by default.</span></span>

## <a name="create-a-generic-team-member-through-role-assignment-on-tasks"></a><span data-ttu-id="34bbc-147">कार्यों पर भूमिका असाइनमेंट के माध्यम से एक जेनेरिक टीम सदस्य बनाएँ</span><span class="sxs-lookup"><span data-stu-id="34bbc-147">Create a generic team member through role assignment on tasks</span></span>

<span data-ttu-id="34bbc-148">यह विधि सुनिश्चित करता है कि संसाधनों के पास कार्यों के लिए पर्याप्त बुकिंग मौजूद हैं.</span><span class="sxs-lookup"><span data-stu-id="34bbc-148">This method assures that resources have enough bookings for tasks.</span></span> <span data-ttu-id="34bbc-149">सबसे पहले, आप एक कार्यों पर ऐसा प्लेसहोल्डर या जेनेरिक संसाधन बनाते हैं, जो उन नामित संसाधन के गुणों का वर्णन करता है, जिसे आप उस कार्य पर लगाना चाहते हैं, इसके लिए आप कार्यों पर भूमिकाएँ असाइन करने के बाद एक टीम उत्पन्न करते हैं.</span><span class="sxs-lookup"><span data-stu-id="34bbc-149">First, you create a placeholder or generic resource that describes the characteristics of the named resource you ultimately want to work on the tasks by generating a team after assigning roles to tasks.</span></span> <span data-ttu-id="34bbc-150">यह आप निम्न तरीके से करते हैं:</span><span class="sxs-lookup"><span data-stu-id="34bbc-150">Here’s how you do this:</span></span>

1. <span data-ttu-id="34bbc-151">कार्य विश्लेषण संरचना पर, एक कार्य का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="34bbc-151">On the work breakdown structure, select a task.</span></span>
2. <span data-ttu-id="34bbc-152">संसाधन कक्ष में **असाइन की गई भूमिका** ड्रॉपडाउन चिह्न का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="34bbc-152">Select the **Assigned Role** dropdown icon in the resource cell.</span></span>
3. <span data-ttu-id="34bbc-153">**भूमिका** ड्रॉपडाउन का चयन करें और जेनेरिक संसाधन के लिए भूमिका का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="34bbc-153">Select the **Role** dropdown and select the role for the generic resource.</span></span>
4. <span data-ttu-id="34bbc-154">**ठीक** चुनें।</span><span class="sxs-lookup"><span data-stu-id="34bbc-154">Select **OK**.</span></span>

    > [!div class="mx-imgBorder"] 
    > <span data-ttu-id="34bbc-155">![संसाधन जोड़ने के लिए WBS का उपयोग करने का स्क्रीनशॉट](media/FAQ-Resources-to-Tasks2-4.png "संसाधन जोड़ने के लिए WBS का उपयोग करने का स्क्रीनशॉट")</span><span class="sxs-lookup"><span data-stu-id="34bbc-155">![Screenshot of using WBS to add resource](media/FAQ-Resources-to-Tasks2-4.png "Screenshot of using WBS to add resource")</span></span>
 
<span data-ttu-id="34bbc-156">जब आप WBS में कार्यों पर भूमिकाएँ असाइन करना पूर्ण कर लेते हैं, उसके बाद **प्रोजेक्ट टीम उत्पन्न करें** चयन करें.</span><span class="sxs-lookup"><span data-stu-id="34bbc-156">Once you’ve completed assigning roles to the tasks in the WBS, select **Generate Project Team**.</span></span> <span data-ttu-id="34bbc-157">Project Service कार्य असाइनमेंट को एकीकृत कर भूमिकाओं, संसाधन संगठन इकाइयों, और प्रोजेक्ट कैलेंडर के आधार पर जेनेरिक टीम के न्यूनतम सदस्यों का निर्माण करता है.</span><span class="sxs-lookup"><span data-stu-id="34bbc-157">Project Service creates the minimum number of generic team members based on the roles, resourcing organization units, and project calendar by aggregating the task assignments.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="34bbc-158">![परियोजना टीम बनाने का स्क्रीनशॉट](media/FAQ-Resources-to-Tasks2-5.png "परियोजना टीम बनाने का स्क्रीनशॉट")</span><span class="sxs-lookup"><span data-stu-id="34bbc-158">![Screenshot of generating project team](media/FAQ-Resources-to-Tasks2-5.png "Screenshot of generating project team")</span></span>
 
<span data-ttu-id="34bbc-159">टीम सदस्य ग्रिड पर, आपको जेनेरिक संसाधन प्रकार के संसाधन, भूमिकाओं और पद नाम सहित दिखाई देंगे.</span><span class="sxs-lookup"><span data-stu-id="34bbc-159">On the Team Member grid, you’ll see resources of the Generic Resource type with the role and position name.</span></span> <span data-ttu-id="34bbc-160">यदि कार्य को पूरा करने के लिए किसी एक भूमिका के लिए दो संसाधनों की आवश्यकता है, तो टीम उत्पन्न करें सुविधा टीम के दो सदस्य बनाती है और उन्हें अलग करने के लिए पद नाम का उपयोग करती है.</span><span class="sxs-lookup"><span data-stu-id="34bbc-160">If two resources are needed for a role to complete the work, the Generate Team feature creates two team members and uses position name to set them apart.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="34bbc-161">![दो सामान्य संसाधन जोड़ने का स्क्रीनशॉट](media/FAQ-Resources-to-Tasks2-6.png "दो सामान्य संसाधन जोड़ने का स्क्रीनशॉट")</span><span class="sxs-lookup"><span data-stu-id="34bbc-161">![Screenshot of adding two generic resources](media/FAQ-Resources-to-Tasks2-6.png "Screenshot of adding two generic resources")</span></span>
 
<span data-ttu-id="34bbc-162">आप संसाधन आवश्यकता के अंतर्गत लिंक का चयन करके जेनेरिक टीम के सदस्यों के लिए बैकिंग संसाधन आवश्यकता खोल सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="34bbc-162">You can open the backing resource requirement for the generic team member by selecting the link under Resource Requirement.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="34bbc-163">![बैकिंग संसाधन आवश्यकता खोलने का स्क्रीनशॉट](media/FAQ-Resources-to-Tasks2-7.png "बैकिंग संसाधन आवश्यकता खोलने का स्क्रीनशॉट")</span><span class="sxs-lookup"><span data-stu-id="34bbc-163">![Screenshot of opening backing resource requirement](media/FAQ-Resources-to-Tasks2-7.png "Screenshot of opening backing resource requirement")</span></span>

<span data-ttu-id="34bbc-164">जेनेरिक संसाधन के लिए **बुक** का चयन करें, और उसके बाद आप एक वास्तविक संसाधन ढूँढ़ने और बुक करने के लिए शेड्यूल बोर्ड का उपयोग कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="34bbc-164">Select **Book** for the generic resource, and then you can use the schedule board to find and book a real resource.</span></span> <span data-ttu-id="34bbc-165">आप **अनुरोध सबमिट करें** का चयन करके संसाधन प्रबंधक द्वारा पूर्णता की आवश्यकता भी सबमिट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="34bbc-165">You can also submit the requirement for fulfillment by a resource manager by selecting **Submit Request**.</span></span>

<span data-ttu-id="34bbc-166">जब जेनेरिक संसाधन किसी नामित संसाधन द्वारा पूर्ण कर लिया जाता है, तो जेनेरिक संसाधन को टीम से निकाल दिया जाता है और जेनेरिक संसाधन के लिए कार्य असाइनमेंट उस नामित संसाधन को असाइन कर दिए जाते हैं, जिसने जेनेरिक संसाधन की संसाधन आवश्यकता को पूर्ण किया था.</span><span class="sxs-lookup"><span data-stu-id="34bbc-166">When the generic resource is fulfilled with a named resource, the generic resource is removed from the team and the task assignments for the generic resource are assigned to the named resource that fulfilled the generic resource’s resource requirement.</span></span>
 

