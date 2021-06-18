---
title: प्रोजेक्ट के लिए प्रस्तावित संसाधन
description: यह विषय प्रोजेक्ट संसाधनों का प्रस्ताव देने के बारे में जानकारी प्रदान करता है.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
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
ms.openlocfilehash: 02e47338e34a37e05455e2bc6e6a175210ed6bc7
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997963"
---
# <a name="propose-project-resources"></a><span data-ttu-id="ff043-103">प्रोजेक्ट के लिए प्रस्तावित संसाधन</span><span class="sxs-lookup"><span data-stu-id="ff043-103">Propose project resources</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="ff043-104">संसाधन प्रबंधक संसाधन अनुरोध उपयोग कर प्रोजेक्ट प्रबंधक को संसाधन का प्रस्ताव दे सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="ff043-104">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="ff043-105">अनुरोध ग्रिड या फिर अनुरोध से ही **संसाधन ढूंढें** का चुनाव करें।</span><span class="sxs-lookup"><span data-stu-id="ff043-105">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="ff043-106">**शेड्यूल असिस्टेंट** पृष्ठ पर संसाधन का चयन करें और फिर **संसाधन की बुकिंग करें** पेन में **बुकिंग की स्थिति** फ़ील्ड में **बुक करें** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="ff043-106">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

    ![प्रस्तावित संसाधन चयनित किया गया](media/Resource-Management-image62.png)

<span data-ttu-id="ff043-108">स्थिति से संबंधित निम्न अपडेट्स होंगे:</span><span class="sxs-lookup"><span data-stu-id="ff043-108">The following status updates occur:</span></span>

- <span data-ttu-id="ff043-109">**शेड्यूल असिस्टेंट** पृष्ठ पर स्थिति से जुड़े संकेतक यह बताने के लिए अपडेट किए जाते हैं कि बुकिंग अभी प्रस्तावित ही है, हार्ड-बुक नहीं हुई है।</span><span class="sxs-lookup"><span data-stu-id="ff043-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>

    ![शेड्यूल असिस्टेंट पृष्ठ पर प्रस्तावित बुकिंग के लिए स्थिति का संकेतक](media/Resource-Management-image63.png)

- <span data-ttu-id="ff043-111">संसाधन के लिए अनुरोध किये जाने पर स्थिति **समीक्षा वांछित है** में परिवर्तित हो जाती है।</span><span class="sxs-lookup"><span data-stu-id="ff043-111">On the resource request, the status is changed to **Needs Review**.</span></span>

    ![संसाधन अनुरोध की स्थिति समीक्षा वांछित है में परिवर्तित हो गई है](media/Resource-Management-image64.png)

- <span data-ttu-id="ff043-113">प्रोजेक्ट की **टीम** टैब पर जेनेरिक टीम सदस्य के **अनुरोध की स्थिति** **समीक्षा वांछित है** में परिवर्तित हो जाती है।</span><span class="sxs-lookup"><span data-stu-id="ff043-113">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

    ![प्रोजेक्ट के जेनेरिक टीम सदस्य के अनुरोध की स्थिति टीम टैब पर समीक्षा वांछित है में परिवर्तित हो गयी है।](media/Resource-Management-image48.png)

<span data-ttu-id="ff043-115">प्रोजेक्ट प्रबंधक प्रस्ताव को स्वीकार या अस्वीकार कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="ff043-115">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="ff043-116">संसाधन प्रबंधक संसाधन के लिए अनुरोधों को प्रोसेस करते समय निम्न में से कोई भी दृष्टिकोण अपना सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="ff043-116">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="ff043-117">यदि वांछित समय के लिए कोई एकल संसाधन उपलब्ध नहीं हो तो मांग को पूरा करने के लिए कई संसाधन प्रस्तावित करें।</span><span class="sxs-lookup"><span data-stu-id="ff043-117">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="ff043-118">फिर प्रस्तावित घंटों को कई संसाधनों में बांटा जाता है ताकि वे वांछित समय दे पाएं।</span><span class="sxs-lookup"><span data-stu-id="ff043-118">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="ff043-119">ऐसे मामलों में घंटों का ओवरलैप नहीं हो सकता है।</span><span class="sxs-lookup"><span data-stu-id="ff043-119">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="ff043-120">आवश्यकता से कम संसाधनों का प्रस्ताव दें।</span><span class="sxs-lookup"><span data-stu-id="ff043-120">Propose fewer resources than are required.</span></span> <span data-ttu-id="ff043-121">ऐसे मामले में प्रस्तावित संसाधन क्षमता अनुरोधकर्ता द्वारा मांगे गए घंटों से कम होती है।</span><span class="sxs-lookup"><span data-stu-id="ff043-121">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="ff043-122">इस तरह से जब अनुरोधकर्ता प्रस्तावित संसाधनों को स्वीकृति देता है तो शेष मांग को पूरा करने के लिए संसाधनों की अधूरी मांग पैदा हो जाती है।</span><span class="sxs-lookup"><span data-stu-id="ff043-122">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="ff043-123">यदि मांग को पूरा करने हेतु कोई एकल संसाधन उपलब्ध नहीं हो तो काम को पूरा करने हेतु एक से अधिक संसाधन बुक करें।</span><span class="sxs-lookup"><span data-stu-id="ff043-123">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="ff043-124">आवश्यकता से कम संसाधन बुक करें।</span><span class="sxs-lookup"><span data-stu-id="ff043-124">Book fewer resources than are required.</span></span> <span data-ttu-id="ff043-125">ऐसे मामलों में बुक किये गए घंटे वांछित घंटों से कम होते हैं।</span><span class="sxs-lookup"><span data-stu-id="ff043-125">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="ff043-126">यह सिस्टम आपको बुकिंग के बजाय संसाधनों का प्रस्ताव देने के लिए दिशानिर्देश देता है, ताकि अनुरोधकर्ता शेष मांग को सत्यापित कर सके और उस पर नज़र रख सके।</span><span class="sxs-lookup"><span data-stu-id="ff043-126">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="billable-utilization"></a><span data-ttu-id="ff043-127">बिल करने योग्य उपयोग</span><span class="sxs-lookup"><span data-stu-id="ff043-127">Billable utilization</span></span>

<span data-ttu-id="ff043-128">संसाधनों का लक्षित बिलेबल उपयोग हो सकता है।</span><span class="sxs-lookup"><span data-stu-id="ff043-128">Resources can have a target billable utilization.</span></span> <span data-ttu-id="ff043-129">इस लक्षित उपयोग को या तो संसाधन के डिफ़ॉल्ट रोल में विशेषता के रूप में परिभाषित किया जाता है या व्यक्तिगत बुक करने योग्य संसाधन के रिकॉर्ड पर सेट किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="ff043-129">This target utilization is either defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="ff043-130">उपयोगिता की गणनाएं संसाधनों द्वारा की गई अनुमोदित समय संबंधी प्रविष्टियों का उपयोग कर रिपोर्ट की जाती हैं।</span><span class="sxs-lookup"><span data-stu-id="ff043-130">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="ff043-131">उपयोगिता की गणना के लिए निम्न सूत्र उपयोग किये जाते हैं:</span><span class="sxs-lookup"><span data-stu-id="ff043-131">The following formulas are used to calculate utilization:</span></span>

- <span data-ttu-id="ff043-132">बिलेबल उपयोगिता = वास्तविक चार्जेबल घंटे ÷ संसाधन की क्षमता</span><span class="sxs-lookup"><span data-stu-id="ff043-132">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
- <span data-ttu-id="ff043-133">गैर-बिलेबल उपयोगिता = बिलिंग टाइप आईडी सहित वास्तविक समय = गैर-बिलेबल, पूरक, या उपलब्ध नहीं ÷ संसाधन की क्षमता</span><span class="sxs-lookup"><span data-stu-id="ff043-133">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
- <span data-ttu-id="ff043-134">आंतरिक = बिना बिक्री अनुबंध के लगाया गया वास्तविक समय ÷ संसाधन की क्षमता</span><span class="sxs-lookup"><span data-stu-id="ff043-134">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
- <span data-ttu-id="ff043-135">संसाधन की क्षमता = संसाधन का कार्य समय - कार्यालय से बाहर समय - गैर-कार्य दिवस</span><span class="sxs-lookup"><span data-stu-id="ff043-135">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="ff043-136">आप **संसाधन उपयोगिता** **Resources** पेन में देख सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="ff043-136">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

![संसाधन उपयोगिता दृश्य](media/Resource-Management-image65.png)

<span data-ttu-id="ff043-138">ग्रिड में प्रत्येक सेल किसी प्रदत्त अवधि जैसे कि एक दिन, सप्ताह या महीने में संसाधन की बिलेबल उपयोगिता प्रतिशत का सूचक है।</span><span class="sxs-lookup"><span data-stu-id="ff043-138">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="ff043-139">सेलों को रंगने के लिए निम्न सूत्र उपयोग किए जाते हैं:</span><span class="sxs-lookup"><span data-stu-id="ff043-139">The following formulas are used to color the cells:</span></span>

- <span data-ttu-id="ff043-140">**हरा:** बिलेबल उपयोगिता \>= संसाधन की लक्षित उपयोगिता</span><span class="sxs-lookup"><span data-stu-id="ff043-140">**Green:** Billable utilization \>= Resource target utilization</span></span>
- <span data-ttu-id="ff043-141">**पीला:** लक्षित उपयोगिता - 20 \<= बिलेबल उपयोगिता \< लक्षित उपयोगिता</span><span class="sxs-lookup"><span data-stu-id="ff043-141">**Yellow:** Target utilization – 20 \<= Billable utilization \< Target utilization</span></span>
- <span data-ttu-id="ff043-142">**लाल:** बिलेबल उपयोगिता \< लक्षित उपयोगिता - 20</span><span class="sxs-lookup"><span data-stu-id="ff043-142">**Red:** Billable utilization \< Target utilization – 20</span></span>

<span data-ttu-id="ff043-143">चूंकि **संसाधन की उपयोगिता** दृश्य शेड्यूल बोर्ड पर आधारित है, आप अपने परिणामों को फ़िल्टर करने के लिए शेड्यूल बोर्ड की फ़िल्टरिंग क्षमताओं का उपयोग कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="ff043-143">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="ff043-144">ग्रिड के लिए वांछित है कि आप रोल या व्यक्तिगत संसाधन पर आधारित लक्षित उपयोगिता सेट करें।</span><span class="sxs-lookup"><span data-stu-id="ff043-144">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="ff043-145">यह सेटअप करने के लिए **संसाधन** \> **संसाधनों के रोल** पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="ff043-145">To do this setup, go to **Resources** \> **Resource roles**.</span></span>

<span data-ttu-id="ff043-146">इसके अतिरिक्त प्रत्येक बुक करने योग्य संसाधन के लिए कोई डिफ़ॉल्ट रोल एसाइन किया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="ff043-146">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="ff043-147">**संसाधन** \> **संसाधन** पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="ff043-147">Go to **Resources** \> **Resources**.</span></span> <span data-ttu-id="ff043-148">**Project Service** टैब पर सत्यापित करें कि संसाधन का रोल परिभाषित किया गया है और यह कि इसके लिए **डिफ़ॉल्ट है** फ़ील्ड को **हां** पर सेट किया गया है।</span><span class="sxs-lookup"><span data-stu-id="ff043-148">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field for it is set to **Yes**.</span></span> <span data-ttu-id="ff043-149">जहां **डिफॉल्ट है = नहीं** है, आप अतिरिक्त रोल जोड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="ff043-149">You can add additional roles where **Is Default = No**.</span></span> <span data-ttu-id="ff043-150">उन रोल में, जहाँ **डिफॉल्ट है = हाँ** है, उसका उपयोग उस रोल के लक्ष्य के एवज़ में संसाधन की उपयोगिता का मूल्यांकन करने के लिए किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="ff043-150">The role where the **Is Default = Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

![डिफ़ॉल्ट रोल सेट हो गया है](media/Resource-Management-image67.png)

<span data-ttu-id="ff043-152">**Project Service** टैब पर आप जाकर किसी संसाधन के लिए व्यक्तिगत लक्षित उपयोगिता भी सेट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="ff043-152">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="ff043-153">उस मामले में उपयोगिता की गणना संसाधन के डिफ़ॉल्ट रोल के लक्ष्य के बजाय संसाधन की लक्षित उपयोगिता के आधार पर की जाती है।</span><span class="sxs-lookup"><span data-stu-id="ff043-153">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="ff043-154">किसी संसाधन की उपयोगिता तभी दिखाई जाती है यदि ग्रिड में दिखाई गई अवधि के दौरान उस संसाधन का स्वीकृत, चार्जेबल समय बनता हो।</span><span class="sxs-lookup"><span data-stu-id="ff043-154">Utilization is shown for a resource only if that resource has approved, chargeable time during the period that is shown in the grid.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="ff043-155">संसाधन उपलब्धता</span><span class="sxs-lookup"><span data-stu-id="ff043-155">Resource availability</span></span>

<span data-ttu-id="ff043-156">संसाधन प्रबंधकों के लिए महत्वपूर्ण है कि वे संसाधनों की उपलब्धता देखने और बुकिंग अपडेट करने में सक्षम हों।</span><span class="sxs-lookup"><span data-stu-id="ff043-156">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="ff043-157">कुछ मामलों में कोई औपचारिक मांग (संसाधन का अनुरोध) नहीं होती है लेकिन संसाधन प्रबंधक को ईमेल, फोन कॉल, या इंस्टेंट मेसेज जैसे चैनलों से प्राप्त किसी अनियोजित मांग को पूरा करने के लिए कार्यवाही करनी पड़ सकती है।</span><span class="sxs-lookup"><span data-stu-id="ff043-157">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="ff043-158">संसाधन प्रबंधक संसाधनों और बुकिंग को अपडेट करने के लिए शेड्यूल बोर्ड का उपयोग करते हैं।</span><span class="sxs-lookup"><span data-stu-id="ff043-158">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="ff043-159">संसाधन की उपलब्धता की गणना हेतु संसाधन के कार्य के घंटों को आधार बनाया जाता है।</span><span class="sxs-lookup"><span data-stu-id="ff043-159">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="ff043-160">संसाधनों की बुकिंग से संसाधनों की क्षमता का उपभोग होता है।</span><span class="sxs-lookup"><span data-stu-id="ff043-160">Resource bookings consume the capacity of the resources.</span></span>

![शेड्यूल बोर्ड](media/Resource-Management-image68.png)

<span data-ttu-id="ff043-162">शेड्यूल बोर्ड में बुकिंग, उपलब्धता, और ओवरबुकिंग के अलावा बुकिंग की स्थिति दिखाने के लिए रंगों और शेडिंग का उपयोग किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="ff043-162">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="ff043-163">शेड्यूल बोर्ड की सेटिंग्स में मौजूद एक सेटिंग की मदद से आप लेजेंड दिखा सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="ff043-163">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="ff043-164">यदि शेड्यूल बोर्ड पर किसी व्यक्तिगत बुक करने-योग्य संसाधन के बगल में दाईं तरफ वाला तीर दिखाई देता है तो उस संसाधन को एक्सपैंड कर देखा जा सकता है कि संसाधन को किस कार्य के लिए बुक किया गया है।</span><span class="sxs-lookup"><span data-stu-id="ff043-164">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

![शेड्यूल बोर्ड पर बुक करने-योग्य को एक्सपैंड किया गया](media/Resource-Management-image69.png)

<span data-ttu-id="ff043-166">चूंकि Dynamics 365 Project Service Automation में Universal Resource Scheduling इंजन का उपयोग किया जाता है, आपके पास Dynamics 365 Field Service इंस्टाल होने के मामले में आप प्रोजेक्टओं और शेड्यूलिंग में शामिल अन्य इकाइयों से जुड़ी संसाधन बुकिंग और कार्य आदेश के विवरण देख सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="ff043-166">Because Dynamics 365 Project Service Automation uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

![प्रोजेक्टओं और कार्य आदेशों के लिए संसाधनों की बुकिंग के विवरण](media/Resource-Management-image70.png)

<span data-ttu-id="ff043-168">किसी व्यक्तिगत संसाधन के बारे में अधिक जानकारी पाने के लिए उस पर राइट-क्लिक कर संसाधन कार्ड खोलें।</span><span class="sxs-lookup"><span data-stu-id="ff043-168">To view more details about an individual resource, right-click it to open the resource card.</span></span>

![संसाधन कार्ड](media/Resource-Management-image71.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]