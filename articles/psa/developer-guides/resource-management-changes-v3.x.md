---
title: संसाधन प्रबंधन में परिवर्तन (Project Service Automation 3.x)
description: इस टॉपिक के अंतर्गत संसाधन प्रबंधन के क्षेत्र में परिवर्तन के बारे में जानकारी दी गई है.
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 03/18/2019
ms.topic: article
ms.service: business-applications
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 5f88d7309a5e1171629a72e749bfc01abb64c62a
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5284765"
---
# <a name="resource-management-changes-project-service-automation-3x"></a><span data-ttu-id="d0570-103">संसाधन प्रबंधन में परिवर्तन (Project Service Automation 3.x)</span><span class="sxs-lookup"><span data-stu-id="d0570-103">Resource management changes (Project Service Automation 3.x)</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

<span data-ttu-id="d0570-104">इस टॉपिक के अनुभागों में Dynamics 365 Project Service Automation संस्करण 3.x के संसाधन प्रबंधन क्षेत्र में किए गए परिवर्तनों के बारे में जानकारी प्रदान की गई है.</span><span class="sxs-lookup"><span data-stu-id="d0570-104">The sections of this topic provide information about the changes that have been made to the Resource management area of Dynamics 365 Project Service Automation version 3.x.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="d0570-105">परियोजना अनुमान</span><span class="sxs-lookup"><span data-stu-id="d0570-105">Project estimates</span></span>

<span data-ttu-id="d0570-106">परियोजना के अनुमान **msdyn\_projecttask** निकाय (**परियोजना कार्य**) पर आधारित होने के बजाय **msdyn\_resourceassignment** निकाय (**संसाधन असाइनमेंट**) पर आधारित हैं.</span><span class="sxs-lookup"><span data-stu-id="d0570-106">Instead of being based on the **msdyn\_projecttask** entity (**Project Task**), project estimates are based on the **msdyn\_resourceassignment** entity (**Resource Assignment**).</span></span> <span data-ttu-id="d0570-107">संसाधनों को एसाइनमेंट देना कार्य की शेड्यूलिंग और मूल्य के निर्धारण के लिए "सत्य का स्रोत" बन गया है.</span><span class="sxs-lookup"><span data-stu-id="d0570-107">Resource assignments have become the "source of truth" for task scheduling and pricing.</span></span>

## <a name="line-tasks"></a><span data-ttu-id="d0570-108">पंक्ति कार्य</span><span class="sxs-lookup"><span data-stu-id="d0570-108">Line tasks</span></span>

<span data-ttu-id="d0570-109">PSA 3.x में पंक्ति कार्य अप्रचलित (अवमानित) हो चुके हैं.</span><span class="sxs-lookup"><span data-stu-id="d0570-109">In PSA 3.x, line tasks are obsolete (deprecated).</span></span> <span data-ttu-id="d0570-110">एसाइनमेंट देने में अब पंक्ति कार्यों के बजाय पूरे कार्य इंगित किये जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="d0570-110">Assignments now point to the whole task instead of the line tasks.</span></span>

<span data-ttu-id="d0570-111">निम्न उदाहरण दर्शाता है कि "टेस्ट टास्क" नामक कार्य PSA और PSA 3.x के पूर्व संस्करणों में टीम के A और B नामक सदस्यों को कैसे सौंपा जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0570-111">The following example shows how a task that is named "Test task" is assigned to team members A and B in earlier versions of PSA and in PSA 3.x.</span></span>

- <span data-ttu-id="d0570-112">**PSA 3.x से पूर्व:**</span><span class="sxs-lookup"><span data-stu-id="d0570-112">**Before PSA 3.x:**</span></span>

    - <span data-ttu-id="d0570-113">टेस्ट टास्क</span><span class="sxs-lookup"><span data-stu-id="d0570-113">Test task</span></span>

        - <span data-ttu-id="d0570-114">टेस्ट टास्क - पंक्ति कार्य 1</span><span class="sxs-lookup"><span data-stu-id="d0570-114">Test task – Line task 1</span></span>

            - <span data-ttu-id="d0570-115">A को एसाइनमेंट दिया गया</span><span class="sxs-lookup"><span data-stu-id="d0570-115">Assignment to A</span></span>

        - <span data-ttu-id="d0570-116">टेस्ट टास्क - पंक्ति कार्य 2</span><span class="sxs-lookup"><span data-stu-id="d0570-116">Test task – Line task 2</span></span>

            - <span data-ttu-id="d0570-117">B को एसाइनमेंट दिया गया</span><span class="sxs-lookup"><span data-stu-id="d0570-117">Assignment to B</span></span>

- <span data-ttu-id="d0570-118">**PSA 3.x:**</span><span class="sxs-lookup"><span data-stu-id="d0570-118">**PSA 3.x:**</span></span>

    - <span data-ttu-id="d0570-119">टेस्ट टास्क</span><span class="sxs-lookup"><span data-stu-id="d0570-119">Test task</span></span>

        - <span data-ttu-id="d0570-120">A को एसाइनमेंट दिया गया</span><span class="sxs-lookup"><span data-stu-id="d0570-120">Assignment to A</span></span>
        - <span data-ttu-id="d0570-121">B को एसाइनमेंट दिया गया</span><span class="sxs-lookup"><span data-stu-id="d0570-121">Assignment to B</span></span>

## <a name="unassigned-assignment"></a><span data-ttu-id="d0570-122">अनएसाइंड एसाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="d0570-122">Unassigned assignment</span></span>

<span data-ttu-id="d0570-123">PSA 3.x में अनएसाइंड एसाइनमेंट ऐसा एसाइनमेंट होता है जिसे **NULL** टीम के किसी सदस्य और किसी **NULL** संसाधन को सौंपा जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0570-123">In PSA 3.x, an unassigned assignment is an assignment that is assigned to a **NULL** team member and a **NULL** resource.</span></span> <span data-ttu-id="d0570-124">अनएसाइंड एसाइनमेंट एक-दो मामलों में हो सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="d0570-124">Unassigned assignments can occur in a couple of scenarios:</span></span>

- <span data-ttu-id="d0570-125">यदि कोई कार्य तैयार किया गया है, लेकिन इसे अभी तक किसी भी टीम के सदस्य को एसाइन किया नहीं गया है, तो सदा अनएसाइंड एसाइनमेंट बनता है.</span><span class="sxs-lookup"><span data-stu-id="d0570-125">If a task has been created, but it hasn't yet been assigned to any team member, an unassigned assignment is always created.</span></span> 
- <span data-ttu-id="d0570-126">यदि किसी कार्य के सभी एसाइनमेंट हटा लिए जाते हैं तो उस कार्य के लिए फिर से अनएसाइंड एसाइनमेंट बनाया जाता है।</span><span class="sxs-lookup"><span data-stu-id="d0570-126">If all assignees on a task are removed, an unassigned assignment is re-created for that task.</span></span>

## <a name="scheduling-fields-on-the-project-task-entity"></a><span data-ttu-id="d0570-127">परियोजना कार्य इकाई पर शेड्यूलिंग फ़ील्ड</span><span class="sxs-lookup"><span data-stu-id="d0570-127">Scheduling fields on the Project Task entity</span></span>

<span data-ttu-id="d0570-128">**msdyn\_projecttask** निकाय से फ़ील्ड अवमानित कर दिए गए हैं या फिर **msdyn\_resourceassignment** निकाय पर स्थानान्तरित कर दिए गए हैं या उन्हें अब **msdyn\_projectteam** निकाय (**परियोजना टीम सदस्य**) से संदर्भित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0570-128">The fields on the **msdyn\_projecttask** entity have been deprecated or moved to the **msdyn\_resourceassignment** entity, or they are now referenced from the **msdyn\_projectteam** entity (**Project Team Member**).</span></span>

| <span data-ttu-id="d0570-129">msdyn\_projecttask पर अवमानित फील्ड (परियोजना टास्क)</span><span class="sxs-lookup"><span data-stu-id="d0570-129">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="d0570-130">msdyn\_resourceassignment पर नया फ़ील्ड (संसाधन का एसाइनमेंट)</span><span class="sxs-lookup"><span data-stu-id="d0570-130">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> | <span data-ttu-id="d0570-131">टिप्पणी</span><span class="sxs-lookup"><span data-stu-id="d0570-131">Comment</span></span> |
|---|---|---|
| <span data-ttu-id="d0570-132">msdyn\_assignedresources</span><span class="sxs-lookup"><span data-stu-id="d0570-132">msdyn\_assignedresources</span></span> | <span data-ttu-id="d0570-133">कोई नहीं</span><span class="sxs-lookup"><span data-stu-id="d0570-133">None</span></span> | |
| <span data-ttu-id="d0570-134">msdyn\_assignedteammembers</span><span class="sxs-lookup"><span data-stu-id="d0570-134">msdyn\_assignedteammembers</span></span> | <span data-ttu-id="d0570-135">कोई नहीं</span><span class="sxs-lookup"><span data-stu-id="d0570-135">None</span></span> | |
| <span data-ttu-id="d0570-136">msdyn\_numberofresources</span><span class="sxs-lookup"><span data-stu-id="d0570-136">msdyn\_numberofresources</span></span> | <span data-ttu-id="d0570-137">कोई नहीं</span><span class="sxs-lookup"><span data-stu-id="d0570-137">None</span></span> | |
| <span data-ttu-id="d0570-138">msdyn\_scheduledhours</span><span class="sxs-lookup"><span data-stu-id="d0570-138">msdyn\_scheduledhours</span></span> | <span data-ttu-id="d0570-139">कोई नहीं</span><span class="sxs-lookup"><span data-stu-id="d0570-139">None</span></span> | |
| <span data-ttu-id="d0570-140">msdyn\_effortcontour</span><span class="sxs-lookup"><span data-stu-id="d0570-140">msdyn\_effortcontour</span></span> | <span data-ttu-id="d0570-141">msdyn\_plannedwork</span><span class="sxs-lookup"><span data-stu-id="d0570-141">msdyn\_plannedwork</span></span> | <span data-ttu-id="d0570-142">फ़ील्ड में संग्रहीत JavaScript ऑब्जेक्ट नोटेशन (JSON) का डेटा संरचना प्रारूप बदल दिया गया है.</span><span class="sxs-lookup"><span data-stu-id="d0570-142">The format of the JavaScript Object Notation (JSON) data structure that is stored in the field has been changed.</span></span> |

## <a name="schedule-contour"></a><span data-ttu-id="d0570-143">शेड्यूल कंटूअर</span><span class="sxs-lookup"><span data-stu-id="d0570-143">Schedule contour</span></span>

<span data-ttu-id="d0570-144">इस शेड्यूल कंटूअर को प्रत्येक **संसाधन एसाइनमेंट** इकाई (**msdyn\_resourceassignment**) के **नियोजित कार्य** फ़ील्ड (**msdyn\_plannedwork**) में संग्रहीत किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0570-144">The schedule contour is stored in the **Planned Work** field (**msdyn\_plannedwork**) of each **Resource Assignment** entity (**msdyn\_resourceassignment**).</span></span>

### <a name="structure"></a><span data-ttu-id="d0570-145">संरचना</span><span class="sxs-lookup"><span data-stu-id="d0570-145">Structure</span></span>

<span data-ttu-id="d0570-146">शेड्यूल कंटूअर की नई संरचना में लचीले समय अंतराल होते हैं जिन्हें शेड्यूल के प्रत्येक दिन के लिए परिभाषित किया गया होता है.</span><span class="sxs-lookup"><span data-stu-id="d0570-146">The new structure of the schedule contour consists of flexible time slices that are defined for each day of the schedule.</span></span> <span data-ttu-id="d0570-147">हर समय अंतराल में निम्न गुण होते हैं:</span><span class="sxs-lookup"><span data-stu-id="d0570-147">Each time slice has the following properties:</span></span>

- <span data-ttu-id="d0570-148">**प्रारंभ** - परियोजना कैलेंडर के अनुसार दिन के काम की शुरुआत.</span><span class="sxs-lookup"><span data-stu-id="d0570-148">**Start** – The start of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="d0570-149">**अंत** - परियोजना कैलेंडर के अनुसार दिन के काम का अंत.</span><span class="sxs-lookup"><span data-stu-id="d0570-149">**End** – The end of the working hours for the day, according to the project calendar.</span></span>
- <span data-ttu-id="d0570-150">**घंटे** - दिन में एसाइन किये गए घंटे.</span><span class="sxs-lookup"><span data-stu-id="d0570-150">**Hours** – The number of hours that are assigned on the day.</span></span>

<span data-ttu-id="d0570-151">**उदाहरण**</span><span class="sxs-lookup"><span data-stu-id="d0570-151">**Example**</span></span>

<span data-ttu-id="d0570-152">इस उदाहरण में उस परियोजना कैलेंडर का उपयोग किया गया है, जिसमें कार्य दिवस UTC-8 समय ज़ोन में सुबह 9 बजे से शाम 5 बजे तक होता है.</span><span class="sxs-lookup"><span data-stu-id="d0570-152">This example uses a project calendar where the workday is from 9 AM to 5 PM in the UTC-8 time zone.</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

### <a name="auto-scheduling-and-manual-scheduling"></a><span data-ttu-id="d0570-153">ऑटो-शेड्यूलिंग और मैनुअल शेड्यूलिंग</span><span class="sxs-lookup"><span data-stu-id="d0570-153">Auto-scheduling and manual scheduling</span></span>

<span data-ttu-id="d0570-154">यदि कोई कार्य ऑटो-शेड्यूल किया गया है, तो घंटे फ्रंट-लोडेड हैं, और कार्य की अवधि कम हो सकती है.</span><span class="sxs-lookup"><span data-stu-id="d0570-154">If a task is auto-scheduled, the hours are front-loaded, and the task duration might be reduced.</span></span>

<span data-ttu-id="d0570-155">**उदाहरण**</span><span class="sxs-lookup"><span data-stu-id="d0570-155">**Example**</span></span>

<span data-ttu-id="d0570-156">निम्न कार्य को तीन दिन (3 दिसंबर, 2018 से 5 दिसंबर, 2018) में 18 घंटे के लिए ऑटो-शेड्यूल किया गया है.</span><span class="sxs-lookup"><span data-stu-id="d0570-156">The following task is auto-scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
```

<span data-ttu-id="d0570-157">यदि किसी कार्य को मैन्युअल रूप से शेड्यूल किया गया है तो कार्य के घंटे सभी तिथियों में समान रूप से वितरित किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="d0570-157">If a task is manually scheduled, the hours are evenly distributed to all the dates.</span></span>

<span data-ttu-id="d0570-158">**उदाहरण**</span><span class="sxs-lookup"><span data-stu-id="d0570-158">**Example**</span></span>

<span data-ttu-id="d0570-159">निम्न कार्य को तीन दिन (3 दिसंबर, 2018 से 5 दिसंबर, 2018) में 18 घंटे के लिए मैन्युअल रूप से शेड्यूल किया गया है.</span><span class="sxs-lookup"><span data-stu-id="d0570-159">The following task is manually scheduled for 18 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

```json
[{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":6},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":6},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":6}]
```

### <a name="assignment-unit"></a><span data-ttu-id="d0570-160">एसाइनमेंट यूनिट</span><span class="sxs-lookup"><span data-stu-id="d0570-160">Assignment unit</span></span>

<span data-ttu-id="d0570-161">एसाइनमेंट यूनिट को PSA 3.x में अवमानित कर दिया गया है.</span><span class="sxs-lookup"><span data-stu-id="d0570-161">The assignment unit has been deprecated in PSA 3.x.</span></span> <span data-ttu-id="d0570-162">सभी एसाइन्ड संसाधनों के बीच कार्य के में प्रति दिन लगने वाले प्रयास का समय अब समान रूप से विभाजित किया गया है.</span><span class="sxs-lookup"><span data-stu-id="d0570-162">The task effort hours are now equally divided, per day, among all the assigned resources.</span></span>

<span data-ttu-id="d0570-163">**उदाहरण**</span><span class="sxs-lookup"><span data-stu-id="d0570-163">**Example**</span></span>

<span data-ttu-id="d0570-164">इस उदाहरण में इस कार्य को दो संसाधनों को एसाइन किया गया है और तीन दिनों (3 दिसंबर, 2018 से 5 दिसंबर, 2018) में 36 घंटों के लिए ऑटो-शेड्यूल किया गया है.</span><span class="sxs-lookup"><span data-stu-id="d0570-164">In this example, the task is is assigned to two resources and is auto-scheduled for 36 hours over three days (December 3, 2018, to December 5, 2018).</span></span>

- <span data-ttu-id="d0570-165">असाइनमेंट 1:</span><span class="sxs-lookup"><span data-stu-id="d0570-165">Assignment 1:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

- <span data-ttu-id="d0570-166">असाइनमेंट 2:</span><span class="sxs-lookup"><span data-stu-id="d0570-166">Assignment 2:</span></span>

    ```json
    [{"End":"\/Date(1543885200000)\/","Start":"\/Date(1543856400000)\/","Hours":8},{"End":"\/Date(1543971600000)\/","Start":"\/Date(1543942800000)\/","Hours":8},{"End":"\/Date(1544058000000)\/","Start":"\/Date(1544029200000)\/","Hours":2}]
    ```

## <a name="pricing-dimensions"></a><span data-ttu-id="d0570-167">कीमत निर्धारण के डायमेंशन</span><span class="sxs-lookup"><span data-stu-id="d0570-167">Pricing dimensions</span></span>

<span data-ttu-id="d0570-168">PSA 3.x में संसाधन के मामले में विशिष्ट मूल्य निर्धारण से जुड़े आयाम के फ़ील्ड (जैसे **भूमिका** और **संगठनात्मक इकाई**) **msdyn\_projecttask** इकाई से हटा दिए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="d0570-168">In PSA 3.x, resource-specific pricing dimension fields (such as **Role** and **Organizational Unit**) have been removed from the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="d0570-169">ये फ़ील्ड अब परियोजना के अनुमान तैयार किये जाने के समय संसाधन एसाइनमेंट (**msdyn\_projectteam**) से संबंधित परियोजना टीम सदस्य (**msdyn\_resourceassignment**) से प्राप्त किए जा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="d0570-169">These fields can now be retrieved from the corresponding project team member (**msdyn\_projectteam**) of the resource assignment (**msdyn\_resourceassignment**) when project estimates are generated.</span></span> <span data-ttu-id="d0570-170">एक नया फील्ड, **msdyn\_organizationalunit**, **msdyn\_projectteam** इकाई में जोड़ा गया है.</span><span class="sxs-lookup"><span data-stu-id="d0570-170">A new field, **msdyn\_organizationalunit**, has been added to the **msdyn\_projectteam** entity.</span></span>

| <span data-ttu-id="d0570-171">msdyn\_projecttask पर अवमानित फील्ड (परियोजना टास्क)</span><span class="sxs-lookup"><span data-stu-id="d0570-171">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="d0570-172">इसके बजाए msdyn\_projectteam (परियोजना टीम सदस्य) से फ़ील्ड का उपयोग किया जाता है</span><span class="sxs-lookup"><span data-stu-id="d0570-172">Field from msdyn\_projectteam (Project Team Member) that is used instead</span></span> |
|---|---|
| <span data-ttu-id="d0570-173">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="d0570-173">msdyn\_resourcecategory</span></span> | <span data-ttu-id="d0570-174">msdyn\_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="d0570-174">msdyn\_resourcecategory</span></span> |
| <span data-ttu-id="d0570-175">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="d0570-175">msdyn\_organizationalunit</span></span> | <span data-ttu-id="d0570-176">msdyn\_organizationalunit</span><span class="sxs-lookup"><span data-stu-id="d0570-176">msdyn\_organizationalunit</span></span> |

## <a name="contours"></a><span data-ttu-id="d0570-177">रूपरेखा</span><span class="sxs-lookup"><span data-stu-id="d0570-177">Contours</span></span>

<span data-ttu-id="d0570-178">मूल्य निर्धारण और अनुमान फील्ड को **msdyn\_projecttask** इकाई में अवमानित किया गया है.</span><span class="sxs-lookup"><span data-stu-id="d0570-178">The pricing and estimation contour fields have been deprecated on the **msdyn\_projecttask** entity.</span></span> <span data-ttu-id="d0570-179">इन्हें **msdyn\_resourceassignment** इकाई में स्थानांतरित किया गया है.</span><span class="sxs-lookup"><span data-stu-id="d0570-179">They have been moved to the **msdyn\_resourceassignment** entity.</span></span>

| <span data-ttu-id="d0570-180">msdyn\_projecttask पर अवमानित फील्ड (परियोजना टास्क)</span><span class="sxs-lookup"><span data-stu-id="d0570-180">Deprecated field on msdyn\_projecttask (Project Task)</span></span> | <span data-ttu-id="d0570-181">msdyn\_resourceassignment पर नया फ़ील्ड (संसाधन का एसाइनमेंट)</span><span class="sxs-lookup"><span data-stu-id="d0570-181">New field on msdyn\_resourceassignment (Resource Assignment)</span></span> |
|---|---|
| <span data-ttu-id="d0570-182">msdyn\_costestimatecontour</span><span class="sxs-lookup"><span data-stu-id="d0570-182">msdyn\_costestimatecontour</span></span> | <span data-ttu-id="d0570-183">msdyn\_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="d0570-183">msdyn\_plannedcostcontour</span></span> |
| <span data-ttu-id="d0570-184">msdyn\_salesestimatecontour</span><span class="sxs-lookup"><span data-stu-id="d0570-184">msdyn\_salesestimatecontour</span></span> | <span data-ttu-id="d0570-185">msdyn\_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="d0570-185">msdyn\_plannedsalescontour</span></span> |

<span data-ttu-id="d0570-186">निम्न फील्ड को **msdyn\_resourceassignment** इकाई में शामिल किया गया है:</span><span class="sxs-lookup"><span data-stu-id="d0570-186">The following fields have been added to the **msdyn\_resourceassignment** entity:</span></span>

* <span data-ttu-id="d0570-187">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="d0570-187">msdyn\_plannedcost</span></span>
* <span data-ttu-id="d0570-188">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="d0570-188">msdyn\_plannedsales</span></span>

<span data-ttu-id="d0570-189">नियोजित, वास्तविक और शेष लागत और बिक्री से जुड़े निम्न फील्ड **msdyn\_projecttask** इकाई में अपरिवर्तित हैं:</span><span class="sxs-lookup"><span data-stu-id="d0570-189">The following fields for planned, actual, and remaining cost and sales are unchanged on the **msdyn\_projecttask** entity:</span></span>

* <span data-ttu-id="d0570-190">msdyn\_plannedcost</span><span class="sxs-lookup"><span data-stu-id="d0570-190">msdyn\_plannedcost</span></span>
* <span data-ttu-id="d0570-191">msdyn\_plannedsales</span><span class="sxs-lookup"><span data-stu-id="d0570-191">msdyn\_plannedsales</span></span>
* <span data-ttu-id="d0570-192">msdyn\_actualcost</span><span class="sxs-lookup"><span data-stu-id="d0570-192">msdyn\_actualcost</span></span>
* <span data-ttu-id="d0570-193">msdyn\_actualsales</span><span class="sxs-lookup"><span data-stu-id="d0570-193">msdyn\_actualsales</span></span>
* <span data-ttu-id="d0570-194">msdyn\_remainingcost</span><span class="sxs-lookup"><span data-stu-id="d0570-194">msdyn\_remainingcost</span></span>
* <span data-ttu-id="d0570-195">msdyn\_remainingsales</span><span class="sxs-lookup"><span data-stu-id="d0570-195">msdyn\_remainingsales</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]