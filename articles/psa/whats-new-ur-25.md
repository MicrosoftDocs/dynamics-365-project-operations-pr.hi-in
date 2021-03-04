---
title: Project Service Automation के अपडेट रिलीज़ 25, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 25, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 10/26/2020
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
ms.openlocfilehash: aabee3fe755e33d2c0f01a96b6f53a68957bc041
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/10/2021
ms.locfileid: "5143751"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-25-v3"></a><span data-ttu-id="7ca3d-103">Project Service Automation के अपडेट रिलीज़ 25, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है</span><span class="sxs-lookup"><span data-stu-id="7ca3d-103">What's new or changed in Project Service Automation Update Release 25, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="7ca3d-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="7ca3d-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="7ca3d-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="7ca3d-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="7ca3d-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="7ca3d-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="7ca3d-107">इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="7ca3d-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="7ca3d-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="7ca3d-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="7ca3d-109">यह विषय उन सुविधाओं और सुधारों को सूचीबद्ध करता है, जो नए हैं या Project Service Automation V3, अद्यतन रिलीज़ 25 के लिए बदल गए हैं. इस संस्करण की बिल्ड संख्या V 3.10.43.76 है और आमतौर पर अक्टूबर 2020 में स्वयं-अद्यतन के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="7ca3d-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 25 This version has a build number of V 3.10.43.76 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-25"></a><span data-ttu-id="7ca3d-110">अपडेट रिलीज़ 25</span><span class="sxs-lookup"><span data-stu-id="7ca3d-110">Update Release 25</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="7ca3d-111">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="7ca3d-111">Bug fixes</span></span>

<span data-ttu-id="7ca3d-112">**समय और व्यय**</span><span class="sxs-lookup"><span data-stu-id="7ca3d-112">**Time and Expense**</span></span>

<span data-ttu-id="7ca3d-113">निम्न समस्या को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="7ca3d-113">The following issue has been fixed:</span></span>

- <span data-ttu-id="7ca3d-114">पुनः प्राप्त किया जा रहे हैं बहुत बड़े अंतराल के आधार पर अतिरिक्त डेटा दिखा रहा समय प्रविष्टि चार्ट.</span><span class="sxs-lookup"><span data-stu-id="7ca3d-114">Time entry chart showing additional data based on too large of an interval being retrieved.</span></span>

<span data-ttu-id="7ca3d-115">**संसाधन प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="7ca3d-115">**Resource Management**</span></span>

<span data-ttu-id="7ca3d-116">निम्न समस्या को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="7ca3d-116">The following issue has been fixed:</span></span>

- <span data-ttu-id="7ca3d-117">यदि उच्च संस्करण पैच पहले से मौजूद है, तो Universal Resource Scheduling पैच आयात को छोड़ने के लिए जोड़ा गया Package Deployer कोड.</span><span class="sxs-lookup"><span data-stu-id="7ca3d-117">Added package deployer code to skip the Universal Resource Scheduling patch import if a higher version patch already exists.</span></span>

<span data-ttu-id="7ca3d-118">**परियोजना प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="7ca3d-118">**Project Management**</span></span>

<span data-ttu-id="7ca3d-119">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="7ca3d-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="7ca3d-120">सही राउंडिंग और विनिमय दर की विसंगतियों के परिणामस्वरूप परियोजना ट्रैकिंग ग्रिड में गलत नियोजित लागत.</span><span class="sxs-lookup"><span data-stu-id="7ca3d-120">Corrected rounding and exchange rate discrepancies resulting in incorrect planned cost in the project tracking grid.</span></span>
- <span data-ttu-id="7ca3d-121">**परियोजना** प्रपत्र पर दो या अधिक प्रतिक्रिया ग्रिड को दिखाने की क्षमता का समर्थन.</span><span class="sxs-lookup"><span data-stu-id="7ca3d-121">Support the ability to display two or more react grids on the **Project** form.</span></span>
- <span data-ttu-id="7ca3d-122">कैलेंडर समाप्ति दिनांक के बाद कार्य को असाइन करने की क्षमता, जिसके परिणामस्वरूप एक असफल संसाधन असाइनमेंट होता है, को हल करने के लिए प्रदान किया गया सत्यापन.</span><span class="sxs-lookup"><span data-stu-id="7ca3d-122">Provided validation to address the ability to assign a task past the calendar end date, which results in a failed resource assignment.</span></span>
- <span data-ttu-id="7ca3d-123">निम्न से उत्पन्न नल संदर्भ अपवाद को हल करने के लिए बेहतर त्रुटि हैंडलिंग:</span><span class="sxs-lookup"><span data-stu-id="7ca3d-123">Improved error handling to address Null Reference Exception generated from the following:</span></span>

    - <span data-ttu-id="7ca3d-124">**PreValidateProjectTeamMemberCreate** प्लग-इन</span><span class="sxs-lookup"><span data-stu-id="7ca3d-124">**PreValidateProjectTeamMemberCreate** plug-in</span></span>
    - <span data-ttu-id="7ca3d-125">**PreValidateProjectTaskCreate** जब बिना किसी संबद्ध परियोजना के परियोजना कार्य बनाया जाता है</span><span class="sxs-lookup"><span data-stu-id="7ca3d-125">**PreValidateProjectTaskCreate** when a project task is created without an associated project</span></span>
    - <span data-ttu-id="7ca3d-126">**PreProjectTeamMemberCreate** प्लग-इन</span><span class="sxs-lookup"><span data-stu-id="7ca3d-126">**PreProjectTeamMemberCreate** plug-in</span></span>
    - <span data-ttu-id="7ca3d-127">**PostProjectTeamMemberDelete** प्लग-इन</span><span class="sxs-lookup"><span data-stu-id="7ca3d-127">**PostProjectTeamMemberDelete** plug-in</span></span>
    - <span data-ttu-id="7ca3d-128">**PreValidateProjectTaskDelete** प्लग-इन</span><span class="sxs-lookup"><span data-stu-id="7ca3d-128">**PreValidateProjectTaskDelete** plug-in</span></span>

<span data-ttu-id="7ca3d-129">**Sales**</span><span class="sxs-lookup"><span data-stu-id="7ca3d-129">**Sales**</span></span>

<span data-ttu-id="7ca3d-130">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="7ca3d-130">The following issues have been fixed:</span></span>

- <span data-ttu-id="7ca3d-131">**परियोजना को कॉपी करें: HelperResource प्रबंधन का अनुमान लगाता है** से उत्पन्न नल संदर्भ अपवाद को हल करने के लिए बेहतर त्रुटि हैंडलिंग: </span><span class="sxs-lookup"><span data-stu-id="7ca3d-131">Improved error handling to address Null Reference Exceptions generated from **Copy Project: Estimates HelperResource Management**.</span></span>
- <span data-ttu-id="7ca3d-132">**समय और सामग्री बिलिंग बैकलॉग** पर **इनवॉइस के लिए तैयार नहीं** बिलिंग स्थिति को साफ़ नहीं करता.</span><span class="sxs-lookup"><span data-stu-id="7ca3d-132">**Not ready to Invoice** on a **Time and Material Billing Backlog** doesn't clear the billing status.</span></span>
- <span data-ttu-id="7ca3d-133">**भूमिका मूल्य** और **बैकलॉग आइटम** टैब पर सही किया गया गलत लेबल **मूल्य** बटन.</span><span class="sxs-lookup"><span data-stu-id="7ca3d-133">Corrected mislabeled **Prices** buttons on the **Role Price** and **Catalog Items** tab.</span></span>
