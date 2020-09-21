---
title: प्रोजेक्ट प्रगति और लागत उपभोग
description: इस विषय में प्रोजेक्ट की प्रगति और लागत की खपत का पता लगाने के बारे में जानकारी दी गई है।
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 0d742164-5469-421d-8917-63160a81f651
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 8aa5814938129f30885d8161a7c86197ab013364
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3752074"
---
# <a name="project-progress-and-cost-consumption"></a><span data-ttu-id="d5d87-103">प्रोजेक्ट प्रगति और लागत उपभोग</span><span class="sxs-lookup"><span data-stu-id="d5d87-103">Project progress and cost consumption</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="d5d87-104">शेड्यूल के समक्ष प्रगति का पता लगाने की ज़रूरत हर उद्योग की अलग-अलग होती है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-104">The need to track progress against a schedule varies by industry.</span></span> <span data-ttu-id="d5d87-105">कुछ उद्योग सूक्ष्म स्तर पर ट्रैक करते हैं जबकि कुछ उद्योगों में व्यापक स्तर पर ट्रैक किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-105">Some industries track at a granular level, whereas other industries track at a higher level.</span></span> <span data-ttu-id="d5d87-106">इस विषय में बताया गया है कि अपने संगठन की ज़रूरतों को पूरा करने के लिए शेड्यूल कैसे किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-106">This topic shows how to schedule in order to meet your organization's requirements.</span></span>

## <a name="effort-tracking-view"></a><span data-ttu-id="d5d87-107">प्रयास ट्रैकिंग दृश्य</span><span class="sxs-lookup"><span data-stu-id="d5d87-107">Effort tracking view</span></span>

<span data-ttu-id="d5d87-108">**प्रयास ट्रैकिंग** व्यू शेड्यूल में टास्क की प्रगति का पता लगाता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-108">The **Effort tracking** view tracks the progress of tasks in the schedule.</span></span> <span data-ttu-id="d5d87-109">यह टास्क पर किए गए वास्तविक प्रयास घंटों की तुलना उस टास्क के योजित प्रयास घंटों से करता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-109">It compares the actual effort hours that have been spent on a task to the planned effort hours for that task.</span></span> <span data-ttu-id="d5d87-110">PSA में ट्रैकिंग मैट्रिक्स का परिकलन करने के लिए इन फार्मूलों का प्रयोग किया जाता है:</span><span class="sxs-lookup"><span data-stu-id="d5d87-110">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="d5d87-111">प्रगति का प्रतिशत = अब तक किए गए वास्तविक प्रयास ÷ टास्क के लिए योजित प्रयास</span><span class="sxs-lookup"><span data-stu-id="d5d87-111">Progress percentage = Actual effort spent to date ÷ Planned effort for the task</span></span> 
- <span data-ttu-id="d5d87-112">पूरा करने का अनुमान (ETC) = नियोजित प्रयास - अब तक किए गए वास्तविक प्रयास</span><span class="sxs-lookup"><span data-stu-id="d5d87-112">Estimate to complete (ETC) = Planned effort – Actual effort spent to date</span></span> 
- <span data-ttu-id="d5d87-113">समापन का अनुमान (EAC) = शेष प्रयास + अब तक किए गए वास्तविक प्रयास</span><span class="sxs-lookup"><span data-stu-id="d5d87-113">Estimate at complete (EAC) = Remaining effort + Actual effort spent to date</span></span> 
- <span data-ttu-id="d5d87-114">अनुमानित प्रयास भिन्नता = योजित प्रयास – EAC</span><span class="sxs-lookup"><span data-stu-id="d5d87-114">Projected effort variance = Planned effort – EAC</span></span>

<span data-ttu-id="d5d87-115">PSA टास्क पर प्रयास भिन्नता का अनुमान दिखाता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-115">PSA shows a projection of the effort variance on the task.</span></span> <span data-ttu-id="d5d87-116">यदि EAC योजित प्रयास से अधिक है तो अनुमान लगाया जाता है कि टास्क को पूरा करने में मूल रूप से योजित समय से अधिक समय लगेगा।</span><span class="sxs-lookup"><span data-stu-id="d5d87-116">If the EAC is more than the planned effort, the task is projected to take more time than was originally planned.</span></span> <span data-ttu-id="d5d87-117">इसलिए, यह शेड्यूल से पीछे है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-117">Therefore, it's behind schedule.</span></span> <span data-ttu-id="d5d87-118">यदि EAC योजित प्रयास से कम है तो अनुमान लगाया जाता है कि टास्क पूरा करने में मूल रूप से योजित समय से कम समय लगेगा।</span><span class="sxs-lookup"><span data-stu-id="d5d87-118">If the EAC is less than the planned effort, the task is projected to take less time than was originally planned.</span></span> <span data-ttu-id="d5d87-119">इसलिए, यह शेड्यूल से आगे है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-119">Therefore, it's ahead of schedule.</span></span>

## <a name="re-projecting-effort"></a><span data-ttu-id="d5d87-120">पुन: प्रोजेक्ट के प्रयास</span><span class="sxs-lookup"><span data-stu-id="d5d87-120">Re-projecting effort</span></span>

<span data-ttu-id="d5d87-121">टास्क के मूल अनुमानों को संशोधित करना प्रोजेक्ट मैनेजर के लिए आम बात है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-121">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="d5d87-122">प्रोजेक्ट की चालू अवस्था के बारे में, प्रोजेक्ट का दोबारा अनुमान करना प्राक्कलनों को लेकर प्रोजेक्ट मैनेजर के विचार होते हैं।</span><span class="sxs-lookup"><span data-stu-id="d5d87-122">Project re-projections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="d5d87-123">बहरहाल, हम इस बात की सिफारिश नहीं करते कि प्रोजेक्ट मैनेजर बेसलाइन अंकों को बदलें क्योंकि प्रोजेक्ट की बेसलाइन प्रोजेक्ट के शेड्यूल और लागत के प्राक्कलनों की सच्चाई के स्थापित स्रोत होती है और लागत अनुमान और प्रोजेक्ट के सभी भागीदार उस पर सहमत होते हैं।</span><span class="sxs-lookup"><span data-stu-id="d5d87-123">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="d5d87-124">ऐसे दो तरीके हैं जिसमें परियोजना मैनेजर टास्क के प्रयासों का दोबारा अनुमान कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="d5d87-124">There are two ways that a project manager can re-project effort on tasks:</span></span>

- <span data-ttu-id="d5d87-125">टास्क पर वास्तविक शेष प्रयास के एक नए अनुमान के साथ डिफ़ॉल्ट ETC को ओवरराइड करें।</span><span class="sxs-lookup"><span data-stu-id="d5d87-125">Override the default ETC with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="d5d87-126">टास्क पर सही प्रगति के एक नए अनुमान के साथ डिफ़ॉल्ट प्रगति प्रतिशत को ओवरराइड करें।</span><span class="sxs-lookup"><span data-stu-id="d5d87-126">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="d5d87-127">इनमें से प्रत्येक तरीके में टास्क के ETC, EAC और प्रगति के प्रतिशत और टास्क पर अनुमानित प्रयास भिन्नता का दोबारा परिकलन करना होता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-127">Each of these approaches cause a recalculation of the task's ETC, EAC, and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="d5d87-128">समरी टास्क पर EAC, ETC और प्रगति के प्रतिशत का भी दोबारा परिकलन किया जाता है और प्रयास की भिन्नता का नया अनुमान किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-128">The EAC, ETC, and progress percentage on the summary tasks are also recalculated, and produce a new projection of effort variance.</span></span>

## <a name="re-projection-of-effort-on-summary-tasks"></a><span data-ttu-id="d5d87-129">सारांश टास्क पर प्रयास का दोबारा अनुमान</span><span class="sxs-lookup"><span data-stu-id="d5d87-129">Re-projection of effort on summary tasks</span></span>

<span data-ttu-id="d5d87-130">सारांश टास्क या कंटेनर टास्क के प्रयास का दोबारा अनुमान किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-130">Effort on summary tasks or container tasks can be re-projected.</span></span> <span data-ttu-id="d5d87-131">इस बात से संबंध न रखते हुए कि यूज़र शेष प्रयास या समरी टास्क पर प्रगति के प्रतिशत का इस्तेमाल करते हुए दोबारा अनुमान करता है या नहीं, निम्नलिखित परिकलन करना होगा:</span><span class="sxs-lookup"><span data-stu-id="d5d87-131">Regardless of whether the user re-projects by using the remaining effort or the progress percentage on the summary tasks, the following set of calculations begins:</span></span>

- <span data-ttu-id="d5d87-132">EAC, ETC और टास्क पर प्रगति के प्रतिशत का परिकलन किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-132">The EAC, ETC, and progress percentage on the task are calculated.</span></span>
- <span data-ttu-id="d5d87-133">नए EAC को छोटे टास्क में उसी अनुपात में नीचे वितरित किया जाता है जिस अनुपात में टास्क में मूल EAC था।</span><span class="sxs-lookup"><span data-stu-id="d5d87-133">The new EAC is distributed down to the child tasks in the same proportion as the original EAC was on the task.</span></span>
- <span data-ttu-id="d5d87-134">प्रत्येक वैयक्तिक टास्क के नए EAC से लेकर लीफ नोड टास्क तक का परिकलन किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-134">The new EAC on each of the individualt tasks down to the leaf node tasks is calculated.</span></span> 
- <span data-ttu-id="d5d87-135">लीफ नोड के नीचे प्रभावित छोटे टास्क में उनका ETC होते हैं और EAC के मूल्य के आधार पर प्रगति के प्रतिशत का दोबारा परिकलन किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-135">The affected child tasks down to the leaf nodes have their ETC and progress percentage recalculated based on the EAC value.</span></span> <span data-ttu-id="d5d87-136">इसके कारण टास्क के प्रयास भिन्नता का नया अनुमान करना होता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-136">This results in a new projection for the effort variance of the task.</span></span> 
- <span data-ttu-id="d5d87-137">समरी टास्क के EAC का रूट नोड तक दोबारा परिकलन किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-137">The EACs of the summary tasks all the way to the root node are recalculated.</span></span>

### <a name="cost-tracking-view"></a><span data-ttu-id="d5d87-138">लागत ट्रैकिंग दृश्य</span><span class="sxs-lookup"><span data-stu-id="d5d87-138">Cost tracking view</span></span> 

<span data-ttu-id="d5d87-139">**लागत ट्रैकिंग** व्यू टास्क पर खर्च की गई वास्तविक लागत और टास्क पर योजित लागत की तुलना करता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-139">The **Cost tracking** view compares the actual cost that was spent on a task to the planned cost on a task.</span></span> 

> [!NOTE]
> <span data-ttu-id="d5d87-140">यह दृश्य केवल श्रम लागत दर्शाता है और इसमें खर्च के अनुमानों की लागतें शामिल नहीं होती।</span><span class="sxs-lookup"><span data-stu-id="d5d87-140">This view shows only labor costs and doesn’t include costs from the expense estimates.</span></span> 

<span data-ttu-id="d5d87-141">PSA में ट्रैकिंग मैट्रिक्स का परिकलन करने के लिए इन फार्मूलों का प्रयोग किया जाता है:</span><span class="sxs-lookup"><span data-stu-id="d5d87-141">PSA uses the following formulas to calculate the tracking metrics:</span></span>

- <span data-ttu-id="d5d87-142">खपत लागत का प्रतिशत = अब तक खर्च की गई वास्तविक लागत ÷ टास्क के लिए योजित लागत</span><span class="sxs-lookup"><span data-stu-id="d5d87-142">Percentage of cost consumed = Actual cost spent to date ÷ Planned cost for the task</span></span>
- <span data-ttu-id="d5d87-143">पूरा करने की लागत (CTC) = योजित लागत - तिथि तक खर्च की गई वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="d5d87-143">Cost to complete (CTC) = Planned cost – Actual cost spent to date</span></span>
- <span data-ttu-id="d5d87-144">EAC = CTC + अब तक खर्च की गई वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="d5d87-144">EAC = CTC + Actual cost spent to date</span></span>
- <span data-ttu-id="d5d87-145">अनुमानित लागत भिन्नता = योजित लागत – EAC</span><span class="sxs-lookup"><span data-stu-id="d5d87-145">Projected cost variance = Planned cost – EAC</span></span>

<span data-ttu-id="d5d87-146">लागत भिन्नता का अनुमान टास्क पर दिखाया जाता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-146">A projection of the cost variance is shown on the task.</span></span> <span data-ttu-id="d5d87-147">यदि EAC योजित लागत से अधिक होता है तो टास्क के बारे में यह अनुमान लगाया जाता है कि उसकी लागत मूल रूप से योजित लागत से अधिक होगी।</span><span class="sxs-lookup"><span data-stu-id="d5d87-147">If the EAC is more than the planned cost, the task is projected to cost more than was originally planned.</span></span> <span data-ttu-id="d5d87-148">इसलिए, यह बजट से अधिक होगा।</span><span class="sxs-lookup"><span data-stu-id="d5d87-148">Therefore, it's trending over budget.</span></span> <span data-ttu-id="d5d87-149">यदि EAC योजित लागत से कम है तो टास्क के बारे में यह अनुमान लगाया जाता है कि उसकी लागत मूल रूप से योजित लागत से कम होगी।</span><span class="sxs-lookup"><span data-stu-id="d5d87-149">If the EAC is less than the planned cost, the task is projected to cost less than was originally planned.</span></span> <span data-ttu-id="d5d87-150">इसलिए, यह बजट से कम होगा।</span><span class="sxs-lookup"><span data-stu-id="d5d87-150">Therefore, it's trending under budget.</span></span>

## <a name="project-managers-re-projection-of-cost"></a><span data-ttu-id="d5d87-151">प्रोजेक्ट मैनेजर द्वारा लागत का दोबारा अनुमान लगाना</span><span class="sxs-lookup"><span data-stu-id="d5d87-151">Project manager’s re-projection of cost</span></span>

<span data-ttu-id="d5d87-152">जब प्रयास का दोबारा अनुमान लगाया जाता है, तो CTC, EAC, आई लागत का प्रतिशत और अनुमानित लागत भिन्नता सभी का **लागत ट्रैकिंग** दृश्य में दोबारा परिकलन किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-152">When effort is re-projected, the CTC, EAC, percentage of cost consumed, and projected cost variance are all recalculated in the **Cost tracking** view.</span></span>

## <a name="project-status-summary"></a><span data-ttu-id="d5d87-153">प्रोजेक्ट स्थिति सारांश</span><span class="sxs-lookup"><span data-stu-id="d5d87-153">Project status summary</span></span>

<span data-ttu-id="d5d87-154">**प्रयास ट्रैकिंग** और **लागत ट्रैकिंग** दृश्य में ट्रैकिंग डेटा प्रोजेक्ट रूट नोड में प्रगति और आई लागत, समरी टास्क और लीफ नोड टास्क स्तर दिखाता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-154">Tracking data in the **Effort tracking** and **Cost tracking** views shows the progress and cost consumption at the project root node, summary tasks, and leaf node tasks levels.</span></span> <span data-ttu-id="d5d87-155">**प्रोजेक्ट एंटिटी** पेज पर **स्थिति** खंड प्रोजेक्ट-स्तर के स्टेटस का समरी दिखाता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-155">The **Status** section on the **Project entity** page shows a summary of project-level status.</span></span>

## <a name="status-summary-fields"></a><span data-ttu-id="d5d87-156">स्थिति सारांश फ़ील्ड</span><span class="sxs-lookup"><span data-stu-id="d5d87-156">Status summary fields</span></span>

<span data-ttu-id="d5d87-157">**संपूर्ण परियोजना स्थिति** फील्ड एक एडिट करने योग्य फील्ड होता है जो प्रोजेक्ट का संपूर्ण स्टेटस दिखाता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-157">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="d5d87-158">इसमें बढ़ते जोखिम को दर्शाने के लिए हरे, पीले और लाल जैसे कलर-कोडिंग का इस्तेमाल किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-158">It uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> <span data-ttu-id="d5d87-159">**टिप्पणियाँ** फील्ड से प्रोजेक्ट मैनेजर स्टेटस के बारे में विशेष टिप्पणियां दर्ज कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="d5d87-159">The **Comments** field lets the project manager enter specific comments about the status.</span></span> <span data-ttu-id="d5d87-160">फील्ड **पर स्थिति अद्यतन** एडिट नहीं किया जा सकता और इसका वैल्यू टाइमस्टैम्प होता है जो स्टेटस के अंतिम बार अपडेट करने को बताता है।</span><span class="sxs-lookup"><span data-stu-id="d5d87-160">The **Status updated on** field is not editable and the value is a timestamp that indicates when the status was last updated.</span></span>

<span data-ttu-id="d5d87-161">**शेड्यूल प्रदर्शन** और **लागत प्रदर्शन** फील्ड ट्रैकिंग की तारीख से सेट किए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="d5d87-161">The **Schedule performance** and **Cost performance** fields are set from the tracking date.</span></span> <span data-ttu-id="d5d87-162">जब **प्रयास ट्रैकिंग** व्यू में रूट नोड के लिए शेड्यूल और लागत भिन्नता पोज़िटिव होते हैं तो आप इन फील्ड को **Ahead** में सेट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="d5d87-162">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, you can set these fields to **Ahead**.</span></span> <span data-ttu-id="d5d87-163">जब रूट नोड के लिए शेड्यूल और लागत भिन्नता निगेटिव होते हैं तो आप इन फील्ड को **पीछे** में सेट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="d5d87-163">When the schedule and cost variance for the root node are negative, you can set them to **Behind**.</span></span>
