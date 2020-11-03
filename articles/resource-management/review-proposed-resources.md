---
title: प्रस्तावित संसाधनों की समीक्षा करें
description: इस टॉपिक में प्रोजेक्ट के संसाधनों का प्रस्ताव देने के बारे में जानकारी प्रदान की गई है।
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: ad5cbdeb5fe05e6115eb024833a8d58b626ea4c9
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077667"
---
# <a name="review-proposed-resources"></a><span data-ttu-id="85412-103">प्रस्तावित संसाधनों की समीक्षा करें</span><span class="sxs-lookup"><span data-stu-id="85412-103">Review proposed resources</span></span>

<span data-ttu-id="85412-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="85412-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="85412-105">संसाधन प्रबंधक संसाधन अनुरोध उपयोग कर प्रोजेक्ट प्रबंधक को संसाधन का प्रस्ताव दे सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="85412-105">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="85412-106">अनुरोध ग्रिड या फिर अनुरोध से ही **संसाधन ढूंढें** का चुनाव करें।</span><span class="sxs-lookup"><span data-stu-id="85412-106">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="85412-107">**शेड्यूल असिस्टेंट** पृष्ठ पर संसाधन का चयन करें और फिर **संसाधन की बुकिंग करें** पेन में **बुकिंग की स्थिति** फ़ील्ड में **बुक करें** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="85412-107">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

<span data-ttu-id="85412-108">स्थिति से संबंधित निम्न अपडेट्स होंगे:</span><span class="sxs-lookup"><span data-stu-id="85412-108">The following status updates occur:</span></span>

- <span data-ttu-id="85412-109">**शेड्यूल असिस्टेंट** पृष्ठ पर स्थिति से जुड़े संकेतक यह बताने के लिए अपडेट किए जाते हैं कि बुकिंग अभी प्रस्तावित ही है, हार्ड-बुक नहीं हुई है।</span><span class="sxs-lookup"><span data-stu-id="85412-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>
- <span data-ttu-id="85412-110">संसाधन के लिए अनुरोध किये जाने पर स्थिति **समीक्षा वांछित है** में परिवर्तित हो जाती है।</span><span class="sxs-lookup"><span data-stu-id="85412-110">On the resource request, the status is changed to **Needs Review**.</span></span>
- <span data-ttu-id="85412-111">प्रोजेक्ट की **टीम** टैब पर जेनेरिक टीम सदस्य के **अनुरोध की स्थिति** **समीक्षा वांछित है** में परिवर्तित हो जाती है।</span><span class="sxs-lookup"><span data-stu-id="85412-111">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

<span data-ttu-id="85412-112">प्रोजेक्ट प्रबंधक प्रस्ताव को स्वीकार या अस्वीकार कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="85412-112">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="85412-113">संसाधन प्रबंधक संसाधन के लिए अनुरोधों को प्रोसेस करते समय निम्न में से कोई भी दृष्टिकोण अपना सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="85412-113">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="85412-114">यदि वांछित समय के लिए कोई एकल संसाधन उपलब्ध नहीं हो तो मांग को पूरा करने के लिए कई संसाधन प्रस्तावित करें।</span><span class="sxs-lookup"><span data-stu-id="85412-114">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="85412-115">फिर प्रस्तावित घंटों को कई संसाधनों में बांटा जाता है ताकि वे वांछित समय दे पाएं।</span><span class="sxs-lookup"><span data-stu-id="85412-115">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="85412-116">ऐसे मामलों में घंटों का ओवरलैप नहीं हो सकता है।</span><span class="sxs-lookup"><span data-stu-id="85412-116">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="85412-117">आवश्यकता से कम संसाधनों का प्रस्ताव दें।</span><span class="sxs-lookup"><span data-stu-id="85412-117">Propose fewer resources than are required.</span></span> <span data-ttu-id="85412-118">ऐसे मामले में प्रस्तावित संसाधन क्षमता अनुरोधकर्ता द्वारा मांगे गए घंटों से कम होती है।</span><span class="sxs-lookup"><span data-stu-id="85412-118">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="85412-119">इस तरह से जब अनुरोधकर्ता प्रस्तावित संसाधनों को स्वीकृति देता है तो शेष मांग को पूरा करने के लिए संसाधनों की अधूरी मांग पैदा हो जाती है।</span><span class="sxs-lookup"><span data-stu-id="85412-119">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="85412-120">यदि मांग को पूरा करने हेतु कोई एकल संसाधन उपलब्ध नहीं हो तो काम को पूरा करने हेतु एक से अधिक संसाधन बुक करें।</span><span class="sxs-lookup"><span data-stu-id="85412-120">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="85412-121">आवश्यकता से कम संसाधन बुक करें।</span><span class="sxs-lookup"><span data-stu-id="85412-121">Book fewer resources than are required.</span></span> <span data-ttu-id="85412-122">ऐसे मामलों में बुक किये गए घंटे वांछित घंटों से कम होते हैं।</span><span class="sxs-lookup"><span data-stu-id="85412-122">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="85412-123">यह सिस्टम आपको बुकिंग के बजाय संसाधनों का प्रस्ताव देने के लिए दिशानिर्देश देता है, ताकि अनुरोधकर्ता शेष मांग को सत्यापित कर सके और उस पर नज़र रख सके।</span><span class="sxs-lookup"><span data-stu-id="85412-123">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="billable-utilization"></a><span data-ttu-id="85412-124">बिल करने योग्य उपयोग</span><span class="sxs-lookup"><span data-stu-id="85412-124">Billable utilization</span></span>

<span data-ttu-id="85412-125">संसाधनों का लक्षित बिलेबल उपयोग हो सकता है।</span><span class="sxs-lookup"><span data-stu-id="85412-125">Resources can have a target billable utilization.</span></span> <span data-ttu-id="85412-126">इस लक्षित उपयोग को या तो संसाधन के डिफ़ॉल्ट रोल में विशेषता के रूप में परिभाषित किया जाता है या व्यक्तिगत बुक करने योग्य संसाधन के रिकॉर्ड पर सेट किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="85412-126">This target utilization is either defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="85412-127">उपयोगिता की गणनाएं संसाधनों द्वारा की गई अनुमोदित समय संबंधी प्रविष्टियों का उपयोग कर रिपोर्ट की जाती हैं।</span><span class="sxs-lookup"><span data-stu-id="85412-127">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="85412-128">उपयोगिता की गणना के लिए निम्न सूत्र उपयोग किये जाते हैं:</span><span class="sxs-lookup"><span data-stu-id="85412-128">The following formulas are used to calculate utilization:</span></span>

- <span data-ttu-id="85412-129">बिलेबल उपयोगिता = वास्तविक चार्जेबल घंटे ÷ संसाधन की क्षमता</span><span class="sxs-lookup"><span data-stu-id="85412-129">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
- <span data-ttu-id="85412-130">गैर-बिलेबल उपयोगिता = बिलिंग टाइप आईडी सहित वास्तविक समय = गैर-बिलेबल, पूरक, या उपलब्ध नहीं ÷ संसाधन की क्षमता</span><span class="sxs-lookup"><span data-stu-id="85412-130">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
- <span data-ttu-id="85412-131">आंतरिक = बिना बिक्री अनुबंध के लगाया गया वास्तविक समय ÷ संसाधन की क्षमता</span><span class="sxs-lookup"><span data-stu-id="85412-131">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
- <span data-ttu-id="85412-132">संसाधन की क्षमता = संसाधन का कार्य समय - कार्यालय से बाहर समय - गैर-कार्य दिवस</span><span class="sxs-lookup"><span data-stu-id="85412-132">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="85412-133">आप **संसाधन उपयोगिता** **Resources** पेन में देख सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="85412-133">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

<span data-ttu-id="85412-134">ग्रिड में प्रत्येक सेल किसी प्रदत्त अवधि जैसे कि एक दिन, सप्ताह या महीने में संसाधन की बिलेबल उपयोगिता प्रतिशत का सूचक है।</span><span class="sxs-lookup"><span data-stu-id="85412-134">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="85412-135">सेलों को रंगने के लिए निम्न सूत्र उपयोग किए जाते हैं:</span><span class="sxs-lookup"><span data-stu-id="85412-135">The following formulas are used to color the cells:</span></span>

- <span data-ttu-id="85412-136">**हरा:** बिलेबल उपयोगिता \>= संसाधन की लक्षित उपयोगिता</span><span class="sxs-lookup"><span data-stu-id="85412-136">**Green:** Billable utilization \>= Resource target utilization</span></span>
- <span data-ttu-id="85412-137">**पीला:** लक्षित उपयोगिता - 20 \<= बिलेबल उपयोगिता \< लक्षित उपयोगिता</span><span class="sxs-lookup"><span data-stu-id="85412-137">**Yellow:** Target utilization – 20 \<= Billable utilization \< Target utilization</span></span>
- <span data-ttu-id="85412-138">**लाल:** बिलेबल उपयोगिता \< लक्षित उपयोगिता - 20</span><span class="sxs-lookup"><span data-stu-id="85412-138">**Red:** Billable utilization \< Target utilization – 20</span></span>

<span data-ttu-id="85412-139">चूंकि **संसाधन की उपयोगिता** दृश्य शेड्यूल बोर्ड पर आधारित है, आप अपने परिणामों को फ़िल्टर करने के लिए शेड्यूल बोर्ड की फ़िल्टरिंग क्षमताओं का उपयोग कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="85412-139">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="85412-140">ग्रिड के लिए वांछित है कि आप रोल या व्यक्तिगत संसाधन पर आधारित लक्षित उपयोगिता सेट करें।</span><span class="sxs-lookup"><span data-stu-id="85412-140">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="85412-141">यह सेटअप करने के लिए **संसाधन** \> **संसाधनों के रोल** पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="85412-141">To do this setup, go to **Resources** \> **Resource roles**.</span></span>

<span data-ttu-id="85412-142">इसके अतिरिक्त प्रत्येक बुक करने योग्य संसाधन के लिए कोई डिफ़ॉल्ट रोल एसाइन किया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="85412-142">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="85412-143">**संसाधन** \> **संसाधन** पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="85412-143">Go to **Resources** \> **Resources**.</span></span> <span data-ttu-id="85412-144">**Project Service** टैब पर सत्यापित करें कि संसाधन का रोल परिभाषित किया गया है और यह कि इसके लिए **डिफ़ॉल्ट है** फ़ील्ड को **हां** पर सेट किया गया है।</span><span class="sxs-lookup"><span data-stu-id="85412-144">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field for it is set to **Yes**.</span></span> <span data-ttu-id="85412-145">जहां **डिफॉल्ट है = नहीं** है, आप अतिरिक्त रोल जोड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="85412-145">You can add additional roles where **Is Default = No**.</span></span> <span data-ttu-id="85412-146">उन रोल में, जहाँ **डिफॉल्ट है = हाँ** है, उसका उपयोग उस रोल के लक्ष्य के एवज़ में संसाधन की उपयोगिता का मूल्यांकन करने के लिए किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="85412-146">The role where the **Is Default = Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

<span data-ttu-id="85412-147">**Project Service** टैब पर आप जाकर किसी संसाधन के लिए व्यक्तिगत लक्षित उपयोगिता भी सेट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="85412-147">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="85412-148">उस मामले में उपयोगिता की गणना संसाधन के डिफ़ॉल्ट रोल के लक्ष्य के बजाय संसाधन की लक्षित उपयोगिता के आधार पर की जाती है।</span><span class="sxs-lookup"><span data-stu-id="85412-148">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="85412-149">किसी संसाधन की उपयोगिता तभी दिखाई जाती है यदि ग्रिड में दिखाई गई अवधि के दौरान उस संसाधन का स्वीकृत, चार्जेबल समय बनता हो।</span><span class="sxs-lookup"><span data-stu-id="85412-149">Utilization is shown for a resource only if that resource has approved, chargeable time during the period that is shown in the grid.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="85412-150">संसाधन उपलब्धता</span><span class="sxs-lookup"><span data-stu-id="85412-150">Resource availability</span></span>

<span data-ttu-id="85412-151">संसाधन प्रबंधकों के लिए महत्वपूर्ण है कि वे संसाधनों की उपलब्धता देखने और बुकिंग अपडेट करने में सक्षम हों।</span><span class="sxs-lookup"><span data-stu-id="85412-151">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="85412-152">कुछ मामलों में कोई औपचारिक मांग (संसाधन का अनुरोध) नहीं होती है लेकिन संसाधन प्रबंधक को ईमेल, फोन कॉल, या इंस्टेंट मेसेज जैसे चैनलों से प्राप्त किसी अनियोजित मांग को पूरा करने के लिए कार्यवाही करनी पड़ सकती है।</span><span class="sxs-lookup"><span data-stu-id="85412-152">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="85412-153">संसाधन प्रबंधक संसाधनों और बुकिंग को अपडेट करने के लिए शेड्यूल बोर्ड का उपयोग करते हैं।</span><span class="sxs-lookup"><span data-stu-id="85412-153">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="85412-154">संसाधन की उपलब्धता की गणना हेतु संसाधन के कार्य के घंटों को आधार बनाया जाता है।</span><span class="sxs-lookup"><span data-stu-id="85412-154">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="85412-155">संसाधनों की बुकिंग से संसाधनों की क्षमता का उपभोग होता है।</span><span class="sxs-lookup"><span data-stu-id="85412-155">Resource bookings consume the capacity of the resources.</span></span>

<span data-ttu-id="85412-156">शेड्यूल बोर्ड में बुकिंग, उपलब्धता, और ओवरबुकिंग के अलावा बुकिंग की स्थिति दिखाने के लिए रंगों और शेडिंग का उपयोग किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="85412-156">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="85412-157">शेड्यूल बोर्ड की सेटिंग्स में मौजूद एक सेटिंग की मदद से आप लेजेंड दिखा सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="85412-157">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="85412-158">यदि शेड्यूल बोर्ड पर किसी व्यक्तिगत बुक करने-योग्य संसाधन के बगल में दाईं तरफ वाला तीर दिखाई देता है तो उस संसाधन को एक्सपैंड कर देखा जा सकता है कि संसाधन को किस कार्य के लिए बुक किया गया है।</span><span class="sxs-lookup"><span data-stu-id="85412-158">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

<span data-ttu-id="85412-159">चूंकि Dynamics 365 Project Operations में Universal Resource Scheduling इंजन का उपयोग किया जाता है, आपके पास Dynamics 365 Field Service इंस्टाल होने के मामले में आप प्रोजेक्टओं और शेड्यूलिंग में शामिल अन्य इकाइयों से जुड़ी संसाधन बुकिंग और कार्य आदेश के विवरण देख सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="85412-159">Because Dynamics 365 Project Operations uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

<span data-ttu-id="85412-160">किसी व्यक्तिगत संसाधन के बारे में अधिक जानकारी पाने के लिए उस पर राइट-क्लिक कर संसाधन कार्ड खोलें।</span><span class="sxs-lookup"><span data-stu-id="85412-160">To view more details about an individual resource, right-click it to open the resource card.</span></span>

