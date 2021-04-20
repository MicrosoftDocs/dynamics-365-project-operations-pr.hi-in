---
title: निकाय शेड्यूलिंग के साथ संचालन करने के लिए शेड्यूल APIs का उपयोग करें
description: यह विषय अनुसूची APIs का उपयोग करने के लिए जानकारी और नमूने प्रदान करता है.
author: sigitac
manager: Annbe
ms.date: 04/07/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a50a2c6220bb49de8146d0758019827e120e0526
ms.sourcegitcommit: 8ff9fe396db6dec581c21cd6bb9acc2691c815b0
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/07/2021
ms.locfileid: "5868131"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="a3bc3-103">निकाय शेड्यूलिंग के साथ संचालन करने के लिए शेड्यूल APIs का उपयोग करें</span><span class="sxs-lookup"><span data-stu-id="a3bc3-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="a3bc3-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="a3bc3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="a3bc3-105">इस विषय में नोट की गई कुछ या सभी कार्यक्षमता पूर्वावलोकन रिलीज के हिस्से के रूप में उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="a3bc3-106">सामग्री और कार्यक्षमता परिवर्तन के अधीन हैं.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="a3bc3-107">शेड्यूलिंग निकाय</span><span class="sxs-lookup"><span data-stu-id="a3bc3-107">Scheduling entities</span></span>

<span data-ttu-id="a3bc3-108">शेड्यूल APIs **निकाय शेड्यूलिंग** के साथ निर्माण, अपडेट और हटाने के संचालन को करने की क्षमता प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="a3bc3-109">इन निकायों को वेब के लिए परियोजना में शेड्यूलिंग इंजन के माध्यम से प्रबंधित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="a3bc3-110">पहले Dynamics 365 Project Operations रिलीज़ में **निकाय शेड्यूलिंग** के साथ संचालन बनाएं, अपडेट करें और मिटाएं.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="a3bc3-111">निम्नलिखित तालिका **निकाय शेड्यूलिंग** की पूरी लिस्ट प्रदान करती है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="a3bc3-112">निकाय का नाम</span><span class="sxs-lookup"><span data-stu-id="a3bc3-112">Entity name</span></span>  | <span data-ttu-id="a3bc3-113">निकाय तार्किक नाम</span><span class="sxs-lookup"><span data-stu-id="a3bc3-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="a3bc3-114">Project</span><span class="sxs-lookup"><span data-stu-id="a3bc3-114">Project</span></span> | <span data-ttu-id="a3bc3-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="a3bc3-115">msdyn_project</span></span> |
| <span data-ttu-id="a3bc3-116">परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="a3bc3-116">Project Task</span></span>  | <span data-ttu-id="a3bc3-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="a3bc3-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="a3bc3-118">परियोजना कार्य निर्भरता</span><span class="sxs-lookup"><span data-stu-id="a3bc3-118">Project Task Dependency</span></span>  | <span data-ttu-id="a3bc3-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="a3bc3-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="a3bc3-120">संसाधन असाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="a3bc3-120">Resource Assignment</span></span> | <span data-ttu-id="a3bc3-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="a3bc3-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="a3bc3-122">परियोजना बकेट</span><span class="sxs-lookup"><span data-stu-id="a3bc3-122">Project Bucket</span></span>  | <span data-ttu-id="a3bc3-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="a3bc3-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="a3bc3-124">परियोजना टीम सदस्य</span><span class="sxs-lookup"><span data-stu-id="a3bc3-124">Project Team Member</span></span> | <span data-ttu-id="a3bc3-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="a3bc3-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="a3bc3-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="a3bc3-126">OperationSet</span></span>

<span data-ttu-id="a3bc3-127">OperationSet एक यूनिट-ऑफ-वर्क पैटर्न है जिसका उपयोग तब किया जा सकता है जब शेड्यूल प्रभावित करने वाले कई अनुरोधों को लेनदेन के भीतर संसाधित किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="a3bc3-128">APIs शेड्यूल करें</span><span class="sxs-lookup"><span data-stu-id="a3bc3-128">Schedule APIs</span></span>

<span data-ttu-id="a3bc3-129">यह वर्तमान शेड्यूल APIs की लिस्ट है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="a3bc3-130">**msdyn_CreateProjectV1**: इस API का उपयोग एक प्रोज़ेक्ट बनाने के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="a3bc3-131">प्रोज़ेक्ट और डिफॉल्ट प्रोज़ेक्ट बकेट तुरंत बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="a3bc3-132">**msdyn_CreateTeamMemberV1**: इस API का उपयोग प्रोज़ेक्ट टीम के सदस्य बनाने के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="a3bc3-133">टीम के सदस्य का रिकार्ड तुरंत बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="a3bc3-134">**msdyn_CreateOperationSetV1**: इस एपीआई का उपयोग कई अनुरोधों को शेड्यूल करने के लिए किया जा सकता है जिन्हें लेनदेन के भीतर किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="a3bc3-135">**msdyn_PSSCreateV1**: इस एपीआई का उपयोग एक निकाय बनाने के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="a3bc3-136">निकाय शेड्यूलिंग संस्थाओं में से कोई भी हो सकता है जो निर्माण ऑपरेशन का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="a3bc3-137">**msdyn_PSSCreateV1**: इस API का उपयोग एक निकाय अपडेट के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="a3bc3-138">निकाय शेड्यूलिंग संस्थाओं में से कोई भी हो सकता है जो अपडेट ऑपरेशन का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="a3bc3-139">**msdyn_PSSDeleteV1**: इस API को हटाने के लिए एक निकाय इस्तेमाल किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="a3bc3-140">निकाय शेड्यूलिंग संस्थाओं में से कोई भी हो सकता है जो डिलीट ऑपरेशन का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="a3bc3-141">**msdyn_ExecuteOperationSetV1**: इस एपीआई का उपयोग दिए गए ऑपरेशन सेट के भीतर सभी संचालनों को निष्पादित करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="a3bc3-142">OperationSet के साथ शेड्यूल APIs का उपयोग करना</span><span class="sxs-lookup"><span data-stu-id="a3bc3-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="a3bc3-143">क्योंकि दोनों के साथ रिकॉर्ड **CreateProjectV1** और **CreateTeamMemberV1** तुरंत बनाए जाते हैं, इन APIs का उपयोग सीधे **OperationSet** में नहीं किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="a3bc3-144">हालांकि, आप आवश्यक रिकॉर्ड बनाने, **OperationSet** बनाने के लिए API का उपयोग कर सकते हैं, और फिर **OperationSet** में इन पूर्व-निर्मित रिकॉर्ड का उपयोग कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="a3bc3-145">समर्थित संचालन</span><span class="sxs-lookup"><span data-stu-id="a3bc3-145">Supported operations</span></span>

| <span data-ttu-id="a3bc3-146">निकाय शेड्यूलिंग</span><span class="sxs-lookup"><span data-stu-id="a3bc3-146">Scheduling entity</span></span> | <span data-ttu-id="a3bc3-147">निर्माण करें</span><span class="sxs-lookup"><span data-stu-id="a3bc3-147">Create</span></span> | <span data-ttu-id="a3bc3-148">अद्यतित करें</span><span class="sxs-lookup"><span data-stu-id="a3bc3-148">Update</span></span> | <span data-ttu-id="a3bc3-149">हटाएं</span><span class="sxs-lookup"><span data-stu-id="a3bc3-149">Delete</span></span> | <span data-ttu-id="a3bc3-150">महत्वपूर्ण विचार</span><span class="sxs-lookup"><span data-stu-id="a3bc3-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="a3bc3-151">परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="a3bc3-151">Project task</span></span> | <span data-ttu-id="a3bc3-152">हाँ</span><span class="sxs-lookup"><span data-stu-id="a3bc3-152">Yes</span></span> | <span data-ttu-id="a3bc3-153">हाँ</span><span class="sxs-lookup"><span data-stu-id="a3bc3-153">Yes</span></span> | <span data-ttu-id="a3bc3-154">हाँ</span><span class="sxs-lookup"><span data-stu-id="a3bc3-154">Yes</span></span> | <span data-ttu-id="a3bc3-155">कुछ नहीं</span><span class="sxs-lookup"><span data-stu-id="a3bc3-155">None</span></span> |
| <span data-ttu-id="a3bc3-156">प्रोज़ेक्ट कार्य निर्भरता</span><span class="sxs-lookup"><span data-stu-id="a3bc3-156">Project task dependency</span></span> | <span data-ttu-id="a3bc3-157">हाँ</span><span class="sxs-lookup"><span data-stu-id="a3bc3-157">Yes</span></span> | <span data-ttu-id="a3bc3-158">हाँ</span><span class="sxs-lookup"><span data-stu-id="a3bc3-158">Yes</span></span> | | <span data-ttu-id="a3bc3-159">प्रोज़ेक्ट कार्य निर्भरता रिकॉर्ड अपडेट नहीं किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="a3bc3-160">इसके बजाय, एक पुराना रिकॉर्ड हटाया जा सकता है और एक नया रिकॉर्ड बनाया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="a3bc3-161">रिसोर्स असाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="a3bc3-161">Resource assignment</span></span> | <span data-ttu-id="a3bc3-162">हाँ</span><span class="sxs-lookup"><span data-stu-id="a3bc3-162">Yes</span></span> | <span data-ttu-id="a3bc3-163">हाँ</span><span class="sxs-lookup"><span data-stu-id="a3bc3-163">Yes</span></span> | | <span data-ttu-id="a3bc3-164">निम्नलिखित फ़ील्ड के साथ संचालन का समर्थन नहीं किया जाता है: **BookableResourceID**, **प्रयास**,**EffortCompleted**, **EffortRemaining**, और **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="a3bc3-165">संसाधन असाइनमेंट रिकॉर्ड अपडेट नहीं किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="a3bc3-166">इसके बदले पुराना रिकॉर्ड डिलीट किया जा सकता है और नया रिकॉर्ड बनाया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="a3bc3-167">प्रोज़ेक्ट बकेट</span><span class="sxs-lookup"><span data-stu-id="a3bc3-167">Project bucket</span></span> | <span data-ttu-id="a3bc3-168">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="a3bc3-168">N/A</span></span> | <span data-ttu-id="a3bc3-169">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="a3bc3-169">N/A</span></span> | <span data-ttu-id="a3bc3-170">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="a3bc3-170">N/A</span></span> | <span data-ttu-id="a3bc3-171">डिफ़ॉल्ट बकेट **CreateProjectV1** API का उपयोग करके बनाई गई है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="a3bc3-172">प्रोजेक्ट टीम सदस्य</span><span class="sxs-lookup"><span data-stu-id="a3bc3-172">Project team member</span></span> | <span data-ttu-id="a3bc3-173">हाँ</span><span class="sxs-lookup"><span data-stu-id="a3bc3-173">Yes</span></span> | <span data-ttu-id="a3bc3-174">हाँ</span><span class="sxs-lookup"><span data-stu-id="a3bc3-174">Yes</span></span> | <span data-ttu-id="a3bc3-175">हाँ</span><span class="sxs-lookup"><span data-stu-id="a3bc3-175">Yes</span></span> | <span data-ttu-id="a3bc3-176">बनाने के ऑपरेशन के लिए, **CreateTeamMemberV1** API का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="a3bc3-177">Project</span><span class="sxs-lookup"><span data-stu-id="a3bc3-177">Project</span></span> | <span data-ttu-id="a3bc3-178">हाँ</span><span class="sxs-lookup"><span data-stu-id="a3bc3-178">Yes</span></span> | <span data-ttu-id="a3bc3-179">हाँ</span><span class="sxs-lookup"><span data-stu-id="a3bc3-179">Yes</span></span> | <span data-ttu-id="a3bc3-180">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="a3bc3-180">N/A</span></span> | <span data-ttu-id="a3bc3-181">निम्नलिखित फ़ील्ड के साथ संचालन का समर्थन नहीं किया जाता है: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **प्रयास**, **EffortCompleted**, **EffortRemaining**, **प्रगति**, **समाप्त करें**, **TaskEarliestStart**, और **अवधि**.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="a3bc3-182">इन APIs को निकाय ऑब्जेक्ट्स के साथ बुलाया जा सकता है जिसमें कस्टम फ़ील्ड शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="a3bc3-183">ID संपत्ति वैकल्पिक है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-183">The ID property is optional.</span></span> <span data-ttu-id="a3bc3-184">यदि यह प्रदान किया जाता है, तो सिस्टम इसका उपयोग करने का प्रयास करता है और यदि इसका उपयोग नहीं किया जा सकता है तो अपवाद प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="a3bc3-185">यदि यह प्रदान नहीं किया जाता है, तो सिस्टम इसे उत्पन्न करेगा.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-185">If it isn't provided, the system will generate it.</span></span>

## <a name="limitations-and-known-issues"></a><span data-ttu-id="a3bc3-186">सीमाएं और ज्ञात मुद्दे</span><span class="sxs-lookup"><span data-stu-id="a3bc3-186">Limitations and known issues</span></span>
<span data-ttu-id="a3bc3-187">निम्नलिखित सीमाओं और ज्ञात मुद्दों की एक लिस्ट है:</span><span class="sxs-lookup"><span data-stu-id="a3bc3-187">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="a3bc3-188">शेड्यूल एपीआई का उपयोग केवल **Microsoft प्रोज़ेक्ट लाइसेंस वाले** उपयोगकर्ताओं द्वारा किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-188">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="a3bc3-189">उनका इनके द्वारा उपयोग नहीं किया जा सकता है:</span><span class="sxs-lookup"><span data-stu-id="a3bc3-189">They can't be used by:</span></span>
    - <span data-ttu-id="a3bc3-190">अनुप्रयोग उपयोगकर्ता</span><span class="sxs-lookup"><span data-stu-id="a3bc3-190">Application users</span></span>
    - <span data-ttu-id="a3bc3-191">सिस्टम उपयोगकर्ता</span><span class="sxs-lookup"><span data-stu-id="a3bc3-191">System users</span></span>
    - <span data-ttu-id="a3bc3-192">एकीकरण उपयोगकर्ता</span><span class="sxs-lookup"><span data-stu-id="a3bc3-192">Integration users</span></span>
    - <span data-ttu-id="a3bc3-193">अन्य उपयोगकर्ता जिनके पास आवश्यक लाइसेंस नहीं है</span><span class="sxs-lookup"><span data-stu-id="a3bc3-193">Other users that don't have the required license</span></span>
- <span data-ttu-id="a3bc3-194">प्रत्येक **OperationSet** में अधिकतम 100 संचालन हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-194">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="a3bc3-195">प्रत्येक उपयोगकर्ता के पास अधिकतम 10 खुला **OperationSets** हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-195">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="a3bc3-196">Project Operations वर्तमान में एक प्रोज़ेक्ट पर अधिकतम 500 कुल कार्यों का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-196">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="a3bc3-197">**OperationSet** विफलता की स्थिति और विफलता लॉग वर्तमान में उपलब्ध नहीं हैं.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-197">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- <span data-ttu-id="a3bc3-198">शेड्यूल एपीआई सार्वजनिक पूर्वावलोकन में हैं.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-198">Schedule APIs are in Public preview.</span></span> <span data-ttu-id="a3bc3-199">उत्पादन परिवेश में इन एपीआई का उपयोग करना Microsoft द्वारा समर्थित नहीं है.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-199">Using these APIs in a Production environment isn't supported by Microsoft.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="a3bc3-200">नमूना परिदृश्य</span><span class="sxs-lookup"><span data-stu-id="a3bc3-200">Sample scenario</span></span>

<span data-ttu-id="a3bc3-201">इस परिदृश्य में, आप एक प्रोज़ेक्ट, एक टीम के सदस्य, चार कार्य और दो संसाधन कार्य बनाएंगे.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-201">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="a3bc3-202">इसके बाद, आप एक कार्य को अपडेट करेंगे, प्रोज़ेक्ट को अपडेट करेंगे, एक कार्य को हटा देंगे, एक संसाधन असाइनमेंट को हटा देंगे,और एक कार्य निर्भरता बनाएंगे.</span><span class="sxs-lookup"><span data-stu-id="a3bc3-202">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

```C#
Entity project = CreateProject();
project.Id = CallCreateProjectAction(project);
var projectReference = project.ToEntityReference();

var teamMember = new Entity("msdyn_projectteam", Guid.NewGuid());
teamMember["msdyn_name"] = $"TM {DateTime.Now.ToShortTimeString()}";
teamMember["msdyn_project"] = projectReference;
var createTeamMemberResponse = CallCreateTeamMemberAction(teamMember);

var description = $"My demo {DateTime.Now.ToShortTimeString()}";
var operationSetId = CallCreateOperationSetAction(project.Id, description);

var task1 = GetTask("1WW", projectReference);
var task2 = GetTask("2XX", projectReference, task1.ToEntityReference());
var task3 = GetTask("3YY", projectReference);
var task4 = GetTask("4ZZ";, projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment"R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

varassignment1Response = CallPssCreateAction(assignment1, operationSetId);
varassignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

varassignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a><span data-ttu-id="a3bc3-203">अतिरिक्त नमूने</span><span class="sxs-lookup"><span data-stu-id="a3bc3-203">Additional samples</span></span>

```C#
#region Call actions 

///<summary>
/// Calls the action to create an operationSet
/// </summary>
/// <paramname="projectId">project id for the operations to be included in this operationSet>/param>
/// <paramname="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
privatestring CallCreateOperationSetAction(Guid projectId, string description)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_CreateOperationSetV1");
    operationSetRequest["ProjectId"] = projectId.ToString();
    operationSetRequest["Description"] = description;
    OrganizationResponse response = organizationService.Execute(operationSetRequest);
    return response["OperationSetId"].ToString();
}

/// <summary>
/// Calls the action to create an entity, only Task and Resource Assignment for now
/// </summary>
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary<
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssUpdateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssUpdateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task and Resource Assignment for now
/// <summary>
/// <paramname="recordId">Id of the record to be deleted</param>
/// <paramname="entityLogicalName">Entity logical name of the record</param>
/// <paramname="operationSetId">OperationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssDeleteAction(string recordId, string entityLogicalName, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssDeleteV1");
    operationSetRequest["RecordId"] = recordId;
    operationSetRequest["EntityLogicalName"] = entityLogicalName;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to execute requests in an operationSet
/// <summary>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallExecuteOperationSetAction(string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_ExecuteOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// This can be used to abandon an operationSet that is no longer needed
/// </summary>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
protected OperationSetResponse CallAbandonOperationSetAction(Guid operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_AbandonOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId.ToString();
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to create a new project
/// </summary>
/// <paramname="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1";
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);

    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <paramname="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
privatestring CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject><OperationSetResponse>
    ((string)orgResponse.Results["OperationSetResponse";]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet(";msdyn_project", "msdyn_name");
    var getDefaultBucket = new QueryExpression("msdyn_projectbucket")
    {
        ColumnSet = columnsToFetch,
        Criteria =
        {
            Conditions =
            {
                new ConditionExpression("msdyn_project", ConditionOperator.Equal, projectReference.Id),
                new ConditionExpression("msdyn_name", ConditionOperator.Equal, "Bucket 1")
            }
        }
    };
    return organizationService.RetrieveMultiple(getDefaultBucket);
}

private Entity GetBucket(EntityReference projectReference)
{
    var bucketCollection = GetDefaultBucket(projectReference);
    if (bucketCollection.Entities.Count > 0)
    {
    return bucketCollection[0].ToEntity<Entity>();
    }

    throw new Exception($"Please open project with id {projectReference.Id} in the Dynamics UI and navigate to the Tasks tab");
}

private Entity CreateProject()
{
    var project = new Entity("msdyn_project", Guid.NewGuid());
    project["msdyn_subject"] = $"Proj {DateTime.Now.ToShortTimeString()}";
    return project;
}

private Entity GetTask(string name, EntityReference projectReference, EntityReference parentReference = null)
{
    var task = new Entity("msdyn_projecttask", Guid.NewGuid());
    task["msdyn_project"] = projectReference;
    task["msdyn_subject"] = name;
    task["msdyn_effort";] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
        task["new_custom1"] = "Just my test";
        task[";new_age"] = 98;
        task["new_amount"] = 591.34m;
        task["new_isready"] = new OptionSetValue(100000000);
    */

    if (parentReference == null)
    {
        task["msdyn_outlinelevel"] = 1;
    }
    else
    {
        task["msdyn_parenttask"] = parentReference;
    }
    return task;
}

private Entity GetResourceAssignment(string name, Entity teamMember, Entity task, Entity project)
{
    var assignment = new Entity("msdyn_resourceassignment", Guid.NewGuid());
    assignment["msdyn_projectteamid"] = teamMember.ToEntityReference();
    assignment["msdyn_taskid"] = task.ToEntityReference();
    assignment["msdyn_projectid"] = project.ToEntityReference();
    assignment["msdyn_name"] = name;
    assignment["msdyn_start"] = DateTime.Now;
    assignment["msdyn_finish"] = DateTime.Now;
    return assignment;
}

protected Entity GetTaskDependency(Entity project, Entity predecessor, Entity successor)
{
    var taskDependency = new Entity("msdyn_projecttaskdependency", Guid.NewGuid());
    taskDependency["msdyn_project"] = project.ToEntityReference();
    taskDependency["msdyn_predecessortask"] = predecessor.ToEntityReference();
    taskDependency["msdyn_successortask"] = successor.ToEntityReference();
    taskDependency["msdyn_linktype"] = new OptionSetValue(192350000);
    return taskDependency;
}

#endregion

#region OperationSetResponse DataContract --- Sample code ----

[DataContract]
publicclassOperationSetResponse
{
    [DataMember(Name = "operationSetId")]
    public Guid OperationSetId { get; set; }

    [DataMember(Name = "operationSetDetailId")]
    public Guid OperationSetDetailId { get; set; }

    [DataMember(Name = "operationType")]
    publicstring OperationType { get; set; }

    [DataMember(Name = "recordId")]
    publicstring RecordId { get; set; }

    [DataMember(Name = "correlationId")]
    publicstring CorrelationId { get; set; }
}

#endregion
```
