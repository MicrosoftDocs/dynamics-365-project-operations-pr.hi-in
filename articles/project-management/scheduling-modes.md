---
title: शेड्यूलिंग मोड
description: यह विषय शेड्यूलिंग मोड के बारे में जानकारी प्रदान करता है.
author: ruhercul
ms.date: 05/28/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 508ff1df8f7e31066712fab6f8871dfdb107a43b
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116709"
---
# <a name="scheduling-modes"></a><span data-ttu-id="cc169-103">शेड्यूलिंग मोड</span><span class="sxs-lookup"><span data-stu-id="cc169-103">Scheduling modes</span></span>

<span data-ttu-id="cc169-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="cc169-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="cc169-105">Dynamics 365 Project Operations संगठनों के लिए यह निर्धारित करने की क्षमता प्रदान करता है कि वे वर्क ब्रेकडाउन संरचना के भीतर कार्यों में मुख्य चर में परिवर्तन कैसे प्रबंधित करते हैं.</span><span class="sxs-lookup"><span data-stu-id="cc169-105">Dynamics 365 Project Operations provides the ability for organizations to define how they manage changes to key variables in tasks within the work breakdown structure.</span></span> <span data-ttu-id="cc169-106">संगठन की विशिष्ट आवश्यकताओं के आधार पर, प्रोजेक्ट प्रबंधक प्रोजेक्ट बनाते समय शेड्यूलिंग मोड में परिवर्तन कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="cc169-106">Based on the specific needs of the organization, Project Managers can make changes to the scheduling mode when a project is created.</span></span>

<span data-ttu-id="cc169-107">Project Operations में तीन शेड्यूलिंग मोड उपलब्ध हैं:</span><span class="sxs-lookup"><span data-stu-id="cc169-107">There are three scheduling modes available in Project Operations:</span></span>

  - <span data-ttu-id="cc169-108">निश्चित अवधि (यह डिफ़ॉल्ट मोड है)</span><span class="sxs-lookup"><span data-stu-id="cc169-108">Fixed duration (this is the default mode)</span></span>
  - <span data-ttu-id="cc169-109">निर्धारित प्रयास (*कार्य*)</span><span class="sxs-lookup"><span data-stu-id="cc169-109">Fixed effort (*Work*)</span></span>
  - <span data-ttu-id="cc169-110">निश्चित इकाइयाँ</span><span class="sxs-lookup"><span data-stu-id="cc169-110">Fixed units</span></span>

<span data-ttu-id="cc169-111">किसी विशिष्ट शेड्यूलिंग मोड की परिभाषा से प्रभावित मान निम्न सूत्र द्वारा निर्धारित किए जाते हैं:</span><span class="sxs-lookup"><span data-stu-id="cc169-111">The values impacted by the definition of a specific scheduling mode are determined by the following formula:</span></span>

  <span data-ttu-id="cc169-112">प्रयास = अवधि x इकाइयां</span><span class="sxs-lookup"><span data-stu-id="cc169-112">Effort  = Duration x Units</span></span>

<span data-ttu-id="cc169-113">जब आप किसी प्रोजेक्ट के शेड्यूलिंग मोड को निर्धारित करते हैं, तो आप इनमें से एक मान सेट कर रहे होते हैं, जिसे तब बदला नहीं जा सकता.</span><span class="sxs-lookup"><span data-stu-id="cc169-113">When you define a project’s scheduling mode, you are setting one of these values, which then can't be changed.</span></span> <span data-ttu-id="cc169-114">इस मान को एक स्थिर मान के रूप में रखने से उस मान पर प्राथमिकता बन जाती है, जो अन्य दो मानों को बदलने पर सिस्टम को इसे नहीं बदलने की सूचना देता है.</span><span class="sxs-lookup"><span data-stu-id="cc169-114">Holding this value as a constant places a priority on that value, which notifies the system not to change it when the other two values change.</span></span> <span data-ttu-id="cc169-115">निम्न तालिका एक विशिष्ट मोड के चयन के प्रभावों के बारे में जानकारी देती है.</span><span class="sxs-lookup"><span data-stu-id="cc169-115">The following table provides information about the impacts of selecting a specific mode.</span></span>

| <span data-ttu-id="cc169-116">**इस कार्य में**</span><span class="sxs-lookup"><span data-stu-id="cc169-116">**In this task**</span></span>             | <span data-ttu-id="cc169-117">**यदि आप इकाइयों को संशोधित करते हैं**</span><span class="sxs-lookup"><span data-stu-id="cc169-117">**If you revise units**</span></span>   | <span data-ttu-id="cc169-118">**यदि आप अवधि को संशोधित करते हैं**</span><span class="sxs-lookup"><span data-stu-id="cc169-118">**If you revise duration**</span></span> | <span data-ttu-id="cc169-119">**यदि आप प्रयास को संशोधित करते हैं**</span><span class="sxs-lookup"><span data-stu-id="cc169-119">**If you revise effort**</span></span>  |
|----------------------|---------------------------|----------------------------|---------------------------|
| <span data-ttu-id="cc169-120">निर्धारित इकाई कार्य</span><span class="sxs-lookup"><span data-stu-id="cc169-120">Fixed units task</span></span>     | <span data-ttu-id="cc169-121">अवधि पुनःपरिकलित है.</span><span class="sxs-lookup"><span data-stu-id="cc169-121">Duration is recalculated.</span></span> | <span data-ttu-id="cc169-122">प्रयास पुनःपरिकलित है.</span><span class="sxs-lookup"><span data-stu-id="cc169-122">Effort is recalculated.</span></span>    | <span data-ttu-id="cc169-123">अवधि पुनःपरिकलित है.</span><span class="sxs-lookup"><span data-stu-id="cc169-123">Duration is recalculated.</span></span> |
| <span data-ttu-id="cc169-124">निर्धारित प्रयास कार्य</span><span class="sxs-lookup"><span data-stu-id="cc169-124">Fixed effort task</span></span>    | <span data-ttu-id="cc169-125">अवधि पुनःपरिकलित है.</span><span class="sxs-lookup"><span data-stu-id="cc169-125">Duration is recalculated.</span></span> | <span data-ttu-id="cc169-126">इकाई पुनःपरिकलित है.</span><span class="sxs-lookup"><span data-stu-id="cc169-126">Units are recalculated.</span></span>    | <span data-ttu-id="cc169-127">अवधि पुनःपरिकलित है.</span><span class="sxs-lookup"><span data-stu-id="cc169-127">Duration is recalculated.</span></span> |
| <span data-ttu-id="cc169-128">निश्चित अवधि का कार्य</span><span class="sxs-lookup"><span data-stu-id="cc169-128">Fixed duration task</span></span>  | <span data-ttu-id="cc169-129">प्रयास पुनःपरिकलित है.</span><span class="sxs-lookup"><span data-stu-id="cc169-129">Effort is recalculated.</span></span>   | <span data-ttu-id="cc169-130">प्रयास पुनःपरिकलित है.</span><span class="sxs-lookup"><span data-stu-id="cc169-130">Effort is recalculated.</span></span>    | <span data-ttu-id="cc169-131">इकाई पुनःपरिकलित है.</span><span class="sxs-lookup"><span data-stu-id="cc169-131">Units are recalculated.</span></span>   |

<span data-ttu-id="cc169-132">किसी दिए गए मोड के आशयों के बारे में अधिक जानकारी के लिए, देखें [अधिक सटीक शेड्यूलिंग के लिए कार्य प्रकार बदलें](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span><span class="sxs-lookup"><span data-stu-id="cc169-132">For more information about the implications of a given mode, see [Change the task type for more accurate scheduling](https://support.microsoft.com/en-us/office/change-the-task-type-for-more-accurate-scheduling-b0b969ad-45bc-4e9e-8967-435587548a72).</span></span> <span data-ttu-id="cc169-133">विषय में, **प्रयास** के बजाय **कार्य** शब्द का उपयोग किया गया है.</span><span class="sxs-lookup"><span data-stu-id="cc169-133">In the topic, the term **Work** is used instead of **Effort**.</span></span>

## <a name="change-the-organizations-scheduling-mode"></a><span data-ttu-id="cc169-134">संगठन का शेड्यूलिंग मोड बदलें</span><span class="sxs-lookup"><span data-stu-id="cc169-134">Change the organization’s scheduling mode</span></span>

<span data-ttu-id="cc169-135">किसी संगठन के शेड्यूलिंग मोड को निर्धारित करने के लिए निम्नलिखित चरणों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="cc169-135">Complete the following steps to define the scheduling mode of an organization.</span></span>

1. <span data-ttu-id="cc169-136">**सेटिंग** \> **सामान्य** \> **पैरामीटर** पर जाएं, और फिर प्रोजेक्ट पैरामीटर का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="cc169-136">Go to **Settings** \> **General** \> **Parameters**, and then select the project parameter.</span></span> 
2. <span data-ttu-id="cc169-137">**प्रोजेक्ट पैरामीटर** पृष्ठ पर, संगठन के लिए डिफ़ॉल्ट शेड्यूलिंग मोड का चयन करें, और फिर एक नया प्रोजेक्ट बनाते समय प्रोजेक्ट मैनेजर की सेटिंग को ओवरराइड करने की क्षमता को परिभाषित करें.</span><span class="sxs-lookup"><span data-stu-id="cc169-137">On the **Project Parameters** page, select the default scheduling mode for the organization, and then define ability for the Project manager to override the setting when creating a new project.</span></span>

## <a name="change-the-scheduling-mode-setting-on-a-project"></a><span data-ttu-id="cc169-138">किसी प्रोजेक्ट पर शेड्यूलिंग मोड सेटिंग बदलें</span><span class="sxs-lookup"><span data-stu-id="cc169-138">Change the scheduling mode setting on a project</span></span>

<span data-ttu-id="cc169-139">यदि कोई संगठन प्रोजेक्ट प्रबंधक को डिफ़ॉल्ट शेड्यूलिंग मोड को ओवरराइड करने की अनुमति देता है, तो प्रोजेक्ट मैनेजर एक नया प्रोजेक्ट बनाते समय उसमें परिवर्तन कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="cc169-139">If an organization allows the Project manager to override the default scheduling mode, the Project manager can make that change when they create a new project.</span></span> <span data-ttu-id="cc169-140">हालाँकि, प्रोजेक्ट सहेजे जाने के बाद, शेड्यूलिंग मोड बदला नहीं जा सकता.</span><span class="sxs-lookup"><span data-stu-id="cc169-140">However, after the project has been saved, the scheduling mode can't be changed.</span></span>

## <a name="copied-projects"></a><span data-ttu-id="cc169-141">कॉपी किए गए प्रोजेक्ट</span><span class="sxs-lookup"><span data-stu-id="cc169-141">Copied projects</span></span>

<span data-ttu-id="cc169-142">क्योंकि एक प्रोजेक्ट तब बनाया जाता है जब कॉपी प्रोजेक्ट एक्शन लिया जाता है, प्रोजेक्ट मैनेजर शेड्यूलिंग मोड सेट नहीं कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="cc169-142">Because a project is created when the copy project action is taken, the Project manager can't set the scheduling mode.</span></span> <span data-ttu-id="cc169-143">गंतव्य प्रोजेक्ट हमेशा संगठनात्मक स्तर पर निर्धारित मोड के लिए डिफ़ॉल्ट होगी.</span><span class="sxs-lookup"><span data-stu-id="cc169-143">The destination project will always default to the mode defined at the organizational level.</span></span>

## <a name="copied-tasks"></a><span data-ttu-id="cc169-144">कॉपी किए गए कार्य</span><span class="sxs-lookup"><span data-stu-id="cc169-144">Copied tasks</span></span>

<span data-ttu-id="cc169-145">जब किसी कार्य को एक प्रोजेक्ट से दूसरे में कॉपी किया जाता है, तो कार्य गंतव्य प्रोजेक्ट का शेड्यूलिंग मोड इनहेरिट करता है.</span><span class="sxs-lookup"><span data-stu-id="cc169-145">When a task is copied from one project to another, the task inherits the scheduling mode of the destination project.</span></span>
