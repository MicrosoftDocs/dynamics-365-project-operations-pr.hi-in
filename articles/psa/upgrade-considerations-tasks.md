---
title: कार्य की विवरण संरचना के लिए अपग्रेड संबंधी विचार
description: इस टॉपिक में Project Service Automation 2.x से 3.x के मामले में कार्य की विवरण संरचना को अपग्रेड करने के बारे में जानकारी प्रदान की गई है।
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
author: ruhercul
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
ms.openlocfilehash: 0b75fd372732f42a3557aaa5eccec1f24a644941
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4121805"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a><span data-ttu-id="6d70b-103">कार्य की विवरण संरचना के लिए अपग्रेड संबंधी विचार</span><span class="sxs-lookup"><span data-stu-id="6d70b-103">Upgrade considerations for the work breakdown structure</span></span>
<span data-ttu-id="6d70b-104">इस टॉपिक में Project Service Automation 2.x से 3.x के मामले में कार्य की विवरण संरचना को अपग्रेड करने के बारे में जानकारी प्रदान की गई है।</span><span class="sxs-lookup"><span data-stu-id="6d70b-104">This topic provides information about upgrading the work breakdown structure from Project Service Automation 2.x to 3.x.</span></span> <span data-ttu-id="6d70b-105">इस टॉपिक में Project Service Automation (PSA) में किसी परियोजना के स्वास्थ्य को परिभाषित किया गया है, जो सफल अपग्रेड के लिए आवश्यक है।</span><span class="sxs-lookup"><span data-stu-id="6d70b-105">This topic defines the healthy state of a project in Project Service Automation (PSA) that is required for a successful upgrade.</span></span> <span data-ttu-id="6d70b-106">आम पायी जाने वाली ब्लॉकिंग परिस्थितियों के बारे में भी जानकारी दी गई है, जो अपग्रेड को विफल बना सकती हैं।</span><span class="sxs-lookup"><span data-stu-id="6d70b-106">There is also information about the common blocking conditions that will cause upgrade to fail.</span></span> <span data-ttu-id="6d70b-107">किसी परियोजना शेड्यूल में परियोजना टास्क और उनके कार्यों को परिभाषित करने के बारे में अधिक जानकारी के लिए [प्रोजेक्ट शेड्यूल](project-creating.md) देखें।</span><span class="sxs-lookup"><span data-stu-id="6d70b-107">For more information about defining project tasks and their functions within a project schedule, see [Project schedules](project-creating.md).</span></span>

## <a name="key-entities"></a><span data-ttu-id="6d70b-108">प्रमुख इकाइयां</span><span class="sxs-lookup"><span data-stu-id="6d70b-108">Key entities</span></span>
<span data-ttu-id="6d70b-109">पहले से ही संसाधनों से लैस किसी सटीक कार्य विवरण संरचना को परिभाषित करने हेतु आपको निम्न इकाइयों की आवश्यकता होगी:</span><span class="sxs-lookup"><span data-stu-id="6d70b-109">For an accurate work breakdown structure that is already loaded with resources, the following entities are required:</span></span>

- [<span data-ttu-id="6d70b-110">परियोजना</span><span class="sxs-lookup"><span data-stu-id="6d70b-110">Project</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project)
- [<span data-ttu-id="6d70b-111">परियोजना टीम</span><span class="sxs-lookup"><span data-stu-id="6d70b-111">Project Team</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam)
- [<span data-ttu-id="6d70b-112">परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="6d70b-112">Project Task</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask)
- [<span data-ttu-id="6d70b-113">संसाधन असाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="6d70b-113">Resource Assignments</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment)
- [<span data-ttu-id="6d70b-114">परियोजना कार्य निर्भरता</span><span class="sxs-lookup"><span data-stu-id="6d70b-114">Project Task Dependency</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency)
- [<span data-ttu-id="6d70b-115">बुक करने योग्य संसाधन</span><span class="sxs-lookup"><span data-stu-id="6d70b-115">Bookable Resources</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/bookableresource)

<span data-ttu-id="6d70b-116">संसाधनों से लैस किसी कार्य विवरण संरचना को परिभाषित करने हेतु आपको निम्न चरण पूरे करने होंगे:</span><span class="sxs-lookup"><span data-stu-id="6d70b-116">To define a resource loaded work breakdown structure, you must complete the following steps:</span></span>

1. <span data-ttu-id="6d70b-117">कोई नई परियोजना बनाएं।</span><span class="sxs-lookup"><span data-stu-id="6d70b-117">Create a new project.</span></span> <span data-ttu-id="6d70b-118">नई परियोजना बनाने के बारे में अधिक जानकारी के लिए [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project) देखें।</span><span class="sxs-lookup"><span data-stu-id="6d70b-118">For more information about how to create a new project, see [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project).</span></span>
2. <span data-ttu-id="6d70b-119">एक या एक से अधिक टास्क बनाएं।</span><span class="sxs-lookup"><span data-stu-id="6d70b-119">Create one or more tasks.</span></span> <span data-ttu-id="6d70b-120">टास्क बनाने के तरीके के बारे में अधिक जानकारी के लिए [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).</span><span class="sxs-lookup"><span data-stu-id="6d70b-120">For more information about how to create a task, see [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).</span></span>
3. <span data-ttu-id="6d70b-121">टास्क की डिपेंडेंसी को परिभाषित करें।</span><span class="sxs-lookup"><span data-stu-id="6d70b-121">Define the task dependencies.</span></span> <span data-ttu-id="6d70b-122">अधिक जानकारी के लिए, देखें [परियोजना कार्य निर्भरता](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency) ।</span><span class="sxs-lookup"><span data-stu-id="6d70b-122">For more information, see [Project Task Dependency](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency).</span></span>
4. <span data-ttu-id="6d70b-123">परियोजना टीम के सदस्यों को परियोजना एसाइन करें।</span><span class="sxs-lookup"><span data-stu-id="6d70b-123">Assign project team members to the project.</span></span> <span data-ttu-id="6d70b-124">अधिक जानकारी के लिए [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam) देखें।</span><span class="sxs-lookup"><span data-stu-id="6d70b-124">For more information, see [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam).</span></span>
5. <span data-ttu-id="6d70b-125">परियोजना टीम के सदस्यों को कार्य एसाइन करें।</span><span class="sxs-lookup"><span data-stu-id="6d70b-125">Assign project team members to the tasks.</span></span> <span data-ttu-id="6d70b-126">अधिक जानकारी के लिए [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment) देखें।</span><span class="sxs-lookup"><span data-stu-id="6d70b-126">For more information, see [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment).</span></span>

## <a name="project-team-relationships"></a><span data-ttu-id="6d70b-127">परियोजना टीम के संबंध</span><span class="sxs-lookup"><span data-stu-id="6d70b-127">Project team relationships</span></span>

<span data-ttu-id="6d70b-128">सफल अपग्रेड पाने के लिए निम्न संबंधों को सही ढंग से बनाए रखा जाना चाहिए:</span><span class="sxs-lookup"><span data-stu-id="6d70b-128">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>
- <span data-ttu-id="6d70b-129">परियोजना टीम के सभी सदस्य किसी बुक करने-योग्य संसाधन से जुड़े होने चाहिए।</span><span class="sxs-lookup"><span data-stu-id="6d70b-129">All project team members must be associated with a bookable resource.</span></span>
- <span data-ttu-id="6d70b-130">परियोजना टीम के सभी सदस्य उसी परियोजना से जुड़े होने चाहिए।</span><span class="sxs-lookup"><span data-stu-id="6d70b-130">All project team members must be associated with the same project.</span></span> 

## <a name="project-task-relationships"></a><span data-ttu-id="6d70b-131">परियोजना टास्क से जुड़े संबंध</span><span class="sxs-lookup"><span data-stu-id="6d70b-131">Project task relationships</span></span>
<span data-ttu-id="6d70b-132">सफल अपग्रेड पाने के लिए निम्न संबंधों को सही ढंग से बनाए रखा जाना चाहिए:</span><span class="sxs-lookup"><span data-stu-id="6d70b-132">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="6d70b-133">कोई भी संबंधित टास्क उसी परियोजना से ही जुड़े होने चाहिए।</span><span class="sxs-lookup"><span data-stu-id="6d70b-133">Any related tasks must be associated with the same project.</span></span>
- <span data-ttu-id="6d70b-134">हर लाइन टास्क में एक पैरेंट टास्क होना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="6d70b-134">Every line task must have a parent task.</span></span>
- <span data-ttu-id="6d70b-135">प्रत्येक टास्क के लिए एक पैरेंट परियोजना होनी चाहिए।</span><span class="sxs-lookup"><span data-stu-id="6d70b-135">Every task must have a parent project.</span></span>

### <a name="valid-conditions"></a><span data-ttu-id="6d70b-136">मान्य स्थितियां</span><span class="sxs-lookup"><span data-stu-id="6d70b-136">Valid conditions</span></span>

- <span data-ttu-id="6d70b-137">सभी टास्क की अवधि एक घंटे के बराबर या उससे अधिक (> =) और 1,800,000 मिनट (1,250 दिन) से कम होनी चाहिए.\*</span><span class="sxs-lookup"><span data-stu-id="6d70b-137">All task durations must be greater than or equal to (>=) one hour and less than 1,800,000 minutes (1,250 days).\*</span></span>
- <span data-ttu-id="6d70b-138">किसी भी टास्क की प्रारंभ तिथि 2000/01/01 से पहले की नहीं होनी चाहिए.\*</span><span class="sxs-lookup"><span data-stu-id="6d70b-138">All tasks must have a start date no earlier than 2000/01/01.\*</span></span>
- <span data-ttu-id="6d70b-139">किसी भी टास्क की प्रारंभ तिथि आज से 17 साल के बाद वाली नहीं होनी चाहिए.\*</span><span class="sxs-lookup"><span data-stu-id="6d70b-139">All tasks must have a start date no later than 17 years from the present day.\*</span></span>
- <span data-ttu-id="6d70b-140">सभी टास्क की प्रारम्भ तिथि उनकी समाप्ति तिथि के बराबर या उससे पहले होनी चाहिए.</span><span class="sxs-lookup"><span data-stu-id="6d70b-140">All tasks must have a start date earlier or equal to their finish date.</span></span>
- <span data-ttu-id="6d70b-141">क्लासिफिकेशन से जुड़े सभी लेनदेन के मामलों (व्यय, सामग्री, टैक्स और समय) में **डिफ़ॉल्ट यूनिट** और **यूनिट समूह** के लिए मान होना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="6d70b-141">All transaction types on classifications (Expense, Material, Tax, and Time) must have values for **Default Unit** and **Unit Group**.</span></span>
- <span data-ttu-id="6d70b-142">तिथि के अक्षरों वाले फॉर्मेट से परेहज करें।</span><span class="sxs-lookup"><span data-stu-id="6d70b-142">Date formats with letters should be avoided.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="6d70b-143">संभावित मिटीगेशन चरण</span><span class="sxs-lookup"><span data-stu-id="6d70b-143">Potential mitigation steps</span></span>
- <span data-ttu-id="6d70b-144">उन परियोजना कार्यों की पहचान करने के लिए उन्नत खोज का उपयोग करें, जिनकी कोई परियोजना आईडी नहीं है.</span><span class="sxs-lookup"><span data-stu-id="6d70b-144">Use Advanced Find to identify Project tasks that do not contain a Project ID.</span></span>
- <span data-ttu-id="6d70b-145">उन परियोजना कार्यों की पहचानने के लिए उन्नत खोज का उपयोग करें, जहां शेड्यूल की गई अवधि > 1,800,000 से अधिक है.</span><span class="sxs-lookup"><span data-stu-id="6d70b-145">Use Advanced Find to identify Project tasks where the scheduled duration is greater than > 1,800,000.</span></span>
- <span data-ttu-id="6d70b-146">कोई भी डेटा परिवर्तन करने से पहले, आपको उस इकाई से जुड़े किसी भी अनुकूलन की जांच करनी चाहिए जिसके कारण डेटा खराब स्थिति में आ सकता है.</span><span class="sxs-lookup"><span data-stu-id="6d70b-146">Prior to making any data changes, you should investigate any customizations associated with the entity that may have led to getting the data into a bad state.</span></span> <span data-ttu-id="6d70b-147">किसी भी डेटा-संबंधित अपडेट के साथ आगे बढ़ने से पहले इन अनुकूलन को संबोधित किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="6d70b-147">These customizations should be addressed before proceeding with any data-related updates.</span></span>
- <span data-ttu-id="6d70b-148">ओरफनड के रूप में पहचाने गए कार्यों के लिए, यदि इन कार्यों की आवश्यकता नहीं है या यदि वे सही पैरेंट परियोजना से जुड़े होने चाहिए, तो इन्हें हटाने पर विचार करें.</span><span class="sxs-lookup"><span data-stu-id="6d70b-148">For the identified tasks that have been orphaned, consider deleting these tasks if they are not needed or if they should be associated with the correct parent project.</span></span>
- <span data-ttu-id="6d70b-149">ऐसे किसी भी कार्य के लिए, जहां अवधि 1,250 दिनों से अधिक है, यदि संभव हो, तो कुल अवधि दर्शाने के लिए कई कार्यों को जोड़ने पर विचार करें.</span><span class="sxs-lookup"><span data-stu-id="6d70b-149">For any tasks where the duration is greater than 1,250 days, consider adding multiple tasks to represent the total duration, if feasible.</span></span>

> [!NOTE]
> <span data-ttu-id="6d70b-150">तारे के चिह्न (\*) वाली आइटमों की सीमाएं हैं, जो इस तथ्य के कारण हैं कि कस्टमर रिलेशनशिप मैनेजमेंट (CRM) केवल 7,320 रेकरेन्स एक्सपेंशन को समर्थित करता है.</span><span class="sxs-lookup"><span data-stu-id="6d70b-150">Items noted with an asterisk (\*) have limits that are due to the fact that customer relationship management (CRM) supports only 7,320 recurrence expansions.</span></span> <span data-ttu-id="6d70b-151">आपको इस सीमा के अंदर ही रहना है।</span><span class="sxs-lookup"><span data-stu-id="6d70b-151">You must stay below this limit.</span></span>

## <a name="resource-assignment-relationships"></a><span data-ttu-id="6d70b-152">संसाधनों की एसाइनमेंट से जुड़े संबंध</span><span class="sxs-lookup"><span data-stu-id="6d70b-152">Resource Assignment relationships</span></span>
<span data-ttu-id="6d70b-153">सफल अपग्रेड पाने के लिए निम्न संबंधों को सही ढंग से बनाए रखा जाना चाहिए:</span><span class="sxs-lookup"><span data-stu-id="6d70b-153">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="6d70b-154">कार्य विश्लेषण संरचना में एसाइन किए गए सभी संसाधन एक ही परियोजना से संबंधित होने चाहिए.</span><span class="sxs-lookup"><span data-stu-id="6d70b-154">All Resource Assignments in a work breakdown structure must be related to the same project.</span></span>
- <span data-ttu-id="6d70b-155">कार्य विश्लेषण संरचना में एसाइन किए गए सभी संसाधन एक ही परियोजना के परियोजना टीम सदस्यों से संबंधित होने चाहिए.</span><span class="sxs-lookup"><span data-stu-id="6d70b-155">All Resource Assignments in a work breakdown structure must be associated to project team members in the same project.</span></span>

### <a name="potential-mitigation-steps"></a><span data-ttu-id="6d70b-156">संभावित मिटीगेशन चरण</span><span class="sxs-lookup"><span data-stu-id="6d70b-156">Potential mitigation steps</span></span>
- <span data-ttu-id="6d70b-157">उन सभी कार्यों की पहचान करें, जो उपरोक्त वर्णित शर्तों के बाहर हैं.</span><span class="sxs-lookup"><span data-stu-id="6d70b-157">Identify all tasks that fall outside the conditions described above.</span></span>  
- <span data-ttu-id="6d70b-158">कोई भी संसाधन असाइनमेंट, जो अब मान्य नहीं हैं, उन्हें हटा दिया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="6d70b-158">Any Resource Assignments that are no longer valid should be deleted.</span></span>

## <a name="project-task-dependency-relationships"></a><span data-ttu-id="6d70b-159">परियोजना टास्क डिपेंडेंसी संबंध</span><span class="sxs-lookup"><span data-stu-id="6d70b-159">Project task dependency relationships</span></span>
<span data-ttu-id="6d70b-160">सफल अपग्रेड पाने के लिए निम्न संबंधों को सही ढंग से बनाए रखा जाना चाहिए:</span><span class="sxs-lookup"><span data-stu-id="6d70b-160">To ensure a successful upgrade, the following relationships must be correctly maintained:</span></span>

- <span data-ttu-id="6d70b-161">सभी परियोजना टास्क डिपेंडेंसी संबंध एक ही परियोजना से संबंधित होनी चाहिए।</span><span class="sxs-lookup"><span data-stu-id="6d70b-161">All project task dependencies must be related to the same project.</span></span>
- <span data-ttu-id="6d70b-162">किसी टास्क की डिपेंडेंसी को एक से अधिक बार संदर्भित नहीं किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="6d70b-162">A task can't have the same dependency referenced more than once.</span></span>
