---
title: संसाधन प्रबंधक मार्गदर्शिका
description: Project Service में संसाधन प्रबंधन मार्गदर्शिका
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 4a26a384dfaf6b974ed35105434152e655ff6444
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077908"
---
# <a name="resource-manager-guide-project-service"></a><span data-ttu-id="64019-103">संसाधन प्रबंधक मार्गदर्शिका (Project Service)</span><span class="sxs-lookup"><span data-stu-id="64019-103">Resource manager guide (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="64019-104">[!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] में [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] क्षमताएँ आपको सही परियोजना के लिए सही समय पर सही संसाधन ढूँढ़ने और सभी संसाधनों का दक्षतापूर्वक उपयोग सुनिश्चित करने में मदद करती हैं.</span><span class="sxs-lookup"><span data-stu-id="64019-104">The [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] help you find the right resources at the right time for the right project and make sure all resources are utilized efficiently.</span></span>  
  
 <span data-ttu-id="64019-105">[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] के साथ अपनी कंपनी के सलाहकार दक्षता के साथ और प्रभावी रूप से परिनियोजित करें.</span><span class="sxs-lookup"><span data-stu-id="64019-105">Deploy your company’s consultants efficiently and effectively with the [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)].</span></span> <span data-ttu-id="64019-106">यह आपको वे उपकरण प्रदान करती हैं जिनकी आवश्‍यकता आपको अपनी आवश्‍यकताओं, परामर्शक परियोजनाओं के शेड्यूल और अपने परामर्शकों के कौशल और उपलब्‍धता के आधार पर संसाधन शेड्यूल करने में पड़ती है.</span><span class="sxs-lookup"><span data-stu-id="64019-106">These provide you with the tools you need to schedule resources based on the requirements and schedules of consulting projects and on the skills and availability of your consultants.</span></span> <span data-ttu-id="64019-107">आप शीघ्रता से सर्वाधिक योग्‍य परामर्शक ढूँढ़ सकते हैं, जो परियोजनाओं पर कार्य करने के लिए उपलब्ध हैं, और आप आसानी दे देख सकते हैं कि कैसे उन्‍हें प्रत्‍येक परियोजना के कार्यों के दौरान बेहतर तरीके से शेड्यूल किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="64019-107">You can quickly find the most qualified consultants who are available to work on projects, and you can easily see how to better schedule them during the course of each project.</span></span>  
  
 <span data-ttu-id="64019-108">संसाधन शेड्यूलिंग आपकी निम्न कार्य करने में मदद करती है:</span><span class="sxs-lookup"><span data-stu-id="64019-108">Resource scheduling helps you do the following:</span></span>  
  
- <span data-ttu-id="64019-109">परियोजनाओं के लिए संसाधनों का मेल कराने में, यह इस बात पर निर्भर करता है कि उनका कौशल और दक्षता स्‍तर कितनी अच्छी तरह से परियोजना संसाधन आवश्‍यकताओं के साथ मेल खाता है.</span><span class="sxs-lookup"><span data-stu-id="64019-109">Match resources to projects, based on how well their skills and proficiency levels match the project resource requirements.</span></span>  
  
- <span data-ttu-id="64019-110">किसी संसाधन के शेड्यूल को किसी परियोजना कैलेंडर के साथ मेल कराने में, यह इस बात पर आधारित होता है कि उनकी उपलब्‍धता क्‍या है और शेड्यूल किए गए विराम कितने हैं.</span><span class="sxs-lookup"><span data-stu-id="64019-110">Match a resource’s schedule to a project calendar, based on their availability and scheduled time off.</span></span> <span data-ttu-id="64019-111">रंग-कोड युक्त कैलेंडर आपको संसाधनों की उपलब्‍धता के बारे में दृश्य क्‍यू प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="64019-111">The color-coded calendar gives you visual cues about resource availability.</span></span>  
  
- <span data-ttu-id="64019-112">प्रत्येक परामर्शक की क्षमता की समीक्षा करें और निर्धारित करें कि उस क्षमता का उपयोग कैसे किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="64019-112">Review the capacity of each consultant and determine how that capacity is currently used.</span></span> <span data-ttu-id="64019-113">इससे आपको यह पता लगाने में मदद मिल सकती है कि कहाँ आपके परामर्शक का उपयोग क्षमता से कम हो सकता है, कहाँ अधिक, या क्‍या वे अपनी क्षमता के अनुसार कार्य कर रहे हैं अथवा नहीं.</span><span class="sxs-lookup"><span data-stu-id="64019-113">This can help you find where a consultant might be under- or over-utilized, or if they’re working at capacity.</span></span>  
  
- <span data-ttu-id="64019-114">एक परियोजना के लिए किसी कर्मचारी को उसकी क्षमता के अनुसार प्रतिशत या कार्य के घंटों की निर्धारित संख्या असाइन करें.</span><span class="sxs-lookup"><span data-stu-id="64019-114">Assign a percentage or a specific number of hours for a worker’s capacity to a project.</span></span>  
  
- <span data-ttu-id="64019-115">समूह संसाधन बुकिंग बनाएँ.</span><span class="sxs-lookup"><span data-stu-id="64019-115">Make group resource bookings.</span></span>  
  
- <span data-ttu-id="64019-116">संसाधनों को सॉफ़्ट बुक या हार्ड बुक करें और एक चरण में सॉफ़्ट-बुक घंटों को हार्ड-बुक घंटों में परिवर्तित करें.</span><span class="sxs-lookup"><span data-stu-id="64019-116">Soft book or hard book resources, and convert soft-booked hours into hard-booked hours in one step.</span></span>  
  
- <span data-ttu-id="64019-117">स्‍वचालित रूप से एक ऐसी परियोजना टीम बनाएँ, जो परियोजना के लिए कार्य विश्लेषण संरचना में परिभाषित संसाधनों पर आधारित हो.</span><span class="sxs-lookup"><span data-stu-id="64019-117">Automatically form a project team based on resources defined in a work breakdown structure for a project.</span></span>  
  
- <span data-ttu-id="64019-118">संसाधन अनुरोधों (बुक करने, प्रस्तावित करने, प्रतिस्थापक संसाधनों को ढूँढ़ने) को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="64019-118">Fulfill resource requests (book, propose, find substitute resources).</span></span>  
  
- <span data-ttu-id="64019-119">एक केंद्रीय मॉडल (संसाधन प्रबंधक असाइन करता है) या हाइब्रिड मॉडल (संसाधन प्रबंधक और अन्य प्रबंधक असाइन कर सकते हैं) के अनुसार संसाधन असाइन करें.</span><span class="sxs-lookup"><span data-stu-id="64019-119">Assign resources according to a central (resource manager assigns) or hybrid model (resource manager and other managers can assign).</span></span> <span data-ttu-id="64019-120">एक केंद्रीय बनाम हाइब्रिड संसाधन प्रबंधन मॉडल सेट करने के बारे में अधिक जानकारी के लिए, [अतिरिक्त पैरामीटर सेटिंग कॉन्फ़िगर करें (Project Service)](../psa/configure-additional-parameters-settings.md) देखें.</span><span class="sxs-lookup"><span data-stu-id="64019-120">For more information about setting a central versus hybrid resource management model, see [Configure additional parameters settings (Project Service)](../psa/configure-additional-parameters-settings.md).</span></span>  
  
  <span data-ttu-id="64019-121">आप समूची परियोजना में संसाधनों को दक्षतापूर्वक प्रबंधित कर सकते हैं और सुनिश्चित कर सकते हैं कि उस परियोजना में उचित रूप से स्‍टाफ़ दिया गया है.</span><span class="sxs-lookup"><span data-stu-id="64019-121">You can manage resources efficiently across projects and ensure that projects are staffed appropriately.</span></span> <span data-ttu-id="64019-122">आपको निम्न कार्य करना आवश्‍यक है:</span><span class="sxs-lookup"><span data-stu-id="64019-122">You’ll need to perform the following tasks:</span></span>  
  
- <span data-ttu-id="64019-123">[संसाधन अनुरोध प्रबंधित करें](../psa/manage-resource-requests.md).</span><span class="sxs-lookup"><span data-stu-id="64019-123">[Manage resource requests](../psa/manage-resource-requests.md).</span></span> <span data-ttu-id="64019-124">अपने परामर्शकों की कौशल दक्षताएँ, सही परियोजनाओं के साथ मेल कराएँ.</span><span class="sxs-lookup"><span data-stu-id="64019-124">Match the skills and proficiencies of your consultants to the right projects.</span></span>  
  
- <span data-ttu-id="64019-125">[संसाधन की उपलब्धता देखें](../psa/view-resource-availability.md).</span><span class="sxs-lookup"><span data-stu-id="64019-125">[View resource availability](../psa/view-resource-availability.md).</span></span> <span data-ttu-id="64019-126">कैलेंडर दृश्य में परामर्शकों की उपलब्धता की जाँच करें.</span><span class="sxs-lookup"><span data-stu-id="64019-126">Check consultants’ availability in a calendar view.</span></span>  
  
- <span data-ttu-id="64019-127">[संसाधन उपयोग देखें](../psa/view-resource-utilization.md).</span><span class="sxs-lookup"><span data-stu-id="64019-127">[View resource utilization](../psa/view-resource-utilization.md).</span></span> <span data-ttu-id="64019-128">वह समय प्रतिशत देखें जिनमें आपके परामर्शक वर्तमान में बुक हैं.</span><span class="sxs-lookup"><span data-stu-id="64019-128">See the percentage of time that your consultants are currently booked.</span></span>  
  
- <span data-ttu-id="64019-129">[परियोजना के लिए संसाधन शेड्यूल करें](../psa/schedule-resources-project.md).</span><span class="sxs-lookup"><span data-stu-id="64019-129">[Schedule resources for a project](../psa/schedule-resources-project.md).</span></span> <span data-ttu-id="64019-130">प्रोजेक्ट के लिए सलाहकार शेड्यूल करें.</span><span class="sxs-lookup"><span data-stu-id="64019-130">Schedule consultants for a project.</span></span>  
  
  <span data-ttu-id="64019-131">अलग-अलग परियोजनाओं के लिए संसाधन अनुरोधों को सबमिट करने के बारे में अधिक जानकारी के लिए, [संसाधन अनुरोध सबमिट करें](../psa/submit-resource-requests.md)  देखें.</span><span class="sxs-lookup"><span data-stu-id="64019-131">For more information about submitting resource requests for individual projects, see [Submit resource requests](../psa/submit-resource-requests.md).</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="64019-132">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="64019-132">See Also</span></span>  
 <span data-ttu-id="64019-133">[Project Service का ओवरव्यू](../psa/overview.md) </span><span class="sxs-lookup"><span data-stu-id="64019-133">[Overview of Project Service](../psa/overview.md) </span></span>  
 <span data-ttu-id="64019-134">[व्यवस्थापक मार्गदर्शिका](../psa/admin-guide.md) </span><span class="sxs-lookup"><span data-stu-id="64019-134">[Administrator Guide](../psa/admin-guide.md) </span></span>  
 <span data-ttu-id="64019-135">[खाता प्रबंधक मार्गदर्शिका](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="64019-135">[Account Manager Guiden](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="64019-136">[परियोजना प्रबंधक मार्गदर्शिका](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="64019-136">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 [<span data-ttu-id="64019-137">समय, व्यय और सहयोग मार्गदर्शिका</span><span class="sxs-lookup"><span data-stu-id="64019-137">Time, Expense, and Collaboration Guide</span></span>](../psa/time-expense-collaboration-guide.md)
