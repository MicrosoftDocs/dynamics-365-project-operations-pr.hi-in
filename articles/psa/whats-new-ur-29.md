---
title: Project Service Automation के अपडेट रिलीज़ 29, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 29, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/22/2021
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
ms.openlocfilehash: 2ac47974b9cc8386c7446136faf48724de73efce
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948638"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-29-v3"></a><span data-ttu-id="b6812-103">Project Service Automation के अपडेट रिलीज़ 29, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है</span><span class="sxs-lookup"><span data-stu-id="b6812-103">What's new or changed in Project Service Automation Update Release 29, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="b6812-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="b6812-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="b6812-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="b6812-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="b6812-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="b6812-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="b6812-107">इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="b6812-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="b6812-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="b6812-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="b6812-109">यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 29 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="b6812-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 29.</span></span> <span data-ttu-id="b6812-110">इस संस्करण की बिल्ड संख्या V3.10.47.7 है और आमतौर से फरवरी 2021 में स्वयं-अद्यतन के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="b6812-110">This version has a build number of V3.10.47.7 and is generally available through a self-update in February 2021.</span></span>

## <a name="update-release-29"></a><span data-ttu-id="b6812-111">अपडेट रिलीज़ 29</span><span class="sxs-lookup"><span data-stu-id="b6812-111">Update Release 29</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="b6812-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="b6812-112">Bug fixes</span></span>

<span data-ttu-id="b6812-113">**समय और व्यय**</span><span class="sxs-lookup"><span data-stu-id="b6812-113">**Time and Expense**</span></span>

<span data-ttu-id="b6812-114">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="b6812-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="b6812-115">उपयोगकर्ता समय प्रविष्टि ग्रिड में गैर-कार्य दिवसों में लॉग किए गए कार्य समय को नहीं देख सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="b6812-115">Users can't see working hours logged on non-working days in the time entry grid.</span></span>
- <span data-ttu-id="b6812-116">स्वीकृत व्यय प्रविष्टियों को ग्रिड पर संपादित किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b6812-116">Approved expense entries can be edited on the grid.</span></span>

<span data-ttu-id="b6812-117">**परियोजना प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="b6812-117">**Project Management**</span></span>

<span data-ttu-id="b6812-118">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="b6812-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="b6812-119">संसाधन असाइनमेंट के प्रयास ऋणात्मक नहीं हो सकते सुनिश्चित करने के लिए सत्यापन तर्क उपलब्ध नहीं है.</span><span class="sxs-lookup"><span data-stu-id="b6812-119">Missing validation logic to ensure resource assignment effort hours can't be negative.</span></span>
- <span data-ttu-id="b6812-120">कस्टम क्रिया, **AssignResourcesForTask** केवल बदले गए फ़ील्ड के बजाय सभी फ़ील्ड अपडेट करता है.</span><span class="sxs-lookup"><span data-stu-id="b6812-120">The custom action, **AssignResourcesForTask** updates all fields instead of only changed fields.</span></span>
- <span data-ttu-id="b6812-121">उन प्लग-इन या कार्यप्रवाह वाले परिवेश में किसी परियोजना की प्रतिलिपि बनाते समय, जो **CreateProject** इवेंट पर पंजीकृत हैं, अब अगर **CopyWBSToProject** विफल हो जाता है, तो **msdyn_bulkgenerationstatus** एट्रिब्यूट अद्यतन नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="b6812-121">When copying a project in an environment with plug-ins or workflows that are registered on the **CreateProject** event, the **msdyn_bulkgenerationstatus** attribute isn't updated if the **CopyWBSToProject** fails.</span></span>
- <span data-ttu-id="b6812-122">जब आप परियोजना कैलेंडर का विस्तार करते हैं, तो कार्य दिवस आरोही क्रम में सॉर्ट नहीं किए जाते हैं, जिससे कुछ परियोजना कार्य अपडेट विफल हो जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="b6812-122">When you expand the project calendar, the working days aren't sorted in ascending order causing some project task updates to fail.</span></span>
- <span data-ttu-id="b6812-123">किसी मौजूदा परियोजना पर परियोजना प्रबंधन को बदलने से संगठनात्मक इकाई डिफ़ॉल्ट तर्क ट्रिगर हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="b6812-123">Changing the Project Manager on an existing project triggers the organizational unit defaulting logic.</span></span>

<span data-ttu-id="b6812-124">**सेल्स**</span><span class="sxs-lookup"><span data-stu-id="b6812-124">**Sales**</span></span>

<span data-ttu-id="b6812-125">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="b6812-125">The following issues have been fixed:</span></span>

- <span data-ttu-id="b6812-126">**अनुबंध** पृष्ठ पर **अनुबंध प्रदर्शन** टैब प्रारंभ के दौरान चुपचाप से विफल रहता है, जब कोई अनुबंध पंक्ति मौजूद नहीं होती है.</span><span class="sxs-lookup"><span data-stu-id="b6812-126">The **Contract Performance** tab on the **Contract** page fails silently during initialization when no contract lines are present.</span></span>