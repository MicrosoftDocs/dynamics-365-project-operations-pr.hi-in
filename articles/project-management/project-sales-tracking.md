---
title: परियोजना विक्रय ट्रैकिंग
description: यह विषय इस बात की जानकारी प्रदान करता है कि Project Operations किसी परियोजना पर श्रम राजस्व के विरुद्ध कैसे प्रगति करता है.
author: rumant
manager: AnnBe
ms.date: 03/24/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 438c44dcfaf9677075eb07688c1e65c6e7053755
ms.sourcegitcommit: a1f9f92546ab5d8d8e5a4710ce4c96414ea55d14
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2021
ms.locfileid: "5711053"
---
# <a name="project-sales-tracking"></a><span data-ttu-id="66260-103">परियोजना विक्रय ट्रैकिंग</span><span class="sxs-lookup"><span data-stu-id="66260-103">Project sales tracking</span></span>

<span data-ttu-id="66260-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="66260-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="66260-105">Dynamics 365 Project Operations श्रम अनुमानों को ट्रैक करता है और परियोजना की योजना पर जानकारी के सबसे कम आवश्यक स्तर में खर्च करता है.</span><span class="sxs-lookup"><span data-stu-id="66260-105">Dynamics 365 Project Operations tracks labor estimates and revenue at the lowest required granularity on a project plan.</span></span> <span data-ttu-id="66260-106">श्रम राजस्व का अनुमान नियोजित प्रयास और जेनेरिक या नामित संसाधनों पर आधारित है जो प्रोज़ेक्ट की योजना में प्रत्येक लीफ़ नोड कार्य को सौंपे जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="66260-106">The estimate of labor revenue is based on the planned effort and the generic or named resources that are assigned to each leaf node task in the project plan.</span></span> <span data-ttu-id="66260-107">जब प्रोज़ेक्ट शुरू होता है और लोग प्रोज़ेक्ट के विभिन्न कार्यों के लिए समय की रिपोर्ट करना शुरू करते हैं, तो श्रम पर वास्तविक राजस्व संक्षेप में प्रस्तुत किया जाता है जो अनुमानों की गणना शुरू करता है.</span><span class="sxs-lookup"><span data-stu-id="66260-107">When the project begins and people start to report time on various project tasks, the actual revenue on labor is summarized which starts a calculation of the projections.</span></span>

## <a name="labor-revenue-tracking-view"></a><span data-ttu-id="66260-108">श्रम राजस्व ट्रैकिंग व्यू</span><span class="sxs-lookup"><span data-stu-id="66260-108">Labor revenue tracking view</span></span>

<span data-ttu-id="66260-109">**लागत ट्रैकिंग** दृश्य खोलने के लिए आप **परियोजनाएं** पेज में **ट्रैंकिंग** टैब पर  **ट्रैंकिंग** > **लागत** चुन सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="66260-109">On the **Projects** page, on the **Tracking** tab, you can select **Tracking** > **Cost** to open the **Cost Tracking** view.</span></span> <span data-ttu-id="66260-110">या आप **राजस्व ट्रैकिंग** दृश्य खोलने के लिए **उपयोग** > **बिल दर** चुन सकते हैं, जो परियोजना योजना में प्रत्येक कार्य पर श्रम राजस्व की प्रगति को दर्शाता है.</span><span class="sxs-lookup"><span data-stu-id="66260-110">Or, you can select **Use** > **Bill Rate** to open the **Revenue Tracking** view, which shows the progress of labor revenue on each task in the project plan.</span></span> <span data-ttu-id="66260-111">यह दृश्य कार्य की योजनाबद्ध श्रम राजस्व के लिए किसी कार्य पर खर्च की गई वास्तविक श्रम राजस्व की तुलना भी करता है.</span><span class="sxs-lookup"><span data-stu-id="66260-111">This view also compares the actual labor revenue spent on a task to the task's planned labor revenue.</span></span> <span data-ttu-id="66260-112">Project Operations श्रम राजस्व के आंकड़ों की गणना करने के लिए निम्नलिखित सूत्रों का उपयोग करता है:</span><span class="sxs-lookup"><span data-stu-id="66260-112">Project Operations uses the following formulas to calculate labor revenue metrics:</span></span>

- <span data-ttu-id="66260-113">**नियोजित राजस्व**: प्रत्येक पत्ती लीफ़ नोड कार्य पर सभी संसाधन कार्यों के अनुमानित बिक्री मूल्य</span><span class="sxs-lookup"><span data-stu-id="66260-113">**Planned Revenue**: Estimated sales values of all resource assignments on each leaf node task</span></span>
- <span data-ttu-id="66260-114">**वास्तविक राजस्व**: कार्य पर दर्ज किए गए समय के लिए सभी बिना बिल वाली बिक्री वास्तविक का योग</span><span class="sxs-lookup"><span data-stu-id="66260-114">**Actual Revenue**: Sum of all unbilled sales actuals for time recorded on the task</span></span>
- <span data-ttu-id="66260-115">**बिल योग्य राजस्व%**: वास्तविक राजस्व ÷ पूरा होने पर राजस्व अनुमान</span><span class="sxs-lookup"><span data-stu-id="66260-115">**Billable Revenue%**: Actual revenue ÷ Revenue estimate at complete</span></span>
- <span data-ttu-id="66260-116">**शेष राजस्व**: पूरा होने पर राजस्व अनुमान - वास्तविक राजस्व</span><span class="sxs-lookup"><span data-stu-id="66260-116">**Remaining Revenue**: Revenue estimate at complete – Actual revenue</span></span>
- <span data-ttu-id="66260-117">**पूरा होने पर अनुमानित राजस्व**: शेष राजस्व + वास्तविक राजस्व</span><span class="sxs-lookup"><span data-stu-id="66260-117">**Estimated Revenue at Complete**: Remaining revenue + Actual revenue</span></span>
- <span data-ttu-id="66260-118">**राजस्व विचरण**: नियोजित राजस्व - पूरा होने पर अनुमानित राजस्व</span><span class="sxs-lookup"><span data-stu-id="66260-118">**Revenue variance**: Planned revenue – Estimated revenue at complete</span></span>


> [!NOTE]
> <span data-ttu-id="66260-119">Project Operations केवल **प्रोज़ेक्ट** पेज पर **ट्रैकिंग** टैब पर श्रम राजस्व दिखाता है. जबकि सामग्री और खर्चों का अनुमान लगाया जा सकता है और खपत के लिए ट्रैक किया जा सकता है, ये राजस्व **ट्रैकिंग** टैब पर दिखाए गए राजस्व में शामिल नहीं हैं . यह टैब केवल प्रयास को पुनः प्रोज़ेक्ट करके श्रम राजस्व को पुनः प्रोज़ेक्ट करने के लिए डिज़ाइन किया गया है.</span><span class="sxs-lookup"><span data-stu-id="66260-119">Project Operations only shows labor revenues on the **Project** page on the **Tracking** tab. While materials and expenses can be estimated and tracked for consumption, these revenues are not included in the revenues shown on the **Tracking** tab. This tab is designed to work only for reprojecting labor revenues by reprojecting effort.</span></span>  
> <span data-ttu-id="66260-120">दिखाई गई सभी राजस्व राशि प्रोज़ेक्ट की लागत विक्रय में परिवर्तित हो जाती है.</span><span class="sxs-lookup"><span data-stu-id="66260-120">All revenue amounts shown are converted to the cost currency of the project.</span></span> <span data-ttu-id="66260-121">परियोजना की लागत मुद्रा परियोजना पर कॉन्ट्रैक्ट करने की इकाई की मुद्रा है.</span><span class="sxs-lookup"><span data-stu-id="66260-121">The cost currency of the project is the currency of the contracting unit on the project.</span></span> <span data-ttu-id="66260-122">निश्चित मूल्य प्रोज़ेक्ट के लिए, **श्रम राजस्व ट्रैकिंग** दृश्य पर राजस्व संख्या प्रासंगिक नहीं है क्योंकि बिना बिल बिक्री वास्तविक समय के अनुमोदन पर दर्ज नहीं किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="66260-122">For fixed price projects, revenue numbers on the **Labor revenue tracking** view aren't relevant because unbilled sales actuals aren't recorded on the approval of time.</span></span>
> <span data-ttu-id="66260-123">प्रोज़ेक्ट के **अनुमान** टैब पर दिखाए गए समय के लिए अनुमानित बिक्री मान **ट्रैकिंग** टैब पर नियोजित राजस्व मूल्य में नहीं जुड़ सकते हैं. इस विसंगति का स्रोत दो संभावित कारणों के कारण है:</span><span class="sxs-lookup"><span data-stu-id="66260-123">The estimated sales values for time that are shown on the **Estimate** tab of the project may not add up to the planned revenue value on the **Tracking** tab. The source of this discrepancy is due to two possible reasons:</span></span>
><ol>
   ><li> <span data-ttu-id="66260-124"><b>अनुमान</b> टैब बिक्री विक्रय में अनुमानित राजस्व दिखाता है, जबकि <b>ट्रैकिंग</b> टैब लागत विक्रय में परिवर्तित नियोजित राजस्व दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="66260-124">The <b>Estimates</b> tab shows estimated revenue in the sales currency, while the <b>Tracking</b> tab shows planned revenue converted to the cost currency.</span></span> </li>
   ><li> <span data-ttu-id="66260-125">जब अनुमानित बिक्री को <b>अनुमान</b> टैब पर दिखाए गए अनुबंध विक्रय में परिवर्तित कर दिया जाता है, तो प्रोज़ेक्ट विक्रय में, रूपांतरण में ऐसे कदम शामिल होते हैं, जिनसे सटीकता का कुछ नुकसान हो सकता है:</span><span class="sxs-lookup"><span data-stu-id="66260-125">When estimated sales are converted to the contract currency as shown on the <b>Estimates</b> tab, to the project currency, the conversion involves steps that could result in some loss of accuracy:</span></span> </li>
><ol>
><li> <span data-ttu-id="66260-126">अनुबंध विक्रय में अनुमानित बिक्री राशि को पहले आधार विक्रय (रूपांतरण 1) में परिवर्तित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="66260-126">The estimated sales amount in the contract currency is first converted to the base currency (conversion 1).</span></span></li>
><li> <span data-ttu-id="66260-127">आधार विक्रय में अनुमानित बिक्री राशि प्रोज़ेक्ट लागत विक्रय (रूपांतरण 2) में परिवर्तित हो जाती है.</span><span class="sxs-lookup"><span data-stu-id="66260-127">The estimated sales amount in the base currency are converted to the project cost currency (conversion 2).</span></span> </li>
></ol>
></ol>
> <span data-ttu-id="66260-128">विक्रय परिशुद्धता दोनों चरणों में लागू की जाती है, जिसके परिणामस्वरूप अनुबंध विक्रय में नियोजित बिक्री से प्रोज़ेक्ट विक्रय में नियोजित राजस्व का विचलन होता है.</span><span class="sxs-lookup"><span data-stu-id="66260-128">Currency precision is applied in both steps, which results in a deviation of the planned revenue in the project currency from the planned sales in the contract currency.</span></span>
   

## <a name="reprojecting-revenues-on-leaf-node-tasks"></a><span data-ttu-id="66260-129">लीफ़ नोड कार्यों पर राजस्व का पुनः प्रोजेक्शन</span><span class="sxs-lookup"><span data-stu-id="66260-129">Reprojecting revenues on leaf node tasks</span></span>

<span data-ttu-id="66260-130">एक लीफ़ नोड कार्य पर श्रम राजस्व को **प्रोज़ेक्ट** पेज पर **ट्रैकिंग** टैब पर सीधे पुनर्प्रोज़ेक्ट नहीं किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="66260-130">Labor revenues on a leaf node task can't be directly reprojected on the **Tracking** tab on the **Project** page.</span></span> <span data-ttu-id="66260-131">हालांकि, आप किसी कार्य पर शेष प्रयास को फिर से पेश करने के लिए **प्रयास की ट्रैकिंग** दृश्य का उपयोग कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="66260-131">However, you can use the **Effort Tracking** view to reproject the remaining effort on a task.</span></span> <span data-ttu-id="66260-132">इससे कार्य पर शेष राजस्व की पुनर्गणना होती है.</span><span class="sxs-lookup"><span data-stu-id="66260-132">This causes a recalculation of the remaining revenue on the task.</span></span> <span data-ttu-id="66260-133">इसके काम करने का वर्णन निम्नलिखित है.</span><span class="sxs-lookup"><span data-stu-id="66260-133">The following is a description of how this works.</span></span>

1. <span data-ttu-id="66260-134">एक प्रोज़ेक्ट प्रबंधक कार्य पर शेष प्रयास के नए अनुमान के साथ **शेष प्रयास** क्षेत्र में डिफ़ॉल्ट मूल्य को अपडेट करके कार्यों पर प्रयास को पुनः अनुमानित कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="66260-134">A project manager can reproject effort on tasks by updating the default value in the **Remaining Effort** field with a new estimate of the remaining effort on the task.</span></span> <span data-ttu-id="66260-135">फिर से पेश करना किसी कार्य पर अनुमानित प्रयास के विचरण में, प्रगति के प्रतिशत में और पूरे (EAC) में कार्य के प्रयास के अनुमान की पुनर्गणना का कारण बनता है.</span><span class="sxs-lookup"><span data-stu-id="66260-135">Reprojecting causes a recalculation of the task's effort estimate at complete (EAC), progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="66260-136">समरी टास्क पर EAC, पूरा होने का अनुमान (ETC), और प्रगति के प्रतिशत का भी दोबारा परिकलन किया जाता है और प्रयास की भिन्नता का नया अनुमान किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="66260-136">The EAC, estimate to complete (ETC), and progress percentage on the summary tasks are also recalculated and produce a new projection of effort variance.</span></span>
2. <span data-ttu-id="66260-137">कार्य पर शेष प्रयास के लिए नए मूल्य के आधार पर, सिस्टम **राजस्व ट्रैकिंग** व्यू पर शेष राजस्व की गणना करता है.</span><span class="sxs-lookup"><span data-stu-id="66260-137">Based on the new value for the remaining effort on the task, the system calculates the remaining revenue on the **Revenue Tracking** view.</span></span> <span data-ttu-id="66260-138">शेष प्रयास के आधार पर शेष राजस्व की गणना करने के लिए, प्रणाली पहले योजनाबद्ध राजस्व या नियोजित प्रयास के रूप में कार्य पर एक घंटे के प्रयास के औसत राजस्व की गणना करती है.</span><span class="sxs-lookup"><span data-stu-id="66260-138">To calculate the remaining revenue based on the remaining effort, the system first calculates the average revenue of one hour of effort on the task as planned revenue or planned effort.</span></span> <span data-ttu-id="66260-139">नियोजित राजस्व कार्य पर सभी संसाधन कार्यों के राजस्व का योग है.</span><span class="sxs-lookup"><span data-stu-id="66260-139">The planned revenue is the sum of the revenue of all resource assignments on the task.</span></span> <span data-ttu-id="66260-140">प्रति घंटे औसत राजस्व का उपयोग कार्य पर नए अनुमानित शेष प्रयास के लिए शेष राजस्व की गणना करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="66260-140">The average revenue per hour is used to compute the remaining revenue for the newly projected remaining effort on the task.</span></span>
3. <span data-ttu-id="66260-141">लीफ़ नोड कार्य पर पूर्ण और राजस्व उपभोग प्रतिशत पर अनुमानित राजस्व की फिर से गणना की जाती है.</span><span class="sxs-lookup"><span data-stu-id="66260-141">The estimated revenue at complete and revenue consumption percentage on the leaf node task are re-calculated.</span></span>
4. <span data-ttu-id="66260-142">समरी टास्क के पूर्ण मूल्य पर राजस्व का रूट नोड तक दोबारा परिकलन किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="66260-142">The revenue at complete value of the summary tasks all the way to the root node are recalculated.</span></span>

## <a name="reprojecting-revenues-on-summary-tasks"></a><span data-ttu-id="66260-143">सारांश कार्यों पर राजस्व का पुनर्प्रोज़ेक्शन</span><span class="sxs-lookup"><span data-stu-id="66260-143">Reprojecting revenues on summary tasks</span></span>

<span data-ttu-id="66260-144">आप सारांश कार्यों या कंटेनर कार्यों पर श्रम राजस्व को फिर से पेश कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="66260-144">You can reproject labor revenue on summary tasks or container tasks.</span></span> <span data-ttu-id="66260-145">हालांकि, आप **प्रोज़ेक्ट** पेज पर **ट्रैकिंग** टैब पर एक सारांश प्रोज़ेक्ट कार्य पर श्रम राजस्व को सीधे पुनर्प्रोज़ेक्ट नहीं कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="66260-145">However, you can't directly reproject labor revenues on a summary project task on the **Tracking** tab on the **Project** page.</span></span> <span data-ttu-id="66260-146">लीफ़ नोड कार्यों के समान, संक्षेपित और कंटेनर कार्यों को **प्रयास की ट्रैकिंग** दृश्य का उपयोग करके फिर से पेश किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="66260-146">Similar to leaf node tasks, reprojecting summary and container tasks can be done using the **Effort Tracking** view.</span></span> <span data-ttu-id="66260-147">इस व्यू में आप सारांश कार्य पर शेष प्रयास को पुनः अनुमान लगा सकते हैं, जिससे सारांश कार्य पर शेष राजस्व की पुनर्गणना हो सकती है.</span><span class="sxs-lookup"><span data-stu-id="66260-147">In this view, you can reproject the remaining effort on a summary task causing a recalculation of the remaining revenue on the summary task.</span></span> <span data-ttu-id="66260-148">इसके काम करने का वर्णन निम्नलिखित है.</span><span class="sxs-lookup"><span data-stu-id="66260-148">The following is a description of how this works.</span></span>

1. <span data-ttu-id="66260-149">एक प्रोज़ेक्ट प्रबंधक कार्य पर **शेष प्रयास** के नए अनुमान के साथ **शेष प्रयास** क्षेत्र में डिफ़ॉल्ट मूल्य को अपडेट करके कार्यों पर प्रयास को पुनः अनुमानित कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="66260-149">A project manager can reproject effort on tasks by updating the default value in the **Remaining Effort** field with a new estimate of the **Remaining Effort** on the task.</span></span> <span data-ttu-id="66260-150">पुनर्प्रोज़ेक्शन पूरा होने पर कार्य के अनुमान (EAC), प्रगति प्रतिशत और किसी कार्य पर अनुमानित प्रयास विचरण पर पुनर्गणना का कारण बनता है.</span><span class="sxs-lookup"><span data-stu-id="66260-150">Reprojecting causes a recalculation of the task's estimate at complete (EAC), progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="66260-151">EAC, ETC और सारांश कार्यों पर प्रगति प्रतिशत की भी पुनर्गणना होती है और प्रयास विचरण के एक नए प्रक्षेपण का उत्पादन करता है.</span><span class="sxs-lookup"><span data-stu-id="66260-151">The EAC, ETC, and progress percentage on the summary tasks are also recalculated and produce a new projection of effort variance.</span></span>
2. <span data-ttu-id="66260-152">कार्य पर **शेष प्रयास** क्षेत्र में नए मूल्य के आधार पर, सिस्टम **राजस्व ट्रैकिंग** व्यू में शेष राजस्व की गणना करता है.</span><span class="sxs-lookup"><span data-stu-id="66260-152">Based on the new value in the **Remaining effort** field on the task, the system calculates the remaining revenue in the **Revenue Tracking** view.</span></span> <span data-ttu-id="66260-153">शेष प्रयास के आधार पर शेष राजस्व की गणना करने के लिए सिस्टम पहले योजनाबद्ध राजस्व या नियोजित प्रयास के रूप में कार्य पर एक घंटे के प्रयास के औसत राजस्व की गणना करता है.</span><span class="sxs-lookup"><span data-stu-id="66260-153">To calculate the remaining revenue based on remaining effort, the system first calculates the average revenue of one hour of effort on the task as planned revenue or planned effort.</span></span> <span data-ttu-id="66260-154">नियोजित राजस्व कार्य पर सभी संसाधन कार्यों के राजस्व का योग है.</span><span class="sxs-lookup"><span data-stu-id="66260-154">The planned revenue is the sum of the revenue of all resource assignments on the task.</span></span> <span data-ttu-id="66260-155">प्रति घंटे इस औसत राजस्व का उपयोग कार्य पर नए अनुमानित शेष प्रयास के राजस्व की गणना करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="66260-155">This average revenue per hour  is then used to calculate the revenue of the newly projected remaining effort on the task.</span></span>
3. <span data-ttu-id="66260-156">सारांश कार्य पर पूरा होने पर अनुमानित राजस्व और राजस्व खपत प्रतिशत की फिर से गणना की जाती है.</span><span class="sxs-lookup"><span data-stu-id="66260-156">The estimated revenue at complete and revenue consumption percentages on the summary task are re-calculated.</span></span>
4. <span data-ttu-id="66260-157">पूरा होने पर अनुमानित राजस्व के लिए नया मूल्य उसी अनुपात में चाइल्ड कार्यों के लिए वितरित किया जाता है जैसा कि मूल नियोजित राजस्व कार्य में था.</span><span class="sxs-lookup"><span data-stu-id="66260-157">The new value for the estimated revenue at complete is distributed down to the child tasks in the same proportion as the original planned revenue was on the task.</span></span>
5. <span data-ttu-id="66260-158">प्रत्येक वैयक्तिक टास्क के नए अनुमानित राजस्व पूर्ण से लेकर लीफ नोड टास्क तक का परिकलन किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="66260-158">The new estimated revenue at complete on each of the individual tasks down to the leaf node tasks is calculated.</span></span> <span data-ttu-id="66260-159">इस मूल्य के आधार पर, नीचे लीफ़ नोड्स तक प्रभावित चाइल्ड कार्यों के लिए उनकी शेष राजस्व और राजस्व खपत प्रतिशत के पूर्ण मूल्य पर राजस्व के आधार पर पुनर्गणना की जाएगी.</span><span class="sxs-lookup"><span data-stu-id="66260-159">Based on this value, the affected child tasks down to the leaf nodes will have their remaining revenue and revenue consumption percentage recalculated based on the revenue at complete value.</span></span> <span data-ttu-id="66260-160">इसके कारण टास्क के राजस्व भिन्नता का नया अनुमान करना होता है।</span><span class="sxs-lookup"><span data-stu-id="66260-160">This results in a new projection for the revenue variance of the task.</span></span> 
6. <span data-ttu-id="66260-161">समरी टास्क के पूर्ण मूल्य पर राजस्व का रूट नोड तक दोबारा परिकलन किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="66260-161">The revenue at complete value of the summary tasks all the way to the root node are recalculated.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
