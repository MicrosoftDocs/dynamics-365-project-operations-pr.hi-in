---
title: संसाधनों के लिए प्रभार्य उपयोग देखें
description: यह विषय संसाधन उपयोग दृश्य के बारे में जानकारी प्रदान करता है।
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/26/2019
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
ms.openlocfilehash: b07af573bc8d312c45ee4aef50c95942401294fa
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5285935"
---
# <a name="view-chargeable-utilization-for-resources"></a><span data-ttu-id="cc435-103">संसाधनों के लिए प्रभार्य उपयोग देखें</span><span class="sxs-lookup"><span data-stu-id="cc435-103">View chargeable utilization for resources</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]
 
<span data-ttu-id="cc435-104">**Project Service संसाधन उपयोगिता** पेज पर **उपयोगिता दृश्य** प्रत्येक बुक करने योग्य संसाधन के लिए प्रभार्य उपयोगिता को दर्शाता है।</span><span class="sxs-lookup"><span data-stu-id="cc435-104">The **Utilization View** on the **Project Service Resource Utilization** page shows the chargeable utilization for each bookable resource.</span></span> <span data-ttu-id="cc435-105">क्योंकि दृश्य शेड्यूल बोर्ड पर आधारित है, आप एक ही तरह के कई कार्य पाएंगे।</span><span class="sxs-lookup"><span data-stu-id="cc435-105">Because the view is based on the schedule board, you’ll find many of the same functions.</span></span>

> ![उपयोग दृश्य का स्क्रीनशॉट](media/FAQ-utilization-1.png)
 

<span data-ttu-id="cc435-107">प्रभार्य उपयोग का परिकलन इस प्रकार काम करता है:</span><span class="sxs-lookup"><span data-stu-id="cc435-107">The chargeable utilization calculation works as follows:</span></span>

   <span data-ttu-id="cc435-108">प्रभार्य उपयोग = (प्रभार्य वास्तविक घंटे) / (संसाधन क्षमता)</span><span class="sxs-lookup"><span data-stu-id="cc435-108">Chargeable utilization = (Chargeable actual hours) / (resource capacity)</span></span>

<span data-ttu-id="cc435-109">सेल चयनित अवधि (दिन, सप्ताह या महीने) के लिए परिकलित प्रभार्य उपयोगिता को दर्शाती हैं।</span><span class="sxs-lookup"><span data-stu-id="cc435-109">The cells represent the calculated chargeable utilization for the selected period (days, weeks, or months).</span></span>

<span data-ttu-id="cc435-110">प्रत्येक कक्ष में रंग किसी संसाधन लक्षित प्रभार्य उपयोग की तुलना में प्रभार्य उपयोग दिखाते हैं।</span><span class="sxs-lookup"><span data-stu-id="cc435-110">The colors in each cell show the chargeable utilization for a resource as compared to their target chargeable utilization.</span></span> 

<span data-ttu-id="cc435-111">लक्षित उपयोग को संसाधन की डिफ़ॉल्ट भूमिका या स्वयं अलग-अलग संसाधन पर सेट किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="cc435-111">The target utilization can be set on the resource’s default role or on the individual resource itself.</span></span> <span data-ttu-id="cc435-112">परिकलन लक्ष्य के लिए पहले किसी व्यक्ति विशेष को, और फिर संसाधन की डिफ़ॉल्ट भूमिका को देखता है।</span><span class="sxs-lookup"><span data-stu-id="cc435-112">The calculation looks at the individual for the target first, and then to the resource’s default role.</span></span>

## <a name="set-target-on-a-resource"></a><span data-ttu-id="cc435-113">किसी संसाधन पर लक्ष्य सेट करें</span><span class="sxs-lookup"><span data-stu-id="cc435-113">Set target on a resource</span></span>

1. <span data-ttu-id="cc435-114">**संसाधन** \> **संसाधन** पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="cc435-114">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="cc435-115">रिकॉर्ड खोलने के लिए संसाधन चुनें।</span><span class="sxs-lookup"><span data-stu-id="cc435-115">Select a resource to open the record.</span></span> 
3. <span data-ttu-id="cc435-116">**Project Service** टैब पर, आप संसाधन की लक्ष्य उपयोगिता को निर्धारित कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="cc435-116">On the **Project Service** tab, you can set the resource’s target utilization.</span></span>

> ![लक्षित उपयोग सेट करने के लिए Project Service टैब का उपयोग करने का स्क्रीनशॉट](media/FAQ-utilization-2.png)
 
## <a name="set-target-utilization-on-a-role"></a><span data-ttu-id="cc435-118">किसी भूमिका पर लक्ष्य उपयोग सेट करें</span><span class="sxs-lookup"><span data-stu-id="cc435-118">Set target utilization on a role</span></span>

1. <span data-ttu-id="cc435-119">**संसाधन** \> **संसाधन भूमिकाएं** पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="cc435-119">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="cc435-120">किसी रोल का चयन करें और रिकॉर्ड खोलें।</span><span class="sxs-lookup"><span data-stu-id="cc435-120">Select a role and open the record.</span></span> 
3. <span data-ttu-id="cc435-121">भूमिका के लिए लक्षित उपयोग सेट करें।</span><span class="sxs-lookup"><span data-stu-id="cc435-121">Set the target utilization for the role.</span></span>

> ![लक्षित उपयोग सेट करने के लिए संसाधन भूमिकाएँ का उपयोग करने का स्क्रीनशॉट](media/FAQ-utilization-3.png)
 
## <a name="calculate-chargeable-utilization-for-a-resource"></a><span data-ttu-id="cc435-123">किसी संसाधन के लिए प्रभार्य उपयोग का परिकलन करें</span><span class="sxs-lookup"><span data-stu-id="cc435-123">Calculate chargeable utilization for a resource</span></span>

<span data-ttu-id="cc435-124">किसी संसाधन के लिए प्रभार्य उपयोग का परिकलन करने के लिए, आपको कुछ पूर्वावश्यकताओं को पूरा करना होगा।</span><span class="sxs-lookup"><span data-stu-id="cc435-124">To calculate chargeable utilization for a resource, you will need to complete some pre-requisites.</span></span> 

### <a name="set-default-role-for-individual-resource"></a><span data-ttu-id="cc435-125">अलग-अलग संसाधन के लिए डिफ़ॉल्ट भूमिका सेट करें</span><span class="sxs-lookup"><span data-stu-id="cc435-125">Set default role for individual resource</span></span>

<span data-ttu-id="cc435-126">पहले, लक्षित उपयोग को अलग-अलग संसाधन या संसाधन भूमिकाओं पर सेट किया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="cc435-126">First, the target utilization must be set on either the individual resource or on resource roles.</span></span> <span data-ttu-id="cc435-127">यदि आप लक्ष्य के लिए संसाधन भूमिकाओं का उपयोग कर रहे हैं, तो प्रत्येक अलग-अलग संसाधन की एक डिफ़ॉल्ट भूमिका होनी चाहिए।</span><span class="sxs-lookup"><span data-stu-id="cc435-127">If you are using resource roles for targets, each individual resource must have a default role.</span></span> 

1. <span data-ttu-id="cc435-128">इसे सेट करने के लिए, **संसाधन** \> **संसाधन** पर जाएँ।</span><span class="sxs-lookup"><span data-stu-id="cc435-128">To set this, go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="cc435-129">किसी संसाधन का चयन करें, रिकॉर्ड खोलें, और फिर **Project Service** टैब का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="cc435-129">Select a resource, open the record, and then select the **Project Service** tab.</span></span> 
3. <span data-ttu-id="cc435-130">**संसाधन भूमिका** ग्रिड में, सुनिश्चित करें कि संसाधन के लिए एक भूमिका है और **डिफ़ॉल्ट** **हां** पर सेट है।</span><span class="sxs-lookup"><span data-stu-id="cc435-130">In the **Resource Role** grid, make sure there’s one role for the resource and **Is Default** is set to **Yes**.</span></span>
 
### <a name="change-billing-type-for-resource-role"></a><span data-ttu-id="cc435-131">संसाधन भूमिका के लिए बिलिंग प्रकार बदलें</span><span class="sxs-lookup"><span data-stu-id="cc435-131">Change billing type for resource role</span></span>

<span data-ttu-id="cc435-132">संसाधन भूमिकाओं को **प्रभार्य** के बिलिंग प्रकार के लिए सेट किया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="cc435-132">The resource roles must be set to have a billing type of **Chargeable**.</span></span> 

1. <span data-ttu-id="cc435-133">**संसाधन** \> **संसाधन भूमिकाएं** पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="cc435-133">Go to **Resources** \> **Resource Roles**.</span></span> 
2. <span data-ttu-id="cc435-134">वह रिकॉर्ड खोलें जिसे आप अद्यतन करना चाहते हैं, और फिर बिलिंग प्रकार डिफ़ॉल्ट को **प्रभार्य** पर सेट करें।</span><span class="sxs-lookup"><span data-stu-id="cc435-134">Open the record you want to update, and then set the billing type default to **Chargeable**.</span></span>

### <a name="set-working-hours-for-resource-role"></a><span data-ttu-id="cc435-135">संसाधन भूमिका के लिए कार्य घंटे सेट करें</span><span class="sxs-lookup"><span data-stu-id="cc435-135">Set working hours for resource role</span></span>
 
<span data-ttu-id="cc435-136">परिकलन क्षमता के लिए संसाधन के पास कार्य के घंटे होना आवश्यक है।</span><span class="sxs-lookup"><span data-stu-id="cc435-136">The resource must have working hours for the capacity calculation.</span></span> 

1. <span data-ttu-id="cc435-137">**संसाधन** \> **संसाधन** पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="cc435-137">Go to **Resources** \> **Resources**.</span></span> 
2. <span data-ttu-id="cc435-138">रिकॉर्ड खोलने के लिए संसाधन चुनें, और फिर **कार्य के घंटे दिखाएँ** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="cc435-138">Select a resource to open the record, and then select **Show Work Hours**.</span></span> 
3. <span data-ttu-id="cc435-139">आप **संसाधन सूची** दृश्य से **कार्य घंटे टेम्पलेट** लागू करके संसाधनों की सूची का सामूहिक-अद्यतन कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="cc435-139">You can bulk-update the list of resources by applying a **Work Hour Template** from the **Resource List** view.</span></span>

## <a name="troubleshooting-chargeable-actual-hours"></a><span data-ttu-id="cc435-140">समस्या निवारण प्रभार्य वास्तविक घंटे</span><span class="sxs-lookup"><span data-stu-id="cc435-140">Troubleshooting chargeable actual hours</span></span>

<span data-ttu-id="cc435-141">प्रभार्य वास्तविक घंटे **वास्तविक** निकाय से लिए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="cc435-141">The chargeable actual hours are sourced from the **Actuals** entity.</span></span> <span data-ttu-id="cc435-142">**प्रभार्य** के बिलिंग प्रकार वाले वास्तविक परिकलन में शामिल होते हैं और, इस कारण से आपके पास ऐसे प्रोजेक्ट्स होने चाहिए जहाँ वास्तविक प्रभार्य हैं।</span><span class="sxs-lookup"><span data-stu-id="cc435-142">Actuals with a billing type of **Chargeable** are included in the calculation and, for this reason, you must have projects where the actuals that are chargeable.</span></span>

<span data-ttu-id="cc435-143">यदि आप प्रभार्य उपयोग नहीं देख रहे हैं, तो यहाँ कुछ चीज़ें दी गई हैं जिन्हें आप देख सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="cc435-143">If you are not seeing chargeable utilization, here are some things you can check:</span></span>

- <span data-ttu-id="cc435-144">संसाधन के पास क्षमता के लिए निर्धारित किए गए कार्य के घंटे हैं।</span><span class="sxs-lookup"><span data-stu-id="cc435-144">The resource has working hours defined for capacity.</span></span>
- <span data-ttu-id="cc435-145">संसाधन के पास अलग-अलग निर्धारित उपयोग लक्ष्य है या उसे एक डिफ़ॉल्ट भूमिका असाइन की गई है।</span><span class="sxs-lookup"><span data-stu-id="cc435-145">The resource has either an individually defined utilization target or has a default role assigned to it.</span></span> <span data-ttu-id="cc435-146">भूमिका के लिए उपयोग लक्ष्य निर्धारित है।</span><span class="sxs-lookup"><span data-stu-id="cc435-146">The role has a utilization target defined for it.</span></span>
- <span data-ttu-id="cc435-147">वास्तविक के पास उस अवधि के लिए **प्रभार्य** का बिलिंग प्रकार है जिसके लिए आप उपयोग के परिकलन की अपेक्षा कर रहे हैं।</span><span class="sxs-lookup"><span data-stu-id="cc435-147">Actuals have a billing type of **Chargeable** for the period you are expecting a utilization calculation for.</span></span> <span data-ttu-id="cc435-148">निम्नलिखित को जांचें कि क्या आप वास्तविक को प्रभार्य के अलावा बिलिंग प्रकारों के साथ देख रहे हैं:</span><span class="sxs-lookup"><span data-stu-id="cc435-148">Check the following if you are seeing actuals with billing types other than chargeable:</span></span>

  - <span data-ttu-id="cc435-149">वास्तविक में उपयोग की गई भूमिका में प्रभार्य के अलावा कोई अन्य डिफ़ॉल्ट बिलिंग प्रकार है।</span><span class="sxs-lookup"><span data-stu-id="cc435-149">The role used on the actual has a default billing type of something other than chargeable.</span></span>
  - <span data-ttu-id="cc435-150">प्रोजेक्ट का समर्थन करने वाली प्रोजेक्ट अनुबंध पंक्ति में भूमिका को गैर-प्रभार्य पर सेट किया गया है।</span><span class="sxs-lookup"><span data-stu-id="cc435-150">The role on the project contract line backing the project has been set to non-chargeable.</span></span>
  - <span data-ttu-id="cc435-151">प्रोजेक्ट की कोई संबद्ध अनुबंध पंक्ति नहीं है।</span><span class="sxs-lookup"><span data-stu-id="cc435-151">The project does not have an associated contract line.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]