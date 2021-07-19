---
title: संसाधन प्रबंधन मोड का अवलोकन
description: यह विषय Dynamics 365 Project Operations में संसाधन प्रबंधन कार्यक्षमता के बारे में जानकारी प्रदान करता है.
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.custom: intro-internal
ms.openlocfilehash: 41265534661e51565bf31105ef69cec9b3b181c3
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 07/07/2021
ms.locfileid: "6367893"
---
# <a name="resource-management-modes-overview"></a><span data-ttu-id="9264b-103">संसाधन प्रबंधन मोड ओवरव्यू</span><span class="sxs-lookup"><span data-stu-id="9264b-103">Resource management modes overview</span></span>

<span data-ttu-id="9264b-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="9264b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="9264b-105">Dynamics 365 Project Operations समग्र बुकिंग प्रवाह को निष्पादित करने हेतु आपके लिए दो मोड का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="9264b-105">Dynamics 365 Project Operations supports two modes in order for you to execute the overall booking flow.</span></span> <span data-ttu-id="9264b-106">प्रबंधन के मोड को एक परियोजना मापदंड के रूप में परिभाषित किया गया है और यदि आपके व्यवसाय को बदलने की आवश्यकता है, तो इसे संशोधित किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="9264b-106">The mode of management is defined as a project parameter and can be modified if your business needs change.</span></span>    

## <a name="central-mode"></a><span data-ttu-id="9264b-107">केंद्रीय मोड</span><span class="sxs-lookup"><span data-stu-id="9264b-107">Central mode</span></span>
<span data-ttu-id="9264b-108">परियोजनाओं के लिए संसाधनों के आवंटन को केंद्रीकृत करने वाले संगठनों के लिए, केंद्रीय मोड यह सुनिश्चित करने का एक तरीका प्रदान करता है कि परियोजना प्रबंधक परियोजना स्तर पर संसाधन आवश्यकताओं को परिभाषित कर सकें।</span><span class="sxs-lookup"><span data-stu-id="9264b-108">For organizations who centralize the allocation for resources to projects, the Central mode provides a way to ensure Project managers can define resource requirements at the project level.</span></span> <span data-ttu-id="9264b-109">संसाधन आवश्यकताओं की पूर्ति एक संसाधन प्रबंधक को सौंप दी जाती है।</span><span class="sxs-lookup"><span data-stu-id="9264b-109">Fulfillment of the resource requirements is delegated to a Resource manager.</span></span> <span data-ttu-id="9264b-110">परियोजना प्रबंधक संसाधन प्रबंधक द्वारा प्रस्तावित संसाधनों को स्वीकार या अस्वीकार कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="9264b-110">Project managers can accept or reject resources that are proposed by the Resource manager.</span></span>

![केंद्रीय मोड](./media/resource-management-central.png)

<span data-ttu-id="9264b-112">केंद्रीय मोड वाले संसाधनों का प्रबंधन करने के लिए, देखें:</span><span class="sxs-lookup"><span data-stu-id="9264b-112">To manage resources with the Central mode, see:</span></span>

- [<span data-ttu-id="9264b-113">किसी भी कार्य में जेनेरिक बुक करने-योग्य संसाधनों को असाइन करें और संसाधनों की ज़रूरतों को जेनरेट करें</span><span class="sxs-lookup"><span data-stu-id="9264b-113">Assign generic bookable resources to a task and generate resource requirements</span></span>](/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="9264b-114">संसाधनों की आवश्यकताओं से नामित संसाधनों को बुक करें</span><span class="sxs-lookup"><span data-stu-id="9264b-114">Book named resources from resource requirements</span></span>](/dynamics365/project-service/book-named-resource)
- [<span data-ttu-id="9264b-115">कोई संसाधन अनुरोध सबमिट करें</span><span class="sxs-lookup"><span data-stu-id="9264b-115">Submit a resource request</span></span>](/dynamics365/project-service/submit-resource-request)
- [<span data-ttu-id="9264b-116">संसाधन अनुरोध को पूरा करें</span><span class="sxs-lookup"><span data-stu-id="9264b-116">Fulfill a resource request</span></span>](/dynamics365/project-service/resource-management-fulfill-requests)
- [<span data-ttu-id="9264b-117">संसाधनों हेतु अनुरोध में से प्रस्तावित परियोजना के किसी संसाधन को स्वीकार या अस्वीकार करें</span><span class="sxs-lookup"><span data-stu-id="9264b-117">Accept or reject a proposed project resource from a resource request</span></span>](/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a><span data-ttu-id="9264b-118">हाइब्रिड मोड</span><span class="sxs-lookup"><span data-stu-id="9264b-118">Hybrid mode</span></span>
<span data-ttu-id="9264b-119">संसाधनों के आवंटन में लचीलापन चाहने वाले संगठनों के लिए, हाइब्रिड मोड परियोजना प्रबंधकों और संसाधन प्रबंधकों दोनों को संसाधनों को बुक करने की क्षमता देता है।</span><span class="sxs-lookup"><span data-stu-id="9264b-119">For organizations who require flexibility in the allocation of resources, the hybrid mode enables both Project managers and Resource managers the ability to book resources.</span></span>

![हाइब्रिड मोड](./media/resource-management-hybrid.png)

<span data-ttu-id="9264b-121">समर्थित केंद्रीय मोड प्रक्रिया के अलावा, हाइब्रिड मोड में अन्य सभी समर्थित बुकिंग प्रवाह को प्रबंधित करने के लिए निम्नलिखित विषयों को देखें:</span><span class="sxs-lookup"><span data-stu-id="9264b-121">In addition to the supported Central mode process, see the following topics to manage all other supported booking flows in the Hybrid mode:</span></span>

<span data-ttu-id="9264b-122">एक संसाधन सीधे परियोजना में बुक करें:</span><span class="sxs-lookup"><span data-stu-id="9264b-122">Book a resource directly to a project:</span></span>
- [<span data-ttu-id="9264b-123">एक प्रोजेक्ट टीम को बुक करने योग्य संसाधनों का नाम और कार्यों को असाइन करें</span><span class="sxs-lookup"><span data-stu-id="9264b-123">Book named bookable resources to a project team and assign tasks</span></span>](/dynamics365/project-service/assign-named-bookable-resource)

<span data-ttu-id="9264b-124">संसाधन आवश्यकता से संसाधन बुक करें:</span><span class="sxs-lookup"><span data-stu-id="9264b-124">Book a resource from a resource requirement:</span></span>
- [<span data-ttu-id="9264b-125">किसी भी कार्य में जेनेरिक बुक करने-योग्य संसाधनों को असाइन करें और संसाधनों की ज़रूरतों को जेनरेट करें</span><span class="sxs-lookup"><span data-stu-id="9264b-125">Assign generic bookable resources to a task and generate resource requirements</span></span>](/dynamics365/project-service/assign-generic-bookable-resource)
- [<span data-ttu-id="9264b-126">संसाधनों की आवश्यकताओं से नामित संसाधनों को बुक करें</span><span class="sxs-lookup"><span data-stu-id="9264b-126">Book named resources from resource requirements</span></span>](/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]