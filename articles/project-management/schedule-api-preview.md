---
title: शेड्यूलिंग निकायों के साथ संचालन करने के लिए प्रोजेक्ट शेड्यूल API का उपयोग करें
description: यह विषय प्रोजेक्ट शेड्यूल API का उपयोग करने के लिए जानकारी और नमूने प्रदान करता है.
author: sigitac
ms.date: 06/22/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4915261c08a3271a919e04084e92a14b297c1b35
ms.sourcegitcommit: 2f16c2bc7c8350676a6a380c61fffa9958db6a0b
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/22/2021
ms.locfileid: "6293229"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a><span data-ttu-id="23acf-103">शेड्यूलिंग निकायों के साथ संचालन करने के लिए प्रोजेक्ट शेड्यूल API का उपयोग करें</span><span class="sxs-lookup"><span data-stu-id="23acf-103">Use Project schedule APIs to perform operations with Scheduling entities</span></span>

<span data-ttu-id="23acf-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="23acf-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT] 
> <span data-ttu-id="23acf-105">इस विषय में नोट की गई कुछ या सभी कार्यक्षमता पूर्वावलोकन रिलीज के हिस्से के रूप में उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="23acf-105">Some or all of the functionality noted in this topic is available as part of a preview release.</span></span> <span data-ttu-id="23acf-106">सामग्री और कार्यक्षमता परिवर्तन के अधीन हैं.</span><span class="sxs-lookup"><span data-stu-id="23acf-106">The content and the functionality are subject to change.</span></span> 

## <a name="scheduling-entities"></a><span data-ttu-id="23acf-107">शेड्यूलिंग निकाय</span><span class="sxs-lookup"><span data-stu-id="23acf-107">Scheduling entities</span></span>

<span data-ttu-id="23acf-108">प्रोजेक्ट शेड्यूल API **शेड्यूलिंग निकाय** के साथ ऑपरेशन बनाने, अपडेट करने और हटाने की क्षमता प्रदान करते हैं.</span><span class="sxs-lookup"><span data-stu-id="23acf-108">Project schedule APIs provide the ability to perform create, update, and delete operations with **Scheduling entities**.</span></span> <span data-ttu-id="23acf-109">इन निकायों को वेब के लिए परियोजना में शेड्यूलिंग इंजन के माध्यम से प्रबंधित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-109">These entities are managed through the Scheduling engine in Project for the web.</span></span> <span data-ttu-id="23acf-110">पहले Dynamics 365 Project Operations रिलीज़ में **निकाय शेड्यूलिंग** के साथ संचालन बनाएं, अपडेट करें और मिटाएं.</span><span class="sxs-lookup"><span data-stu-id="23acf-110">Create, update, and delete operations with **Scheduling entities** were restricted in earlier Dynamics 365 Project Operations releases.</span></span>

<span data-ttu-id="23acf-111">निम्न तालिका प्रोजेक्ट शेड्यूल निकायों की पूरी सूची प्रदान करती है.</span><span class="sxs-lookup"><span data-stu-id="23acf-111">The following table provides a full list of the Project schedule entities.</span></span>

| <span data-ttu-id="23acf-112">निकाय का नाम</span><span class="sxs-lookup"><span data-stu-id="23acf-112">Entity name</span></span>  | <span data-ttu-id="23acf-113">निकाय तार्किक नाम</span><span class="sxs-lookup"><span data-stu-id="23acf-113">Entity logical name</span></span> |
| --- | --- |
| <span data-ttu-id="23acf-114">Project</span><span class="sxs-lookup"><span data-stu-id="23acf-114">Project</span></span> | <span data-ttu-id="23acf-115">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="23acf-115">msdyn_project</span></span> |
| <span data-ttu-id="23acf-116">परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="23acf-116">Project Task</span></span>  | <span data-ttu-id="23acf-117">msdyn_projecttask</span><span class="sxs-lookup"><span data-stu-id="23acf-117">msdyn_projecttask</span></span>  |
| <span data-ttu-id="23acf-118">परियोजना कार्य निर्भरता</span><span class="sxs-lookup"><span data-stu-id="23acf-118">Project Task Dependency</span></span>  | <span data-ttu-id="23acf-119">msdyn_projecttaskdependency</span><span class="sxs-lookup"><span data-stu-id="23acf-119">msdyn_projecttaskdependency</span></span>  |
| <span data-ttu-id="23acf-120">संसाधन असाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="23acf-120">Resource Assignment</span></span> | <span data-ttu-id="23acf-121">msdyn_resourceassignment</span><span class="sxs-lookup"><span data-stu-id="23acf-121">msdyn_resourceassignment</span></span> |
| <span data-ttu-id="23acf-122">परियोजना बकेट</span><span class="sxs-lookup"><span data-stu-id="23acf-122">Project Bucket</span></span>  | <span data-ttu-id="23acf-123">msdyn_projectbucket</span><span class="sxs-lookup"><span data-stu-id="23acf-123">msdyn_projectbucket</span></span> |
| <span data-ttu-id="23acf-124">परियोजना टीम सदस्य</span><span class="sxs-lookup"><span data-stu-id="23acf-124">Project Team Member</span></span> | <span data-ttu-id="23acf-125">msdyn_projectteam</span><span class="sxs-lookup"><span data-stu-id="23acf-125">msdyn_projectteam</span></span> |

## <a name="operationset"></a><span data-ttu-id="23acf-126">OperationSet</span><span class="sxs-lookup"><span data-stu-id="23acf-126">OperationSet</span></span>

<span data-ttu-id="23acf-127">OperationSet एक यूनिट-ऑफ-वर्क पैटर्न है जिसका उपयोग तब किया जा सकता है जब शेड्यूल प्रभावित करने वाले कई अनुरोधों को लेनदेन के भीतर संसाधित किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="23acf-127">OperationSet is a unit-of-work pattern that can be used when several schedule impacting requests must be processed within a transaction.</span></span>

## <a name="project-schedule-apis"></a><span data-ttu-id="23acf-128">प्रोजेक्ट शेड्यूल API</span><span class="sxs-lookup"><span data-stu-id="23acf-128">Project schedule APIs</span></span>

<span data-ttu-id="23acf-129">निम्नलिखित वर्तमान प्रोजेक्ट शेड्यूल API की सूची है.</span><span class="sxs-lookup"><span data-stu-id="23acf-129">The following is a list of current Project schedule APIs.</span></span>

- <span data-ttu-id="23acf-130">**msdyn_CreateProjectV1**: इस API का उपयोग एक प्रोज़ेक्ट बनाने के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-130">**msdyn_CreateProjectV1**: This API can be used to create a project.</span></span> <span data-ttu-id="23acf-131">प्रोज़ेक्ट और डिफॉल्ट प्रोज़ेक्ट बकेट तुरंत बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-131">The project and default project bucket is created immediately.</span></span>
- <span data-ttu-id="23acf-132">**msdyn_CreateTeamMemberV1**: इस API का उपयोग प्रोज़ेक्ट टीम के सदस्य बनाने के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-132">**msdyn_CreateTeamMemberV1**: This API can be used to create a project team member.</span></span> <span data-ttu-id="23acf-133">टीम के सदस्य का रिकार्ड तुरंत बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-133">The team member record is created immediately.</span></span>
- <span data-ttu-id="23acf-134">**msdyn_CreateOperationSetV1**: इस एपीआई का उपयोग कई अनुरोधों को शेड्यूल करने के लिए किया जा सकता है जिन्हें लेनदेन के भीतर किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="23acf-134">**msdyn_CreateOperationSetV1**: This API can be used to schedule several requests that must be performed within a transaction.</span></span>
- <span data-ttu-id="23acf-135">**msdyn_PSSCreateV1**: इस एपीआई का उपयोग एक निकाय बनाने के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-135">**msdyn_PSSCreateV1**: This API can be used to create an entity.</span></span> <span data-ttu-id="23acf-136">निकाय कोई भी प्रोजेक्ट शेड्यूलिंग निकाय हो सकता है, जो निर्माण कार्य का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-136">The entity can be any of the Project scheduling entities that support the create operation.</span></span>
- <span data-ttu-id="23acf-137">**msdyn_PSSCreateV1**: इस API का उपयोग एक निकाय अपडेट के लिए किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-137">**msdyn_PSSUpdateV1**: This API can be used to update an entity.</span></span> <span data-ttu-id="23acf-138">निकाय कोई भी प्रोजेक्ट शेड्यूलिंग निकाय हो सकता है, जो अपडेट कार्य का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-138">The entity can be any of the Project scheduling entities that support the update operation.</span></span>
- <span data-ttu-id="23acf-139">**msdyn_PSSDeleteV1**: इस API को हटाने के लिए एक निकाय इस्तेमाल किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-139">**msdyn_PSSDeleteV1**: This API can be used to delete an entity.</span></span> <span data-ttu-id="23acf-140">निकाय कोई भी प्रोजेक्ट शेड्यूलिंग निकाय हो सकता है, जो हटाने के कार्य का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-140">The entity can be any of the Project scheduling entities that support the delete operation.</span></span>
- <span data-ttu-id="23acf-141">**msdyn_ExecuteOperationSetV1**: इस एपीआई का उपयोग दिए गए ऑपरेशन सेट के भीतर सभी संचालनों को निष्पादित करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-141">**msdyn_ExecuteOperationSetV1**: This API is used to execute all of the operations within the given operation set.</span></span>

## <a name="using-project-schedule-apis-with-operationset"></a><span data-ttu-id="23acf-142">ऑपरेशनसेट के साथ प्रोजेक्ट शेड्यूल API का उपयोग करना</span><span class="sxs-lookup"><span data-stu-id="23acf-142">Using Project schedule APIs with OperationSet</span></span>

<span data-ttu-id="23acf-143">क्योंकि दोनों के साथ रिकॉर्ड **CreateProjectV1** और **CreateTeamMemberV1** तुरंत बनाए जाते हैं, इन APIs का उपयोग सीधे **OperationSet** में नहीं किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-143">Because records with both **CreateProjectV1** and **CreateTeamMemberV1** are created immediately, these APIs can't be used in the **OperationSet** directly.</span></span> <span data-ttu-id="23acf-144">हालांकि, आप आवश्यक रिकॉर्ड बनाने, **OperationSet** बनाने के लिए API का उपयोग कर सकते हैं, और फिर **OperationSet** में इन पूर्व-निर्मित रिकॉर्ड का उपयोग कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="23acf-144">However, you can use the API to create needed records, create an **OperationSet**, and then use these pre-created records in the **OperationSet**.</span></span>

## <a name="supported-operations"></a><span data-ttu-id="23acf-145">समर्थित संचालन</span><span class="sxs-lookup"><span data-stu-id="23acf-145">Supported operations</span></span>

| <span data-ttu-id="23acf-146">निकाय शेड्यूलिंग</span><span class="sxs-lookup"><span data-stu-id="23acf-146">Scheduling entity</span></span> | <span data-ttu-id="23acf-147">निर्माण करें</span><span class="sxs-lookup"><span data-stu-id="23acf-147">Create</span></span> | <span data-ttu-id="23acf-148">अद्यतित करें</span><span class="sxs-lookup"><span data-stu-id="23acf-148">Update</span></span> | <span data-ttu-id="23acf-149">हटाएं</span><span class="sxs-lookup"><span data-stu-id="23acf-149">Delete</span></span> | <span data-ttu-id="23acf-150">महत्वपूर्ण विचार</span><span class="sxs-lookup"><span data-stu-id="23acf-150">Important considerations</span></span> |
| --- | --- | --- | --- | --- |
<span data-ttu-id="23acf-151">परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="23acf-151">Project task</span></span> | <span data-ttu-id="23acf-152">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-152">Yes</span></span> | <span data-ttu-id="23acf-153">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-153">Yes</span></span> | <span data-ttu-id="23acf-154">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-154">Yes</span></span> | <span data-ttu-id="23acf-155">कुछ नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-155">None</span></span> |
| <span data-ttu-id="23acf-156">प्रोज़ेक्ट कार्य निर्भरता</span><span class="sxs-lookup"><span data-stu-id="23acf-156">Project task dependency</span></span> | <span data-ttu-id="23acf-157">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-157">Yes</span></span> | <span data-ttu-id="23acf-158">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-158">Yes</span></span> | | <span data-ttu-id="23acf-159">प्रोज़ेक्ट कार्य निर्भरता रिकॉर्ड अपडेट नहीं किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="23acf-159">Project task dependency records aren't updated.</span></span> <span data-ttu-id="23acf-160">इसके बजाय, एक पुराना रिकॉर्ड हटाया जा सकता है और एक नया रिकॉर्ड बनाया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-160">Instead, an old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="23acf-161">रिसोर्स असाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="23acf-161">Resource assignment</span></span> | <span data-ttu-id="23acf-162">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-162">Yes</span></span> | <span data-ttu-id="23acf-163">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-163">Yes</span></span> | | <span data-ttu-id="23acf-164">निम्नलिखित फ़ील्ड के साथ संचालन का समर्थन नहीं किया जाता है: **BookableResourceID**, **प्रयास**,**EffortCompleted**, **EffortRemaining**, और **PlannedWork**.</span><span class="sxs-lookup"><span data-stu-id="23acf-164">Operations with the following fields aren't supported: **BookableResourceID**, **Effort**, **EffortCompleted**, **EffortRemaining**, and **PlannedWork**.</span></span> <span data-ttu-id="23acf-165">संसाधन असाइनमेंट रिकॉर्ड अपडेट नहीं किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="23acf-165">Resource assignment records aren't updated.</span></span> <span data-ttu-id="23acf-166">इसके बदले पुराना रिकॉर्ड डिलीट किया जा सकता है और नया रिकॉर्ड बनाया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-166">Instead, the old record can be deleted and a new record can be created.</span></span> |
| <span data-ttu-id="23acf-167">प्रोज़ेक्ट बकेट</span><span class="sxs-lookup"><span data-stu-id="23acf-167">Project bucket</span></span> | <span data-ttu-id="23acf-168">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-168">N/A</span></span> | <span data-ttu-id="23acf-169">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-169">N/A</span></span> | <span data-ttu-id="23acf-170">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-170">N/A</span></span> | <span data-ttu-id="23acf-171">डिफ़ॉल्ट बकेट **CreateProjectV1** API का उपयोग करके बनाई गई है.</span><span class="sxs-lookup"><span data-stu-id="23acf-171">The default bucket is created using the **CreateProjectV1** API.</span></span> |
| <span data-ttu-id="23acf-172">प्रोजेक्ट टीम सदस्य</span><span class="sxs-lookup"><span data-stu-id="23acf-172">Project team member</span></span> | <span data-ttu-id="23acf-173">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-173">Yes</span></span> | <span data-ttu-id="23acf-174">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-174">Yes</span></span> | <span data-ttu-id="23acf-175">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-175">Yes</span></span> | <span data-ttu-id="23acf-176">बनाने के ऑपरेशन के लिए, **CreateTeamMemberV1** API का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="23acf-176">For the create operation, use the **CreateTeamMemberV1** API.</span></span> |
| <span data-ttu-id="23acf-177">Project</span><span class="sxs-lookup"><span data-stu-id="23acf-177">Project</span></span> | <span data-ttu-id="23acf-178">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-178">Yes</span></span> | <span data-ttu-id="23acf-179">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-179">Yes</span></span> | <span data-ttu-id="23acf-180">लागू नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-180">N/A</span></span> | <span data-ttu-id="23acf-181">निम्नलिखित फ़ील्ड के साथ संचालन का समर्थन नहीं किया जाता है: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **प्रयास**, **EffortCompleted**, **EffortRemaining**, **प्रगति**, **समाप्त करें**, **TaskEarliestStart**, और **अवधि**.</span><span class="sxs-lookup"><span data-stu-id="23acf-181">Operations with the following fields aren't supported: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **Effort**, **EffortCompleted**, **EffortRemaining**, **Progress**, **Finish**, **TaskEarliestStart**, and **Duration**.</span></span> |

<span data-ttu-id="23acf-182">इन APIs को निकाय ऑब्जेक्ट्स के साथ बुलाया जा सकता है जिसमें कस्टम फ़ील्ड शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="23acf-182">These APIs can be called with entity objects that include custom fields.</span></span>

<span data-ttu-id="23acf-183">ID संपत्ति वैकल्पिक है.</span><span class="sxs-lookup"><span data-stu-id="23acf-183">The ID property is optional.</span></span> <span data-ttu-id="23acf-184">यदि यह प्रदान किया जाता है, तो सिस्टम इसका उपयोग करने का प्रयास करता है और यदि इसका उपयोग नहीं किया जा सकता है तो अपवाद प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-184">If it's provided, the system attempts to use it and throws an exception if it can't be used.</span></span> <span data-ttu-id="23acf-185">यदि यह प्रदान नहीं किया जाता है, तो सिस्टम इसे उत्पन्न करेगा.</span><span class="sxs-lookup"><span data-stu-id="23acf-185">If it isn't provided, the system will generate it.</span></span>

## <a name="restricted-fields"></a><span data-ttu-id="23acf-186">प्रतिबंधित फील्ड</span><span class="sxs-lookup"><span data-stu-id="23acf-186">Restricted fields</span></span>

<span data-ttu-id="23acf-187">निम्न तालिका उन क्षेत्रों को परिभाषित करती है जो **बनाएं** और **संपादित करें** से प्रतिबंधित हैं.</span><span class="sxs-lookup"><span data-stu-id="23acf-187">The following tables define the fields that are restricted from **Create** and **Edit.**</span></span>

### <a name="project-task"></a><span data-ttu-id="23acf-188">परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="23acf-188">Project task</span></span>

| <span data-ttu-id="23acf-189">**तार्किक नाम**</span><span class="sxs-lookup"><span data-stu-id="23acf-189">**Logical name**</span></span>                       | <span data-ttu-id="23acf-190">**बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="23acf-190">**Can create**</span></span> | <span data-ttu-id="23acf-191">**संपादित कर सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="23acf-191">**Can edit**</span></span>     |
|----------------------------------------|----------------|------------------|
| <span data-ttu-id="23acf-192">msdyn_actualcost</span><span class="sxs-lookup"><span data-stu-id="23acf-192">msdyn_actualcost</span></span>                       | <span data-ttu-id="23acf-193">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-193">no</span></span>             | <span data-ttu-id="23acf-194">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-194">no</span></span>               |
| <span data-ttu-id="23acf-195">msdyn_actualcost_base</span><span class="sxs-lookup"><span data-stu-id="23acf-195">msdyn_actualcost_base</span></span>                  | <span data-ttu-id="23acf-196">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-196">no</span></span>             | <span data-ttu-id="23acf-197">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-197">no</span></span>               |
| <span data-ttu-id="23acf-198">msdyn_actualend</span><span class="sxs-lookup"><span data-stu-id="23acf-198">msdyn_actualend</span></span>                        | <span data-ttu-id="23acf-199">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-199">no</span></span>             | <span data-ttu-id="23acf-200">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-200">no</span></span>               |
| <span data-ttu-id="23acf-201">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="23acf-201">msdyn_actualsales</span></span>                      | <span data-ttu-id="23acf-202">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-202">no</span></span>             | <span data-ttu-id="23acf-203">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-203">no</span></span>               |
| <span data-ttu-id="23acf-204">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="23acf-204">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="23acf-205">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-205">no</span></span>             | <span data-ttu-id="23acf-206">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-206">no</span></span>               |
| <span data-ttu-id="23acf-207">msdyn_actualstart</span><span class="sxs-lookup"><span data-stu-id="23acf-207">msdyn_actualstart</span></span>                      | <span data-ttu-id="23acf-208">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-208">no</span></span>             | <span data-ttu-id="23acf-209">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-209">no</span></span>               |
| <span data-ttu-id="23acf-210">msdyn_costatcompleteestimate</span><span class="sxs-lookup"><span data-stu-id="23acf-210">msdyn_costatcompleteestimate</span></span>           | <span data-ttu-id="23acf-211">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-211">no</span></span>             | <span data-ttu-id="23acf-212">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-212">no</span></span>               |
| <span data-ttu-id="23acf-213">msdyn_costatcompleteestimate_base</span><span class="sxs-lookup"><span data-stu-id="23acf-213">msdyn_costatcompleteestimate_base</span></span>      | <span data-ttu-id="23acf-214">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-214">no</span></span>             | <span data-ttu-id="23acf-215">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-215">no</span></span>               |
| <span data-ttu-id="23acf-216">msdyn_costconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="23acf-216">msdyn_costconsumptionpercentage</span></span>        | <span data-ttu-id="23acf-217">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-217">no</span></span>             | <span data-ttu-id="23acf-218">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-218">no</span></span>               |
| <span data-ttu-id="23acf-219">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="23acf-219">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="23acf-220">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-220">no</span></span>             | <span data-ttu-id="23acf-221">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-221">no</span></span>               |
| <span data-ttu-id="23acf-222">msdyn_effortestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="23acf-222">msdyn_effortestimateatcomplete</span></span>         | <span data-ttu-id="23acf-223">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-223">no</span></span>             | <span data-ttu-id="23acf-224">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-224">no</span></span>               |
| <span data-ttu-id="23acf-225">msdyn_iscritical</span><span class="sxs-lookup"><span data-stu-id="23acf-225">msdyn_iscritical</span></span>                       | <span data-ttu-id="23acf-226">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-226">no</span></span>             | <span data-ttu-id="23acf-227">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-227">no</span></span>               |
| <span data-ttu-id="23acf-228">msdyn_iscriticalname</span><span class="sxs-lookup"><span data-stu-id="23acf-228">msdyn_iscriticalname</span></span>                   | <span data-ttu-id="23acf-229">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-229">no</span></span>             | <span data-ttu-id="23acf-230">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-230">no</span></span>               |
| <span data-ttu-id="23acf-231">msdyn_ismanual</span><span class="sxs-lookup"><span data-stu-id="23acf-231">msdyn_ismanual</span></span>                         | <span data-ttu-id="23acf-232">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-232">no</span></span>             | <span data-ttu-id="23acf-233">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-233">no</span></span>               |
| <span data-ttu-id="23acf-234">msdyn_ismanualname</span><span class="sxs-lookup"><span data-stu-id="23acf-234">msdyn_ismanualname</span></span>                     | <span data-ttu-id="23acf-235">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-235">no</span></span>             | <span data-ttu-id="23acf-236">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-236">no</span></span>               |
| <span data-ttu-id="23acf-237">msdyn_ismilestone</span><span class="sxs-lookup"><span data-stu-id="23acf-237">msdyn_ismilestone</span></span>                      | <span data-ttu-id="23acf-238">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-238">no</span></span>             | <span data-ttu-id="23acf-239">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-239">no</span></span>               |
| <span data-ttu-id="23acf-240">msdyn_ismilestonename</span><span class="sxs-lookup"><span data-stu-id="23acf-240">msdyn_ismilestonename</span></span>                  | <span data-ttu-id="23acf-241">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-241">no</span></span>             | <span data-ttu-id="23acf-242">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-242">no</span></span>               |
| <span data-ttu-id="23acf-243">msdyn_LinkStatus</span><span class="sxs-lookup"><span data-stu-id="23acf-243">msdyn_LinkStatus</span></span>                       | <span data-ttu-id="23acf-244">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-244">no</span></span>             | <span data-ttu-id="23acf-245">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-245">no</span></span>               |
| <span data-ttu-id="23acf-246">msdyn_linkstatusname</span><span class="sxs-lookup"><span data-stu-id="23acf-246">msdyn_linkstatusname</span></span>                   | <span data-ttu-id="23acf-247">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-247">no</span></span>             | <span data-ttu-id="23acf-248">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-248">no</span></span>               |
| <span data-ttu-id="23acf-249">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="23acf-249">msdyn_msprojectclientid</span></span>                | <span data-ttu-id="23acf-250">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-250">no</span></span>             | <span data-ttu-id="23acf-251">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-251">no</span></span>               |
| <span data-ttu-id="23acf-252">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="23acf-252">msdyn_plannedcost</span></span>                      | <span data-ttu-id="23acf-253">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-253">no</span></span>             | <span data-ttu-id="23acf-254">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-254">no</span></span>               |
| <span data-ttu-id="23acf-255">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="23acf-255">msdyn_plannedcost_base</span></span>                 | <span data-ttu-id="23acf-256">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-256">no</span></span>             | <span data-ttu-id="23acf-257">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-257">no</span></span>               |
| <span data-ttu-id="23acf-258">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="23acf-258">msdyn_plannedsales</span></span>                     | <span data-ttu-id="23acf-259">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-259">no</span></span>             | <span data-ttu-id="23acf-260">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-260">no</span></span>               |
| <span data-ttu-id="23acf-261">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="23acf-261">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="23acf-262">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-262">no</span></span>             | <span data-ttu-id="23acf-263">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-263">no</span></span>               |
| <span data-ttu-id="23acf-264">msdyn_pluginprocessingdata</span><span class="sxs-lookup"><span data-stu-id="23acf-264">msdyn_pluginprocessingdata</span></span>             | <span data-ttu-id="23acf-265">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-265">no</span></span>             | <span data-ttu-id="23acf-266">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-266">no</span></span>               |
| <span data-ttu-id="23acf-267">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="23acf-267">msdyn_progress</span></span>                         | <span data-ttu-id="23acf-268">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-268">no</span></span>             | <span data-ttu-id="23acf-269">नही ( P4W के लिए हां)</span><span class="sxs-lookup"><span data-stu-id="23acf-269">no (yes for P4W)</span></span> |
| <span data-ttu-id="23acf-270">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="23acf-270">msdyn_remainingcost</span></span>                    | <span data-ttu-id="23acf-271">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-271">no</span></span>             | <span data-ttu-id="23acf-272">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-272">no</span></span>               |
| <span data-ttu-id="23acf-273">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="23acf-273">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="23acf-274">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-274">no</span></span>             | <span data-ttu-id="23acf-275">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-275">no</span></span>               |
| <span data-ttu-id="23acf-276">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="23acf-276">msdyn_remainingsales</span></span>                   | <span data-ttu-id="23acf-277">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-277">no</span></span>             | <span data-ttu-id="23acf-278">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-278">no</span></span>               |
| <span data-ttu-id="23acf-279">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="23acf-279">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="23acf-280">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-280">no</span></span>             | <span data-ttu-id="23acf-281">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-281">no</span></span>               |
| <span data-ttu-id="23acf-282">msdyn_requestedhours</span><span class="sxs-lookup"><span data-stu-id="23acf-282">msdyn_requestedhours</span></span>                   | <span data-ttu-id="23acf-283">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-283">no</span></span>             | <span data-ttu-id="23acf-284">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-284">no</span></span>               |
| <span data-ttu-id="23acf-285">msdyn_resourcecategory</span><span class="sxs-lookup"><span data-stu-id="23acf-285">msdyn_resourcecategory</span></span>                 | <span data-ttu-id="23acf-286">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-286">no</span></span>             | <span data-ttu-id="23acf-287">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-287">no</span></span>               |
| <span data-ttu-id="23acf-288">msdyn_resourcecategoryname</span><span class="sxs-lookup"><span data-stu-id="23acf-288">msdyn_resourcecategoryname</span></span>             | <span data-ttu-id="23acf-289">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-289">no</span></span>             | <span data-ttu-id="23acf-290">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-290">no</span></span>               |
| <span data-ttu-id="23acf-291">msdyn_resourceorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="23acf-291">msdyn_resourceorganizationalunitid</span></span>     | <span data-ttu-id="23acf-292">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-292">no</span></span>             | <span data-ttu-id="23acf-293">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-293">no</span></span>               |
| <span data-ttu-id="23acf-294">msdyn_resourceorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="23acf-294">msdyn_resourceorganizationalunitidname</span></span> | <span data-ttu-id="23acf-295">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-295">no</span></span>             | <span data-ttu-id="23acf-296">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-296">no</span></span>               |
| <span data-ttu-id="23acf-297">msdyn_salesconsumptionpercentage</span><span class="sxs-lookup"><span data-stu-id="23acf-297">msdyn_salesconsumptionpercentage</span></span>       | <span data-ttu-id="23acf-298">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-298">no</span></span>             | <span data-ttu-id="23acf-299">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-299">no</span></span>               |
| <span data-ttu-id="23acf-300">msdyn_salesestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="23acf-300">msdyn_salesestimateatcomplete</span></span>          | <span data-ttu-id="23acf-301">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-301">no</span></span>             | <span data-ttu-id="23acf-302">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-302">no</span></span>               |
| <span data-ttu-id="23acf-303">msdyn_salesestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="23acf-303">msdyn_salesestimateatcomplete_base</span></span>     | <span data-ttu-id="23acf-304">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-304">no</span></span>             | <span data-ttu-id="23acf-305">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-305">no</span></span>               |
| <span data-ttu-id="23acf-306">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="23acf-306">msdyn_salesvariance</span></span>                    | <span data-ttu-id="23acf-307">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-307">no</span></span>             | <span data-ttu-id="23acf-308">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-308">no</span></span>               |
| <span data-ttu-id="23acf-309">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="23acf-309">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="23acf-310">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-310">no</span></span>             | <span data-ttu-id="23acf-311">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-311">no</span></span>               |
| <span data-ttu-id="23acf-312">msdyn_scheduleddurationminutes</span><span class="sxs-lookup"><span data-stu-id="23acf-312">msdyn_scheduleddurationminutes</span></span>         | <span data-ttu-id="23acf-313">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-313">no</span></span>             | <span data-ttu-id="23acf-314">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-314">no</span></span>               |
| <span data-ttu-id="23acf-315">msdyn_scheduledend</span><span class="sxs-lookup"><span data-stu-id="23acf-315">msdyn_scheduledend</span></span>                     | <span data-ttu-id="23acf-316">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-316">no</span></span>             | <span data-ttu-id="23acf-317">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-317">no</span></span>               |
| <span data-ttu-id="23acf-318">msdyn_scheduledstart</span><span class="sxs-lookup"><span data-stu-id="23acf-318">msdyn_scheduledstart</span></span>                   | <span data-ttu-id="23acf-319">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-319">no</span></span>             | <span data-ttu-id="23acf-320">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-320">no</span></span>               |
| <span data-ttu-id="23acf-321">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="23acf-321">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="23acf-322">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-322">no</span></span>             | <span data-ttu-id="23acf-323">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-323">no</span></span>               |
| <span data-ttu-id="23acf-324">msdyn_skipupdateestimateline</span><span class="sxs-lookup"><span data-stu-id="23acf-324">msdyn_skipupdateestimateline</span></span>           | <span data-ttu-id="23acf-325">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-325">no</span></span>             | <span data-ttu-id="23acf-326">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-326">no</span></span>               |
| <span data-ttu-id="23acf-327">msdyn_skipupdateestimatelinename</span><span class="sxs-lookup"><span data-stu-id="23acf-327">msdyn_skipupdateestimatelinename</span></span>       | <span data-ttu-id="23acf-328">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-328">no</span></span>             | <span data-ttu-id="23acf-329">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-329">no</span></span>               |
| <span data-ttu-id="23acf-330">msdyn_summary</span><span class="sxs-lookup"><span data-stu-id="23acf-330">msdyn_summary</span></span>                          | <span data-ttu-id="23acf-331">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-331">no</span></span>             | <span data-ttu-id="23acf-332">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-332">no</span></span>               |
| <span data-ttu-id="23acf-333">msdyn_varianceofcost</span><span class="sxs-lookup"><span data-stu-id="23acf-333">msdyn_varianceofcost</span></span>                   | <span data-ttu-id="23acf-334">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-334">no</span></span>             | <span data-ttu-id="23acf-335">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-335">no</span></span>               |
| <span data-ttu-id="23acf-336">msdyn_varianceofcost_base</span><span class="sxs-lookup"><span data-stu-id="23acf-336">msdyn_varianceofcost_base</span></span>              | <span data-ttu-id="23acf-337">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-337">no</span></span>             | <span data-ttu-id="23acf-338">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-338">no</span></span>               |

### <a name="project-task-dependency"></a><span data-ttu-id="23acf-339">प्रोज़ेक्ट कार्य निर्भरता</span><span class="sxs-lookup"><span data-stu-id="23acf-339">Project task dependency</span></span>

| <span data-ttu-id="23acf-340">**तार्किक नाम**</span><span class="sxs-lookup"><span data-stu-id="23acf-340">**Logical name**</span></span>              | <span data-ttu-id="23acf-341">**बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="23acf-341">**Can create**</span></span> | <span data-ttu-id="23acf-342">**संपादित कर सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="23acf-342">**Can edit**</span></span> |
|-------------------------------|----------------|--------------|
| <span data-ttu-id="23acf-343">msdyn_linktype</span><span class="sxs-lookup"><span data-stu-id="23acf-343">msdyn_linktype</span></span>                | <span data-ttu-id="23acf-344">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-344">no</span></span>             | <span data-ttu-id="23acf-345">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-345">no</span></span>           |
| <span data-ttu-id="23acf-346">msdyn_linktypename</span><span class="sxs-lookup"><span data-stu-id="23acf-346">msdyn_linktypename</span></span>            | <span data-ttu-id="23acf-347">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-347">no</span></span>             | <span data-ttu-id="23acf-348">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-348">no</span></span>           |
| <span data-ttu-id="23acf-349">msdyn_predecessortask</span><span class="sxs-lookup"><span data-stu-id="23acf-349">msdyn_predecessortask</span></span>         | <span data-ttu-id="23acf-350">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-350">yes</span></span>            | <span data-ttu-id="23acf-351">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-351">no</span></span>           |
| <span data-ttu-id="23acf-352">msdyn_predecessortaskname</span><span class="sxs-lookup"><span data-stu-id="23acf-352">msdyn_predecessortaskname</span></span>     | <span data-ttu-id="23acf-353">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-353">yes</span></span>            | <span data-ttu-id="23acf-354">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-354">no</span></span>           |
| <span data-ttu-id="23acf-355">msdyn_project</span><span class="sxs-lookup"><span data-stu-id="23acf-355">msdyn_project</span></span>                 | <span data-ttu-id="23acf-356">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-356">yes</span></span>            | <span data-ttu-id="23acf-357">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-357">no</span></span>           |
| <span data-ttu-id="23acf-358">msdyn_projectname</span><span class="sxs-lookup"><span data-stu-id="23acf-358">msdyn_projectname</span></span>             | <span data-ttu-id="23acf-359">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-359">yes</span></span>            | <span data-ttu-id="23acf-360">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-360">no</span></span>           |
| <span data-ttu-id="23acf-361">msdyn_projecttaskdependencyid</span><span class="sxs-lookup"><span data-stu-id="23acf-361">msdyn_projecttaskdependencyid</span></span> | <span data-ttu-id="23acf-362">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-362">yes</span></span>            | <span data-ttu-id="23acf-363">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-363">no</span></span>           |
| <span data-ttu-id="23acf-364">msdyn_successortask</span><span class="sxs-lookup"><span data-stu-id="23acf-364">msdyn_successortask</span></span>           | <span data-ttu-id="23acf-365">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-365">yes</span></span>            | <span data-ttu-id="23acf-366">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-366">no</span></span>           |
| <span data-ttu-id="23acf-367">msdyn_successortaskname</span><span class="sxs-lookup"><span data-stu-id="23acf-367">msdyn_successortaskname</span></span>       | <span data-ttu-id="23acf-368">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-368">yes</span></span>            | <span data-ttu-id="23acf-369">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-369">no</span></span>           |

### <a name="resource-assignment"></a><span data-ttu-id="23acf-370">रिसोर्स असाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="23acf-370">Resource assignment</span></span>

| <span data-ttu-id="23acf-371">**तार्किक नाम**</span><span class="sxs-lookup"><span data-stu-id="23acf-371">**Logical name**</span></span>             | <span data-ttu-id="23acf-372">**बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="23acf-372">**Can create**</span></span> | <span data-ttu-id="23acf-373">**संपादित कर सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="23acf-373">**Can edit**</span></span> |
|------------------------------|----------------|--------------|
| <span data-ttu-id="23acf-374">msdyn_bookableresourceid</span><span class="sxs-lookup"><span data-stu-id="23acf-374">msdyn_bookableresourceid</span></span>     | <span data-ttu-id="23acf-375">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-375">yes</span></span>            | <span data-ttu-id="23acf-376">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-376">no</span></span>           |
| <span data-ttu-id="23acf-377">msdyn_bookableresourceidname</span><span class="sxs-lookup"><span data-stu-id="23acf-377">msdyn_bookableresourceidname</span></span> | <span data-ttu-id="23acf-378">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-378">yes</span></span>            | <span data-ttu-id="23acf-379">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-379">no</span></span>           |
| <span data-ttu-id="23acf-380">msdyn_bookingstatusid</span><span class="sxs-lookup"><span data-stu-id="23acf-380">msdyn_bookingstatusid</span></span>        | <span data-ttu-id="23acf-381">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-381">no</span></span>             | <span data-ttu-id="23acf-382">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-382">no</span></span>           |
| <span data-ttu-id="23acf-383">msdyn_bookingstatusidname</span><span class="sxs-lookup"><span data-stu-id="23acf-383">msdyn_bookingstatusidname</span></span>    | <span data-ttu-id="23acf-384">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-384">no</span></span>             | <span data-ttu-id="23acf-385">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-385">no</span></span>           |
| <span data-ttu-id="23acf-386">msdyn_committype</span><span class="sxs-lookup"><span data-stu-id="23acf-386">msdyn_committype</span></span>             | <span data-ttu-id="23acf-387">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-387">no</span></span>             | <span data-ttu-id="23acf-388">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-388">no</span></span>           |
| <span data-ttu-id="23acf-389">msdyn_committypename</span><span class="sxs-lookup"><span data-stu-id="23acf-389">msdyn_committypename</span></span>         | <span data-ttu-id="23acf-390">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-390">no</span></span>             | <span data-ttu-id="23acf-391">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-391">no</span></span>           |
| <span data-ttu-id="23acf-392">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="23acf-392">msdyn_effort</span></span>                 | <span data-ttu-id="23acf-393">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-393">no</span></span>             | <span data-ttu-id="23acf-394">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-394">no</span></span>           |
| <span data-ttu-id="23acf-395">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="23acf-395">msdyn_effortcompleted</span></span>        | <span data-ttu-id="23acf-396">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-396">no</span></span>             | <span data-ttu-id="23acf-397">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-397">no</span></span>           |
| <span data-ttu-id="23acf-398">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="23acf-398">msdyn_effortremaining</span></span>        | <span data-ttu-id="23acf-399">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-399">no</span></span>             | <span data-ttu-id="23acf-400">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-400">no</span></span>           |
| <span data-ttu-id="23acf-401">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="23acf-401">msdyn_finish</span></span>                 | <span data-ttu-id="23acf-402">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-402">no</span></span>             | <span data-ttu-id="23acf-403">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-403">no</span></span>           |
| <span data-ttu-id="23acf-404">msdyn_plannedcost</span><span class="sxs-lookup"><span data-stu-id="23acf-404">msdyn_plannedcost</span></span>            | <span data-ttu-id="23acf-405">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-405">no</span></span>             | <span data-ttu-id="23acf-406">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-406">no</span></span>           |
| <span data-ttu-id="23acf-407">msdyn_plannedcost_base</span><span class="sxs-lookup"><span data-stu-id="23acf-407">msdyn_plannedcost_base</span></span>       | <span data-ttu-id="23acf-408">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-408">no</span></span>             | <span data-ttu-id="23acf-409">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-409">no</span></span>           |
| <span data-ttu-id="23acf-410">msdyn_plannedcostcontour</span><span class="sxs-lookup"><span data-stu-id="23acf-410">msdyn_plannedcostcontour</span></span>     | <span data-ttu-id="23acf-411">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-411">no</span></span>             | <span data-ttu-id="23acf-412">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-412">no</span></span>           |
| <span data-ttu-id="23acf-413">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="23acf-413">msdyn_plannedsales</span></span>           | <span data-ttu-id="23acf-414">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-414">no</span></span>             | <span data-ttu-id="23acf-415">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-415">no</span></span>           |
| <span data-ttu-id="23acf-416">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="23acf-416">msdyn_plannedsales_base</span></span>      | <span data-ttu-id="23acf-417">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-417">no</span></span>             | <span data-ttu-id="23acf-418">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-418">no</span></span>           |
| <span data-ttu-id="23acf-419">msdyn_plannedsalescontour</span><span class="sxs-lookup"><span data-stu-id="23acf-419">msdyn_plannedsalescontour</span></span>    | <span data-ttu-id="23acf-420">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-420">no</span></span>             | <span data-ttu-id="23acf-421">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-421">no</span></span>           |
| <span data-ttu-id="23acf-422">msdyn_plannedwork</span><span class="sxs-lookup"><span data-stu-id="23acf-422">msdyn_plannedwork</span></span>            | <span data-ttu-id="23acf-423">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-423">no</span></span>             | <span data-ttu-id="23acf-424">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-424">no</span></span>           |
| <span data-ttu-id="23acf-425">msdyn_projectid</span><span class="sxs-lookup"><span data-stu-id="23acf-425">msdyn_projectid</span></span>              | <span data-ttu-id="23acf-426">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-426">yes</span></span>            | <span data-ttu-id="23acf-427">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-427">no</span></span>           |
| <span data-ttu-id="23acf-428">msdyn_projectidname</span><span class="sxs-lookup"><span data-stu-id="23acf-428">msdyn_projectidname</span></span>          | <span data-ttu-id="23acf-429">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-429">no</span></span>             | <span data-ttu-id="23acf-430">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-430">no</span></span>           |
| <span data-ttu-id="23acf-431">msdyn_projectteamid</span><span class="sxs-lookup"><span data-stu-id="23acf-431">msdyn_projectteamid</span></span>          | <span data-ttu-id="23acf-432">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-432">no</span></span>             | <span data-ttu-id="23acf-433">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-433">no</span></span>           |
| <span data-ttu-id="23acf-434">msdyn_projectteamidname</span><span class="sxs-lookup"><span data-stu-id="23acf-434">msdyn_projectteamidname</span></span>      | <span data-ttu-id="23acf-435">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-435">no</span></span>             | <span data-ttu-id="23acf-436">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-436">no</span></span>           |
| <span data-ttu-id="23acf-437">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="23acf-437">msdyn_start</span></span>                  | <span data-ttu-id="23acf-438">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-438">no</span></span>             | <span data-ttu-id="23acf-439">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-439">no</span></span>           |
| <span data-ttu-id="23acf-440">msdyn_taskid</span><span class="sxs-lookup"><span data-stu-id="23acf-440">msdyn_taskid</span></span>                 | <span data-ttu-id="23acf-441">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-441">no</span></span>             | <span data-ttu-id="23acf-442">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-442">no</span></span>           |
| <span data-ttu-id="23acf-443">msdyn_taskidname</span><span class="sxs-lookup"><span data-stu-id="23acf-443">msdyn_taskidname</span></span>             | <span data-ttu-id="23acf-444">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-444">no</span></span>             | <span data-ttu-id="23acf-445">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-445">no</span></span>           |
| <span data-ttu-id="23acf-446">msdyn_userresourceid</span><span class="sxs-lookup"><span data-stu-id="23acf-446">msdyn_userresourceid</span></span>         | <span data-ttu-id="23acf-447">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-447">no</span></span>             | <span data-ttu-id="23acf-448">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-448">no</span></span>           |

### <a name="project-team-member"></a><span data-ttu-id="23acf-449">प्रोजेक्ट टीम सदस्य</span><span class="sxs-lookup"><span data-stu-id="23acf-449">Project team member</span></span>

| <span data-ttu-id="23acf-450">**तार्किक नाम**</span><span class="sxs-lookup"><span data-stu-id="23acf-450">**Logical name**</span></span>                                 | <span data-ttu-id="23acf-451">**बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="23acf-451">**Can create**</span></span> | <span data-ttu-id="23acf-452">**संपादित कर सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="23acf-452">**Can edit**</span></span> |
|--------------------------------------------------|----------------|--------------|
| <span data-ttu-id="23acf-453">msdyn_calendarid</span><span class="sxs-lookup"><span data-stu-id="23acf-453">msdyn_calendarid</span></span>                                 | <span data-ttu-id="23acf-454">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-454">no</span></span>             | <span data-ttu-id="23acf-455">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-455">no</span></span>           |
| <span data-ttu-id="23acf-456">msdyn_creategenericteammemberwithrequirementname</span><span class="sxs-lookup"><span data-stu-id="23acf-456">msdyn_creategenericteammemberwithrequirementname</span></span> | <span data-ttu-id="23acf-457">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-457">no</span></span>             | <span data-ttu-id="23acf-458">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-458">no</span></span>           |
| <span data-ttu-id="23acf-459">msdyn_deletestatus</span><span class="sxs-lookup"><span data-stu-id="23acf-459">msdyn_deletestatus</span></span>                               | <span data-ttu-id="23acf-460">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-460">no</span></span>             | <span data-ttu-id="23acf-461">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-461">no</span></span>           |
| <span data-ttu-id="23acf-462">msdyn_deletestatusname</span><span class="sxs-lookup"><span data-stu-id="23acf-462">msdyn_deletestatusname</span></span>                           | <span data-ttu-id="23acf-463">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-463">no</span></span>             | <span data-ttu-id="23acf-464">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-464">no</span></span>           |
| <span data-ttu-id="23acf-465">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="23acf-465">msdyn_effort</span></span>                                     | <span data-ttu-id="23acf-466">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-466">no</span></span>             | <span data-ttu-id="23acf-467">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-467">no</span></span>           |
| <span data-ttu-id="23acf-468">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="23acf-468">msdyn_effortcompleted</span></span>                            | <span data-ttu-id="23acf-469">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-469">no</span></span>             | <span data-ttu-id="23acf-470">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-470">no</span></span>           |
| <span data-ttu-id="23acf-471">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="23acf-471">msdyn_effortremaining</span></span>                            | <span data-ttu-id="23acf-472">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-472">no</span></span>             | <span data-ttu-id="23acf-473">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-473">no</span></span>           |
| <span data-ttu-id="23acf-474">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="23acf-474">msdyn_finish</span></span>                                     | <span data-ttu-id="23acf-475">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-475">no</span></span>             | <span data-ttu-id="23acf-476">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-476">no</span></span>           |
| <span data-ttu-id="23acf-477">msdyn_hardbookedhours</span><span class="sxs-lookup"><span data-stu-id="23acf-477">msdyn_hardbookedhours</span></span>                            | <span data-ttu-id="23acf-478">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-478">no</span></span>             | <span data-ttu-id="23acf-479">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-479">no</span></span>           |
| <span data-ttu-id="23acf-480">msdyn_hours</span><span class="sxs-lookup"><span data-stu-id="23acf-480">msdyn_hours</span></span>                                      | <span data-ttu-id="23acf-481">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-481">no</span></span>             | <span data-ttu-id="23acf-482">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-482">no</span></span>           |
| <span data-ttu-id="23acf-483">msdyn_markedfordeletiontimer</span><span class="sxs-lookup"><span data-stu-id="23acf-483">msdyn_markedfordeletiontimer</span></span>                     | <span data-ttu-id="23acf-484">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-484">no</span></span>             | <span data-ttu-id="23acf-485">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-485">no</span></span>           |
| <span data-ttu-id="23acf-486">msdyn_markedfordeletiontimestamp</span><span class="sxs-lookup"><span data-stu-id="23acf-486">msdyn_markedfordeletiontimestamp</span></span>                 | <span data-ttu-id="23acf-487">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-487">no</span></span>             | <span data-ttu-id="23acf-488">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-488">no</span></span>           |
| <span data-ttu-id="23acf-489">msdyn_msprojectclientid</span><span class="sxs-lookup"><span data-stu-id="23acf-489">msdyn_msprojectclientid</span></span>                          | <span data-ttu-id="23acf-490">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-490">no</span></span>             | <span data-ttu-id="23acf-491">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-491">no</span></span>           |
| <span data-ttu-id="23acf-492">msdyn_percentage</span><span class="sxs-lookup"><span data-stu-id="23acf-492">msdyn_percentage</span></span>                                 | <span data-ttu-id="23acf-493">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-493">no</span></span>             | <span data-ttu-id="23acf-494">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-494">no</span></span>           |
| <span data-ttu-id="23acf-495">msdyn_requiredhours</span><span class="sxs-lookup"><span data-stu-id="23acf-495">msdyn_requiredhours</span></span>                              | <span data-ttu-id="23acf-496">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-496">no</span></span>             | <span data-ttu-id="23acf-497">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-497">no</span></span>           |
| <span data-ttu-id="23acf-498">msdyn_softbookedhours</span><span class="sxs-lookup"><span data-stu-id="23acf-498">msdyn_softbookedhours</span></span>                            | <span data-ttu-id="23acf-499">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-499">no</span></span>             | <span data-ttu-id="23acf-500">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-500">no</span></span>           |
| <span data-ttu-id="23acf-501">msdyn_start</span><span class="sxs-lookup"><span data-stu-id="23acf-501">msdyn_start</span></span>                                      | <span data-ttu-id="23acf-502">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-502">no</span></span>             | <span data-ttu-id="23acf-503">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-503">no</span></span>           |

### <a name="project"></a><span data-ttu-id="23acf-504">Project</span><span class="sxs-lookup"><span data-stu-id="23acf-504">Project</span></span>

| <span data-ttu-id="23acf-505">**तार्किक नाम**</span><span class="sxs-lookup"><span data-stu-id="23acf-505">**Logical name**</span></span>                       | <span data-ttu-id="23acf-506">**बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="23acf-506">**Can create**</span></span> | <span data-ttu-id="23acf-507">**संपादित कर सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="23acf-507">**Can edit**</span></span> |
|----------------------------------------|----------------|--------------|
| <span data-ttu-id="23acf-508">msdyn_actualexpensecost</span><span class="sxs-lookup"><span data-stu-id="23acf-508">msdyn_actualexpensecost</span></span>                | <span data-ttu-id="23acf-509">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-509">no</span></span>             | <span data-ttu-id="23acf-510">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-510">no</span></span>           |
| <span data-ttu-id="23acf-511">msdyn_actualexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="23acf-511">msdyn_actualexpensecost_base</span></span>           | <span data-ttu-id="23acf-512">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-512">no</span></span>             | <span data-ttu-id="23acf-513">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-513">no</span></span>           |
| <span data-ttu-id="23acf-514">msdyn_actuallaborcost</span><span class="sxs-lookup"><span data-stu-id="23acf-514">msdyn_actuallaborcost</span></span>                  | <span data-ttu-id="23acf-515">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-515">no</span></span>             | <span data-ttu-id="23acf-516">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-516">no</span></span>           |
| <span data-ttu-id="23acf-517">msdyn_actuallaborcost_base</span><span class="sxs-lookup"><span data-stu-id="23acf-517">msdyn_actuallaborcost_base</span></span>             | <span data-ttu-id="23acf-518">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-518">no</span></span>             | <span data-ttu-id="23acf-519">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-519">no</span></span>           |
| <span data-ttu-id="23acf-520">msdyn_actualsales</span><span class="sxs-lookup"><span data-stu-id="23acf-520">msdyn_actualsales</span></span>                      | <span data-ttu-id="23acf-521">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-521">no</span></span>             | <span data-ttu-id="23acf-522">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-522">no</span></span>           |
| <span data-ttu-id="23acf-523">msdyn_actualsales_base</span><span class="sxs-lookup"><span data-stu-id="23acf-523">msdyn_actualsales_base</span></span>                 | <span data-ttu-id="23acf-524">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-524">no</span></span>             | <span data-ttu-id="23acf-525">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-525">no</span></span>           |
| <span data-ttu-id="23acf-526">msdyn_contractlineproject</span><span class="sxs-lookup"><span data-stu-id="23acf-526">msdyn_contractlineproject</span></span>              | <span data-ttu-id="23acf-527">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-527">yes</span></span>            | <span data-ttu-id="23acf-528">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-528">no</span></span>           |
| <span data-ttu-id="23acf-529">msdyn_contractorganizationalunitid</span><span class="sxs-lookup"><span data-stu-id="23acf-529">msdyn_contractorganizationalunitid</span></span>     | <span data-ttu-id="23acf-530">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-530">yes</span></span>            | <span data-ttu-id="23acf-531">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-531">no</span></span>           |
| <span data-ttu-id="23acf-532">msdyn_contractorganizationalunitidname</span><span class="sxs-lookup"><span data-stu-id="23acf-532">msdyn_contractorganizationalunitidname</span></span> | <span data-ttu-id="23acf-533">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-533">yes</span></span>            | <span data-ttu-id="23acf-534">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-534">no</span></span>           |
| <span data-ttu-id="23acf-535">msdyn_costconsumption</span><span class="sxs-lookup"><span data-stu-id="23acf-535">msdyn_costconsumption</span></span>                  | <span data-ttu-id="23acf-536">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-536">no</span></span>             | <span data-ttu-id="23acf-537">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-537">no</span></span>           |
| <span data-ttu-id="23acf-538">msdyn_costestimateatcomplete</span><span class="sxs-lookup"><span data-stu-id="23acf-538">msdyn_costestimateatcomplete</span></span>           | <span data-ttu-id="23acf-539">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-539">no</span></span>             | <span data-ttu-id="23acf-540">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-540">no</span></span>           |
| <span data-ttu-id="23acf-541">msdyn_costestimateatcomplete_base</span><span class="sxs-lookup"><span data-stu-id="23acf-541">msdyn_costestimateatcomplete_base</span></span>      | <span data-ttu-id="23acf-542">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-542">no</span></span>             | <span data-ttu-id="23acf-543">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-543">no</span></span>           |
| <span data-ttu-id="23acf-544">msdyn_costvariance</span><span class="sxs-lookup"><span data-stu-id="23acf-544">msdyn_costvariance</span></span>                     | <span data-ttu-id="23acf-545">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-545">no</span></span>             | <span data-ttu-id="23acf-546">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-546">no</span></span>           |
| <span data-ttu-id="23acf-547">msdyn_costvariance_base</span><span class="sxs-lookup"><span data-stu-id="23acf-547">msdyn_costvariance_base</span></span>                | <span data-ttu-id="23acf-548">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-548">no</span></span>             | <span data-ttu-id="23acf-549">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-549">no</span></span>           |
| <span data-ttu-id="23acf-550">msdyn_duration</span><span class="sxs-lookup"><span data-stu-id="23acf-550">msdyn_duration</span></span>                         | <span data-ttu-id="23acf-551">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-551">no</span></span>             | <span data-ttu-id="23acf-552">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-552">no</span></span>           |
| <span data-ttu-id="23acf-553">msdyn_effort</span><span class="sxs-lookup"><span data-stu-id="23acf-553">msdyn_effort</span></span>                           | <span data-ttu-id="23acf-554">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-554">no</span></span>             | <span data-ttu-id="23acf-555">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-555">no</span></span>           |
| <span data-ttu-id="23acf-556">msdyn_effortcompleted</span><span class="sxs-lookup"><span data-stu-id="23acf-556">msdyn_effortcompleted</span></span>                  | <span data-ttu-id="23acf-557">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-557">no</span></span>             | <span data-ttu-id="23acf-558">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-558">no</span></span>           |
| <span data-ttu-id="23acf-559">msdyn_effortestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="23acf-559">msdyn_effortestimateatcompleteeac</span></span>      | <span data-ttu-id="23acf-560">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-560">no</span></span>             | <span data-ttu-id="23acf-561">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-561">no</span></span>           |
| <span data-ttu-id="23acf-562">msdyn_effortremaining</span><span class="sxs-lookup"><span data-stu-id="23acf-562">msdyn_effortremaining</span></span>                  | <span data-ttu-id="23acf-563">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-563">no</span></span>             | <span data-ttu-id="23acf-564">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-564">no</span></span>           |
| <span data-ttu-id="23acf-565">msdyn_finish</span><span class="sxs-lookup"><span data-stu-id="23acf-565">msdyn_finish</span></span>                           | <span data-ttu-id="23acf-566">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-566">yes</span></span>            | <span data-ttu-id="23acf-567">हाँ</span><span class="sxs-lookup"><span data-stu-id="23acf-567">yes</span></span>          |
| <span data-ttu-id="23acf-568">msdyn_globalrevisiontoken</span><span class="sxs-lookup"><span data-stu-id="23acf-568">msdyn_globalrevisiontoken</span></span>              | <span data-ttu-id="23acf-569">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-569">no</span></span>             | <span data-ttu-id="23acf-570">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-570">no</span></span>           |
| <span data-ttu-id="23acf-571">msdyn_islinkedtomsprojectclient</span><span class="sxs-lookup"><span data-stu-id="23acf-571">msdyn_islinkedtomsprojectclient</span></span>        | <span data-ttu-id="23acf-572">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-572">no</span></span>             | <span data-ttu-id="23acf-573">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-573">no</span></span>           |
| <span data-ttu-id="23acf-574">msdyn_islinkedtomsprojectclientname</span><span class="sxs-lookup"><span data-stu-id="23acf-574">msdyn_islinkedtomsprojectclientname</span></span>    | <span data-ttu-id="23acf-575">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-575">no</span></span>             | <span data-ttu-id="23acf-576">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-576">no</span></span>           |
| <span data-ttu-id="23acf-577">msdyn_linkeddocumenturl</span><span class="sxs-lookup"><span data-stu-id="23acf-577">msdyn_linkeddocumenturl</span></span>                | <span data-ttu-id="23acf-578">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-578">no</span></span>             | <span data-ttu-id="23acf-579">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-579">no</span></span>           |
| <span data-ttu-id="23acf-580">msdyn_msprojectdocument</span><span class="sxs-lookup"><span data-stu-id="23acf-580">msdyn_msprojectdocument</span></span>                | <span data-ttu-id="23acf-581">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-581">no</span></span>             | <span data-ttu-id="23acf-582">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-582">no</span></span>           |
| <span data-ttu-id="23acf-583">msdyn_msprojectdocumentname</span><span class="sxs-lookup"><span data-stu-id="23acf-583">msdyn_msprojectdocumentname</span></span>            | <span data-ttu-id="23acf-584">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-584">no</span></span>             | <span data-ttu-id="23acf-585">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-585">no</span></span>           |
| <span data-ttu-id="23acf-586">msdyn_plannedexpensecost</span><span class="sxs-lookup"><span data-stu-id="23acf-586">msdyn_plannedexpensecost</span></span>               | <span data-ttu-id="23acf-587">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-587">no</span></span>             | <span data-ttu-id="23acf-588">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-588">no</span></span>           |
| <span data-ttu-id="23acf-589">msdyn_plannedexpensecost_base</span><span class="sxs-lookup"><span data-stu-id="23acf-589">msdyn_plannedexpensecost_base</span></span>          | <span data-ttu-id="23acf-590">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-590">no</span></span>             | <span data-ttu-id="23acf-591">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-591">no</span></span>           |
| <span data-ttu-id="23acf-592">msdyn_plannedlaborcost</span><span class="sxs-lookup"><span data-stu-id="23acf-592">msdyn_plannedlaborcost</span></span>                 | <span data-ttu-id="23acf-593">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-593">no</span></span>             | <span data-ttu-id="23acf-594">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-594">no</span></span>           |
| <span data-ttu-id="23acf-595">msdyn_plannedlaborcost_base</span><span class="sxs-lookup"><span data-stu-id="23acf-595">msdyn_plannedlaborcost_base</span></span>            | <span data-ttu-id="23acf-596">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-596">no</span></span>             | <span data-ttu-id="23acf-597">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-597">no</span></span>           |
| <span data-ttu-id="23acf-598">msdyn_plannedsales</span><span class="sxs-lookup"><span data-stu-id="23acf-598">msdyn_plannedsales</span></span>                     | <span data-ttu-id="23acf-599">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-599">no</span></span>             | <span data-ttu-id="23acf-600">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-600">no</span></span>           |
| <span data-ttu-id="23acf-601">msdyn_plannedsales_base</span><span class="sxs-lookup"><span data-stu-id="23acf-601">msdyn_plannedsales_base</span></span>                | <span data-ttu-id="23acf-602">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-602">no</span></span>             | <span data-ttu-id="23acf-603">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-603">no</span></span>           |
| <span data-ttu-id="23acf-604">msdyn_progress</span><span class="sxs-lookup"><span data-stu-id="23acf-604">msdyn_progress</span></span>                         | <span data-ttu-id="23acf-605">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-605">no</span></span>             | <span data-ttu-id="23acf-606">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-606">no</span></span>           |
| <span data-ttu-id="23acf-607">msdyn_remainingcost</span><span class="sxs-lookup"><span data-stu-id="23acf-607">msdyn_remainingcost</span></span>                    | <span data-ttu-id="23acf-608">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-608">no</span></span>             | <span data-ttu-id="23acf-609">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-609">no</span></span>           |
| <span data-ttu-id="23acf-610">msdyn_remainingcost_base</span><span class="sxs-lookup"><span data-stu-id="23acf-610">msdyn_remainingcost_base</span></span>               | <span data-ttu-id="23acf-611">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-611">no</span></span>             | <span data-ttu-id="23acf-612">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-612">no</span></span>           |
| <span data-ttu-id="23acf-613">msdyn_remainingsales</span><span class="sxs-lookup"><span data-stu-id="23acf-613">msdyn_remainingsales</span></span>                   | <span data-ttu-id="23acf-614">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-614">no</span></span>             | <span data-ttu-id="23acf-615">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-615">no</span></span>           |
| <span data-ttu-id="23acf-616">msdyn_remainingsales_base</span><span class="sxs-lookup"><span data-stu-id="23acf-616">msdyn_remainingsales_base</span></span>              | <span data-ttu-id="23acf-617">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-617">no</span></span>             | <span data-ttu-id="23acf-618">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-618">no</span></span>           |
| <span data-ttu-id="23acf-619">msdyn_replaylogheader</span><span class="sxs-lookup"><span data-stu-id="23acf-619">msdyn_replaylogheader</span></span>                  | <span data-ttu-id="23acf-620">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-620">no</span></span>             | <span data-ttu-id="23acf-621">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-621">no</span></span>           |
| <span data-ttu-id="23acf-622">msdyn_salesconsumption</span><span class="sxs-lookup"><span data-stu-id="23acf-622">msdyn_salesconsumption</span></span>                 | <span data-ttu-id="23acf-623">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-623">no</span></span>             | <span data-ttu-id="23acf-624">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-624">no</span></span>           |
| <span data-ttu-id="23acf-625">msdyn_salesestimateatcompleteeac</span><span class="sxs-lookup"><span data-stu-id="23acf-625">msdyn_salesestimateatcompleteeac</span></span>       | <span data-ttu-id="23acf-626">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-626">no</span></span>             | <span data-ttu-id="23acf-627">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-627">no</span></span>           |
| <span data-ttu-id="23acf-628">msdyn_salesestimateatcompleteeac_base</span><span class="sxs-lookup"><span data-stu-id="23acf-628">msdyn_salesestimateatcompleteeac_base</span></span>  | <span data-ttu-id="23acf-629">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-629">no</span></span>             | <span data-ttu-id="23acf-630">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-630">no</span></span>           |
| <span data-ttu-id="23acf-631">msdyn_salesvariance</span><span class="sxs-lookup"><span data-stu-id="23acf-631">msdyn_salesvariance</span></span>                    | <span data-ttu-id="23acf-632">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-632">no</span></span>             | <span data-ttu-id="23acf-633">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-633">no</span></span>           |
| <span data-ttu-id="23acf-634">msdyn_salesvariance_base</span><span class="sxs-lookup"><span data-stu-id="23acf-634">msdyn_salesvariance_base</span></span>               | <span data-ttu-id="23acf-635">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-635">no</span></span>             | <span data-ttu-id="23acf-636">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-636">no</span></span>           |
| <span data-ttu-id="23acf-637">msdyn_scheduleperformance</span><span class="sxs-lookup"><span data-stu-id="23acf-637">msdyn_scheduleperformance</span></span>              | <span data-ttu-id="23acf-638">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-638">no</span></span>             | <span data-ttu-id="23acf-639">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-639">no</span></span>           |
| <span data-ttu-id="23acf-640">msdyn_scheduleperformancename</span><span class="sxs-lookup"><span data-stu-id="23acf-640">msdyn_scheduleperformancename</span></span>          | <span data-ttu-id="23acf-641">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-641">no</span></span>             | <span data-ttu-id="23acf-642">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-642">no</span></span>           |
| <span data-ttu-id="23acf-643">msdyn_schedulevariance</span><span class="sxs-lookup"><span data-stu-id="23acf-643">msdyn_schedulevariance</span></span>                 | <span data-ttu-id="23acf-644">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-644">no</span></span>             | <span data-ttu-id="23acf-645">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-645">no</span></span>           |
| <span data-ttu-id="23acf-646">msdyn_taskearlieststart</span><span class="sxs-lookup"><span data-stu-id="23acf-646">msdyn_taskearlieststart</span></span>                | <span data-ttu-id="23acf-647">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-647">no</span></span>             | <span data-ttu-id="23acf-648">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-648">no</span></span>           |
| <span data-ttu-id="23acf-649">msdyn_teamsize</span><span class="sxs-lookup"><span data-stu-id="23acf-649">msdyn_teamsize</span></span>                         | <span data-ttu-id="23acf-650">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-650">no</span></span>             | <span data-ttu-id="23acf-651">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-651">no</span></span>           |
| <span data-ttu-id="23acf-652">msdyn_teamsize_date</span><span class="sxs-lookup"><span data-stu-id="23acf-652">msdyn_teamsize_date</span></span>                    | <span data-ttu-id="23acf-653">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-653">no</span></span>             | <span data-ttu-id="23acf-654">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-654">no</span></span>           |
| <span data-ttu-id="23acf-655">msdyn_teamsize_state</span><span class="sxs-lookup"><span data-stu-id="23acf-655">msdyn_teamsize_state</span></span>                   | <span data-ttu-id="23acf-656">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-656">no</span></span>             | <span data-ttu-id="23acf-657">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-657">no</span></span>           |
| <span data-ttu-id="23acf-658">msdyn_totalactualcost</span><span class="sxs-lookup"><span data-stu-id="23acf-658">msdyn_totalactualcost</span></span>                  | <span data-ttu-id="23acf-659">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-659">no</span></span>             | <span data-ttu-id="23acf-660">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-660">no</span></span>           |
| <span data-ttu-id="23acf-661">msdyn_totalactualcost_base</span><span class="sxs-lookup"><span data-stu-id="23acf-661">msdyn_totalactualcost_base</span></span>             | <span data-ttu-id="23acf-662">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-662">no</span></span>             | <span data-ttu-id="23acf-663">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-663">no</span></span>           |
| <span data-ttu-id="23acf-664">msdyn_totalplannedcost</span><span class="sxs-lookup"><span data-stu-id="23acf-664">msdyn_totalplannedcost</span></span>                 | <span data-ttu-id="23acf-665">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-665">no</span></span>             | <span data-ttu-id="23acf-666">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-666">no</span></span>           |
| <span data-ttu-id="23acf-667">msdyn_totalplannedcost_base</span><span class="sxs-lookup"><span data-stu-id="23acf-667">msdyn_totalplannedcost_base</span></span>            | <span data-ttu-id="23acf-668">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-668">no</span></span>             | <span data-ttu-id="23acf-669">नहीं</span><span class="sxs-lookup"><span data-stu-id="23acf-669">no</span></span>           |


## <a name="limitations-and-known-issues"></a><span data-ttu-id="23acf-670">सीमाएं और ज्ञात मुद्दे</span><span class="sxs-lookup"><span data-stu-id="23acf-670">Limitations and known issues</span></span>
<span data-ttu-id="23acf-671">निम्नलिखित सीमाओं और ज्ञात मुद्दों की एक लिस्ट है:</span><span class="sxs-lookup"><span data-stu-id="23acf-671">The following is a list of limitations and known issues:</span></span>

- <span data-ttu-id="23acf-672">प्रोजेक्ट शेड्यूल API का उपयोग केवल **Microsoft प्रोजेक्ट लाइसेंस वाले उपयोगकर्ता** के द्वारा किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-672">Project Schedule APIs can only be used by **Users with Microsoft Project License.**</span></span> <span data-ttu-id="23acf-673">उनका इनके द्वारा उपयोग नहीं किया जा सकता है:</span><span class="sxs-lookup"><span data-stu-id="23acf-673">They can't be used by:</span></span>
    - <span data-ttu-id="23acf-674">अनुप्रयोग उपयोगकर्ता</span><span class="sxs-lookup"><span data-stu-id="23acf-674">Application users</span></span>
    - <span data-ttu-id="23acf-675">सिस्टम उपयोगकर्ता</span><span class="sxs-lookup"><span data-stu-id="23acf-675">System users</span></span>
    - <span data-ttu-id="23acf-676">एकीकरण उपयोगकर्ता</span><span class="sxs-lookup"><span data-stu-id="23acf-676">Integration users</span></span>
    - <span data-ttu-id="23acf-677">अन्य उपयोगकर्ता जिनके पास आवश्यक लाइसेंस नहीं है</span><span class="sxs-lookup"><span data-stu-id="23acf-677">Other users that don't have the required license</span></span>
- <span data-ttu-id="23acf-678">प्रत्येक **OperationSet** में अधिकतम 100 संचालन हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="23acf-678">Each **OperationSet** can only have a maximum of 100 operations.</span></span>
- <span data-ttu-id="23acf-679">प्रत्येक उपयोगकर्ता के पास अधिकतम 10 खुला **OperationSets** हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="23acf-679">Each user can only have a maximum of 10 open **OperationSets**.</span></span>
- <span data-ttu-id="23acf-680">Project Operations वर्तमान में एक प्रोज़ेक्ट पर अधिकतम 500 कुल कार्यों का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="23acf-680">Project Operations currently supports a maximum of 500 total tasks on a project.</span></span>
- <span data-ttu-id="23acf-681">**OperationSet** विफलता की स्थिति और विफलता लॉग वर्तमान में उपलब्ध नहीं हैं.</span><span class="sxs-lookup"><span data-stu-id="23acf-681">**OperationSet** failure status and failure logs aren't currently available.</span></span>
- [<span data-ttu-id="23acf-682">प्रोजेक्ट और कार्यों पर लिमिट और बाउंड्री</span><span class="sxs-lookup"><span data-stu-id="23acf-682">Limits and boundaries on projects and tasks</span></span>](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a><span data-ttu-id="23acf-683">त्रुटि हैंडलिंग</span><span class="sxs-lookup"><span data-stu-id="23acf-683">Error handling</span></span>

   - <span data-ttu-id="23acf-684">ऑपरेशन सेट से उत्पन्न त्रुटियों की समीक्षा करने के लिए, **सेटिंग** \> **शेड्यूल इंटीग्रेशन** \> **ऑपरेशन सेट्स** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="23acf-684">To review errors generated from the Operation Sets, go to **Settings** \> **Schedule Integration** \> **Operations Sets**.</span></span>
   - <span data-ttu-id="23acf-685">प्रोजेक्ट शेड्यूल सेवा से उत्पन्न त्रुटियों की समीक्षा करने के लिए, **समायोजन** \> **अनुसूची एकीकरण** \> **PSS त्रुटि लॉग** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="23acf-685">To review errors generated from the Project schedule Service, go to **Settings** \> **Schedule Integration** \> **PSS Error Logs**.</span></span>

## <a name="sample-scenario"></a><span data-ttu-id="23acf-686">नमूना परिदृश्य</span><span class="sxs-lookup"><span data-stu-id="23acf-686">Sample scenario</span></span>

<span data-ttu-id="23acf-687">इस परिदृश्य में, आप एक प्रोज़ेक्ट, एक टीम के सदस्य, चार कार्य और दो संसाधन कार्य बनाएंगे.</span><span class="sxs-lookup"><span data-stu-id="23acf-687">In this scenario, you will create a project, a team member, four tasks, and two resource assignments.</span></span> <span data-ttu-id="23acf-688">इसके बाद, आप एक कार्य को अपडेट करेंगे, प्रोज़ेक्ट को अपडेट करेंगे, एक कार्य को हटा देंगे, एक संसाधन असाइनमेंट को हटा देंगे,और एक कार्य निर्भरता बनाएंगे.</span><span class="sxs-lookup"><span data-stu-id="23acf-688">Next, you will update one task, update the project, delete one task, delete one resource assignment, and create a task dependency.</span></span>

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

## <a name="additional-samples"></a><span data-ttu-id="23acf-689">अतिरिक्त नमूने</span><span class="sxs-lookup"><span data-stu-id="23acf-689">Additional samples</span></span>

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
