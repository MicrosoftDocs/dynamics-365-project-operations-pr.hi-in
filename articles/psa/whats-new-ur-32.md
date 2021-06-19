---
title: Project Service Automation के अपडेट रिलीज़ 32, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 32, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/01/2021
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
ms.openlocfilehash: 11bf451ef4f24e2301ffde4f86a556a8a4fe30b0
ms.sourcegitcommit: 886102894244887d72e5a6213071e8d8a52c9d48
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/01/2021
ms.locfileid: "6129668"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-32-v3"></a><span data-ttu-id="fa7c3-103">Project Service Automation के अपडेट रिलीज़ 32, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है</span><span class="sxs-lookup"><span data-stu-id="fa7c3-103">What's new or changed in Project Service Automation Update Release 32, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="fa7c3-104">हमें Microsoft Dynamics 365 Project Service Automation अनुप्रयोग के लिए नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-104">We're pleased to announce the latest update for the Microsoft Dynamics 365 Project Service Automation app.</span></span> <span data-ttu-id="fa7c3-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="fa7c3-106">यह Dynamics 365 9.x से मेल के योग्य है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-106">It's compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="fa7c3-107">इस रिलीज़ में अद्यतन करने के लिए, Dynamics 365 ऑनलाइन समाधान के लिए व्यवस्थापन केंद्र पृष्ठ पर जाएं और अद्यतन इंस्टॉल करें.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page, and install the update.</span></span> <span data-ttu-id="fa7c3-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="fa7c3-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="fa7c3-109">यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 32 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 32.</span></span> <span data-ttu-id="fa7c3-110">इस संस्करण की बिल्ड संख्या V3.10.53.108 है और आम तौर पर जून 2021 में स्वयं-अपडेट के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-110">This version has a build number of V3.10.53.108 and is generally available through a self-update in June 2021.</span></span>

## <a name="update-release-32"></a><span data-ttu-id="fa7c3-111">अपडेट रिलीज़ 32</span><span class="sxs-lookup"><span data-stu-id="fa7c3-111">Update Release 32</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="fa7c3-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="fa7c3-112">Bug fixes</span></span>

#### <a name="general"></a><span data-ttu-id="fa7c3-113">सामान्य</span><span class="sxs-lookup"><span data-stu-id="fa7c3-113">General</span></span>

- <span data-ttu-id="fa7c3-114">जब कोई बड़ा अपग्रेड विफल हो जाता है, तो यह सुनिश्चित करने के लिए कि साझा निकाय अब भी पहुंच योग्य हैं, केवल मुख्य अनुप्रयोग प्रविष्टि बिंदु अवरुद्ध किए जाने चाहिए.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-114">When a major upgrade fails, only the main application entry points should be blocked, to ensure that shared entities are still accessible.</span></span>

#### <a name="time-and-expense"></a><span data-ttu-id="fa7c3-115">समय और व्यय</span><span class="sxs-lookup"><span data-stu-id="fa7c3-115">Time and Expense</span></span>

<span data-ttu-id="fa7c3-116">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="fa7c3-116">The following issues have been fixed:</span></span>

- <span data-ttu-id="fa7c3-117">**TimeEntriesImportFromResourceAssignment** संसाधन असाइनमेंट कंटूर स्लाइस के प्रारंभ और समाप्ति समय को बनाए नहीं रखता है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-117">**TimeEntriesImportFromResourceAssignment** doesn't maintain the start and end times of the resource assignment contour slice.</span></span>
- <span data-ttu-id="fa7c3-118">जब आप **समय प्रविष्टि** ग्रिड पर **प्रविष्टि खोलें** चुनते हैं, तो आपको अन्य प्रपत्रों का चयन करने से रोका जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-118">When you select **Open Entry** on the **Time Entry** grid, you might be prevented from selecting other forms.</span></span>
- <span data-ttu-id="fa7c3-119">जब आप समय प्रविष्टियों में असाइनमेंट आयात करते हैं, तो क्लाइंट कोड क्वेरी लंबा URL उत्पन्न कर सकती है जो क्वेरी को विफल कर देता है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-119">While you import assignments to time entries, the client code query could generate a long URL that fails the query.</span></span>
- <span data-ttu-id="fa7c3-120">**समय प्रविष्टि** ग्रिड में, किसी सेल से मान हटाए जाने के बाद, फ़ोकस ग्रिड में नहीं रहता है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-120">In the **Time Entry** grid, after a value is deleted from a cell, the focus doesn't remain in the grid.</span></span>
- <span data-ttu-id="fa7c3-121">**अस्वीकार करें** बटन को नए अनुमोदनों के लिए **अनुमोदन संसाधित किए जा रहे हैं** दृश्य से हटा दिया गया है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-121">The **Reject** button has been removed from the **Processing approvals** view for modern approvals.</span></span>
- <span data-ttu-id="fa7c3-122">समय प्रविष्टि एकमुश्त अनुमोदन की स्थिरता और प्रदर्शन गतिरोध और **समय प्रविष्टि** निकाय से संबंधित अनुकूलन को उचित रूप से प्रबंधित करने में विफलता से प्रभावित होते हैं.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-122">The stability and performance of time entry bulk approval are affected by deadlocks and a failure to appropriately handle customizations that are related to the **Time Entry** entity.</span></span>

#### <a name="project-planning"></a><span data-ttu-id="fa7c3-123">परियोजना नियोजन</span><span class="sxs-lookup"><span data-stu-id="fa7c3-123">Project Planning</span></span>

- <span data-ttu-id="fa7c3-124">शून्य संदर्भ अपवाद तब उत्पन्न होता है, जब आप किसी ऐसे प्रोजेक्ट को अपडेट करते हैं जिसमें **अनुबंध इकाई** फ़ील्ड में शून्य मान होता है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-124">A null reference exception is generated when you update a project that has a null value in the **Contracting Unit** field.</span></span>
- <span data-ttu-id="fa7c3-125">**प्रोजेक्ट योग रीफ्रेश करें** किसी प्रोजेक्ट पर शेष लागत और शेष बिक्री की गलत गणना करता है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-125">**Refresh Project Totals** incorrectly calculates the remaining cost and remaining sales on a project.</span></span>
- <span data-ttu-id="fa7c3-126">अनावश्यक मूल्य निर्धारण गुणना उस प्रदर्शन को प्रभावित करते हैं, जो संसाधन असाइनमेंट रूपरेखा पर अपडेट से संबंधित है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-126">Redundant pricing calculations affect performance that is related to updates on resource assignment contours.</span></span>

#### <a name="resource-management"></a><span data-ttu-id="fa7c3-127">संसाधन प्रबंधन</span><span class="sxs-lookup"><span data-stu-id="fa7c3-127">Resource Management</span></span>

<span data-ttu-id="fa7c3-128">निम्न समस्या को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="fa7c3-128">The following issue has been fixed:</span></span>

- <span data-ttu-id="fa7c3-129">जब बुक करने योग्य संसाधन की कैलेंडर क्षमता 1 से अधिक होती है, तो Project Service Automation क्षमता को गलत तरीके से 0 (शून्य) के रूप में प्रकट करता है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-129">When a bookable resource's calendar capacity is more than 1, Project Service Automation incorrectly recognizes the capacity as 0 (zero).</span></span> <span data-ttu-id="fa7c3-130">इसलिए, शेड्यूल दृश्य में अनंत लूप उत्पन्न होता है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-130">Therefore, an infinite loop occurs in the schedule view.</span></span>

#### <a name="sales"></a><span data-ttu-id="fa7c3-131">सेल्स</span><span class="sxs-lookup"><span data-stu-id="fa7c3-131">Sales</span></span>

<span data-ttu-id="fa7c3-132">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="fa7c3-132">The following issues have been fixed:</span></span>

- <span data-ttu-id="fa7c3-133">जब जर्नल पंक्ति बनाई जाती है, जिसमें कस्टम लेनदेन प्रकार होता है, तो निम्न शून्य संदर्भ अपवाद उत्पन्न होता है: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitWithTransactionType(TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-133">When a journal line is created that has a custom transaction type, the following null reference exception occurs: *Microsoft.Dynamics.ProjectService.Plugins.JournalLinePlugins.ValidateUnitScheduleAndUnitWithTransactionType(TransactionTypetransactionType, TransactionTypeCode transTypeCodeFromPlugin)*.</span></span>
- <span data-ttu-id="fa7c3-134">किसी कोटेशन की कॉपी बनाने से पहले निष्क्रिय की गई भूमिकाओं और श्रेणियों को नए कॉपी किए गए कोटेशन की प्रभार्य भूमिकाओं और श्रेणियों में नहीं जोड़ा जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-134">Roles and categories that are inactivated before a quotation is copied should not be added to chargeable roles and categories of the newly copied quotation.</span></span>
- <span data-ttu-id="fa7c3-135">दस्तावेज़ तिथि और लेखा तिथि, प्रारंभ तिथि के साथ संरेखित नहीं हैं जो इनवॉइस श्रेणी विवरण पर प्रदान की जाती है जो सीधे ड्राफ्ट इनवॉइस पर बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-135">The document date and accounting date aren't aligned with the start date that is provided on an invoice line detail that is created directly on a draft invoice.</span></span>
- <span data-ttu-id="fa7c3-136">शून्य संदर्भ अपवाद उन परिदृश्यों में उत्पन्न होते हैं जो किसी कोटेशन की कॉपनी बनाने से पहले भूमिकाओं और श्रेणियों के निष्क्रिय होने से संबंधित होते हैं.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-136">Null reference exceptions are generated in scenarios that are related to inactivation of roles and categories before a quotation is copied.</span></span>
- <span data-ttu-id="fa7c3-137">**प्रोजेक्ट** पृष्ठ पर **मूल्य अपडेट करें** कार्रवाई व्यय अनुमानों और सामग्री अनुमानों को अपडेट नहीं करती है.</span><span class="sxs-lookup"><span data-stu-id="fa7c3-137">The **Update Prices** action on the **Projects** page doesn't update expense estimates and material estimates.</span></span>
