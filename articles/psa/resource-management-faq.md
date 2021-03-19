---
title: संसाधन प्रबंधन FAQ
description: यह विषय संसाधन प्रबंधन के बारे में अक्सर पूछे जाने वाले प्रश्नों के उत्तर प्रदान करता है।
author: ruhercul
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: 20562b98ccc8451ab57dd42fb8c2f9f303811dbe
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5283145"
---
# <a name="resource-management-faq"></a><span data-ttu-id="a2b8b-103">संसाधन प्रबंधन FAQ</span><span class="sxs-lookup"><span data-stu-id="a2b8b-103">Resource management FAQ</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

## <a name="what-is-the-difference-between-a-team-member-and-a-resource-requirement"></a><span data-ttu-id="a2b8b-104">टीम के सदस्य और संसाधन की आवश्यकता के बीच क्या अंतर है?</span><span class="sxs-lookup"><span data-stu-id="a2b8b-104">What is the difference between a team member and a resource requirement?</span></span>

<span data-ttu-id="a2b8b-105">एक परियोजना टीम के सदस्य को कार्य सौंपा जा सकता है, बुक किया जा सकता है या ओवरबुक किया जा सकता है, और एक अनुमोदनकर्ता के रूप में स्थापित किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-105">A project team member can be assigned to tasks, booked or overbooked, and set as an approver.</span></span> <span data-ttu-id="a2b8b-106">एक संसाधन की आवश्यकता डिमांड के ड्राफ्ट नोट के रूप में, एक परियोजना टीम के सदस्य के बिना मौजूद हो सकती है।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-106">A resource requirement can exist without a project team member, as a draft note of demand.</span></span> 

## <a name="what-is-the-difference-between-proposed-and-soft-booked-hours"></a><span data-ttu-id="a2b8b-107">प्रस्तावित और सॉफ्ट-बुक किए गए घंटों के बीच क्या अंतर है?</span><span class="sxs-lookup"><span data-stu-id="a2b8b-107">What is the difference between proposed and soft-booked hours?</span></span>

<span data-ttu-id="a2b8b-108">प्रस्तावित घंटे और सॉफ्ट-बुक किए गये घंटे दृश्यता में भिन्न होते हैं।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-108">Proposed hours and soft-booked hours differ in visibility.</span></span> <span data-ttu-id="a2b8b-109">प्रस्तावित घंटे केवल संसाधन प्रबंधकों और परियोजना प्रबंधक को दिखाई देते हैं जिन्होंने संसाधन अनुरोध का उपयोग करके मांग आरंभ की है।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-109">Proposed hours are visible only to resource managers and the project manager who initiated the demand by using a resource request.</span></span> <span data-ttu-id="a2b8b-110">सॉफ्ट-बुक घंटे अनुसूची बोर्ड तक पहुंच रखने वाले किसी भी व्यक्ति को दिखाई देते हैं।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-110">Soft-booked hours are visible to anyone who has access to the Schedule Board.</span></span>

## <a name="how-can-i-see-the-soft-booked-hours-for-resources-on-a-team"></a><span data-ttu-id="a2b8b-111">मैं किसी टीम पर संसाधनों के लिए सॉफ्ट-बुक किए गए घंटे कैसे देख सकता हूं?</span><span class="sxs-lookup"><span data-stu-id="a2b8b-111">How can I see the soft-booked hours for resources on a team?</span></span>

<span data-ttu-id="a2b8b-112">जब आप संसाधन की आवश्यकता को बुक करते हैं तो सॉफ्ट बुकिंग की जा सकती है।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-112">Soft bookings can made when you book a resource requirement.</span></span> <span data-ttu-id="a2b8b-113">संसाधन जो किसी प्रोजेक्ट टीम पर सॉफ्ट-बुक किए जाते हैं, टीम के सदस्यों के रूप में दिखाई देते हैं, जिनके पास सॉफ्ट-बुक्ड घंटे हैं।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-113">Resources that are soft-booked on a project team appear as team members who have soft-booked hours.</span></span> <span data-ttu-id="a2b8b-114">वे शेड्यूल बोर्ड में भी दिखाई देते हैं।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-114">They also appear on the Schedule Board.</span></span>

## <a name="how-do-i-change-the-required-hours-and-the-start-and-end-dates-for-a-resource-generic-or-named-that-i-booked"></a><span data-ttu-id="a2b8b-115">संसाधन (सामान्य या नामित) जिसे मैंने बुक किया था, उसके लिए मैं आवश्यक घंटों और आरंभ और समाप्ति तिथियों को कैसे बदल सकता हूँ?</span><span class="sxs-lookup"><span data-stu-id="a2b8b-115">How do I change the required hours, and the start and end dates, for a resource (generic or named) that I booked?</span></span>

<span data-ttu-id="a2b8b-116">संसाधन बुक होने के बाद, आवश्यक परिवर्तन करने के लिए **बुकिंग बनाए रखें** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-116">After resources are booked, select **Maintain Bookings** to make any changes that are required.</span></span>

## <a name="what-resources-types-does-project-service-automation-support"></a><span data-ttu-id="a2b8b-117">Project Service Automation कौन से संसाधन प्रकार का समर्थन करते हैं?</span><span class="sxs-lookup"><span data-stu-id="a2b8b-117">What resources types does Project Service Automation support?</span></span>

<span data-ttu-id="a2b8b-118">**उपयोगकर्ता** और **संपर्क** ही केवल वे संसाधन प्रकार हैं, जो Microsoft Dynamics 365 Project Service Automation में समर्थित हैं।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-118">**User** and **Contact** are the only resource types that are supported in Dynamics 365 Project Service Automation.</span></span> <span data-ttu-id="a2b8b-119">यद्यपि आप अन्य प्रकार के संसाधन बना सकते हैं (उदाहरण के लिए, **उपकरण** और **समूह**), उनके लिए कोई आद्योपान्त प्रक्रिया नहीं है।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-119">Although you can create other types of resources (for example, **Equipment** and **Group**), no end-to-end use case is supported for them.</span></span>

## <a name="what-is-the-difference-between-an-assignment-and-a-booking"></a><span data-ttu-id="a2b8b-120">असाइनमेंट और बुकिंग में क्या अंतर है?</span><span class="sxs-lookup"><span data-stu-id="a2b8b-120">What is the difference between an assignment and a booking?</span></span>

<span data-ttu-id="a2b8b-121">असाइनमेंट्स, प्रोजेक्ट शेड्यूल में प्रोजेक्ट कार्यों के लिए संसाधनों का असाइनमेंट हैं।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-121">Assignments are the assignment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="a2b8b-122">संसाधन, वास्तविक या सामान्य संसाधन हो सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-122">The resources can be either real or generic resources.</span></span> <span data-ttu-id="a2b8b-123">बुकिंग किसी परियोजना के लिए संसाधनों का कठिन या आसान आवंटन है।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-123">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="a2b8b-124">हार्ड बुकिंग किसी संसाधन की क्षमता का उपभोग करते हैं।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-124">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="a2b8b-125">आदर्श रूप से, वास्तविक संसाधनों के लिए, बुकिंग और असाइनमेंट आपस में सहमत होना चाहिए, क्योंकि वे अलग नहीं हैं।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-125">Ideally, for real resources, the bookings and assignments should agree, because they don't differ.</span></span> <span data-ttu-id="a2b8b-126">हालाँकि, PSA इस समझौते को लागू नहीं करता है।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-126">However, PSA doesn't enforce this agreement.</span></span> <span data-ttu-id="a2b8b-127">समायोजन दृश्य एक परियोजना प्रबंधक स्थानों को दिखाता है, जहां संसाधन की बुकिंग और असाइनमेंट सहमत नहीं होते हैं।</span><span class="sxs-lookup"><span data-stu-id="a2b8b-127">The Reconciliation view shows a project manager places where a resource's bookings and assignments don't agree.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]