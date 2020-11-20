---
title: प्रस्तावित संसाधनों की समीक्षा करें
description: इस टॉपिक में प्रोजेक्ट के संसाधनों का प्रस्ताव देने के बारे में जानकारी प्रदान की गई है।
author: ruhercul
manager: AnnBe
ms.date: 11/05/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
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
ms.openlocfilehash: 54a0924da17eac86e2fa400540e629f6d803aa35
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401175"
---
# <a name="review-proposed-resources"></a><span data-ttu-id="a7942-103">प्रस्तावित संसाधनों की समीक्षा करें</span><span class="sxs-lookup"><span data-stu-id="a7942-103">Review proposed resources</span></span>

<span data-ttu-id="a7942-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="a7942-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a7942-105">संसाधन प्रबंधक संसाधन अनुरोध उपयोग कर प्रोजेक्ट प्रबंधक को संसाधन का प्रस्ताव दे सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="a7942-105">Resource managers can propose a resource to the project manager by using a resource request.</span></span>

1. <span data-ttu-id="a7942-106">अनुरोध ग्रिड या फिर अनुरोध से ही **संसाधन ढूंढें** का चुनाव करें।</span><span class="sxs-lookup"><span data-stu-id="a7942-106">From the request grid or the request itself, select **Find Resources**.</span></span>
2. <span data-ttu-id="a7942-107">**शेड्यूल असिस्टेंट** पृष्ठ पर संसाधन का चयन करें और फिर **संसाधन की बुकिंग करें** पेन में **बुकिंग की स्थिति** फ़ील्ड में **बुक करें** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="a7942-107">On the **Schedule Assistant** page, select the resource, and then, in the **Create Resource Booking** pane, in the **Booking Status** field, select **Book**.</span></span>

<span data-ttu-id="a7942-108">स्थिति से संबंधित निम्न अपडेट्स होंगे:</span><span class="sxs-lookup"><span data-stu-id="a7942-108">The following status updates occur:</span></span>

- <span data-ttu-id="a7942-109">**शेड्यूल असिस्टेंट** पृष्ठ पर स्थिति से जुड़े संकेतक यह बताने के लिए अपडेट किए जाते हैं कि बुकिंग अभी प्रस्तावित ही है, हार्ड-बुक नहीं हुई है।</span><span class="sxs-lookup"><span data-stu-id="a7942-109">On the **Schedule Assistant** page, the status indicators are updated to indicate that the booking is proposed, not hard-booked.</span></span>
- <span data-ttu-id="a7942-110">संसाधन के लिए अनुरोध किये जाने पर स्थिति **समीक्षा वांछित है** में परिवर्तित हो जाती है।</span><span class="sxs-lookup"><span data-stu-id="a7942-110">On the resource request, the status is changed to **Needs Review**.</span></span>
- <span data-ttu-id="a7942-111">प्रोजेक्ट की **टीम** टैब पर जेनेरिक टीम सदस्य के **अनुरोध की स्थिति** **समीक्षा वांछित है** में परिवर्तित हो जाती है।</span><span class="sxs-lookup"><span data-stu-id="a7942-111">On the **Team** tab of the project, the generic team member's **Request Status** value is changed to **Needs Review**.</span></span>

<span data-ttu-id="a7942-112">प्रोजेक्ट प्रबंधक प्रस्ताव को स्वीकार या अस्वीकार कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="a7942-112">The project manager can either accept or reject the proposal.</span></span>

<span data-ttu-id="a7942-113">संसाधन प्रबंधक संसाधन के लिए अनुरोधों को प्रोसेस करते समय निम्न में से कोई भी दृष्टिकोण अपना सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="a7942-113">When resource managers process resource requests, they can use any of the following approaches:</span></span>

- <span data-ttu-id="a7942-114">यदि वांछित समय के लिए कोई एकल संसाधन उपलब्ध नहीं हो तो मांग को पूरा करने के लिए कई संसाधन प्रस्तावित करें।</span><span class="sxs-lookup"><span data-stu-id="a7942-114">Propose multiple resources to satisfy the demand if no single resource is available to fulfill the required hours.</span></span> <span data-ttu-id="a7942-115">फिर प्रस्तावित घंटों को कई संसाधनों में बांटा जाता है ताकि वे वांछित समय दे पाएं।</span><span class="sxs-lookup"><span data-stu-id="a7942-115">Proposed hours are then split among multiple resources that can satisfy the required hours.</span></span> <span data-ttu-id="a7942-116">ऐसे मामलों में घंटों का ओवरलैप नहीं हो सकता है।</span><span class="sxs-lookup"><span data-stu-id="a7942-116">In this scenario, the hours can't overlap.</span></span>
- <span data-ttu-id="a7942-117">आवश्यकता से कम संसाधनों का प्रस्ताव दें।</span><span class="sxs-lookup"><span data-stu-id="a7942-117">Propose fewer resources than are required.</span></span> <span data-ttu-id="a7942-118">ऐसे मामले में प्रस्तावित संसाधन क्षमता अनुरोधकर्ता द्वारा मांगे गए घंटों से कम होती है।</span><span class="sxs-lookup"><span data-stu-id="a7942-118">In this scenario, the proposed resource capacity is less than the required hours that the requestor specified.</span></span> <span data-ttu-id="a7942-119">इस तरह से जब अनुरोधकर्ता प्रस्तावित संसाधनों को स्वीकृति देता है तो शेष मांग को पूरा करने के लिए संसाधनों की अधूरी मांग पैदा हो जाती है।</span><span class="sxs-lookup"><span data-stu-id="a7942-119">Therefore, when the requestor accepts the proposed resources, an unfulfilled resource requirement is created to capture the remaining demand.</span></span>
- <span data-ttu-id="a7942-120">यदि मांग को पूरा करने हेतु कोई एकल संसाधन उपलब्ध नहीं हो तो काम को पूरा करने हेतु एक से अधिक संसाधन बुक करें।</span><span class="sxs-lookup"><span data-stu-id="a7942-120">Book multiple resources to satisfy the demand if no single resource is available to complete the work.</span></span>
- <span data-ttu-id="a7942-121">आवश्यकता से कम संसाधन बुक करें।</span><span class="sxs-lookup"><span data-stu-id="a7942-121">Book fewer resources than are required.</span></span> <span data-ttu-id="a7942-122">ऐसे मामलों में बुक किये गए घंटे वांछित घंटों से कम होते हैं।</span><span class="sxs-lookup"><span data-stu-id="a7942-122">In this scenario, the booked hours are fewer than the required hours.</span></span> <span data-ttu-id="a7942-123">यह सिस्टम आपको बुकिंग के बजाय संसाधनों का प्रस्ताव देने के लिए दिशानिर्देश देता है, ताकि अनुरोधकर्ता शेष मांग को सत्यापित कर सके और उस पर नज़र रख सके।</span><span class="sxs-lookup"><span data-stu-id="a7942-123">The system guides you to propose resources instead of bookings, so that the requestor can verify and keep track of remaining demand.</span></span>

## <a name="resource-availability"></a><span data-ttu-id="a7942-124">संसाधन उपलब्धता</span><span class="sxs-lookup"><span data-stu-id="a7942-124">Resource availability</span></span>

<span data-ttu-id="a7942-125">संसाधन प्रबंधकों के लिए महत्वपूर्ण है कि वे संसाधनों की उपलब्धता देखने और बुकिंग अपडेट करने में सक्षम हों।</span><span class="sxs-lookup"><span data-stu-id="a7942-125">It's critical that resource managers be able to view the availability of resources and update bookings.</span></span> <span data-ttu-id="a7942-126">कुछ मामलों में कोई औपचारिक मांग (संसाधन का अनुरोध) नहीं होती है लेकिन संसाधन प्रबंधक को ईमेल, फोन कॉल, या इंस्टेंट मेसेज जैसे चैनलों से प्राप्त किसी अनियोजित मांग को पूरा करने के लिए कार्यवाही करनी पड़ सकती है।</span><span class="sxs-lookup"><span data-stu-id="a7942-126">In some cases, there is no formal demand (resource request), but a resource manager must respond to an unplanned demand that comes through channels such as an email, phone call, or instant message.</span></span> <span data-ttu-id="a7942-127">संसाधन प्रबंधक संसाधनों और बुकिंग को अपडेट करने के लिए शेड्यूल बोर्ड का उपयोग करते हैं।</span><span class="sxs-lookup"><span data-stu-id="a7942-127">Resource managers use the Schedule Board to update resources and bookings.</span></span>

<span data-ttu-id="a7942-128">संसाधन की उपलब्धता की गणना हेतु संसाधन के कार्य के घंटों को आधार बनाया जाता है।</span><span class="sxs-lookup"><span data-stu-id="a7942-128">Resource work hours are used as the basis for calculating the availability of a resource.</span></span> <span data-ttu-id="a7942-129">संसाधनों की बुकिंग से संसाधनों की क्षमता का उपभोग होता है।</span><span class="sxs-lookup"><span data-stu-id="a7942-129">Resource bookings consume the capacity of the resources.</span></span>

<span data-ttu-id="a7942-130">शेड्यूल बोर्ड में बुकिंग, उपलब्धता, और ओवरबुकिंग के अलावा बुकिंग की स्थिति दिखाने के लिए रंगों और शेडिंग का उपयोग किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="a7942-130">The Schedule Board uses colors and shading to show bookings, availability, and overbookings, and also the status of bookings.</span></span> <span data-ttu-id="a7942-131">शेड्यूल बोर्ड की सेटिंग्स में मौजूद एक सेटिंग की मदद से आप लेजेंड दिखा सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="a7942-131">A setting in the Schedule Board settings lets you show a legend.</span></span>

<span data-ttu-id="a7942-132">यदि शेड्यूल बोर्ड पर किसी व्यक्तिगत बुक करने-योग्य संसाधन के बगल में दाईं तरफ वाला तीर दिखाई देता है तो उस संसाधन को एक्सपैंड कर देखा जा सकता है कि संसाधन को किस कार्य के लिए बुक किया गया है।</span><span class="sxs-lookup"><span data-stu-id="a7942-132">If a right-pointing arrow appears next to an individual bookable resource on the Schedule Board, the resource can be expanded to show details of the work that the resource is booked on.</span></span>

<span data-ttu-id="a7942-133">चूंकि Dynamics 365 Project Operations में Universal Resource Scheduling इंजन का उपयोग किया जाता है, आपके पास Dynamics 365 Field Service इंस्टाल होने के मामले में आप प्रोजेक्टओं और शेड्यूलिंग में शामिल अन्य इकाइयों से जुड़ी संसाधन बुकिंग और कार्य आदेश के विवरण देख सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a7942-133">Because Dynamics 365 Project Operations uses the Universal Resource Scheduling engine, if you also have Dynamics 365 Field Service installed, you can view the details of resource bookings for projects, work orders, and any other entities that you've extended scheduling to.</span></span>

<span data-ttu-id="a7942-134">किसी व्यक्तिगत संसाधन के बारे में अधिक जानकारी पाने के लिए उस पर राइट-क्लिक कर संसाधन कार्ड खोलें।</span><span class="sxs-lookup"><span data-stu-id="a7942-134">To view more details about an individual resource, right-click it to open the resource card.</span></span>

