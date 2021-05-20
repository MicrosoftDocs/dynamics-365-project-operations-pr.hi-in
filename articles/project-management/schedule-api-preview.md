---
title: निकाय शेड्यूलिंग के साथ संचालन करने के लिए शेड्यूल APIs का उपयोग करें
description: यह विषय अनुसूची APIs का उपयोग करने के लिए जानकारी और नमूने प्रदान करता है.
author: sigitac
manager: Annbe
ms.date: 04/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: e03f4e6c49a835206b23cade3fabe3fd26693441
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/27/2021
ms.locfileid: "5950806"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="ecfe3-103">निकाय शेड्यूलिंग के साथ संचालन करने के लिए शेड्यूल APIs का उपयोग करें</span><span class="sxs-lookup"><span data-stu-id="ecfe3-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="ecfe3-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="ecfe3-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="ecfe3-105">इस विषय में नोट की गई कुछ या सभी कार्यक्षमता पूर्वावलोकन रिलीज के हिस्से के रूप में उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="ecfe3-106">सामग्री और कार्यक्षमता परिवर्तन के अधीन हैं.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="ecfe3-107">शेड्यूलिंग निकाय</span><span class="sxs-lookup"><span data-stu-id="ecfe3-107">Scheduling entities</span></span>

<span data-ttu-id="ecfe3-108">शेड्यूल APIs **निकाय शेड्यूलिंग** के साथ निर्माण, अपडेट और हटाने के संचालन को करने की क्षमता प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="ecfe3-109">इन निकायों को वेब के लिए परियोजना में शेड्यूलिंग इंजन के माध्यम से प्रबंधित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="ecfe3-110">पहले Dynamics 365 Project Operations रिलीज़ में **निकाय शेड्यूलिंग** के साथ संचालन बनाएं, अपडेट करें और मिटाएं.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="ecfe3-111">निम्नलिखित तालिका **निकाय शेड्यूलिंग** की पूरी लिस्ट प्रदान करती है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="ecfe3-112">निकाय का नाम</span><span class="sxs-lookup"><span data-stu-id="ecfe3-112">Entity name</span></span>  | <span data-ttu-id="ecfe3-113">निकाय तार्किक नाम</span><span class="sxs-lookup"><span data-stu-id="ecfe3-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="ecfe3-114">Project</span><span class="sxs-lookup"><span data-stu-id="ecfe3-114">Project</span></span> | <span data-ttu-id="ecfe3-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="ecfe3-115">msdyn_project</span></span> |
| <span data-ttu-id="ecfe3-116">परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="ecfe3-116">Project Task</span></span>  | <span data-ttu-id="ecfe3-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="ecfe3-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="ecfe3-118">परियोजना कार्य निर्भरता</span><span class="sxs-lookup"><span data-stu-id="ecfe3-118">Project Task Dependency</span></span>  | <span data-ttu-id="ecfe3-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="ecfe3-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="ecfe3-120">संसाधन असाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="ecfe3-120">Resource Assignment</span></span> | <span data-ttu-id="ecfe3-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="ecfe3-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="ecfe3-122">परियोजना बकेट</span><span class="sxs-lookup"><span data-stu-id="ecfe3-122">Project Bucket</span></span>  | <span data-ttu-id="ecfe3-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="ecfe3-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="ecfe3-124">परियोजना टीम सदस्य</span><span class="sxs-lookup"><span data-stu-id="ecfe3-124">Project Team Member</span></span> | <span data-ttu-id="ecfe3-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="ecfe3-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="ecfe3-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="ecfe3-126">OperationSet</span></span>

<span data-ttu-id="ecfe3-127">OperationSet एक यूनिट-ऑफ-वर्क पैटर्न है जिसका उपयोग तब किया जा सकता है जब शेड्यूल प्रभावित करने वाले कई अनुरोधों को लेनदेन के भीतर संसाधित किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="ecfe3-128">APIs शेड्यूल करें</span><span class="sxs-lookup"><span data-stu-id="ecfe3-128">Schedule APIs</span></span>

<span data-ttu-id="ecfe3-129">यह वर्तमान शेड्यूल APIs की लिस्ट है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="ecfe3-130">**msdyn_CreateProjectV1**: इस API का उपयोग एक प्रोज़ेक्ट बनाने के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="ecfe3-131">प्रोज़ेक्ट और डिफॉल्ट प्रोज़ेक्ट बकेट तुरंत बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="ecfe3-132">**msdyn_CreateTeamMemberV1**: इस API का उपयोग प्रोज़ेक्ट टीम के सदस्य बनाने के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="ecfe3-133">टीम के सदस्य का रिकार्ड तुरंत बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="ecfe3-134">**msdyn_CreateOperationSetV1**: इस एपीआई का उपयोग कई अनुरोधों को शेड्यूल करने के लिए किया जा सकता है जिन्हें लेनदेन के भीतर किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="ecfe3-135">**msdyn_PSSCreateV1**: इस एपीआई का उपयोग एक निकाय बनाने के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="ecfe3-136">निकाय शेड्यूलिंग संस्थाओं में से कोई भी हो सकता है जो निर्माण ऑपरेशन का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="ecfe3-137">**msdyn_PSSCreateV1**: इस API का उपयोग एक निकाय अपडेट के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="ecfe3-138">निकाय शेड्यूलिंग संस्थाओं में से कोई भी हो सकता है जो अपडेट ऑपरेशन का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="ecfe3-139">**msdyn_PSSDeleteV1**: इस API को हटाने के लिए एक निकाय इस्तेमाल किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="ecfe3-140">निकाय शेड्यूलिंग संस्थाओं में से कोई भी हो सकता है जो डिलीट ऑपरेशन का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="ecfe3-141">**msdyn_ExecuteOperationSetV1**: इस एपीआई का उपयोग दिए गए ऑपरेशन सेट के भीतर सभी संचालनों को निष्पादित करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="ecfe3-142">OperationSet के साथ शेड्यूल APIs का उपयोग करना</span><span class="sxs-lookup"><span data-stu-id="ecfe3-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="ecfe3-143">क्योंकि दोनों के साथ रिकॉर्ड **CreateProjectV1** और **CreateTeamMemberV1** तुरंत बनाए जाते हैं, इन APIs का उपयोग सीधे **OperationSet** में नहीं किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="ecfe3-144">हालांकि, आप आवश्यक रिकॉर्ड बनाने, **OperationSet** बनाने के लिए API का उपयोग कर सकते हैं, और फिर **OperationSet** में इन पूर्व-निर्मित रिकॉर्ड का उपयोग कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="ecfe3-145">समर्थित संचालन</span><span class="sxs-lookup"><span data-stu-id="ecfe3-145">Supported operations</span></span>

| <span data-ttu-id="ecfe3-146">निकाय शेड्यूलिंग</span><span class="sxs-lookup"><span data-stu-id="ecfe3-146">Scheduling entity</span></span> | <span data-ttu-id="ecfe3-147">निर्माण करें</span><span class="sxs-lookup"><span data-stu-id="ecfe3-147">Create</span></span> | <span data-ttu-id="ecfe3-148">अद्यतित करें</span><span class="sxs-lookup"><span data-stu-id="ecfe3-148">Update</span></span> | <span data-ttu-id="ecfe3-149">हटाएं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-149">Delete</span></span> | <span data-ttu-id="ecfe3-150">महत्वपूर्ण विचार</span><span class="sxs-lookup"><span data-stu-id="ecfe3-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="ecfe3-151">परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="ecfe3-151">Project task</span></span> | <span data-ttu-id="ecfe3-152">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-152">Yes</span></span> | <span data-ttu-id="ecfe3-153">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-153">Yes</span></span> | <span data-ttu-id="ecfe3-154">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-154">Yes</span></span> | <span data-ttu-id="ecfe3-155">कुछ नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-155">None</span></span> |
| <span data-ttu-id="ecfe3-156">प्रोज़ेक्ट कार्य निर्भरता</span><span class="sxs-lookup"><span data-stu-id="ecfe3-156">Project task dependency</span></span> | <span data-ttu-id="ecfe3-157">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-157">Yes</span></span> | <span data-ttu-id="ecfe3-158">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-158">Yes</span></span> | | <span data-ttu-id="ecfe3-159">प्रोज़ेक्ट कार्य निर्भरता रिकॉर्ड अपडेट नहीं किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="ecfe3-160">इसके बजाय, एक पुराना रिकॉर्ड हटाया जा सकता है और एक नया रिकॉर्ड बनाया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="ecfe3-161">रिसोर्स असाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="ecfe3-161">Resource assignment</span></span> | <span data-ttu-id="ecfe3-162">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-162">Yes</span></span> | <span data-ttu-id="ecfe3-163">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-163">Yes</span></span> | | <span data-ttu-id="ecfe3-164">निम्नलिखित फ़ील्ड के साथ संचालन का समर्थन नहीं किया जाता है: **BookableResourceID**, **प्रयास**,**EffortCompleted**, **EffortRemaining**, और **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="ecfe3-165">संसाधन असाइनमेंट रिकॉर्ड अपडेट नहीं किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="ecfe3-166">इसके बदले पुराना रिकॉर्ड डिलीट किया जा सकता है और नया रिकॉर्ड बनाया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="ecfe3-167">प्रोज़ेक्ट बकेट</span><span class="sxs-lookup"><span data-stu-id="ecfe3-167">Project bucket</span></span> | <span data-ttu-id="ecfe3-168">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-168">N/A</span></span> | <span data-ttu-id="ecfe3-169">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-169">N/A</span></span> | <span data-ttu-id="ecfe3-170">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-170">N/A</span></span> | <span data-ttu-id="ecfe3-171">डिफ़ॉल्ट बकेट **CreateProjectV1** API का उपयोग करके बनाई गई है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="ecfe3-172">प्रोजेक्ट टीम सदस्य</span><span class="sxs-lookup"><span data-stu-id="ecfe3-172">Project team member</span></span> | <span data-ttu-id="ecfe3-173">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-173">Yes</span></span> | <span data-ttu-id="ecfe3-174">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-174">Yes</span></span> | <span data-ttu-id="ecfe3-175">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-175">Yes</span></span> | <span data-ttu-id="ecfe3-176">बनाने के ऑपरेशन के लिए, **CreateTeamMemberV1** API का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="ecfe3-177">Project</span><span class="sxs-lookup"><span data-stu-id="ecfe3-177">Project</span></span> | <span data-ttu-id="ecfe3-178">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-178">Yes</span></span> | <span data-ttu-id="ecfe3-179">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-179">Yes</span></span> | <span data-ttu-id="ecfe3-180">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-180">N/A</span></span> | <span data-ttu-id="ecfe3-181">निम्नलिखित फ़ील्ड के साथ संचालन का समर्थन नहीं किया जाता है: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **प्रयास**, **EffortCompleted**, **EffortRemaining**, **प्रगति**, **समाप्त करें**, **TaskEarliestStart**, और **अवधि**.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="ecfe3-182">इन APIs को निकाय ऑब्जेक्ट्स के साथ बुलाया जा सकता है जिसमें कस्टम फ़ील्ड शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="ecfe3-183">ID संपत्ति वैकल्पिक है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-183">The ID property is optional.</span></span> <span data-ttu-id="ecfe3-184">यदि यह प्रदान किया जाता है, तो सिस्टम इसका उपयोग करने का प्रयास करता है और यदि इसका उपयोग नहीं किया जा सकता है तो अपवाद प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="ecfe3-185">यदि यह प्रदान नहीं किया जाता है, तो सिस्टम इसे उत्पन्न करेगा.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="ecfe3-186">प्रतिबंधित फील्ड</span><span class="sxs-lookup"><span data-stu-id="ecfe3-186">Restricted fields</span></span>

<span data-ttu-id="ecfe3-187">निम्न तालिका उन क्षेत्रों को परिभाषित करती है जो **बनाएं** और **संपादित करें** से प्रतिबंधित हैं.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="ecfe3-188">परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="ecfe3-188">Project task</span></span>

| <span data-ttu-id="ecfe3-189">**तार्किक नाम**</span><span class="sxs-lookup"><span data-stu-id="ecfe3-189">**Logical name**</span></span>                       | <span data-ttu-id="ecfe3-190">**बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="ecfe3-190">**Can create**</span></span> | <span data-ttu-id="ecfe3-191">**संपादित कर सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="ecfe3-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="ecfe3-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="ecfe3-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="ecfe3-193">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-193">no</span></span>             | <span data-ttu-id="ecfe3-194">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-194">no</span></span>               |
| <span data-ttu-id="ecfe3-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="ecfe3-196">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-196">no</span></span>             | <span data-ttu-id="ecfe3-197">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-197">no</span></span>               |
| <span data-ttu-id="ecfe3-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="ecfe3-198">msdyn_actualend</span></span>                        | <span data-ttu-id="ecfe3-199">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-199">no</span></span>             | <span data-ttu-id="ecfe3-200">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-200">no</span></span>               |
| <span data-ttu-id="ecfe3-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="ecfe3-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="ecfe3-202">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-202">no</span></span>             | <span data-ttu-id="ecfe3-203">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-203">no</span></span>               |
| <span data-ttu-id="ecfe3-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="ecfe3-205">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-205">no</span></span>             | <span data-ttu-id="ecfe3-206">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-206">no</span></span>               |
| <span data-ttu-id="ecfe3-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="ecfe3-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="ecfe3-208">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-208">no</span></span>             | <span data-ttu-id="ecfe3-209">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-209">no</span></span>               |
| <span data-ttu-id="ecfe3-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="ecfe3-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="ecfe3-211">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-211">no</span></span>             | <span data-ttu-id="ecfe3-212">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-212">no</span></span>               |
| <span data-ttu-id="ecfe3-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="ecfe3-214">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-214">no</span></span>             | <span data-ttu-id="ecfe3-215">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-215">no</span></span>               |
| <span data-ttu-id="ecfe3-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="ecfe3-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="ecfe3-217">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-217">no</span></span>             | <span data-ttu-id="ecfe3-218">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-218">no</span></span>               |
| <span data-ttu-id="ecfe3-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="ecfe3-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="ecfe3-220">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-220">no</span></span>             | <span data-ttu-id="ecfe3-221">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-221">no</span></span>               |
| <span data-ttu-id="ecfe3-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="ecfe3-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="ecfe3-223">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-223">no</span></span>             | <span data-ttu-id="ecfe3-224">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-224">no</span></span>               |
| <span data-ttu-id="ecfe3-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="ecfe3-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="ecfe3-226">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-226">no</span></span>             | <span data-ttu-id="ecfe3-227">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-227">no</span></span>               |
| <span data-ttu-id="ecfe3-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="ecfe3-229">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-229">no</span></span>             | <span data-ttu-id="ecfe3-230">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-230">no</span></span>               |
| <span data-ttu-id="ecfe3-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="ecfe3-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="ecfe3-232">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-232">no</span></span>             | <span data-ttu-id="ecfe3-233">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-233">no</span></span>               |
| <span data-ttu-id="ecfe3-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="ecfe3-235">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-235">no</span></span>             | <span data-ttu-id="ecfe3-236">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-236">no</span></span>               |
| <span data-ttu-id="ecfe3-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="ecfe3-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="ecfe3-238">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-238">no</span></span>             | <span data-ttu-id="ecfe3-239">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-239">no</span></span>               |
| <span data-ttu-id="ecfe3-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="ecfe3-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="ecfe3-241">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-241">no</span></span>             | <span data-ttu-id="ecfe3-242">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-242">no</span></span>               |
| <span data-ttu-id="ecfe3-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="ecfe3-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="ecfe3-244">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-244">no</span></span>             | <span data-ttu-id="ecfe3-245">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-245">no</span></span>               |
| <span data-ttu-id="ecfe3-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="ecfe3-247">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-247">no</span></span>             | <span data-ttu-id="ecfe3-248">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-248">no</span></span>               |
| <span data-ttu-id="ecfe3-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="ecfe3-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="ecfe3-250">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-250">no</span></span>             | <span data-ttu-id="ecfe3-251">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-251">no</span></span>               |
| <span data-ttu-id="ecfe3-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="ecfe3-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="ecfe3-253">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-253">no</span></span>             | <span data-ttu-id="ecfe3-254">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-254">no</span></span>               |
| <span data-ttu-id="ecfe3-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="ecfe3-256">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-256">no</span></span>             | <span data-ttu-id="ecfe3-257">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-257">no</span></span>               |
| <span data-ttu-id="ecfe3-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="ecfe3-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="ecfe3-259">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-259">no</span></span>             | <span data-ttu-id="ecfe3-260">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-260">no</span></span>               |
| <span data-ttu-id="ecfe3-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="ecfe3-262">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-262">no</span></span>             | <span data-ttu-id="ecfe3-263">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-263">no</span></span>               |
| <span data-ttu-id="ecfe3-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="ecfe3-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="ecfe3-265">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-265">no</span></span>             | <span data-ttu-id="ecfe3-266">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-266">no</span></span>               |
| <span data-ttu-id="ecfe3-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="ecfe3-267">msdyn_progress</span></span>                         | <span data-ttu-id="ecfe3-268">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-268">no</span></span>             | <span data-ttu-id="ecfe3-269">नही ( P4W के लिए हां)</span><span class="sxs-lookup"><span data-stu-id="ecfe3-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="ecfe3-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="ecfe3-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="ecfe3-271">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-271">no</span></span>             | <span data-ttu-id="ecfe3-272">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-272">no</span></span>               |
| <span data-ttu-id="ecfe3-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="ecfe3-274">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-274">no</span></span>             | <span data-ttu-id="ecfe3-275">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-275">no</span></span>               |
| <span data-ttu-id="ecfe3-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="ecfe3-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="ecfe3-277">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-277">no</span></span>             | <span data-ttu-id="ecfe3-278">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-278">no</span></span>               |
| <span data-ttu-id="ecfe3-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="ecfe3-280">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-280">no</span></span>             | <span data-ttu-id="ecfe3-281">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-281">no</span></span>               |
| <span data-ttu-id="ecfe3-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="ecfe3-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="ecfe3-283">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-283">no</span></span>             | <span data-ttu-id="ecfe3-284">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-284">no</span></span>               |
| <span data-ttu-id="ecfe3-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="ecfe3-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="ecfe3-286">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-286">no</span></span>             | <span data-ttu-id="ecfe3-287">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-287">no</span></span>               |
| <span data-ttu-id="ecfe3-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="ecfe3-289">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-289">no</span></span>             | <span data-ttu-id="ecfe3-290">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-290">no</span></span>               |
| <span data-ttu-id="ecfe3-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="ecfe3-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="ecfe3-292">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-292">no</span></span>             | <span data-ttu-id="ecfe3-293">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-293">no</span></span>               |
| <span data-ttu-id="ecfe3-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="ecfe3-295">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-295">no</span></span>             | <span data-ttu-id="ecfe3-296">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-296">no</span></span>               |
| <span data-ttu-id="ecfe3-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="ecfe3-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="ecfe3-298">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-298">no</span></span>             | <span data-ttu-id="ecfe3-299">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-299">no</span></span>               |
| <span data-ttu-id="ecfe3-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="ecfe3-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="ecfe3-301">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-301">no</span></span>             | <span data-ttu-id="ecfe3-302">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-302">no</span></span>               |
| <span data-ttu-id="ecfe3-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="ecfe3-304">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-304">no</span></span>             | <span data-ttu-id="ecfe3-305">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-305">no</span></span>               |
| <span data-ttu-id="ecfe3-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="ecfe3-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="ecfe3-307">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-307">no</span></span>             | <span data-ttu-id="ecfe3-308">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-308">no</span></span>               |
| <span data-ttu-id="ecfe3-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="ecfe3-310">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-310">no</span></span>             | <span data-ttu-id="ecfe3-311">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-311">no</span></span>               |
| <span data-ttu-id="ecfe3-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="ecfe3-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="ecfe3-313">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-313">no</span></span>             | <span data-ttu-id="ecfe3-314">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-314">no</span></span>               |
| <span data-ttu-id="ecfe3-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="ecfe3-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="ecfe3-316">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-316">no</span></span>             | <span data-ttu-id="ecfe3-317">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-317">no</span></span>               |
| <span data-ttu-id="ecfe3-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="ecfe3-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="ecfe3-319">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-319">no</span></span>             | <span data-ttu-id="ecfe3-320">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-320">no</span></span>               |
| <span data-ttu-id="ecfe3-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="ecfe3-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="ecfe3-322">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-322">no</span></span>             | <span data-ttu-id="ecfe3-323">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-323">no</span></span>               |
| <span data-ttu-id="ecfe3-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="ecfe3-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="ecfe3-325">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-325">no</span></span>             | <span data-ttu-id="ecfe3-326">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-326">no</span></span>               |
| <span data-ttu-id="ecfe3-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="ecfe3-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="ecfe3-328">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-328">no</span></span>             | <span data-ttu-id="ecfe3-329">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-329">no</span></span>               |
| <span data-ttu-id="ecfe3-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="ecfe3-330">msdyn_summary</span></span>                          | <span data-ttu-id="ecfe3-331">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-331">no</span></span>             | <span data-ttu-id="ecfe3-332">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-332">no</span></span>               |
| <span data-ttu-id="ecfe3-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="ecfe3-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="ecfe3-334">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-334">no</span></span>             | <span data-ttu-id="ecfe3-335">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-335">no</span></span>               |
| <span data-ttu-id="ecfe3-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="ecfe3-337">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-337">no</span></span>             | <span data-ttu-id="ecfe3-338">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="ecfe3-339">प्रोज़ेक्ट कार्य निर्भरता</span><span class="sxs-lookup"><span data-stu-id="ecfe3-339">Project task dependency</span></span>

| <span data-ttu-id="ecfe3-340">**तार्किक नाम**</span><span class="sxs-lookup"><span data-stu-id="ecfe3-340">**Logical name**</span></span>              | <span data-ttu-id="ecfe3-341">**बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="ecfe3-341">**Can create**</span></span> | <span data-ttu-id="ecfe3-342">**संपादित कर सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="ecfe3-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="ecfe3-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="ecfe3-343">msdyn_linktype</span></span>                | <span data-ttu-id="ecfe3-344">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-344">no</span></span>             | <span data-ttu-id="ecfe3-345">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-345">no</span></span>           |
| <span data-ttu-id="ecfe3-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="ecfe3-346">msdyn_linktypename</span></span>            | <span data-ttu-id="ecfe3-347">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-347">no</span></span>             | <span data-ttu-id="ecfe3-348">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-348">no</span></span>           |
| <span data-ttu-id="ecfe3-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="ecfe3-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="ecfe3-350">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-350">yes</span></span>            | <span data-ttu-id="ecfe3-351">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-351">no</span></span>           |
| <span data-ttu-id="ecfe3-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="ecfe3-353">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-353">yes</span></span>            | <span data-ttu-id="ecfe3-354">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-354">no</span></span>           |
| <span data-ttu-id="ecfe3-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="ecfe3-355">msdyn_project</span></span>                 | <span data-ttu-id="ecfe3-356">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-356">yes</span></span>            | <span data-ttu-id="ecfe3-357">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-357">no</span></span>           |
| <span data-ttu-id="ecfe3-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-358">msdyn_projectname</span></span>             | <span data-ttu-id="ecfe3-359">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-359">yes</span></span>            | <span data-ttu-id="ecfe3-360">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-360">no</span></span>           |
| <span data-ttu-id="ecfe3-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="ecfe3-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="ecfe3-362">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-362">yes</span></span>            | <span data-ttu-id="ecfe3-363">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-363">no</span></span>           |
| <span data-ttu-id="ecfe3-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="ecfe3-364">msdyn_successortask</span></span>           | <span data-ttu-id="ecfe3-365">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-365">yes</span></span>            | <span data-ttu-id="ecfe3-366">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-366">no</span></span>           |
| <span data-ttu-id="ecfe3-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="ecfe3-368">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-368">yes</span></span>            | <span data-ttu-id="ecfe3-369">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="ecfe3-370">रिसोर्स असाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="ecfe3-370">Resource assignment</span></span>

| <span data-ttu-id="ecfe3-371">**तार्किक नाम**</span><span class="sxs-lookup"><span data-stu-id="ecfe3-371">**Logical name**</span></span>             | <span data-ttu-id="ecfe3-372">**बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="ecfe3-372">**Can create**</span></span> | <span data-ttu-id="ecfe3-373">**संपादित कर सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="ecfe3-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="ecfe3-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="ecfe3-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="ecfe3-375">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-375">yes</span></span>            | <span data-ttu-id="ecfe3-376">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-376">no</span></span>           |
| <span data-ttu-id="ecfe3-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="ecfe3-378">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-378">yes</span></span>            | <span data-ttu-id="ecfe3-379">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-379">no</span></span>           |
| <span data-ttu-id="ecfe3-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="ecfe3-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="ecfe3-381">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-381">no</span></span>             | <span data-ttu-id="ecfe3-382">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-382">no</span></span>           |
| <span data-ttu-id="ecfe3-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="ecfe3-384">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-384">no</span></span>             | <span data-ttu-id="ecfe3-385">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-385">no</span></span>           |
| <span data-ttu-id="ecfe3-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="ecfe3-386">msdyn_committype</span></span>             | <span data-ttu-id="ecfe3-387">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-387">no</span></span>             | <span data-ttu-id="ecfe3-388">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-388">no</span></span>           |
| <span data-ttu-id="ecfe3-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="ecfe3-389">msdyn_committypename</span></span>         | <span data-ttu-id="ecfe3-390">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-390">no</span></span>             | <span data-ttu-id="ecfe3-391">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-391">no</span></span>           |
| <span data-ttu-id="ecfe3-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="ecfe3-392">msdyn_effort</span></span>                 | <span data-ttu-id="ecfe3-393">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-393">no</span></span>             | <span data-ttu-id="ecfe3-394">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-394">no</span></span>           |
| <span data-ttu-id="ecfe3-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="ecfe3-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="ecfe3-396">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-396">no</span></span>             | <span data-ttu-id="ecfe3-397">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-397">no</span></span>           |
| <span data-ttu-id="ecfe3-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="ecfe3-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="ecfe3-399">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-399">no</span></span>             | <span data-ttu-id="ecfe3-400">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-400">no</span></span>           |
| <span data-ttu-id="ecfe3-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="ecfe3-401">msdyn_finish</span></span>                 | <span data-ttu-id="ecfe3-402">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-402">no</span></span>             | <span data-ttu-id="ecfe3-403">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-403">no</span></span>           |
| <span data-ttu-id="ecfe3-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="ecfe3-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="ecfe3-405">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-405">no</span></span>             | <span data-ttu-id="ecfe3-406">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-406">no</span></span>           |
| <span data-ttu-id="ecfe3-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="ecfe3-408">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-408">no</span></span>             | <span data-ttu-id="ecfe3-409">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-409">no</span></span>           |
| <span data-ttu-id="ecfe3-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="ecfe3-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="ecfe3-411">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-411">no</span></span>             | <span data-ttu-id="ecfe3-412">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-412">no</span></span>           |
| <span data-ttu-id="ecfe3-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="ecfe3-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="ecfe3-414">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-414">no</span></span>             | <span data-ttu-id="ecfe3-415">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-415">no</span></span>           |
| <span data-ttu-id="ecfe3-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="ecfe3-417">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-417">no</span></span>             | <span data-ttu-id="ecfe3-418">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-418">no</span></span>           |
| <span data-ttu-id="ecfe3-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="ecfe3-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="ecfe3-420">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-420">no</span></span>             | <span data-ttu-id="ecfe3-421">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-421">no</span></span>           |
| <span data-ttu-id="ecfe3-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="ecfe3-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="ecfe3-423">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-423">no</span></span>             | <span data-ttu-id="ecfe3-424">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-424">no</span></span>           |
| <span data-ttu-id="ecfe3-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="ecfe3-425">msdyn_projectid</span></span>              | <span data-ttu-id="ecfe3-426">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-426">yes</span></span>            | <span data-ttu-id="ecfe3-427">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-427">no</span></span>           |
| <span data-ttu-id="ecfe3-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-428">msdyn_projectidname</span></span>          | <span data-ttu-id="ecfe3-429">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-429">no</span></span>             | <span data-ttu-id="ecfe3-430">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-430">no</span></span>           |
| <span data-ttu-id="ecfe3-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="ecfe3-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="ecfe3-432">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-432">no</span></span>             | <span data-ttu-id="ecfe3-433">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-433">no</span></span>           |
| <span data-ttu-id="ecfe3-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="ecfe3-435">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-435">no</span></span>             | <span data-ttu-id="ecfe3-436">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-436">no</span></span>           |
| <span data-ttu-id="ecfe3-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="ecfe3-437">msdyn_start</span></span>                  | <span data-ttu-id="ecfe3-438">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-438">no</span></span>             | <span data-ttu-id="ecfe3-439">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-439">no</span></span>           |
| <span data-ttu-id="ecfe3-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="ecfe3-440">msdyn_taskid</span></span>                 | <span data-ttu-id="ecfe3-441">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-441">no</span></span>             | <span data-ttu-id="ecfe3-442">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-442">no</span></span>           |
| <span data-ttu-id="ecfe3-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-443">msdyn_taskidname</span></span>             | <span data-ttu-id="ecfe3-444">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-444">no</span></span>             | <span data-ttu-id="ecfe3-445">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-445">no</span></span>           |
| <span data-ttu-id="ecfe3-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="ecfe3-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="ecfe3-447">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-447">no</span></span>             | <span data-ttu-id="ecfe3-448">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="ecfe3-449">प्रोजेक्ट टीम सदस्य</span><span class="sxs-lookup"><span data-stu-id="ecfe3-449">Project team member</span></span>

| <span data-ttu-id="ecfe3-450">**तार्किक नाम**</span><span class="sxs-lookup"><span data-stu-id="ecfe3-450">**Logical name**</span></span>                                 | <span data-ttu-id="ecfe3-451">**बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="ecfe3-451">**Can create**</span></span> | <span data-ttu-id="ecfe3-452">**संपादित कर सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="ecfe3-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="ecfe3-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="ecfe3-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="ecfe3-454">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-454">no</span></span>             | <span data-ttu-id="ecfe3-455">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-455">no</span></span>           |
| <span data-ttu-id="ecfe3-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="ecfe3-457">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-457">no</span></span>             | <span data-ttu-id="ecfe3-458">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-458">no</span></span>           |
| <span data-ttu-id="ecfe3-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="ecfe3-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="ecfe3-460">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-460">no</span></span>             | <span data-ttu-id="ecfe3-461">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-461">no</span></span>           |
| <span data-ttu-id="ecfe3-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="ecfe3-463">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-463">no</span></span>             | <span data-ttu-id="ecfe3-464">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-464">no</span></span>           |
| <span data-ttu-id="ecfe3-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="ecfe3-465">msdyn_effort</span></span>                                     | <span data-ttu-id="ecfe3-466">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-466">no</span></span>             | <span data-ttu-id="ecfe3-467">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-467">no</span></span>           |
| <span data-ttu-id="ecfe3-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="ecfe3-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="ecfe3-469">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-469">no</span></span>             | <span data-ttu-id="ecfe3-470">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-470">no</span></span>           |
| <span data-ttu-id="ecfe3-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="ecfe3-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="ecfe3-472">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-472">no</span></span>             | <span data-ttu-id="ecfe3-473">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-473">no</span></span>           |
| <span data-ttu-id="ecfe3-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="ecfe3-474">msdyn_finish</span></span>                                     | <span data-ttu-id="ecfe3-475">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-475">no</span></span>             | <span data-ttu-id="ecfe3-476">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-476">no</span></span>           |
| <span data-ttu-id="ecfe3-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="ecfe3-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="ecfe3-478">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-478">no</span></span>             | <span data-ttu-id="ecfe3-479">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-479">no</span></span>           |
| <span data-ttu-id="ecfe3-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="ecfe3-480">msdyn_hours</span></span>                                      | <span data-ttu-id="ecfe3-481">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-481">no</span></span>             | <span data-ttu-id="ecfe3-482">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-482">no</span></span>           |
| <span data-ttu-id="ecfe3-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="ecfe3-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="ecfe3-484">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-484">no</span></span>             | <span data-ttu-id="ecfe3-485">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-485">no</span></span>           |
| <span data-ttu-id="ecfe3-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="ecfe3-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="ecfe3-487">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-487">no</span></span>             | <span data-ttu-id="ecfe3-488">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-488">no</span></span>           |
| <span data-ttu-id="ecfe3-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="ecfe3-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="ecfe3-490">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-490">no</span></span>             | <span data-ttu-id="ecfe3-491">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-491">no</span></span>           |
| <span data-ttu-id="ecfe3-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="ecfe3-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="ecfe3-493">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-493">no</span></span>             | <span data-ttu-id="ecfe3-494">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-494">no</span></span>           |
| <span data-ttu-id="ecfe3-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="ecfe3-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="ecfe3-496">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-496">no</span></span>             | <span data-ttu-id="ecfe3-497">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-497">no</span></span>           |
| <span data-ttu-id="ecfe3-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="ecfe3-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="ecfe3-499">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-499">no</span></span>             | <span data-ttu-id="ecfe3-500">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-500">no</span></span>           |
| <span data-ttu-id="ecfe3-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="ecfe3-501">msdyn_start</span></span>                                      | <span data-ttu-id="ecfe3-502">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-502">no</span></span>             | <span data-ttu-id="ecfe3-503">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="ecfe3-504">Project</span><span class="sxs-lookup"><span data-stu-id="ecfe3-504">Project</span></span>

| <span data-ttu-id="ecfe3-505">**तार्किक नाम**</span><span class="sxs-lookup"><span data-stu-id="ecfe3-505">**Logical name**</span></span>                       | <span data-ttu-id="ecfe3-506">**बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="ecfe3-506">**Can create**</span></span> | <span data-ttu-id="ecfe3-507">**संपादित कर सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="ecfe3-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="ecfe3-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="ecfe3-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="ecfe3-509">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-509">no</span></span>             | <span data-ttu-id="ecfe3-510">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-510">no</span></span>           |
| <span data-ttu-id="ecfe3-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="ecfe3-512">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-512">no</span></span>             | <span data-ttu-id="ecfe3-513">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-513">no</span></span>           |
| <span data-ttu-id="ecfe3-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="ecfe3-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="ecfe3-515">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-515">no</span></span>             | <span data-ttu-id="ecfe3-516">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-516">no</span></span>           |
| <span data-ttu-id="ecfe3-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="ecfe3-518">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-518">no</span></span>             | <span data-ttu-id="ecfe3-519">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-519">no</span></span>           |
| <span data-ttu-id="ecfe3-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="ecfe3-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="ecfe3-521">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-521">no</span></span>             | <span data-ttu-id="ecfe3-522">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-522">no</span></span>           |
| <span data-ttu-id="ecfe3-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="ecfe3-524">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-524">no</span></span>             | <span data-ttu-id="ecfe3-525">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-525">no</span></span>           |
| <span data-ttu-id="ecfe3-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="ecfe3-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="ecfe3-527">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-527">yes</span></span>            | <span data-ttu-id="ecfe3-528">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-528">no</span></span>           |
| <span data-ttu-id="ecfe3-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="ecfe3-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="ecfe3-530">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-530">yes</span></span>            | <span data-ttu-id="ecfe3-531">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-531">no</span></span>           |
| <span data-ttu-id="ecfe3-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="ecfe3-533">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-533">yes</span></span>            | <span data-ttu-id="ecfe3-534">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-534">no</span></span>           |
| <span data-ttu-id="ecfe3-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="ecfe3-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="ecfe3-536">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-536">no</span></span>             | <span data-ttu-id="ecfe3-537">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-537">no</span></span>           |
| <span data-ttu-id="ecfe3-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="ecfe3-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="ecfe3-539">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-539">no</span></span>             | <span data-ttu-id="ecfe3-540">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-540">no</span></span>           |
| <span data-ttu-id="ecfe3-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="ecfe3-542">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-542">no</span></span>             | <span data-ttu-id="ecfe3-543">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-543">no</span></span>           |
| <span data-ttu-id="ecfe3-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="ecfe3-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="ecfe3-545">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-545">no</span></span>             | <span data-ttu-id="ecfe3-546">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-546">no</span></span>           |
| <span data-ttu-id="ecfe3-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="ecfe3-548">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-548">no</span></span>             | <span data-ttu-id="ecfe3-549">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-549">no</span></span>           |
| <span data-ttu-id="ecfe3-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="ecfe3-550">msdyn_duration</span></span>                         | <span data-ttu-id="ecfe3-551">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-551">no</span></span>             | <span data-ttu-id="ecfe3-552">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-552">no</span></span>           |
| <span data-ttu-id="ecfe3-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="ecfe3-553">msdyn_effort</span></span>                           | <span data-ttu-id="ecfe3-554">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-554">no</span></span>             | <span data-ttu-id="ecfe3-555">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-555">no</span></span>           |
| <span data-ttu-id="ecfe3-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="ecfe3-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="ecfe3-557">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-557">no</span></span>             | <span data-ttu-id="ecfe3-558">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-558">no</span></span>           |
| <span data-ttu-id="ecfe3-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="ecfe3-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="ecfe3-560">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-560">no</span></span>             | <span data-ttu-id="ecfe3-561">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-561">no</span></span>           |
| <span data-ttu-id="ecfe3-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="ecfe3-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="ecfe3-563">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-563">no</span></span>             | <span data-ttu-id="ecfe3-564">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-564">no</span></span>           |
| <span data-ttu-id="ecfe3-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="ecfe3-565">msdyn_finish</span></span>                           | <span data-ttu-id="ecfe3-566">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-566">yes</span></span>            | <span data-ttu-id="ecfe3-567">हाँ</span><span class="sxs-lookup"><span data-stu-id="ecfe3-567">yes</span></span>          |
| <span data-ttu-id="ecfe3-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="ecfe3-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="ecfe3-569">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-569">no</span></span>             | <span data-ttu-id="ecfe3-570">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-570">no</span></span>           |
| <span data-ttu-id="ecfe3-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="ecfe3-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="ecfe3-572">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-572">no</span></span>             | <span data-ttu-id="ecfe3-573">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-573">no</span></span>           |
| <span data-ttu-id="ecfe3-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="ecfe3-575">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-575">no</span></span>             | <span data-ttu-id="ecfe3-576">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-576">no</span></span>           |
| <span data-ttu-id="ecfe3-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="ecfe3-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="ecfe3-578">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-578">no</span></span>             | <span data-ttu-id="ecfe3-579">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-579">no</span></span>           |
| <span data-ttu-id="ecfe3-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="ecfe3-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="ecfe3-581">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-581">no</span></span>             | <span data-ttu-id="ecfe3-582">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-582">no</span></span>           |
| <span data-ttu-id="ecfe3-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="ecfe3-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="ecfe3-584">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-584">no</span></span>             | <span data-ttu-id="ecfe3-585">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-585">no</span></span>           |
| <span data-ttu-id="ecfe3-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="ecfe3-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="ecfe3-587">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-587">no</span></span>             | <span data-ttu-id="ecfe3-588">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-588">no</span></span>           |
| <span data-ttu-id="ecfe3-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="ecfe3-590">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-590">no</span></span>             | <span data-ttu-id="ecfe3-591">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-591">no</span></span>           |
| <span data-ttu-id="ecfe3-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="ecfe3-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="ecfe3-593">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-593">no</span></span>             | <span data-ttu-id="ecfe3-594">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-594">no</span></span>           |
| <span data-ttu-id="ecfe3-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="ecfe3-596">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-596">no</span></span>             | <span data-ttu-id="ecfe3-597">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-597">no</span></span>           |
| <span data-ttu-id="ecfe3-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="ecfe3-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="ecfe3-599">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-599">no</span></span>             | <span data-ttu-id="ecfe3-600">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-600">no</span></span>           |
| <span data-ttu-id="ecfe3-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="ecfe3-602">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-602">no</span></span>             | <span data-ttu-id="ecfe3-603">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-603">no</span></span>           |
| <span data-ttu-id="ecfe3-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="ecfe3-604">msdyn_progress</span></span>                         | <span data-ttu-id="ecfe3-605">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-605">no</span></span>             | <span data-ttu-id="ecfe3-606">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-606">no</span></span>           |
| <span data-ttu-id="ecfe3-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="ecfe3-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="ecfe3-608">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-608">no</span></span>             | <span data-ttu-id="ecfe3-609">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-609">no</span></span>           |
| <span data-ttu-id="ecfe3-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="ecfe3-611">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-611">no</span></span>             | <span data-ttu-id="ecfe3-612">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-612">no</span></span>           |
| <span data-ttu-id="ecfe3-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="ecfe3-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="ecfe3-614">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-614">no</span></span>             | <span data-ttu-id="ecfe3-615">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-615">no</span></span>           |
| <span data-ttu-id="ecfe3-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="ecfe3-617">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-617">no</span></span>             | <span data-ttu-id="ecfe3-618">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-618">no</span></span>           |
| <span data-ttu-id="ecfe3-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="ecfe3-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="ecfe3-620">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-620">no</span></span>             | <span data-ttu-id="ecfe3-621">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-621">no</span></span>           |
| <span data-ttu-id="ecfe3-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="ecfe3-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="ecfe3-623">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-623">no</span></span>             | <span data-ttu-id="ecfe3-624">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-624">no</span></span>           |
| <span data-ttu-id="ecfe3-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="ecfe3-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="ecfe3-626">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-626">no</span></span>             | <span data-ttu-id="ecfe3-627">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-627">no</span></span>           |
| <span data-ttu-id="ecfe3-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="ecfe3-629">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-629">no</span></span>             | <span data-ttu-id="ecfe3-630">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-630">no</span></span>           |
| <span data-ttu-id="ecfe3-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="ecfe3-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="ecfe3-632">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-632">no</span></span>             | <span data-ttu-id="ecfe3-633">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-633">no</span></span>           |
| <span data-ttu-id="ecfe3-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="ecfe3-635">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-635">no</span></span>             | <span data-ttu-id="ecfe3-636">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-636">no</span></span>           |
| <span data-ttu-id="ecfe3-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="ecfe3-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="ecfe3-638">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-638">no</span></span>             | <span data-ttu-id="ecfe3-639">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-639">no</span></span>           |
| <span data-ttu-id="ecfe3-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="ecfe3-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="ecfe3-641">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-641">no</span></span>             | <span data-ttu-id="ecfe3-642">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-642">no</span></span>           |
| <span data-ttu-id="ecfe3-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="ecfe3-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="ecfe3-644">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-644">no</span></span>             | <span data-ttu-id="ecfe3-645">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-645">no</span></span>           |
| <span data-ttu-id="ecfe3-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="ecfe3-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="ecfe3-647">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-647">no</span></span>             | <span data-ttu-id="ecfe3-648">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-648">no</span></span>           |
| <span data-ttu-id="ecfe3-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="ecfe3-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="ecfe3-650">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-650">no</span></span>             | <span data-ttu-id="ecfe3-651">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-651">no</span></span>           |
| <span data-ttu-id="ecfe3-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="ecfe3-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="ecfe3-653">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-653">no</span></span>             | <span data-ttu-id="ecfe3-654">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-654">no</span></span>           |
| <span data-ttu-id="ecfe3-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="ecfe3-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="ecfe3-656">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-656">no</span></span>             | <span data-ttu-id="ecfe3-657">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-657">no</span></span>           |
| <span data-ttu-id="ecfe3-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="ecfe3-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="ecfe3-659">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-659">no</span></span>             | <span data-ttu-id="ecfe3-660">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-660">no</span></span>           |
| <span data-ttu-id="ecfe3-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="ecfe3-662">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-662">no</span></span>             | <span data-ttu-id="ecfe3-663">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-663">no</span></span>           |
| <span data-ttu-id="ecfe3-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="ecfe3-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="ecfe3-665">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-665">no</span></span>             | <span data-ttu-id="ecfe3-666">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-666">no</span></span>           |
| <span data-ttu-id="ecfe3-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="ecfe3-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="ecfe3-668">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-668">no</span></span>             | <span data-ttu-id="ecfe3-669">नहीं</span><span class="sxs-lookup"><span data-stu-id="ecfe3-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="ecfe3-670">सीमाएं और ज्ञात मुद्दे</span><span class="sxs-lookup"><span data-stu-id="ecfe3-670">Limitations and known issues</span></span>
<span data-ttu-id="ecfe3-671">निम्नलिखित सीमाओं और ज्ञात मुद्दों की एक लिस्ट है:</span><span class="sxs-lookup"><span data-stu-id="ecfe3-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="ecfe3-672">शेड्यूल एपीआई का उपयोग केवल **Microsoft प्रोज़ेक्ट लाइसेंस वाले** उपयोगकर्ताओं द्वारा किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-672">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="ecfe3-673">उनका इनके द्वारा उपयोग नहीं किया जा सकता है:</span><span class="sxs-lookup"><span data-stu-id="ecfe3-673">They can't be used by:</span></span>
    - <span data-ttu-id="ecfe3-674">अनुप्रयोग उपयोगकर्ता</span><span class="sxs-lookup"><span data-stu-id="ecfe3-674">Application users</span></span>
    - <span data-ttu-id="ecfe3-675">सिस्टम उपयोगकर्ता</span><span class="sxs-lookup"><span data-stu-id="ecfe3-675">System users</span></span>
    - <span data-ttu-id="ecfe3-676">एकीकरण उपयोगकर्ता</span><span class="sxs-lookup"><span data-stu-id="ecfe3-676">Integration users</span></span>
    - <span data-ttu-id="ecfe3-677">अन्य उपयोगकर्ता जिनके पास आवश्यक लाइसेंस नहीं है</span><span class="sxs-lookup"><span data-stu-id="ecfe3-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="ecfe3-678">प्रत्येक **OperationSet** में अधिकतम 100 संचालन हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="ecfe3-679">प्रत्येक उपयोगकर्ता के पास अधिकतम 10 खुला **OperationSets** हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="ecfe3-680">Project Operations वर्तमान में एक प्रोज़ेक्ट पर अधिकतम 500 कुल कार्यों का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="ecfe3-681">**OperationSet** विफलता की स्थिति और विफलता लॉग वर्तमान में उपलब्ध नहीं हैं.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- <span data-ttu-id="ecfe3-682">शेड्यूल एपीआई सार्वजनिक पूर्वावलोकन में हैं.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-682">Schedule APIs are in Public preview.</span></span> <span data-ttu-id="ecfe3-683">उत्पादन परिवेश में इन एपीआई का उपयोग करना Microsoft द्वारा समर्थित नहीं है.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-683">Using these APIs in a Production environment isn't supported by Microsoft.</span></span>
- [<span data-ttu-id="ecfe3-684">प्रोजेक्ट और कार्यों पर लिमिट और बाउंड्री</span><span class="sxs-lookup"><span data-stu-id="ecfe3-684">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="ecfe3-685">त्रुटि हैंडलिंग</span><span class="sxs-lookup"><span data-stu-id="ecfe3-685">Error handling</span></span>

   - <span data-ttu-id="ecfe3-686">ऑपरेशन सेट से उत्पन्न त्रुटियों की समीक्षा करने के लिए, **सेटिंग** \> **शेड्यूल इंटीग्रेशन** \> **ऑपरेशन सेट्स** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-686">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="ecfe3-687">प्रोजेक्ट शेड्यूलिंग सेवा से उत्पन्न त्रुटियों की समीक्षा करने के लिए, **सेटिंग** \> **शेड्यूल एकीकरण** \> **PSS त्रुटि लॉग पर** जाएं.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-687">To review errors generated from the Project Scheduling Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="ecfe3-688">नमूना परिदृश्य</span><span class="sxs-lookup"><span data-stu-id="ecfe3-688">Sample scenario</span></span>

<span data-ttu-id="ecfe3-689">इस परिदृश्य में, आप एक प्रोज़ेक्ट, एक टीम के सदस्य, चार कार्य और दो संसाधन कार्य बनाएंगे.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-689">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="ecfe3-690">इसके बाद, आप एक कार्य को अपडेट करेंगे, प्रोज़ेक्ट को अपडेट करेंगे, एक कार्य को हटा देंगे, एक संसाधन असाइनमेंट को हटा देंगे,और एक कार्य निर्भरता बनाएंगे.</span><span class="sxs-lookup"><span data-stu-id="ecfe3-690">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

```csharp
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
var task4 = GetTask("4ZZ", projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment("R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

var assignment1Response = CallPssCreateAction(assignment1, operationSetId);
var assignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

var assignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a><span data-ttu-id="ecfe3-691">अतिरिक्त नमूने</span><span class="sxs-lookup"><span data-stu-id="ecfe3-691">Additional samples</span></span>

```csharp
#region Call actions --- Sample code ----

/// <summary>
/// Calls the action to create an operationSet
/// </summary>
/// <param name="projectId">project id for the operations to be included in this operationSet</param>
/// <param name="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
private string CallCreateOperationSetAction(Guid projectId, string description)
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
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>

private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet Id</param>
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
/// </summary>
/// <param name="recordId">Id of the record to be deleted</param>
/// <param name="entityLogicalName">Entity logical name of the record</param>
/// <param name="operationSetId">OperationSet Id</param>
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
/// </summary>
/// <param name="operationSetId">operationSet id</param>
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
/// <param name="operationSetId">operationSet id</param>
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
/// <param name="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1");
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);
    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <param name="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
private string CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject<OperationSetResponse>((string)orgResponse.Results["OperationSetResponse"]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet("msdyn_project", "msdyn_name");
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
    task["msdyn_effort"] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
    task["new_custom1"] = "Just my test";
    task["new_age"] = 98;
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
public class OperationSetResponse
{
[DataMember(Name = "operationSetId")]
public Guid OperationSetId { get; set; }

[DataMember(Name = "operationSetDetailId")]
public Guid OperationSetDetailId { get; set; }

[DataMember(Name = "operationType")]
public string OperationType { get; set; }

[DataMember(Name = "recordId")]
public string RecordId { get; set; }

[DataMember(Name = "correlationId")]
public string CorrelationId { get; set; }
}

#endregion
```
