---
title: परियोजना कैलेंडर परिभाषित करें
description: यह विषय परियोजना शेड्यूल को ट्रैक करने के लिए परियोजना कैलेंडर इस्तेमाल करने के बारे में जानकारी देता है.
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
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
ms.openlocfilehash: e25b11b6b947627ca2ac88952e74aecccc346c89
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286970"
---
# <a name="define-project-calendars"></a><span data-ttu-id="a6c4e-103">परियोजना कैलेंडर परिभाषित करें</span><span class="sxs-lookup"><span data-stu-id="a6c4e-103">Define project calendars</span></span>

<span data-ttu-id="a6c4e-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="a6c4e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a6c4e-105">प्रोजेक्ट शेड्यूल बनाने के लिए, आपको प्रोजेक्ट कैलेंडर टैम्पलेट बनाना होगा जिसमें प्रति दिन के कार्य घंटे और किसी कारोबार के बंद होने की संख्या परिभाषित की जाती है।</span><span class="sxs-lookup"><span data-stu-id="a6c4e-105">To create a project schedule, you create a project calendar template that defines the number of working hours per day and any business closures.</span></span> <span data-ttu-id="a6c4e-106">प्रोजेक्ट कैलेंडर टैम्पलेट बनाने के लिए, आपको प्रोजेक्ट के **कैलेंडर टैम्पलेट** फील्ड के साथ कार्य टैम्पलेट से जुड़ना होगा.</span><span class="sxs-lookup"><span data-stu-id="a6c4e-106">To create a project calendar template, you associate a work template with the **Calendar template** field for the project.</span></span> <span data-ttu-id="a6c4e-107">कार्य टैम्पलेट बनाने के लिए निम्नलिखित चरणों को पूरा करें।</span><span class="sxs-lookup"><span data-stu-id="a6c4e-107">Follow these steps to create a work template.</span></span>

1. <span data-ttu-id="a6c4e-108">बाएँ नेविगेशन फलक में, **संसाधन** चुनें.</span><span class="sxs-lookup"><span data-stu-id="a6c4e-108">In the left navigation pane, select **Resources**.</span></span> 
2. <span data-ttu-id="a6c4e-109">**संसाधन** लिस्ट पेज में, यूज़र रिकार्ड खालें और उसके बाद **काम के घंटे दिखाएं** चुनें।</span><span class="sxs-lookup"><span data-stu-id="a6c4e-109">On the **Resources** list page, open a user record, and then select **Show Work Hours**.</span></span>

  > [!NOTE]
  > <span data-ttu-id="a6c4e-110">सुनिश्चित करें कि आप ब्राउज़र पेज में पॉप-अप को अनुमत करते हैं।</span><span class="sxs-lookup"><span data-stu-id="a6c4e-110">Make sure that you allow pop-ups on the browser page.</span></span> <span data-ttu-id="a6c4e-111">इससे आप संसाधन के कार्य के घंटे देख सकेंगे।</span><span class="sxs-lookup"><span data-stu-id="a6c4e-111">This lets you see the work hours set for the resource.</span></span>
  
3. <span data-ttu-id="a6c4e-112">**मासिक दृश्य** टैब पर, **सेट अप** चुनें.</span><span class="sxs-lookup"><span data-stu-id="a6c4e-112">On the **Monthly View** tab, select **Set Up**.</span></span> <span data-ttu-id="a6c4e-113">तीन विकल्पों की सूची दिखेगा:</span><span class="sxs-lookup"><span data-stu-id="a6c4e-113">A list of three options appears:</span></span> 

  - <span data-ttu-id="a6c4e-114">नया साप्ताहिक शेड्यूल</span><span class="sxs-lookup"><span data-stu-id="a6c4e-114">New Weekly Schedule</span></span>
  - <span data-ttu-id="a6c4e-115">एक दिन के लिए कार्य शेड्यूल</span><span class="sxs-lookup"><span data-stu-id="a6c4e-115">Work Schedule for One Day</span></span>
  - <span data-ttu-id="a6c4e-116">टाइम ऑफ़</span><span class="sxs-lookup"><span data-stu-id="a6c4e-116">Time Off</span></span>

4. <span data-ttu-id="a6c4e-117">**नया साप्ताहिक शेड्यूल** चुनें और उसके बाद इस रिसोर्स के शेड्यूल के लिए ऑप्शन सेट करें।</span><span class="sxs-lookup"><span data-stu-id="a6c4e-117">Select **New Weekly Schedule**, and then set the options for this resource schedule.</span></span> <span data-ttu-id="a6c4e-118">इसमें आप आवर्ती साप्ताहिक शेड्यूल, दैनिक घंटा पैरामीटर, कारोबार समाप्ति जैसी कई सुविधाएँ सेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a6c4e-118">You can set a recurring weekly schedule, daily hour parameters, business closures, and more.</span></span>
5. <span data-ttu-id="a6c4e-119">डेट रेंज सेट करें, **सहेजें** चुनें और उसके बाद **बंद करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="a6c4e-119">Set the date range, select **Save**, and then select **Close**.</span></span> 
6. <span data-ttu-id="a6c4e-120">**संसाधन** लिस्ट पेज पर वापस जाएँ और उस संसाधन को चुनें जिसे आपने कार्य घंटों के लिए सेट किया था।</span><span class="sxs-lookup"><span data-stu-id="a6c4e-120">Go back to the **Resources** list page, and select the resource that you set the work hours for.</span></span> 
7. <span data-ttu-id="a6c4e-121">कार्य टैम्पलेट सेट करने के लिए **कैलेंडर को इस रूप में सेट करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="a6c4e-121">Select **Set Calendar As** to set the work template.</span></span> 
8. <span data-ttu-id="a6c4e-122">**कार्य टेम्‍पलेट** डॉयलॉग बॉक्स में कार्य टैम्पलेट का नाम दर्ज करें और उसके बाद **लागू करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="a6c4e-122">In the **Work Template** dialog box, enter a name for the work template, and then select **Apply**.</span></span> 

<span data-ttu-id="a6c4e-123">अब आप वर्क टैम्पलेट को प्रोजेक्ट कैलेंडर के टैम्पलेट से जोड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="a6c4e-123">You can now associate the work template with a project calendar template.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]