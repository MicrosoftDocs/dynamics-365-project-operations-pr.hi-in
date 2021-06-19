---
title: परियोजना प्रगति और लागत उपभोग
description: यह विषय प्रोजेक्ट की प्रगति और लागत उपभोग का पता लगाने के बारे में जानकारी प्रदान करता है.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 08/21/2020
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
ms.openlocfilehash: 4fe6adf1a16c1eafc5e37dbd8878dda44cbca230
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6009033"
---
# <a name="project-progress-and-cost-consumption"></a><span data-ttu-id="73836-103">परियोजना प्रगति और लागत उपभोग</span><span class="sxs-lookup"><span data-stu-id="73836-103">Project progress and cost consumption</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="73836-104">शेड्यूल के समक्ष प्रगति का पता लगाने की ज़रूरत हर उद्योग की अलग-अलग होती है।</span><span class="sxs-lookup"><span data-stu-id="73836-104">The need to track progress against a schedule varies by industry.</span></span> <span data-ttu-id="73836-105">कुछ उद्योग सूक्ष्म स्तर पर ट्रैक करते हैं जबकि कुछ उद्योगों में व्यापक स्तर पर ट्रैक किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="73836-105">Some industries track at a granular level, whereas other industries track at a higher level.</span></span> <span data-ttu-id="73836-106">इस विषय में बताया गया है कि अपने संगठन की ज़रूरतों को पूरा करने के लिए शेड्यूल कैसे किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="73836-106">This topic shows how to schedule in order to meet your organization's requirements.</span></span>

## <a name="effort-tracking-view"></a><span data-ttu-id="73836-107">प्रयास ट्रैकिंग दृश्य</span><span class="sxs-lookup"><span data-stu-id="73836-107">Effort tracking view</span></span>

<span data-ttu-id="73836-108">**प्रयास ट्रैकिंग** व्यू शेड्यूल में टास्क की प्रगति का पता लगाता है।</span><span class="sxs-lookup"><span data-stu-id="73836-108">The **Effort tracking** view tracks the progress of tasks in the schedule.</span></span> <span data-ttu-id="73836-109">यह किसी कार्य पर व्‍यतीत किए गए वास्‍तविक कार्य घंटों की तुलना उस कार्य पर नियोजित प्रयास घंटों से करता है.</span><span class="sxs-lookup"><span data-stu-id="73836-109">It compares the actual effort hours spent on a task to the task's planned effort hours.</span></span> <span data-ttu-id="73836-110">Project Service Automation में ट्रैकिंग मैट्रिक्स का परिकलन करने के लिए इन सूत्रों का उपयोग किया जाता है:</span><span class="sxs-lookup"><span data-stu-id="73836-110">Project Service Automation uses the following formulas to calculate the tracking metrics:</span></span>

<span data-ttu-id="73836-111">प्रारंभ में कार्य निर्माण पर: पूर्ण होने पर नियोजित लागत को अनुमानित लागत पर सेट किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="73836-111">Initially on the task creation: Planned cost will be set to the Estimated cost at complete.</span></span> <span data-ttu-id="73836-112">कार्य पर वास्तविक को रिकॉर्ड कर लेने के बाद, प्रयास के लिए ट्रैकिंग दृश्य पर निम्नलिखित गणना की जाएगी</span><span class="sxs-lookup"><span data-stu-id="73836-112">Once Actuals are recorded on the task, the following will be calculation on the Tracking view for Effort</span></span>

- <span data-ttu-id="73836-113">प्रगति प्रतिशत = अब तक किए गए वास्तविक प्रयास ÷ पूर्णता पर अनुमान (EAC)</span><span class="sxs-lookup"><span data-stu-id="73836-113">Progress percentage = Actual effort spent to date ÷ Estimate at complete (EAC)</span></span> 
- <span data-ttu-id="73836-114">पूर्णता का अनुमान (ETC) = पूर्णता पर अनुमान (EAC) - अब तक किए गए वास्तविक प्रयास</span><span class="sxs-lookup"><span data-stu-id="73836-114">Estimate to complete (ETC) = Estimate at complete (EAC)  – Actual effort spent to date</span></span> 
- <span data-ttu-id="73836-115">EAC = शेष प्रयास + अब तक किए गए वास्तविक प्रयास</span><span class="sxs-lookup"><span data-stu-id="73836-115">EAC = Remaining effort + Actual effort spent to date</span></span> 
- <span data-ttu-id="73836-116">अनुमानित प्रयास भिन्नता = योजित प्रयास – EAC</span><span class="sxs-lookup"><span data-stu-id="73836-116">Projected effort variance = Planned effort – EAC</span></span>

<span data-ttu-id="73836-117">Project Service Automation कार्य पर प्रयास भिन्नता का अनुमान दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="73836-117">Project Service Automation shows a projection of the effort variance on the task.</span></span> <span data-ttu-id="73836-118">यदि EAC योजित प्रयास से अधिक है तो अनुमान लगाया जाता है कि टास्क को पूरा करने में मूल रूप से योजित समय से अधिक समय लगेगा।</span><span class="sxs-lookup"><span data-stu-id="73836-118">If the EAC is more than the planned effort, the task is projected to take more time than was originally planned.</span></span> <span data-ttu-id="73836-119">इसलिए, यह शेड्यूल से पीछे है।</span><span class="sxs-lookup"><span data-stu-id="73836-119">Therefore, it's behind schedule.</span></span> <span data-ttu-id="73836-120">यदि EAC योजित प्रयास से कम है तो अनुमान लगाया जाता है कि टास्क पूरा करने में मूल रूप से योजित समय से कम समय लगेगा।</span><span class="sxs-lookup"><span data-stu-id="73836-120">If the EAC is less than the planned effort, the task is projected to take less time than was originally planned.</span></span> <span data-ttu-id="73836-121">इसलिए, यह शेड्यूल से आगे है।</span><span class="sxs-lookup"><span data-stu-id="73836-121">Therefore, it's ahead of schedule.</span></span>

## <a name="reprojecting-effort"></a><span data-ttu-id="73836-122">दोबारा अनुमान लगाने के प्रयास</span><span class="sxs-lookup"><span data-stu-id="73836-122">Reprojecting effort</span></span>

<span data-ttu-id="73836-123">टास्क के मूल अनुमानों को संशोधित करना प्रोजेक्ट मैनेजर के लिए आम बात है।</span><span class="sxs-lookup"><span data-stu-id="73836-123">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="73836-124">परियोजना की चालू अवस्था के बारे में, परियोजना का दोबारा अनुमान लगाना, दृष्टिकोण को लेकर परियोजना प्रबंधक के विचार होते हैं.</span><span class="sxs-lookup"><span data-stu-id="73836-124">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="73836-125">बहरहाल, हम इस बात की सिफारिश नहीं करते कि प्रोजेक्ट मैनेजर बेसलाइन अंकों को बदलें क्योंकि प्रोजेक्ट की बेसलाइन प्रोजेक्ट के शेड्यूल और लागत के प्राक्कलनों की सच्चाई के स्थापित स्रोत होती है और लागत अनुमान और प्रोजेक्ट के सभी भागीदार उस पर सहमत होते हैं।</span><span class="sxs-lookup"><span data-stu-id="73836-125">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="73836-126">ऐसे दो तरीके हैं जिससे परियोजना प्रबंधक कार्यों के प्रयासों का दोबारा अनुमान लगा सकता है:</span><span class="sxs-lookup"><span data-stu-id="73836-126">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="73836-127">टास्क पर वास्तविक शेष प्रयास के एक नए अनुमान के साथ डिफ़ॉल्ट ETC को ओवरराइड करें।</span><span class="sxs-lookup"><span data-stu-id="73836-127">Override the default ETC with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="73836-128">टास्क पर सही प्रगति के एक नए अनुमान के साथ डिफ़ॉल्ट प्रगति प्रतिशत को ओवरराइड करें।</span><span class="sxs-lookup"><span data-stu-id="73836-128">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="73836-129">इनमें से प्रत्येक तरीके में टास्क के ETC, EAC और प्रगति के प्रतिशत और टास्क पर अनुमानित प्रयास भिन्नता का दोबारा परिकलन करना होता है।</span><span class="sxs-lookup"><span data-stu-id="73836-129">Each of these approaches cause a recalculation of the task's ETC, EAC, and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="73836-130">समरी टास्क पर EAC, ETC और प्रगति के प्रतिशत का भी दोबारा परिकलन किया जाता है और प्रयास की भिन्नता का नया अनुमान किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="73836-130">The EAC, ETC, and progress percentage on the summary tasks are also recalculated, and produce a new projection of effort variance.</span></span>

## <a name="reprojection-of-effort-on-summary-tasks"></a><span data-ttu-id="73836-131">सारांश कार्य पर प्रयास का दोबारा अनुमान</span><span class="sxs-lookup"><span data-stu-id="73836-131">Reprojection of effort on summary tasks</span></span>

<span data-ttu-id="73836-132">सारांश कार्यों या कंटेनर कार्यों के प्रयास का दोबारा अनुमान लगाया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="73836-132">Effort on summary tasks or container tasks can be reprojected.</span></span> <span data-ttu-id="73836-133">इस बात से संबंध न रखते हुए कि उपयोगकर्ता शेष प्रयास या सारांशित कार्यों पर प्रगति के प्रतिशत का इस्तेमाल करते हुए दोबारा अनुमान लगाता है या नहीं, परिकलन का निम्न सेट प्रारंभ होता है:</span><span class="sxs-lookup"><span data-stu-id="73836-133">Regardless of whether the user reprojects by using the remaining effort or the progress percentage on the summary tasks, the following set of calculations begins:</span></span>

- <span data-ttu-id="73836-134">EAC, ETC और टास्क पर प्रगति के प्रतिशत का परिकलन किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="73836-134">The EAC, ETC, and progress percentage on the task are calculated.</span></span>
- <span data-ttu-id="73836-135">नए EAC को छोटे टास्क में उसी अनुपात में नीचे वितरित किया जाता है जिस अनुपात में टास्क में मूल EAC था।</span><span class="sxs-lookup"><span data-stu-id="73836-135">The new EAC is distributed down to the child tasks in the same proportion as the original EAC was on the task.</span></span>
- <span data-ttu-id="73836-136">प्रत्येक वैयक्तिक कार्यों के नए EAC से लेकर लीफ नोड कार्यों तक का परिकलन किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="73836-136">The new EAC on each of the individual tasks down to the leaf node tasks is calculated.</span></span> 
- <span data-ttu-id="73836-137">लीफ नोड के नीचे प्रभावित छोटे टास्क में उनका ETC होते हैं और EAC के मूल्य के आधार पर प्रगति के प्रतिशत का दोबारा परिकलन किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="73836-137">The affected child tasks down to the leaf nodes have their ETC and progress percentage recalculated based on the EAC value.</span></span> <span data-ttu-id="73836-138">इसके कारण टास्क के प्रयास भिन्नता का नया अनुमान करना होता है।</span><span class="sxs-lookup"><span data-stu-id="73836-138">This results in a new projection for the effort variance of the task.</span></span> 
- <span data-ttu-id="73836-139">समरी टास्क के EAC का रूट नोड तक दोबारा परिकलन किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="73836-139">The EACs of the summary tasks all the way to the root node are recalculated.</span></span>

### <a name="cost-tracking-view"></a><span data-ttu-id="73836-140">लागत ट्रैकिंग दृश्य</span><span class="sxs-lookup"><span data-stu-id="73836-140">Cost tracking view</span></span> 

<span data-ttu-id="73836-141">**लागत ट्रैकिंग** दृश्य कार्य पर खर्च की गई वास्तविक लागत और कार्य पर नियोजित लागत की तुलना करता है.</span><span class="sxs-lookup"><span data-stu-id="73836-141">The **Cost tracking** view compares the actual cost that was spent on a task to the planned cost.</span></span> 

> [!NOTE]
> <span data-ttu-id="73836-142">यह दृश्य केवल श्रम लागत दर्शाता है और इसमें खर्च के अनुमानों की लागतें शामिल नहीं होती।</span><span class="sxs-lookup"><span data-stu-id="73836-142">This view shows only labor costs and doesn’t include costs from the expense estimates.</span></span> 

<span data-ttu-id="73836-143">Project Service Automation में ट्रैकिंग मैट्रिक्स का परिकलन करने के लिए इन सूत्रों का उपयोग किया जाता है:</span><span class="sxs-lookup"><span data-stu-id="73836-143">Project Service Automation uses the following formulas to calculate the tracking metrics:</span></span>

<span data-ttu-id="73836-144">जब कोई कार्य बनाया जाता है, तो नियोजित लागत पूर्णता पर अनुमानित लागत के बराबर होती है.</span><span class="sxs-lookup"><span data-stu-id="73836-144">When a task is created, the planned cost is equal to the estimated cost at complete.</span></span> <span data-ttu-id="73836-145">कार्य पर वास्तविक को रिकॉर्ड कर लेने के बाद, लागत के लिए **ट्रैकिंग** दृश्य पर निम्नलिखित की गणना की जाती है:</span><span class="sxs-lookup"><span data-stu-id="73836-145">After actuals are recorded on the task, the following is calculated on the **Tracking** view for cost:</span></span>

 - <span data-ttu-id="73836-146">खपत लागत का प्रतिशत = अब तक खर्च की गई वास्तविक लागत ÷ कार्य के लिए पूर्णता पर अनुमानित लागत</span><span class="sxs-lookup"><span data-stu-id="73836-146">Percentage of cost consumed = Actual cost spent to date ÷ Estimated cost at complete for the task</span></span>
 - <span data-ttu-id="73836-147">पूर्णता की लागत (CTC) = पूर्णता पर अनुमानित लागत - अब तक खर्च की गई वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="73836-147">Cost to complete (CTC) = Estimated cost at complete – Actual cost spent to date</span></span>
 - <span data-ttu-id="73836-148">पूर्णता पर अनुमानित लागत = (CTC) + अब तक खर्च की गई वास्तविक लागत</span><span class="sxs-lookup"><span data-stu-id="73836-148">Estimated cost at complete = CTC + Actual cost spent to date</span></span>
 - <span data-ttu-id="73836-149">अनुमानित लागत भिन्नता = नियोजित लागत - पूर्णता पर अनुमानित लागत</span><span class="sxs-lookup"><span data-stu-id="73836-149">Projected cost variance = Planned cost – Estimated cost at complete</span></span>

<span data-ttu-id="73836-150">लागत भिन्नता का अनुमान टास्क पर दिखाया जाता है।</span><span class="sxs-lookup"><span data-stu-id="73836-150">A projection of the cost variance is shown on the task.</span></span> <span data-ttu-id="73836-151">यदि पूर्णता पर अनुमानित लागत नियोजित लागत से अधिक होती है, तो कार्य के बारे में यह अनुमान लगाया जाता है कि उसकी लागत मूल रूप से नियोजित लागत से अधिक होगी.</span><span class="sxs-lookup"><span data-stu-id="73836-151">If the estimated cost at complete is more than the planned cost, the task is projected to cost more than was originally planned.</span></span> <span data-ttu-id="73836-152">इसलिए, यह बजट से अधिक होगा।</span><span class="sxs-lookup"><span data-stu-id="73836-152">Therefore, it's trending over budget.</span></span> <span data-ttu-id="73836-153">यदि पूर्णता पर अनुमानित लागत नियोजित लागत से कम होती है, तो कार्य के बारे में यह अनुमान लगाया जाता है कि उसकी लागत मूल रूप से नियोजित लागत से कम होगी और बजट के भीतर ट्रेंड कर रही है.</span><span class="sxs-lookup"><span data-stu-id="73836-153">If the Estimated cost at complete is less than the planned cost, the task is projected to cost less than was originally planned and is trending under budget.</span></span>

## <a name="project-managers-reprojection-of-cost"></a><span data-ttu-id="73836-154">परियोजना प्रबंधक द्वारा लागत का दोबारा अनुमान लगाना</span><span class="sxs-lookup"><span data-stu-id="73836-154">Project manager’s reprojection of cost</span></span>

<span data-ttu-id="73836-155">जब प्रयास का दोबारा अनुमान लगाया जाता है, तो CTC, पूर्णता पर अनुमानित लागत, आई लागत का प्रतिशत और अनुमानित लागत भिन्नता सभी का **लागत ट्रैकिंग** दृश्य में दोबारा परिकलन किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="73836-155">When effort is reprojected, the CTC, Estimated cost at complete, percentage of cost consumed, and projected cost variance are all recalculated in the **Cost tracking** view.</span></span>

## <a name="project-status-summary"></a><span data-ttu-id="73836-156">प्रोजेक्ट स्थिति सारांश</span><span class="sxs-lookup"><span data-stu-id="73836-156">Project status summary</span></span>

<span data-ttu-id="73836-157">**प्रयास ट्रैकिंग** और **लागत ट्रैकिंग** दृश्य में ट्रैकिंग डेटा प्रोजेक्ट रूट नोड में प्रगति और आई लागत, समरी टास्क और लीफ नोड टास्क स्तर दिखाता है।</span><span class="sxs-lookup"><span data-stu-id="73836-157">Tracking data in the **Effort tracking** and **Cost tracking** views shows the progress and cost consumption at the project root node, summary tasks, and leaf node tasks levels.</span></span> <span data-ttu-id="73836-158">**प्रोजेक्ट एंटिटी** पेज पर **स्थिति** खंड प्रोजेक्ट-स्तर के स्टेटस का समरी दिखाता है।</span><span class="sxs-lookup"><span data-stu-id="73836-158">The **Status** section on the **Project entity** page shows a summary of project-level status.</span></span>

## <a name="status-summary-fields"></a><span data-ttu-id="73836-159">स्थिति सारांश फ़ील्ड</span><span class="sxs-lookup"><span data-stu-id="73836-159">Status summary fields</span></span>

<span data-ttu-id="73836-160">**संपूर्ण परियोजना स्थिति** फील्ड एक एडिट करने योग्य फील्ड होता है जो प्रोजेक्ट का संपूर्ण स्टेटस दिखाता है।</span><span class="sxs-lookup"><span data-stu-id="73836-160">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="73836-161">इसमें बढ़ते जोखिम को दर्शाने के लिए हरे, पीले और लाल जैसे कलर-कोडिंग का इस्तेमाल किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="73836-161">It uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> <span data-ttu-id="73836-162">**टिप्पणियां** फ़ील्ड परियोजना प्रबंधक को स्थिति के बारे में विशिष्ट टिप्पणी दर्ज करने देता है.</span><span class="sxs-lookup"><span data-stu-id="73836-162">The **Comments** field lets the project manager enter specific comments about the status.</span></span> <span data-ttu-id="73836-163">फील्ड **पर स्थिति अद्यतन** एडिट नहीं किया जा सकता और इसका वैल्यू टाइमस्टैम्प होता है जो स्टेटस के अंतिम बार अपडेट करने को बताता है।</span><span class="sxs-lookup"><span data-stu-id="73836-163">The **Status updated on** field is not editable and the value is a timestamp that indicates when the status was last updated.</span></span>

<span data-ttu-id="73836-164">**शेड्यूल प्रदर्शन** और **लागत प्रदर्शन** फील्ड ट्रैकिंग की तारीख से सेट किए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="73836-164">The **Schedule performance** and **Cost performance** fields are set from the tracking date.</span></span> <span data-ttu-id="73836-165">जब **प्रयास ट्रैकिंग** व्यू में रूट नोड के लिए शेड्यूल और लागत भिन्नता पोज़िटिव होते हैं तो आप इन फील्ड को **Ahead** में सेट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="73836-165">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, you can set these fields to **Ahead**.</span></span> <span data-ttu-id="73836-166">जब रूट नोड के लिए शेड्यूल और लागत भिन्नता निगेटिव होते हैं तो आप इन फील्ड को **पीछे** में सेट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="73836-166">When the schedule and cost variance for the root node are negative, you can set them to **Behind**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]