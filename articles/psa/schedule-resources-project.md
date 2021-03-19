---
title: परियोजना के लिए संसाधन शेड्यूल करें
description: Project Service में परियोजना के लिए संसाधन शेड्यूल करने का तरीका
author: JohnPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: f0a234f96419bac58cd932a082010da672e7dcb5
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5282650"
---
# <a name="schedule-resources-for-a-project-project-service"></a><span data-ttu-id="00575-103">परियोजना के लिए संसाधन शेड्यूल करना (Project Service)</span><span class="sxs-lookup"><span data-stu-id="00575-103">Schedule resources for a project (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="00575-104">आपके बुक किए गए संसाधन कैसे हैं, इसका संपूर्ण दृश्य पाने के लिए आप संसाधन उपलब्धता देख सकते हैं या आप कौशल, टीम, स्थान और अन्य विकल्पों के अनुसार दृश्य फ़िल्टर कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="00575-104">You can check resource availability to get an overall view of how booked your resources are, or you can filter the view by skills, team, location, and other options.</span></span>  
  
<span data-ttu-id="00575-105">शेड्यूल बोर्ड संसाधनों की सूची और उनकी उपलब्धता दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="00575-105">The schedule board shows list of resources and their availability.</span></span> <span data-ttu-id="00575-106">**घंटे**, **दिन**, **सप्ताह**, या **महीना** के अनुसार उपलब्धता से दिखाने के लिए दृश्य मोड का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="00575-106">Select a view mode to show availability by **Hours**, **Day**, **Week**, or **Month**.</span></span>  
  
<span data-ttu-id="00575-107">शेड्यूल बोर्ड का उपयोग करने से पहले, उसको सेट अप करना महत्वपूर्ण होता है.</span><span class="sxs-lookup"><span data-stu-id="00575-107">Before you use the schedule board, it’s important to set it up.</span></span> <span data-ttu-id="00575-108">अधिक जानकारी के लिए, [शेड्यूल बोर्ड कॉन्फ़िगर करें (Field Service या Project Service Automation)](https://docs.microsoft.com/dynamics365/field-service/configure-schedule-board).</span><span class="sxs-lookup"><span data-stu-id="00575-108">For more information, see [Configure the schedule board (Field Service or Project Service Automation)](https://docs.microsoft.com/dynamics365/field-service/configure-schedule-board).</span></span>
  
<span data-ttu-id="00575-109">यदि आप किसी पुराने संस्करण का उपयोग कर रहे हैं, तो संसाधन उपलब्धता के लिए, [संसाधन उपलब्धता देखें](../psa/view-resource-availability.md) देखें.</span><span class="sxs-lookup"><span data-stu-id="00575-109">If you are using an older version, for resource availability, see [View resource availability](../psa/view-resource-availability.md).</span></span>  

> [!IMPORTANT]
>  <span data-ttu-id="00575-110">शेड्यूल बोर्ड बुकिंग कार्यक्षमता, जियोकोडिंग, और स्‍थान सेवाओं का उपयोग करने के लिए आपको मानचित्र चालू करना होगा.</span><span class="sxs-lookup"><span data-stu-id="00575-110">To use the schedule board booking functionality, geocoding, and location services, you need to turn on maps.</span></span>  
> 
> 1. <span data-ttu-id="00575-111">मुख्य मेनू में, **संसाधन शेड्यूलिंग** > **व्यवस्थापन** चुनें.</span><span class="sxs-lookup"><span data-stu-id="00575-111">On the main menu, select **Resource Scheduling** > **Administration**.</span></span>  
> 2. <span data-ttu-id="00575-112">**शेड्यूलिंग पैरामीटर्स** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="00575-112">Click **Scheduling parameters**.</span></span>  
> 3. <span data-ttu-id="00575-113">रिकॉर्ड खोलें और **Resource Scheduling Optimization** अनुभाग तक नीचे स्क्रॉल करें.</span><span class="sxs-lookup"><span data-stu-id="00575-113">Open record and scroll down to the **Resource Scheduling Optimization** section.</span></span>  
> 4. <span data-ttu-id="00575-114">**मानचित्र से कनेक्ट करें** फ़ील्ड में, **हाँ** चुनें.</span><span class="sxs-lookup"><span data-stu-id="00575-114">On the **Connect to Maps** field, choose **Yes**.</span></span>  
> 5. <span data-ttu-id="00575-115">शर्तें स्वीकार करें और रिकॉर्ड सहेजें.</span><span class="sxs-lookup"><span data-stu-id="00575-115">Accept terms and save the record.</span></span>  
> 6. <span data-ttu-id="00575-116">मुख्य मेनू में, **Project Service** > **शेड्यूल बोर्ड** चुनें.</span><span class="sxs-lookup"><span data-stu-id="00575-116">On the main menu, select **Project Service** > **Schedule board**.</span></span> <span data-ttu-id="00575-117">यहाँ से, बुकिंग आवश्यकता को मैन्युअल रूप से शेड्यूल करने के कई तरीके हैं:</span><span class="sxs-lookup"><span data-stu-id="00575-117">From here, there are several ways to manually schedule a booking requirement.</span></span> <span data-ttu-id="00575-118">वह तरीका चुनें, जो आपके लिए कारगर हो.</span><span class="sxs-lookup"><span data-stu-id="00575-118">Choose the method that works for you.</span></span>
  
## <a name="find-available-resources"></a><span data-ttu-id="00575-119">उपलब्ध संसाधन ढूँढें</span><span class="sxs-lookup"><span data-stu-id="00575-119">Find available resources</span></span>

1.  <span data-ttu-id="00575-120">**बुकिंग आवश्यकता** सूची से, शेड्यूल न की गई बुकिंग पर राइट-क्लिक करें और निम्न में से कोई एक चुनें:</span><span class="sxs-lookup"><span data-stu-id="00575-120">From the **Booking Requirement** list, right-click an unscheduled booking and choose one of the following:</span></span>  
  
- <span data-ttu-id="00575-121">शेड्यूल बोर्ड पर सूची में से उपलब्ध संसाधन ढूँढने के लिए **उपलब्धता ढूँढें - वर्तमान संसाधन** चुनें.</span><span class="sxs-lookup"><span data-stu-id="00575-121">Choose **Find availability - Current Resources** to find an available resource from the list on the schedule board.</span></span>  
- <span data-ttu-id="00575-122">सिस्टम में मौजूद संसाधनों में से उपलब्ध संसाधन ढूँढने के लिए **उपलब्धता खोजें - सभी संसाधन** चुनें.</span><span class="sxs-lookup"><span data-stu-id="00575-122">Choose **Find availability - All Resources**, to find an available resource from resources in the system</span></span>  
   > [!NOTE]
   >  <span data-ttu-id="00575-123">ऐसा करने पर, फ़िल्टर चयनित बुकिंग आवश्यकता के लिए विकल्प दिखाएँगे.</span><span class="sxs-lookup"><span data-stu-id="00575-123">When you do this, the filters will show options for the selected booking requirement.</span></span>  
  
2. <span data-ttu-id="00575-124">एक उपलब्ध स्लॉट दिखाई देने पर, शेड्यूल बोर्ड पर स्थित समय स्लॉट पर राइट-क्लिक करें और **यहाँ बुक करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="00575-124">When you see an available slot, right-click the time slot on the schedule board and choose **Book Here**.</span></span> <span data-ttu-id="00575-125">या, बुकिंग आवश्यकता को उपलब्ध समय स्लॉट पर खींचें और छोड़ें.</span><span class="sxs-lookup"><span data-stu-id="00575-125">Or, drag and drop the booking requirement to the available time slot.</span></span>  
  

## <a name="book-a-resource-using-the-daily-view-and-find-whos-under-booked"></a><span data-ttu-id="00575-126">दैनिक दृश्य का उपयोग करके कोई संसाधन बुक करें और यह पता लगाएँ कि किसकी बुकिंग कम है</span><span class="sxs-lookup"><span data-stu-id="00575-126">Book a resource using the daily view and find who’s under-booked</span></span>
  
1.  <span data-ttu-id="00575-127">शेड्यूल बोर्ड पर, **दृश्य मोड** चुनें और **दिन** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="00575-127">On the schedule board, select **View Mode** and select **Days**.</span></span>  
  
    <span data-ttu-id="00575-128">यह इसका ग्रिड दृश्य दिखाता है कि कोई संसाधन दिन में कितने घंटे के लिए बुक किया हुआ है और किस दिन वह मुक्त है.</span><span class="sxs-lookup"><span data-stu-id="00575-128">This shows a grid view of how many hours a resource is booked per day and which days they are free.</span></span>  
  
2.  <span data-ttu-id="00575-129">आप जिस संसाधन को बुक करना चाहते हैं उसके नाम पर क्लिक करें और फिर **बुक करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="00575-129">Click the name of the resource you want to book, and then select **Book**.</span></span>  
  
3.  <span data-ttu-id="00575-130">**संसाधन बुकिंग (बनाएँ)** संवाद बॉक्स में, बुकिंग विधि तथा प्रारंभ और समाप्ति समय के साथ वह परियोजना चुनें जिसके लिए आप संसाधन बुक करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="00575-130">On the **Resource booking (create)** dialog box, choose the project that you want to book the resource for along with booking method and start and end times.</span></span>  
  
4.  <span data-ttu-id="00575-131">आपके द्वारा इसे पूर्ण कर लेने के बाद, **बुक करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="00575-131">When you’re done, select **Book**.</span></span>  
  
## <a name="view-to-the-schedule-board"></a><span data-ttu-id="00575-132">शेड्यूल बोर्ड में देखें</span><span class="sxs-lookup"><span data-stu-id="00575-132">View to the schedule board</span></span>
  
1.  <span data-ttu-id="00575-133">सबसे नीचे स्थित सूची में से शेड्यूल न की गई बुकिंग आवश्यकता का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="00575-133">Select an unscheduled booking requirement from the list at the bottom.</span></span>  
  
2.  <span data-ttu-id="00575-134">बुकिंग आवश्यकता को खींचकर शेड्यूल बोर्ड पर उपलब्‍ध संसाधन/समय स्‍लॉट पर लाएँ.</span><span class="sxs-lookup"><span data-stu-id="00575-134">Drag the booking requirement to an available resource/time slot on the schedule board.</span></span>  
  
3.  <span data-ttu-id="00575-135">आपके द्वारा इसे पूर्ण कर लेने के बाद, **बुक करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="00575-135">When you're done, select **Book**.</span></span>  
  
### <a name="additional-resources"></a><span data-ttu-id="00575-136">अतिरिक्त संसाधन</span><span class="sxs-lookup"><span data-stu-id="00575-136">Additional resources</span></span>  
 [<span data-ttu-id="00575-137">संसाधन प्रबंधक मार्गदर्शिका</span><span class="sxs-lookup"><span data-stu-id="00575-137">Resource manager guide</span></span>](../psa/resource-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]