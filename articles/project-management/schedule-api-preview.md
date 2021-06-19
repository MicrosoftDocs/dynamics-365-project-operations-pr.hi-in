---
title: निकाय शेड्यूलिंग के साथ संचालन करने के लिए शेड्यूल APIs का उपयोग करें
description: यह विषय अनुसूची APIs का उपयोग करने के लिए जानकारी और नमूने प्रदान करता है.
author: sigitac
ms.date: 04/27/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4a032dc7bcbdf23fce3c3b2ca63c51d473bd8e26
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116799"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="b4928-103">निकाय शेड्यूलिंग के साथ संचालन करने के लिए शेड्यूल APIs का उपयोग करें</span><span class="sxs-lookup"><span data-stu-id="b4928-103">Use Schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="b4928-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="b4928-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="b4928-105">इस विषय में नोट की गई कुछ या सभी कार्यक्षमता पूर्वावलोकन रिलीज के हिस्से के रूप में उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="b4928-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="b4928-106">सामग्री और कार्यक्षमता परिवर्तन के अधीन हैं.</span><span class="sxs-lookup"><span data-stu-id="b4928-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="b4928-107">शेड्यूलिंग निकाय</span><span class="sxs-lookup"><span data-stu-id="b4928-107">Scheduling entities</span></span>

<span data-ttu-id="b4928-108">शेड्यूल APIs **निकाय शेड्यूलिंग** के साथ निर्माण, अपडेट और हटाने के संचालन को करने की क्षमता प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-108">Schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="b4928-109">इन निकायों को वेब के लिए परियोजना में शेड्यूलिंग इंजन के माध्यम से प्रबंधित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="b4928-110">पहले Dynamics 365 Project Operations रिलीज़ में **निकाय शेड्यूलिंग** के साथ संचालन बनाएं, अपडेट करें और मिटाएं.</span><span class="sxs-lookup"><span data-stu-id="b4928-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="b4928-111">निम्नलिखित तालिका **निकाय शेड्यूलिंग** की पूरी लिस्ट प्रदान करती है.</span><span class="sxs-lookup"><span data-stu-id="b4928-111">The following table provides a full list of the **Scheduling entities**.</span></span>

| <span data-ttu-id="b4928-112">निकाय का नाम</span><span class="sxs-lookup"><span data-stu-id="b4928-112">Entity name</span></span>  | <span data-ttu-id="b4928-113">निकाय तार्किक नाम</span><span class="sxs-lookup"><span data-stu-id="b4928-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="b4928-114">Project</span><span class="sxs-lookup"><span data-stu-id="b4928-114">Project</span></span> | <span data-ttu-id="b4928-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="b4928-115">msdyn_project</span></span> |
| <span data-ttu-id="b4928-116">परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="b4928-116">Project Task</span></span>  | <span data-ttu-id="b4928-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="b4928-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="b4928-118">परियोजना कार्य निर्भरता</span><span class="sxs-lookup"><span data-stu-id="b4928-118">Project Task Dependency</span></span>  | <span data-ttu-id="b4928-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="b4928-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="b4928-120">संसाधन असाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="b4928-120">Resource Assignment</span></span> | <span data-ttu-id="b4928-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="b4928-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="b4928-122">परियोजना बकेट</span><span class="sxs-lookup"><span data-stu-id="b4928-122">Project Bucket</span></span>  | <span data-ttu-id="b4928-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="b4928-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="b4928-124">परियोजना टीम सदस्य</span><span class="sxs-lookup"><span data-stu-id="b4928-124">Project Team Member</span></span> | <span data-ttu-id="b4928-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="b4928-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="b4928-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="b4928-126">OperationSet</span></span>

<span data-ttu-id="b4928-127">OperationSet एक यूनिट-ऑफ-वर्क पैटर्न है जिसका उपयोग तब किया जा सकता है जब शेड्यूल प्रभावित करने वाले कई अनुरोधों को लेनदेन के भीतर संसाधित किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="b4928-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="schedule-apis"></a><span data-ttu-id="b4928-128">APIs शेड्यूल करें</span><span class="sxs-lookup"><span data-stu-id="b4928-128">Schedule APIs</span></span>

<span data-ttu-id="b4928-129">यह वर्तमान शेड्यूल APIs की लिस्ट है.</span><span class="sxs-lookup"><span data-stu-id="b4928-129">The following is a list of current Schedule APIs.</span></span>

- <span data-ttu-id="b4928-130">**msdyn_CreateProjectV1**: इस API का उपयोग एक प्रोज़ेक्ट बनाने के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="b4928-131">प्रोज़ेक्ट और डिफॉल्ट प्रोज़ेक्ट बकेट तुरंत बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="b4928-132">**msdyn_CreateTeamMemberV1**: इस API का उपयोग प्रोज़ेक्ट टीम के सदस्य बनाने के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="b4928-133">टीम के सदस्य का रिकार्ड तुरंत बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="b4928-134">**msdyn_CreateOperationSetV1**: इस एपीआई का उपयोग कई अनुरोधों को शेड्यूल करने के लिए किया जा सकता है जिन्हें लेनदेन के भीतर किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="b4928-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="b4928-135">**msdyn_PSSCreateV1**: इस एपीआई का उपयोग एक निकाय बनाने के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="b4928-136">निकाय शेड्यूलिंग संस्थाओं में से कोई भी हो सकता है जो निर्माण ऑपरेशन का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-136">The entity can be any of the Scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="b4928-137">**msdyn_PSSCreateV1**: इस API का उपयोग एक निकाय अपडेट के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="b4928-138">निकाय शेड्यूलिंग संस्थाओं में से कोई भी हो सकता है जो अपडेट ऑपरेशन का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-138">The entity can be any of the Scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="b4928-139">**msdyn_PSSDeleteV1**: इस API को हटाने के लिए एक निकाय इस्तेमाल किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="b4928-140">निकाय शेड्यूलिंग संस्थाओं में से कोई भी हो सकता है जो डिलीट ऑपरेशन का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-140">The entity can be any of the Scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="b4928-141">**msdyn_ExecuteOperationSetV1**: इस एपीआई का उपयोग दिए गए ऑपरेशन सेट के भीतर सभी संचालनों को निष्पादित करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-schedule-apis-with-operationset"></a><span data-ttu-id="b4928-142">OperationSet के साथ शेड्यूल APIs का उपयोग करना</span><span class="sxs-lookup"><span data-stu-id="b4928-142">Using Schedule APIs with OperationSet</span></span>

<span data-ttu-id="b4928-143">क्योंकि दोनों के साथ रिकॉर्ड **CreateProjectV1** और **CreateTeamMemberV1** तुरंत बनाए जाते हैं, इन APIs का उपयोग सीधे **OperationSet** में नहीं किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="b4928-144">हालांकि, आप आवश्यक रिकॉर्ड बनाने, **OperationSet** बनाने के लिए API का उपयोग कर सकते हैं, और फिर **OperationSet** में इन पूर्व-निर्मित रिकॉर्ड का उपयोग कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="b4928-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="b4928-145">समर्थित संचालन</span><span class="sxs-lookup"><span data-stu-id="b4928-145">Supported operations</span></span>

| <span data-ttu-id="b4928-146">निकाय शेड्यूलिंग</span><span class="sxs-lookup"><span data-stu-id="b4928-146">Scheduling entity</span></span> | <span data-ttu-id="b4928-147">निर्माण करें</span><span class="sxs-lookup"><span data-stu-id="b4928-147">Create</span></span> | <span data-ttu-id="b4928-148">अद्यतित करें</span><span class="sxs-lookup"><span data-stu-id="b4928-148">Update</span></span> | <span data-ttu-id="b4928-149">हटाएं</span><span class="sxs-lookup"><span data-stu-id="b4928-149">Delete</span></span> | <span data-ttu-id="b4928-150">महत्वपूर्ण विचार</span><span class="sxs-lookup"><span data-stu-id="b4928-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="b4928-151">परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="b4928-151">Project task</span></span> | <span data-ttu-id="b4928-152">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-152">Yes</span></span> | <span data-ttu-id="b4928-153">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-153">Yes</span></span> | <span data-ttu-id="b4928-154">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-154">Yes</span></span> | <span data-ttu-id="b4928-155">कुछ नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-155">None</span></span> |
| <span data-ttu-id="b4928-156">प्रोज़ेक्ट कार्य निर्भरता</span><span class="sxs-lookup"><span data-stu-id="b4928-156">Project task dependency</span></span> | <span data-ttu-id="b4928-157">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-157">Yes</span></span> | <span data-ttu-id="b4928-158">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-158">Yes</span></span> | | <span data-ttu-id="b4928-159">प्रोज़ेक्ट कार्य निर्भरता रिकॉर्ड अपडेट नहीं किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="b4928-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="b4928-160">इसके बजाय, एक पुराना रिकॉर्ड हटाया जा सकता है और एक नया रिकॉर्ड बनाया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="b4928-161">रिसोर्स असाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="b4928-161">Resource assignment</span></span> | <span data-ttu-id="b4928-162">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-162">Yes</span></span> | <span data-ttu-id="b4928-163">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-163">Yes</span></span> | | <span data-ttu-id="b4928-164">निम्नलिखित फ़ील्ड के साथ संचालन का समर्थन नहीं किया जाता है: **BookableResourceID**, **प्रयास**,**EffortCompleted**, **EffortRemaining**, और **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="b4928-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="b4928-165">संसाधन असाइनमेंट रिकॉर्ड अपडेट नहीं किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="b4928-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="b4928-166">इसके बदले पुराना रिकॉर्ड डिलीट किया जा सकता है और नया रिकॉर्ड बनाया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="b4928-167">प्रोज़ेक्ट बकेट</span><span class="sxs-lookup"><span data-stu-id="b4928-167">Project bucket</span></span> | <span data-ttu-id="b4928-168">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-168">N/A</span></span> | <span data-ttu-id="b4928-169">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-169">N/A</span></span> | <span data-ttu-id="b4928-170">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-170">N/A</span></span> | <span data-ttu-id="b4928-171">डिफ़ॉल्ट बकेट **CreateProjectV1** API का उपयोग करके बनाई गई है.</span><span class="sxs-lookup"><span data-stu-id="b4928-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="b4928-172">प्रोजेक्ट टीम सदस्य</span><span class="sxs-lookup"><span data-stu-id="b4928-172">Project team member</span></span> | <span data-ttu-id="b4928-173">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-173">Yes</span></span> | <span data-ttu-id="b4928-174">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-174">Yes</span></span> | <span data-ttu-id="b4928-175">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-175">Yes</span></span> | <span data-ttu-id="b4928-176">बनाने के ऑपरेशन के लिए, **CreateTeamMemberV1** API का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="b4928-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="b4928-177">Project</span><span class="sxs-lookup"><span data-stu-id="b4928-177">Project</span></span> | <span data-ttu-id="b4928-178">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-178">Yes</span></span> | <span data-ttu-id="b4928-179">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-179">Yes</span></span> | <span data-ttu-id="b4928-180">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-180">N/A</span></span> | <span data-ttu-id="b4928-181">निम्नलिखित फ़ील्ड के साथ संचालन का समर्थन नहीं किया जाता है: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **प्रयास**, **EffortCompleted**, **EffortRemaining**, **प्रगति**, **समाप्त करें**, **TaskEarliestStart**, और **अवधि**.</span><span class="sxs-lookup"><span data-stu-id="b4928-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="b4928-182">इन APIs को निकाय ऑब्जेक्ट्स के साथ बुलाया जा सकता है जिसमें कस्टम फ़ील्ड शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="b4928-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="b4928-183">ID संपत्ति वैकल्पिक है.</span><span class="sxs-lookup"><span data-stu-id="b4928-183">The ID property is optional.</span></span> <span data-ttu-id="b4928-184">यदि यह प्रदान किया जाता है, तो सिस्टम इसका उपयोग करने का प्रयास करता है और यदि इसका उपयोग नहीं किया जा सकता है तो अपवाद प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="b4928-185">यदि यह प्रदान नहीं किया जाता है, तो सिस्टम इसे उत्पन्न करेगा.</span><span class="sxs-lookup"><span data-stu-id="b4928-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="b4928-186">प्रतिबंधित फील्ड</span><span class="sxs-lookup"><span data-stu-id="b4928-186">Restricted fields</span></span>

<span data-ttu-id="b4928-187">निम्न तालिका उन क्षेत्रों को परिभाषित करती है जो **बनाएं** और **संपादित करें** से प्रतिबंधित हैं.</span><span class="sxs-lookup"><span data-stu-id="b4928-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="b4928-188">परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="b4928-188">Project task</span></span>

| <span data-ttu-id="b4928-189">**तार्किक नाम**</span><span class="sxs-lookup"><span data-stu-id="b4928-189">**Logical name**</span></span>                       | <span data-ttu-id="b4928-190">**बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="b4928-190">**Can create**</span></span> | <span data-ttu-id="b4928-191">**संपादित कर सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="b4928-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="b4928-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="b4928-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="b4928-193">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-193">no</span></span>             | <span data-ttu-id="b4928-194">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-194">no</span></span>               |
| <span data-ttu-id="b4928-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="b4928-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="b4928-196">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-196">no</span></span>             | <span data-ttu-id="b4928-197">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-197">no</span></span>               |
| <span data-ttu-id="b4928-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="b4928-198">msdyn_actualend</span></span>                        | <span data-ttu-id="b4928-199">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-199">no</span></span>             | <span data-ttu-id="b4928-200">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-200">no</span></span>               |
| <span data-ttu-id="b4928-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="b4928-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="b4928-202">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-202">no</span></span>             | <span data-ttu-id="b4928-203">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-203">no</span></span>               |
| <span data-ttu-id="b4928-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="b4928-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="b4928-205">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-205">no</span></span>             | <span data-ttu-id="b4928-206">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-206">no</span></span>               |
| <span data-ttu-id="b4928-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="b4928-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="b4928-208">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-208">no</span></span>             | <span data-ttu-id="b4928-209">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-209">no</span></span>               |
| <span data-ttu-id="b4928-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="b4928-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="b4928-211">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-211">no</span></span>             | <span data-ttu-id="b4928-212">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-212">no</span></span>               |
| <span data-ttu-id="b4928-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="b4928-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="b4928-214">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-214">no</span></span>             | <span data-ttu-id="b4928-215">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-215">no</span></span>               |
| <span data-ttu-id="b4928-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="b4928-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="b4928-217">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-217">no</span></span>             | <span data-ttu-id="b4928-218">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-218">no</span></span>               |
| <span data-ttu-id="b4928-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="b4928-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="b4928-220">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-220">no</span></span>             | <span data-ttu-id="b4928-221">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-221">no</span></span>               |
| <span data-ttu-id="b4928-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="b4928-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="b4928-223">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-223">no</span></span>             | <span data-ttu-id="b4928-224">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-224">no</span></span>               |
| <span data-ttu-id="b4928-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="b4928-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="b4928-226">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-226">no</span></span>             | <span data-ttu-id="b4928-227">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-227">no</span></span>               |
| <span data-ttu-id="b4928-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="b4928-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="b4928-229">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-229">no</span></span>             | <span data-ttu-id="b4928-230">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-230">no</span></span>               |
| <span data-ttu-id="b4928-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="b4928-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="b4928-232">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-232">no</span></span>             | <span data-ttu-id="b4928-233">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-233">no</span></span>               |
| <span data-ttu-id="b4928-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="b4928-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="b4928-235">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-235">no</span></span>             | <span data-ttu-id="b4928-236">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-236">no</span></span>               |
| <span data-ttu-id="b4928-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="b4928-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="b4928-238">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-238">no</span></span>             | <span data-ttu-id="b4928-239">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-239">no</span></span>               |
| <span data-ttu-id="b4928-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="b4928-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="b4928-241">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-241">no</span></span>             | <span data-ttu-id="b4928-242">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-242">no</span></span>               |
| <span data-ttu-id="b4928-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="b4928-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="b4928-244">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-244">no</span></span>             | <span data-ttu-id="b4928-245">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-245">no</span></span>               |
| <span data-ttu-id="b4928-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="b4928-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="b4928-247">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-247">no</span></span>             | <span data-ttu-id="b4928-248">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-248">no</span></span>               |
| <span data-ttu-id="b4928-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="b4928-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="b4928-250">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-250">no</span></span>             | <span data-ttu-id="b4928-251">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-251">no</span></span>               |
| <span data-ttu-id="b4928-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="b4928-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="b4928-253">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-253">no</span></span>             | <span data-ttu-id="b4928-254">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-254">no</span></span>               |
| <span data-ttu-id="b4928-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="b4928-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="b4928-256">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-256">no</span></span>             | <span data-ttu-id="b4928-257">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-257">no</span></span>               |
| <span data-ttu-id="b4928-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="b4928-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="b4928-259">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-259">no</span></span>             | <span data-ttu-id="b4928-260">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-260">no</span></span>               |
| <span data-ttu-id="b4928-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="b4928-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="b4928-262">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-262">no</span></span>             | <span data-ttu-id="b4928-263">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-263">no</span></span>               |
| <span data-ttu-id="b4928-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="b4928-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="b4928-265">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-265">no</span></span>             | <span data-ttu-id="b4928-266">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-266">no</span></span>               |
| <span data-ttu-id="b4928-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="b4928-267">msdyn_progress</span></span>                         | <span data-ttu-id="b4928-268">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-268">no</span></span>             | <span data-ttu-id="b4928-269">नही ( P4W के लिए हां)</span><span class="sxs-lookup"><span data-stu-id="b4928-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="b4928-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="b4928-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="b4928-271">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-271">no</span></span>             | <span data-ttu-id="b4928-272">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-272">no</span></span>               |
| <span data-ttu-id="b4928-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="b4928-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="b4928-274">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-274">no</span></span>             | <span data-ttu-id="b4928-275">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-275">no</span></span>               |
| <span data-ttu-id="b4928-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="b4928-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="b4928-277">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-277">no</span></span>             | <span data-ttu-id="b4928-278">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-278">no</span></span>               |
| <span data-ttu-id="b4928-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="b4928-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="b4928-280">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-280">no</span></span>             | <span data-ttu-id="b4928-281">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-281">no</span></span>               |
| <span data-ttu-id="b4928-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="b4928-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="b4928-283">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-283">no</span></span>             | <span data-ttu-id="b4928-284">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-284">no</span></span>               |
| <span data-ttu-id="b4928-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="b4928-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="b4928-286">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-286">no</span></span>             | <span data-ttu-id="b4928-287">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-287">no</span></span>               |
| <span data-ttu-id="b4928-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="b4928-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="b4928-289">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-289">no</span></span>             | <span data-ttu-id="b4928-290">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-290">no</span></span>               |
| <span data-ttu-id="b4928-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="b4928-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="b4928-292">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-292">no</span></span>             | <span data-ttu-id="b4928-293">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-293">no</span></span>               |
| <span data-ttu-id="b4928-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="b4928-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="b4928-295">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-295">no</span></span>             | <span data-ttu-id="b4928-296">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-296">no</span></span>               |
| <span data-ttu-id="b4928-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="b4928-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="b4928-298">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-298">no</span></span>             | <span data-ttu-id="b4928-299">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-299">no</span></span>               |
| <span data-ttu-id="b4928-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="b4928-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="b4928-301">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-301">no</span></span>             | <span data-ttu-id="b4928-302">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-302">no</span></span>               |
| <span data-ttu-id="b4928-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="b4928-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="b4928-304">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-304">no</span></span>             | <span data-ttu-id="b4928-305">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-305">no</span></span>               |
| <span data-ttu-id="b4928-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="b4928-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="b4928-307">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-307">no</span></span>             | <span data-ttu-id="b4928-308">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-308">no</span></span>               |
| <span data-ttu-id="b4928-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="b4928-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="b4928-310">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-310">no</span></span>             | <span data-ttu-id="b4928-311">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-311">no</span></span>               |
| <span data-ttu-id="b4928-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="b4928-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="b4928-313">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-313">no</span></span>             | <span data-ttu-id="b4928-314">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-314">no</span></span>               |
| <span data-ttu-id="b4928-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="b4928-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="b4928-316">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-316">no</span></span>             | <span data-ttu-id="b4928-317">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-317">no</span></span>               |
| <span data-ttu-id="b4928-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="b4928-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="b4928-319">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-319">no</span></span>             | <span data-ttu-id="b4928-320">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-320">no</span></span>               |
| <span data-ttu-id="b4928-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="b4928-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="b4928-322">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-322">no</span></span>             | <span data-ttu-id="b4928-323">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-323">no</span></span>               |
| <span data-ttu-id="b4928-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="b4928-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="b4928-325">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-325">no</span></span>             | <span data-ttu-id="b4928-326">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-326">no</span></span>               |
| <span data-ttu-id="b4928-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="b4928-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="b4928-328">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-328">no</span></span>             | <span data-ttu-id="b4928-329">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-329">no</span></span>               |
| <span data-ttu-id="b4928-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="b4928-330">msdyn_summary</span></span>                          | <span data-ttu-id="b4928-331">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-331">no</span></span>             | <span data-ttu-id="b4928-332">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-332">no</span></span>               |
| <span data-ttu-id="b4928-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="b4928-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="b4928-334">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-334">no</span></span>             | <span data-ttu-id="b4928-335">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-335">no</span></span>               |
| <span data-ttu-id="b4928-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="b4928-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="b4928-337">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-337">no</span></span>             | <span data-ttu-id="b4928-338">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="b4928-339">प्रोज़ेक्ट कार्य निर्भरता</span><span class="sxs-lookup"><span data-stu-id="b4928-339">Project task dependency</span></span>

| <span data-ttu-id="b4928-340">**तार्किक नाम**</span><span class="sxs-lookup"><span data-stu-id="b4928-340">**Logical name**</span></span>              | <span data-ttu-id="b4928-341">**बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="b4928-341">**Can create**</span></span> | <span data-ttu-id="b4928-342">**संपादित कर सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="b4928-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="b4928-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="b4928-343">msdyn_linktype</span></span>                | <span data-ttu-id="b4928-344">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-344">no</span></span>             | <span data-ttu-id="b4928-345">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-345">no</span></span>           |
| <span data-ttu-id="b4928-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="b4928-346">msdyn_linktypename</span></span>            | <span data-ttu-id="b4928-347">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-347">no</span></span>             | <span data-ttu-id="b4928-348">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-348">no</span></span>           |
| <span data-ttu-id="b4928-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="b4928-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="b4928-350">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-350">yes</span></span>            | <span data-ttu-id="b4928-351">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-351">no</span></span>           |
| <span data-ttu-id="b4928-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="b4928-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="b4928-353">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-353">yes</span></span>            | <span data-ttu-id="b4928-354">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-354">no</span></span>           |
| <span data-ttu-id="b4928-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="b4928-355">msdyn_project</span></span>                 | <span data-ttu-id="b4928-356">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-356">yes</span></span>            | <span data-ttu-id="b4928-357">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-357">no</span></span>           |
| <span data-ttu-id="b4928-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="b4928-358">msdyn_projectname</span></span>             | <span data-ttu-id="b4928-359">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-359">yes</span></span>            | <span data-ttu-id="b4928-360">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-360">no</span></span>           |
| <span data-ttu-id="b4928-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="b4928-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="b4928-362">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-362">yes</span></span>            | <span data-ttu-id="b4928-363">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-363">no</span></span>           |
| <span data-ttu-id="b4928-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="b4928-364">msdyn_successortask</span></span>           | <span data-ttu-id="b4928-365">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-365">yes</span></span>            | <span data-ttu-id="b4928-366">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-366">no</span></span>           |
| <span data-ttu-id="b4928-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="b4928-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="b4928-368">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-368">yes</span></span>            | <span data-ttu-id="b4928-369">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="b4928-370">रिसोर्स असाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="b4928-370">Resource assignment</span></span>

| <span data-ttu-id="b4928-371">**तार्किक नाम**</span><span class="sxs-lookup"><span data-stu-id="b4928-371">**Logical name**</span></span>             | <span data-ttu-id="b4928-372">**बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="b4928-372">**Can create**</span></span> | <span data-ttu-id="b4928-373">**संपादित कर सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="b4928-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="b4928-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="b4928-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="b4928-375">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-375">yes</span></span>            | <span data-ttu-id="b4928-376">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-376">no</span></span>           |
| <span data-ttu-id="b4928-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="b4928-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="b4928-378">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-378">yes</span></span>            | <span data-ttu-id="b4928-379">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-379">no</span></span>           |
| <span data-ttu-id="b4928-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="b4928-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="b4928-381">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-381">no</span></span>             | <span data-ttu-id="b4928-382">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-382">no</span></span>           |
| <span data-ttu-id="b4928-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="b4928-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="b4928-384">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-384">no</span></span>             | <span data-ttu-id="b4928-385">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-385">no</span></span>           |
| <span data-ttu-id="b4928-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="b4928-386">msdyn_committype</span></span>             | <span data-ttu-id="b4928-387">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-387">no</span></span>             | <span data-ttu-id="b4928-388">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-388">no</span></span>           |
| <span data-ttu-id="b4928-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="b4928-389">msdyn_committypename</span></span>         | <span data-ttu-id="b4928-390">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-390">no</span></span>             | <span data-ttu-id="b4928-391">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-391">no</span></span>           |
| <span data-ttu-id="b4928-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="b4928-392">msdyn_effort</span></span>                 | <span data-ttu-id="b4928-393">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-393">no</span></span>             | <span data-ttu-id="b4928-394">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-394">no</span></span>           |
| <span data-ttu-id="b4928-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="b4928-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="b4928-396">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-396">no</span></span>             | <span data-ttu-id="b4928-397">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-397">no</span></span>           |
| <span data-ttu-id="b4928-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="b4928-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="b4928-399">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-399">no</span></span>             | <span data-ttu-id="b4928-400">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-400">no</span></span>           |
| <span data-ttu-id="b4928-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="b4928-401">msdyn_finish</span></span>                 | <span data-ttu-id="b4928-402">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-402">no</span></span>             | <span data-ttu-id="b4928-403">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-403">no</span></span>           |
| <span data-ttu-id="b4928-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="b4928-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="b4928-405">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-405">no</span></span>             | <span data-ttu-id="b4928-406">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-406">no</span></span>           |
| <span data-ttu-id="b4928-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="b4928-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="b4928-408">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-408">no</span></span>             | <span data-ttu-id="b4928-409">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-409">no</span></span>           |
| <span data-ttu-id="b4928-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="b4928-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="b4928-411">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-411">no</span></span>             | <span data-ttu-id="b4928-412">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-412">no</span></span>           |
| <span data-ttu-id="b4928-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="b4928-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="b4928-414">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-414">no</span></span>             | <span data-ttu-id="b4928-415">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-415">no</span></span>           |
| <span data-ttu-id="b4928-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="b4928-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="b4928-417">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-417">no</span></span>             | <span data-ttu-id="b4928-418">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-418">no</span></span>           |
| <span data-ttu-id="b4928-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="b4928-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="b4928-420">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-420">no</span></span>             | <span data-ttu-id="b4928-421">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-421">no</span></span>           |
| <span data-ttu-id="b4928-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="b4928-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="b4928-423">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-423">no</span></span>             | <span data-ttu-id="b4928-424">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-424">no</span></span>           |
| <span data-ttu-id="b4928-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="b4928-425">msdyn_projectid</span></span>              | <span data-ttu-id="b4928-426">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-426">yes</span></span>            | <span data-ttu-id="b4928-427">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-427">no</span></span>           |
| <span data-ttu-id="b4928-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="b4928-428">msdyn_projectidname</span></span>          | <span data-ttu-id="b4928-429">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-429">no</span></span>             | <span data-ttu-id="b4928-430">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-430">no</span></span>           |
| <span data-ttu-id="b4928-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="b4928-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="b4928-432">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-432">no</span></span>             | <span data-ttu-id="b4928-433">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-433">no</span></span>           |
| <span data-ttu-id="b4928-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="b4928-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="b4928-435">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-435">no</span></span>             | <span data-ttu-id="b4928-436">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-436">no</span></span>           |
| <span data-ttu-id="b4928-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="b4928-437">msdyn_start</span></span>                  | <span data-ttu-id="b4928-438">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-438">no</span></span>             | <span data-ttu-id="b4928-439">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-439">no</span></span>           |
| <span data-ttu-id="b4928-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="b4928-440">msdyn_taskid</span></span>                 | <span data-ttu-id="b4928-441">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-441">no</span></span>             | <span data-ttu-id="b4928-442">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-442">no</span></span>           |
| <span data-ttu-id="b4928-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="b4928-443">msdyn_taskidname</span></span>             | <span data-ttu-id="b4928-444">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-444">no</span></span>             | <span data-ttu-id="b4928-445">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-445">no</span></span>           |
| <span data-ttu-id="b4928-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="b4928-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="b4928-447">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-447">no</span></span>             | <span data-ttu-id="b4928-448">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="b4928-449">प्रोजेक्ट टीम सदस्य</span><span class="sxs-lookup"><span data-stu-id="b4928-449">Project team member</span></span>

| <span data-ttu-id="b4928-450">**तार्किक नाम**</span><span class="sxs-lookup"><span data-stu-id="b4928-450">**Logical name**</span></span>                                 | <span data-ttu-id="b4928-451">**बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="b4928-451">**Can create**</span></span> | <span data-ttu-id="b4928-452">**संपादित कर सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="b4928-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="b4928-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="b4928-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="b4928-454">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-454">no</span></span>             | <span data-ttu-id="b4928-455">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-455">no</span></span>           |
| <span data-ttu-id="b4928-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="b4928-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="b4928-457">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-457">no</span></span>             | <span data-ttu-id="b4928-458">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-458">no</span></span>           |
| <span data-ttu-id="b4928-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="b4928-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="b4928-460">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-460">no</span></span>             | <span data-ttu-id="b4928-461">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-461">no</span></span>           |
| <span data-ttu-id="b4928-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="b4928-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="b4928-463">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-463">no</span></span>             | <span data-ttu-id="b4928-464">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-464">no</span></span>           |
| <span data-ttu-id="b4928-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="b4928-465">msdyn_effort</span></span>                                     | <span data-ttu-id="b4928-466">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-466">no</span></span>             | <span data-ttu-id="b4928-467">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-467">no</span></span>           |
| <span data-ttu-id="b4928-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="b4928-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="b4928-469">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-469">no</span></span>             | <span data-ttu-id="b4928-470">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-470">no</span></span>           |
| <span data-ttu-id="b4928-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="b4928-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="b4928-472">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-472">no</span></span>             | <span data-ttu-id="b4928-473">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-473">no</span></span>           |
| <span data-ttu-id="b4928-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="b4928-474">msdyn_finish</span></span>                                     | <span data-ttu-id="b4928-475">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-475">no</span></span>             | <span data-ttu-id="b4928-476">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-476">no</span></span>           |
| <span data-ttu-id="b4928-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="b4928-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="b4928-478">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-478">no</span></span>             | <span data-ttu-id="b4928-479">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-479">no</span></span>           |
| <span data-ttu-id="b4928-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="b4928-480">msdyn_hours</span></span>                                      | <span data-ttu-id="b4928-481">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-481">no</span></span>             | <span data-ttu-id="b4928-482">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-482">no</span></span>           |
| <span data-ttu-id="b4928-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="b4928-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="b4928-484">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-484">no</span></span>             | <span data-ttu-id="b4928-485">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-485">no</span></span>           |
| <span data-ttu-id="b4928-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="b4928-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="b4928-487">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-487">no</span></span>             | <span data-ttu-id="b4928-488">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-488">no</span></span>           |
| <span data-ttu-id="b4928-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="b4928-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="b4928-490">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-490">no</span></span>             | <span data-ttu-id="b4928-491">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-491">no</span></span>           |
| <span data-ttu-id="b4928-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="b4928-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="b4928-493">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-493">no</span></span>             | <span data-ttu-id="b4928-494">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-494">no</span></span>           |
| <span data-ttu-id="b4928-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="b4928-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="b4928-496">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-496">no</span></span>             | <span data-ttu-id="b4928-497">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-497">no</span></span>           |
| <span data-ttu-id="b4928-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="b4928-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="b4928-499">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-499">no</span></span>             | <span data-ttu-id="b4928-500">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-500">no</span></span>           |
| <span data-ttu-id="b4928-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="b4928-501">msdyn_start</span></span>                                      | <span data-ttu-id="b4928-502">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-502">no</span></span>             | <span data-ttu-id="b4928-503">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="b4928-504">Project</span><span class="sxs-lookup"><span data-stu-id="b4928-504">Project</span></span>

| <span data-ttu-id="b4928-505">**तार्किक नाम**</span><span class="sxs-lookup"><span data-stu-id="b4928-505">**Logical name**</span></span>                       | <span data-ttu-id="b4928-506">**बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="b4928-506">**Can create**</span></span> | <span data-ttu-id="b4928-507">**संपादित कर सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="b4928-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="b4928-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="b4928-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="b4928-509">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-509">no</span></span>             | <span data-ttu-id="b4928-510">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-510">no</span></span>           |
| <span data-ttu-id="b4928-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="b4928-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="b4928-512">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-512">no</span></span>             | <span data-ttu-id="b4928-513">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-513">no</span></span>           |
| <span data-ttu-id="b4928-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="b4928-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="b4928-515">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-515">no</span></span>             | <span data-ttu-id="b4928-516">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-516">no</span></span>           |
| <span data-ttu-id="b4928-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="b4928-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="b4928-518">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-518">no</span></span>             | <span data-ttu-id="b4928-519">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-519">no</span></span>           |
| <span data-ttu-id="b4928-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="b4928-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="b4928-521">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-521">no</span></span>             | <span data-ttu-id="b4928-522">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-522">no</span></span>           |
| <span data-ttu-id="b4928-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="b4928-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="b4928-524">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-524">no</span></span>             | <span data-ttu-id="b4928-525">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-525">no</span></span>           |
| <span data-ttu-id="b4928-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="b4928-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="b4928-527">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-527">yes</span></span>            | <span data-ttu-id="b4928-528">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-528">no</span></span>           |
| <span data-ttu-id="b4928-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="b4928-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="b4928-530">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-530">yes</span></span>            | <span data-ttu-id="b4928-531">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-531">no</span></span>           |
| <span data-ttu-id="b4928-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="b4928-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="b4928-533">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-533">yes</span></span>            | <span data-ttu-id="b4928-534">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-534">no</span></span>           |
| <span data-ttu-id="b4928-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="b4928-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="b4928-536">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-536">no</span></span>             | <span data-ttu-id="b4928-537">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-537">no</span></span>           |
| <span data-ttu-id="b4928-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="b4928-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="b4928-539">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-539">no</span></span>             | <span data-ttu-id="b4928-540">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-540">no</span></span>           |
| <span data-ttu-id="b4928-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="b4928-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="b4928-542">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-542">no</span></span>             | <span data-ttu-id="b4928-543">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-543">no</span></span>           |
| <span data-ttu-id="b4928-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="b4928-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="b4928-545">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-545">no</span></span>             | <span data-ttu-id="b4928-546">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-546">no</span></span>           |
| <span data-ttu-id="b4928-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="b4928-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="b4928-548">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-548">no</span></span>             | <span data-ttu-id="b4928-549">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-549">no</span></span>           |
| <span data-ttu-id="b4928-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="b4928-550">msdyn_duration</span></span>                         | <span data-ttu-id="b4928-551">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-551">no</span></span>             | <span data-ttu-id="b4928-552">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-552">no</span></span>           |
| <span data-ttu-id="b4928-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="b4928-553">msdyn_effort</span></span>                           | <span data-ttu-id="b4928-554">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-554">no</span></span>             | <span data-ttu-id="b4928-555">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-555">no</span></span>           |
| <span data-ttu-id="b4928-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="b4928-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="b4928-557">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-557">no</span></span>             | <span data-ttu-id="b4928-558">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-558">no</span></span>           |
| <span data-ttu-id="b4928-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="b4928-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="b4928-560">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-560">no</span></span>             | <span data-ttu-id="b4928-561">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-561">no</span></span>           |
| <span data-ttu-id="b4928-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="b4928-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="b4928-563">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-563">no</span></span>             | <span data-ttu-id="b4928-564">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-564">no</span></span>           |
| <span data-ttu-id="b4928-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="b4928-565">msdyn_finish</span></span>                           | <span data-ttu-id="b4928-566">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-566">yes</span></span>            | <span data-ttu-id="b4928-567">हाँ</span><span class="sxs-lookup"><span data-stu-id="b4928-567">yes</span></span>          |
| <span data-ttu-id="b4928-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="b4928-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="b4928-569">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-569">no</span></span>             | <span data-ttu-id="b4928-570">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-570">no</span></span>           |
| <span data-ttu-id="b4928-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="b4928-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="b4928-572">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-572">no</span></span>             | <span data-ttu-id="b4928-573">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-573">no</span></span>           |
| <span data-ttu-id="b4928-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="b4928-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="b4928-575">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-575">no</span></span>             | <span data-ttu-id="b4928-576">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-576">no</span></span>           |
| <span data-ttu-id="b4928-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="b4928-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="b4928-578">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-578">no</span></span>             | <span data-ttu-id="b4928-579">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-579">no</span></span>           |
| <span data-ttu-id="b4928-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="b4928-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="b4928-581">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-581">no</span></span>             | <span data-ttu-id="b4928-582">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-582">no</span></span>           |
| <span data-ttu-id="b4928-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="b4928-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="b4928-584">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-584">no</span></span>             | <span data-ttu-id="b4928-585">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-585">no</span></span>           |
| <span data-ttu-id="b4928-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="b4928-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="b4928-587">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-587">no</span></span>             | <span data-ttu-id="b4928-588">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-588">no</span></span>           |
| <span data-ttu-id="b4928-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="b4928-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="b4928-590">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-590">no</span></span>             | <span data-ttu-id="b4928-591">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-591">no</span></span>           |
| <span data-ttu-id="b4928-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="b4928-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="b4928-593">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-593">no</span></span>             | <span data-ttu-id="b4928-594">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-594">no</span></span>           |
| <span data-ttu-id="b4928-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="b4928-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="b4928-596">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-596">no</span></span>             | <span data-ttu-id="b4928-597">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-597">no</span></span>           |
| <span data-ttu-id="b4928-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="b4928-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="b4928-599">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-599">no</span></span>             | <span data-ttu-id="b4928-600">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-600">no</span></span>           |
| <span data-ttu-id="b4928-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="b4928-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="b4928-602">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-602">no</span></span>             | <span data-ttu-id="b4928-603">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-603">no</span></span>           |
| <span data-ttu-id="b4928-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="b4928-604">msdyn_progress</span></span>                         | <span data-ttu-id="b4928-605">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-605">no</span></span>             | <span data-ttu-id="b4928-606">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-606">no</span></span>           |
| <span data-ttu-id="b4928-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="b4928-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="b4928-608">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-608">no</span></span>             | <span data-ttu-id="b4928-609">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-609">no</span></span>           |
| <span data-ttu-id="b4928-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="b4928-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="b4928-611">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-611">no</span></span>             | <span data-ttu-id="b4928-612">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-612">no</span></span>           |
| <span data-ttu-id="b4928-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="b4928-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="b4928-614">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-614">no</span></span>             | <span data-ttu-id="b4928-615">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-615">no</span></span>           |
| <span data-ttu-id="b4928-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="b4928-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="b4928-617">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-617">no</span></span>             | <span data-ttu-id="b4928-618">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-618">no</span></span>           |
| <span data-ttu-id="b4928-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="b4928-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="b4928-620">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-620">no</span></span>             | <span data-ttu-id="b4928-621">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-621">no</span></span>           |
| <span data-ttu-id="b4928-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="b4928-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="b4928-623">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-623">no</span></span>             | <span data-ttu-id="b4928-624">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-624">no</span></span>           |
| <span data-ttu-id="b4928-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="b4928-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="b4928-626">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-626">no</span></span>             | <span data-ttu-id="b4928-627">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-627">no</span></span>           |
| <span data-ttu-id="b4928-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="b4928-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="b4928-629">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-629">no</span></span>             | <span data-ttu-id="b4928-630">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-630">no</span></span>           |
| <span data-ttu-id="b4928-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="b4928-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="b4928-632">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-632">no</span></span>             | <span data-ttu-id="b4928-633">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-633">no</span></span>           |
| <span data-ttu-id="b4928-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="b4928-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="b4928-635">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-635">no</span></span>             | <span data-ttu-id="b4928-636">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-636">no</span></span>           |
| <span data-ttu-id="b4928-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="b4928-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="b4928-638">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-638">no</span></span>             | <span data-ttu-id="b4928-639">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-639">no</span></span>           |
| <span data-ttu-id="b4928-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="b4928-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="b4928-641">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-641">no</span></span>             | <span data-ttu-id="b4928-642">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-642">no</span></span>           |
| <span data-ttu-id="b4928-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="b4928-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="b4928-644">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-644">no</span></span>             | <span data-ttu-id="b4928-645">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-645">no</span></span>           |
| <span data-ttu-id="b4928-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="b4928-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="b4928-647">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-647">no</span></span>             | <span data-ttu-id="b4928-648">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-648">no</span></span>           |
| <span data-ttu-id="b4928-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="b4928-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="b4928-650">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-650">no</span></span>             | <span data-ttu-id="b4928-651">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-651">no</span></span>           |
| <span data-ttu-id="b4928-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="b4928-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="b4928-653">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-653">no</span></span>             | <span data-ttu-id="b4928-654">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-654">no</span></span>           |
| <span data-ttu-id="b4928-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="b4928-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="b4928-656">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-656">no</span></span>             | <span data-ttu-id="b4928-657">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-657">no</span></span>           |
| <span data-ttu-id="b4928-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="b4928-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="b4928-659">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-659">no</span></span>             | <span data-ttu-id="b4928-660">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-660">no</span></span>           |
| <span data-ttu-id="b4928-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="b4928-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="b4928-662">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-662">no</span></span>             | <span data-ttu-id="b4928-663">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-663">no</span></span>           |
| <span data-ttu-id="b4928-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="b4928-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="b4928-665">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-665">no</span></span>             | <span data-ttu-id="b4928-666">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-666">no</span></span>           |
| <span data-ttu-id="b4928-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="b4928-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="b4928-668">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-668">no</span></span>             | <span data-ttu-id="b4928-669">नहीं</span><span class="sxs-lookup"><span data-stu-id="b4928-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="b4928-670">सीमाएं और ज्ञात मुद्दे</span><span class="sxs-lookup"><span data-stu-id="b4928-670">Limitations and known issues</span></span>
<span data-ttu-id="b4928-671">निम्नलिखित सीमाओं और ज्ञात मुद्दों की एक लिस्ट है:</span><span class="sxs-lookup"><span data-stu-id="b4928-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="b4928-672">शेड्यूल एपीआई का उपयोग केवल **Microsoft प्रोज़ेक्ट लाइसेंस वाले** उपयोगकर्ताओं द्वारा किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-672">Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="b4928-673">उनका इनके द्वारा उपयोग नहीं किया जा सकता है:</span><span class="sxs-lookup"><span data-stu-id="b4928-673">They can't be used by:</span></span>
    - <span data-ttu-id="b4928-674">अनुप्रयोग उपयोगकर्ता</span><span class="sxs-lookup"><span data-stu-id="b4928-674">Application users</span></span>
    - <span data-ttu-id="b4928-675">सिस्टम उपयोगकर्ता</span><span class="sxs-lookup"><span data-stu-id="b4928-675">System users</span></span>
    - <span data-ttu-id="b4928-676">एकीकरण उपयोगकर्ता</span><span class="sxs-lookup"><span data-stu-id="b4928-676">Integration users</span></span>
    - <span data-ttu-id="b4928-677">अन्य उपयोगकर्ता जिनके पास आवश्यक लाइसेंस नहीं है</span><span class="sxs-lookup"><span data-stu-id="b4928-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="b4928-678">प्रत्येक **OperationSet** में अधिकतम 100 संचालन हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="b4928-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="b4928-679">प्रत्येक उपयोगकर्ता के पास अधिकतम 10 खुला **OperationSets** हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="b4928-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="b4928-680">Project Operations वर्तमान में एक प्रोज़ेक्ट पर अधिकतम 500 कुल कार्यों का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="b4928-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="b4928-681">**OperationSet** विफलता की स्थिति और विफलता लॉग वर्तमान में उपलब्ध नहीं हैं.</span><span class="sxs-lookup"><span data-stu-id="b4928-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- [<span data-ttu-id="b4928-682">प्रोजेक्ट और कार्यों पर लिमिट और बाउंड्री</span><span class="sxs-lookup"><span data-stu-id="b4928-682">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="b4928-683">त्रुटि हैंडलिंग</span><span class="sxs-lookup"><span data-stu-id="b4928-683">Error handling</span></span>

   - <span data-ttu-id="b4928-684">ऑपरेशन सेट से उत्पन्न त्रुटियों की समीक्षा करने के लिए, **सेटिंग** \> **शेड्यूल इंटीग्रेशन** \> **ऑपरेशन सेट्स** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="b4928-684">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="b4928-685">प्रोजेक्ट शेड्यूलिंग सेवा से उत्पन्न त्रुटियों की समीक्षा करने के लिए, **सेटिंग** \> **शेड्यूल एकीकरण** \> **PSS त्रुटि लॉग पर** जाएं.</span><span class="sxs-lookup"><span data-stu-id="b4928-685">To review errors generated from the Project Scheduling Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="b4928-686">नमूना परिदृश्य</span><span class="sxs-lookup"><span data-stu-id="b4928-686">Sample scenario</span></span>

<span data-ttu-id="b4928-687">इस परिदृश्य में, आप एक प्रोज़ेक्ट, एक टीम के सदस्य, चार कार्य और दो संसाधन कार्य बनाएंगे.</span><span class="sxs-lookup"><span data-stu-id="b4928-687">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="b4928-688">इसके बाद, आप एक कार्य को अपडेट करेंगे, प्रोज़ेक्ट को अपडेट करेंगे, एक कार्य को हटा देंगे, एक संसाधन असाइनमेंट को हटा देंगे,और एक कार्य निर्भरता बनाएंगे.</span><span class="sxs-lookup"><span data-stu-id="b4928-688">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

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

## <a name="additional-samples"></a><span data-ttu-id="b4928-689">अतिरिक्त नमूने</span><span class="sxs-lookup"><span data-stu-id="b4928-689">Additional samples</span></span>

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
