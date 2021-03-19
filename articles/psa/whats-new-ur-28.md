---
title: Project Service Automation के अपडेट रिलीज़ 28, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 28, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/26/2021
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
ms.openlocfilehash: 079679302b2d8dac3074732b2392a7b811ac9711
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280220"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-28-v3"></a><span data-ttu-id="52c29-103">Project Service Automation के अपडेट रिलीज़ 28, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है</span><span class="sxs-lookup"><span data-stu-id="52c29-103">What's new or changed in Project Service Automation Update Release 28, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="52c29-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="52c29-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="52c29-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="52c29-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="52c29-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="52c29-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="52c29-107">इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="52c29-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="52c29-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="52c29-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="52c29-109">इस विषय में Project Service Automation V3, अद्यतन रिलीज़ 28 में उपलब्ध सुविधाएँ और सुधार सूचीबद्ध किए गए हैं. इस संस्करण की बिल्ड संख्या V3.10.46.32 है और आमतौर से जनवरी 2021 में स्वयं-अद्यतन के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="52c29-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 28 This version has a build number of V3.10.46.32 and is generally available through a self-update in January 2021.</span></span>

## <a name="update-release-28"></a><span data-ttu-id="52c29-110">अपडेट रिलीज़ 28</span><span class="sxs-lookup"><span data-stu-id="52c29-110">Update Release 28</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="52c29-111">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="52c29-111">Bug fixes</span></span>

<span data-ttu-id="52c29-112">**समय और व्यय**</span><span class="sxs-lookup"><span data-stu-id="52c29-112">**Time and Expense**</span></span>

<span data-ttu-id="52c29-113">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="52c29-113">The following issues have been fixed:</span></span>

- <span data-ttu-id="52c29-114">उपयोगकर्ता, अनुमोदित और सबमिट की गई समय प्रविष्टियों को अद्यतन करने के लिए **सामूहिक संपादन** का उपयोग कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="52c29-114">Users can use **Bulk Edit** to update time entries that have been approved and submitted.</span></span>

<span data-ttu-id="52c29-115">**परियोजना प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="52c29-115">**Project Management**</span></span>

<span data-ttu-id="52c29-116">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="52c29-116">The following issues have been fixed:</span></span>

- <span data-ttu-id="52c29-117">ऐसे मामलों में जहां कार्य GUID को एक संख्या के रूप में व्याख्यायित किया जाता है, कार्यों को **कार्य विश्लेषण संरचना** पृष्ठ पर रिबन में **कार्य संपादित करें** का उपयोग करके संपादन के लिए खोला नहीं जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="52c29-117">In cases where the task GUID is interpreted as a number, tasks can't be opened for edit using **Edit Task** in the ribbon on the **Work Breakdown Structure** page.</span></span>

<span data-ttu-id="52c29-118">**Sales**</span><span class="sxs-lookup"><span data-stu-id="52c29-118">**Sales**</span></span>

<span data-ttu-id="52c29-119">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="52c29-119">The following issues have been fixed:</span></span>

- <span data-ttu-id="52c29-120">जब **GetEstimatesForProject** प्लग-इन इनवोक किया जाता है, तो नल संदर्भ अपवाद जनरेट होता है.</span><span class="sxs-lookup"><span data-stu-id="52c29-120">A null reference exception is generated when the **GetEstimatesForProject** plug-in is invoked.</span></span>
- <span data-ttu-id="52c29-121">माइलस्टोन ग्रिड पर **इनवॉइस के लिए तैयार के रूप में चिह्नित करें** **InvoiceStatus** एट्रिब्यूट को छोड़कर, जो कि अद्यतन है, केवल आंशिक रूप से एट्रिब्यूट को अद्यतन करता है.</span><span class="sxs-lookup"><span data-stu-id="52c29-121">**Mark ready to invoice** on the milestone grid only partially updates attributes, except for the **InvoiceStatus** attribute, which is updated.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]