---
title: Project Service Automation के अपडेट रिलीज़ 30, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 30, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/01/2021
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
ms.openlocfilehash: 3b6b7dba9c2a22587d27006b9972c950fbb454f2
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010428"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-30-v3"></a><span data-ttu-id="4311a-103">Project Service Automation के अपडेट रिलीज़ 30, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है</span><span class="sxs-lookup"><span data-stu-id="4311a-103">What's new or changed in Project Service Automation Update Release 30, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="4311a-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="4311a-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="4311a-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="4311a-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="4311a-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="4311a-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="4311a-107">इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="4311a-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="4311a-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution.md).</span><span class="sxs-lookup"><span data-stu-id="4311a-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution.md).</span></span>

<span data-ttu-id="4311a-109">यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 30 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="4311a-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 30.</span></span> <span data-ttu-id="4311a-110">इस संस्करण की बिल्ड संख्या V3.10.51.61 है और यह आमतौर पर अप्रैल 2021 में एक स्व-अद्यतन के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="4311a-110">This version has a build number of V3.10.51.61 and is generally available through a self-update in April 2021.</span></span>

## <a name="update-release-30"></a><span data-ttu-id="4311a-111">अपडेट रिलीज़ 30</span><span class="sxs-lookup"><span data-stu-id="4311a-111">Update Release 30</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="4311a-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="4311a-112">Bug fixes</span></span>

<span data-ttu-id="4311a-113">**समय और व्यय**</span><span class="sxs-lookup"><span data-stu-id="4311a-113">**Time and Expense**</span></span>

<span data-ttu-id="4311a-114">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="4311a-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="4311a-115">यदि आप **त्वरित बनाएं** पेज पर समय प्रविष्टि बनाते और सहेजते हैं, तो एक त्रुटि होती है, अगर **रोल** फ़ील्ड हटा दिया जाता है.</span><span class="sxs-lookup"><span data-stu-id="4311a-115">An error occurs when you create and save a time entry on the **Quick Create** page if the **Role** field is removed.</span></span>
- <span data-ttu-id="4311a-116">टाइम एंट्री फिल्टर गलत फिल्टर ऑपरेटर लगाता है.</span><span class="sxs-lookup"><span data-stu-id="4311a-116">The Time Entry filter applies the wrong filter operator.</span></span>
- <span data-ttu-id="4311a-117">समय प्रविष्टि नियंत्रण पर **कॉपी वीक** का चयन करते समय कॉपी की गई टाइमशीट स्वचालित रूप से प्रदर्शित नहीं होती है.</span><span class="sxs-lookup"><span data-stu-id="4311a-117">Copied timesheets aren't automatically displayed when you select **Copy Week** on the time entry control.</span></span>

<span data-ttu-id="4311a-118">**संसाधन प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="4311a-118">**Resource Management**</span></span>

<span data-ttu-id="4311a-119">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="4311a-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="4311a-120">जब आप बुकिंग का विस्तार करते हैं, तो हार्ड बुकिंग को सौंपा गया बुकिंग स्थिति गलत है.</span><span class="sxs-lookup"><span data-stu-id="4311a-120">When you extend a booking, the booking status assigned to the hard booking is incorrect.</span></span> <span data-ttu-id="4311a-121">बुकिंग का विस्तार बुकिंग सेटअप मेटाडेटा में **प्रतिबद्ध** के रूप में परिभाषित बुकिंग स्थिति का सम्मान करता है.</span><span class="sxs-lookup"><span data-stu-id="4311a-121">Extending a booking respects the booking status defined as **Committed** in the booking setup metadata.</span></span>
- <span data-ttu-id="4311a-122">जब कोई वैध बुकिंग स्थिति निर्दिष्ट नहीं की जाती है, तो त्रुटि संदेश सही ढंग से स्थानीयकृत नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="4311a-122">When a valid booking status isn't specified, the error message is not correctly localized.</span></span>

<span data-ttu-id="4311a-123">**परियोजना प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="4311a-123">**Project Management**</span></span>

<span data-ttu-id="4311a-124">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="4311a-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="4311a-125">प्रोज़ेक्टओं को एक मुद्रा में नहीं बनाया जा सकता है और किसी अन्य मुद्रा में संबंधित कार्यों को शामिल किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="4311a-125">Projects can't be created in one currency and include related tasks in another currency.</span></span>

<span data-ttu-id="4311a-126">**सेल्स**</span><span class="sxs-lookup"><span data-stu-id="4311a-126">**Sales**</span></span>

<span data-ttu-id="4311a-127">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="4311a-127">The following issues have been fixed:</span></span>

- <span data-ttu-id="4311a-128">जब किसी मूल्य सूची की नकल की जाती है, तो कीमतें अपडेट नहीं की जाती हैं.</span><span class="sxs-lookup"><span data-stu-id="4311a-128">When a price list is copied, prices aren't updated.</span></span>
- <span data-ttu-id="4311a-129">एक उद्धरण को बंद करना विफल रहता है जब लागत विस्तार मूल के लिए एक मूल्य है.</span><span class="sxs-lookup"><span data-stu-id="4311a-129">Closing a quote as won fails when the cost detail has a value for origin.</span></span>
- <span data-ttu-id="4311a-130">**प्रोज़ेक्ट टास्क** इकाई पर, **अनुमानित लागत** को **नियोजित लागत (आधार)** में बदल दिया गया है.</span><span class="sxs-lookup"><span data-stu-id="4311a-130">On the **Project Task** entity, **Estimated Cost** has been renamed to **Planned Cost (Base)**.</span></span>
- <span data-ttu-id="4311a-131">जब इनवॉइस बनाए जाते हैं या हटाए जाते हैं तो एक शून्य संदर्भ अपवाद उत्पन्न होता है.</span><span class="sxs-lookup"><span data-stu-id="4311a-131">A null reference exception is generated when invoices are created or deleted.</span></span>
