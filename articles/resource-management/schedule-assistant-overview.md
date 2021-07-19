---
title: शेड्यूल सहायक का अवलोकन
description: यह विषय पुस्तक संसाधनों के लिए अनुसूची सहायक के साथ काम करने के बारे में जानकारी प्रदान करता है।
author: ruhercul
ms.date: 10/01/2020
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.custom: intro-internal
ms.openlocfilehash: 83583c97e4ecb5f1fdc0d8d98098afe8e12d27e4
ms.sourcegitcommit: 0fafe022731f0e1e8693382ff906e3f8541d34ca
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 07/07/2021
ms.locfileid: "6368118"
---
# <a name="schedule-assistant-overview"></a><span data-ttu-id="7c569-103">शेड्यूल सहायक का अवलोकन</span><span class="sxs-lookup"><span data-stu-id="7c569-103">Schedule assistant overview</span></span>

<span data-ttu-id="7c569-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="7c569-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="7c569-105">अनुसूची सहायक का उपयोग परियोजना प्रबंधक द्वारा परिभाषित आवश्यकताओं के आधार पर संसाधनों को बुक करने के लिए किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="7c569-105">The Schedule assistant is used to book resources based on requirements defined by the Project manager.</span></span> <span data-ttu-id="7c569-106">अनुसूची सहायक संसाधन खोजने के लिए संसाधन आवश्यकता में दिए गए मापदंडों पर निर्भर करता है।</span><span class="sxs-lookup"><span data-stu-id="7c569-106">The schedule assistant relies on the parameters provided in the resource requirement to find the resource.</span></span> <span data-ttu-id="7c569-107">अनुसूची सहायक उन संसाधनों की सिफारिश करता है, जो प्रासंगिक आवश्यकताओं से मेल खाते हैं, जैसे कि टाइम विंडो या ज़रूरी कौशल।</span><span class="sxs-lookup"><span data-stu-id="7c569-107">The Schedule assistant recommends resources that match relevant requirements, like time windows or skills needed.</span></span>

<span data-ttu-id="7c569-108">उपयुक्त संसाधनों की पहचान होने के बाद, संसाधन या परियोजना प्रबंधक कार्य के लिए संसाधन बुक कर सकता है।</span><span class="sxs-lookup"><span data-stu-id="7c569-108">After suitable resources are identified, the Resource or Project manager can book the resource to the work.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c569-109">पूर्वावश्यकताएँ</span><span class="sxs-lookup"><span data-stu-id="7c569-109">Prerequisites</span></span>

<span data-ttu-id="7c569-110">अनुसूची सहायक Universal Resource Scheduling समाधान का एक हिस्सा है।</span><span class="sxs-lookup"><span data-stu-id="7c569-110">The Schedule assistant is a part of the Universal Resource Scheduling solution.</span></span> <span data-ttu-id="7c569-111">यह समाधान Dynamics 365 Project Operations, Dynamics 365 Field Service, और Dynamics 365 Customer Service में शामिल है और साथ स्थापित किया गया है.</span><span class="sxs-lookup"><span data-stu-id="7c569-111">This solution is included and installed with Dynamics 365 Project Operations, Dynamics 365 Field Service, and Dynamics 365 Customer Service.</span></span>

## <a name="matching-requirements-and-resources"></a><span data-ttu-id="7c569-112">मेल खाती आवश्यकताएँ और संसाधन</span><span class="sxs-lookup"><span data-stu-id="7c569-112">Matching requirements and resources</span></span>

<span data-ttu-id="7c569-113">उत्पन्न संसाधन आवश्यकता विवरण पर आधारित है, जैसे कि:</span><span class="sxs-lookup"><span data-stu-id="7c569-113">A generated resource requirement is based on details such as:</span></span>

-   <span data-ttu-id="7c569-114">विशेषताएं</span><span class="sxs-lookup"><span data-stu-id="7c569-114">Characteristics</span></span>
-   <span data-ttu-id="7c569-115">भूमिकाएँ</span><span class="sxs-lookup"><span data-stu-id="7c569-115">Roles</span></span>
-   <span data-ttu-id="7c569-116">व्यवसाय इकाइयाँ</span><span class="sxs-lookup"><span data-stu-id="7c569-116">Business units</span></span>
-   <span data-ttu-id="7c569-117">रिसोर्स की प्राथमिकताएं</span><span class="sxs-lookup"><span data-stu-id="7c569-117">Resource preferences</span></span>
-   <span data-ttu-id="7c569-118">प्रयास कान्टुर</span><span class="sxs-lookup"><span data-stu-id="7c569-118">Effort contours</span></span>
-   <span data-ttu-id="7c569-119">समय क्षेत्र</span><span class="sxs-lookup"><span data-stu-id="7c569-119">Time zone</span></span>

<span data-ttu-id="7c569-120">अनुसूची सहायक इन विवरणों का उपयोग संसाधनों को फ़िल्टर करने के लिए करता है।</span><span class="sxs-lookup"><span data-stu-id="7c569-120">The Schedule assistant uses these details to filter resources.</span></span>

## <a name="launch-the-schedule-assistant"></a><span data-ttu-id="7c569-121">शेड्यूल सहायक लॉन्च करें</span><span class="sxs-lookup"><span data-stu-id="7c569-121">Launch the Schedule assistant</span></span>

<span data-ttu-id="7c569-122">अनुसूची सहायक लॉन्च करने के दो तरीके हैं।</span><span class="sxs-lookup"><span data-stu-id="7c569-122">There are two ways in which the schedule assistant is launched.</span></span> <span data-ttu-id="7c569-123">यदि आप हाइब्रिड मोड का उपयोग कर रहे हैं, तो टीम सदस्य ग्रिड में आप अपूर्ण संसाधन आवश्यकता वाले किसी भी टीम सदस्य को चुन सकते हैं और उसके बाद **बुक** चुनें।</span><span class="sxs-lookup"><span data-stu-id="7c569-123">If you're using the hybrid mode, in the team member grid you can select any team member with an unfulfilled resource requirement, and then select **Book**.</span></span> <span data-ttu-id="7c569-124">यदि आप केंद्रीय मोड का उपयोग कर रहे हैं, तो संसाधन प्रबंधक संसाधन का पता लगाता है और उसे चुनता है।</span><span class="sxs-lookup"><span data-stu-id="7c569-124">If you're using the central mode, the Resource manager finds and selects the resource.</span></span>

## <a name="schedule-assistant-filters"></a><span data-ttu-id="7c569-125">शेड्यूल सहायक फ़िल्टर</span><span class="sxs-lookup"><span data-stu-id="7c569-125">Schedule assistant filters</span></span>

<span data-ttu-id="7c569-126">अनुसूची सहायक चलने के बाद, आवश्यक संसाधन से मिलने वाले विवरण को बाएं फलक में फ़िल्टर मान के रूप में दिखाया जाता है।</span><span class="sxs-lookup"><span data-stu-id="7c569-126">After the Schedule assistant runs, the details from the resource requirement are displayed as filtered values in the left pane.</span></span> <span data-ttu-id="7c569-127">अनुसूची की आवश्यकताओं को पूरा करने के लिए संसाधन प्रबंधक या परियोजना प्रबंधक फ़िल्टर को समायोजित करके परिणाम को सुधार सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="7c569-127">The Resource manager or the Project manager can fine-tune results by adjusting filters to meet the scheduling needs.</span></span>

<span data-ttu-id="7c569-128">फ़िल्टर फलक कार्य-संबंधी विकल्प दिखाता है, जिसमें शामिल हैं:</span><span class="sxs-lookup"><span data-stu-id="7c569-128">The filter pane shows work-related options, including:</span></span>

-   <span data-ttu-id="7c569-129">कार्य का प्रारंभ और समाप्ति दिनांक</span><span class="sxs-lookup"><span data-stu-id="7c569-129">Work start and end</span></span>
-   <span data-ttu-id="7c569-130">विशेषताएं</span><span class="sxs-lookup"><span data-stu-id="7c569-130">Characteristics</span></span>
-   <span data-ttu-id="7c569-131">भूमिकाएँ</span><span class="sxs-lookup"><span data-stu-id="7c569-131">Roles</span></span>
-   <span data-ttu-id="7c569-132">संगठनात्मक इकाइयाँ</span><span class="sxs-lookup"><span data-stu-id="7c569-132">Organizational units</span></span>
-   <span data-ttu-id="7c569-133">संसाधन कंपनी</span><span class="sxs-lookup"><span data-stu-id="7c569-133">Resourcing company</span></span>
-   <span data-ttu-id="7c569-134">संसाधन प्रकार</span><span class="sxs-lookup"><span data-stu-id="7c569-134">Resource types</span></span>
-   <span data-ttu-id="7c569-135">पसंदीदा संसाधन</span><span class="sxs-lookup"><span data-stu-id="7c569-135">Preferred resources</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]