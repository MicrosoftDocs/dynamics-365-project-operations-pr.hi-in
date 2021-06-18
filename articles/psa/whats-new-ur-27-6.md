---
title: Project Service Automation के अद्यतन रिलीज़ 27.6, हॉटफ़िक्स, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: इस विषय में Project Service Automation अद्यतन रिलीज़ 27.6 हॉटफ़िक्स, V3 में उपलब्ध सुविधाएँ और सुधार सूचीबद्ध किए गए हैं.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/17/2021
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
ms.openlocfilehash: 58cb82701e5cb8c549250ce5e3397d5939ec1ea1
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996883"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-276-v3"></a><span data-ttu-id="f0a0e-103">Project Service Automation के अपडेट रिलीज़ 27.6, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है</span><span class="sxs-lookup"><span data-stu-id="f0a0e-103">What's new or changed in Project Service Automation Update Release 27.6, V3</span></span>

<span data-ttu-id="f0a0e-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="f0a0e-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="f0a0e-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="f0a0e-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="f0a0e-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="f0a0e-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="f0a0e-107">इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="f0a0e-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="f0a0e-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="f0a0e-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="f0a0e-109">यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 27.6 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="f0a0e-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 27.6.</span></span> <span data-ttu-id="f0a0e-110">इस वर्ज़न की बिल्ड संख्या V3.10.45.120 है और यह आमतौर पर जनवरी 2021 के सेल्फ-अपडेट के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="f0a0e-110">This version has a build number of V3.10.45.120 and is generally available through a self-update in January 2021.</span></span>

## <a name="update-release-276"></a><span data-ttu-id="f0a0e-111">अपडेट रिलीज़ 27.6</span><span class="sxs-lookup"><span data-stu-id="f0a0e-111">Update Release 27.6</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="f0a0e-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="f0a0e-112">Bug fixes</span></span>


<span data-ttu-id="f0a0e-113">**संसाधन प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="f0a0e-113">**Resource Management**</span></span>

<span data-ttu-id="f0a0e-114">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="f0a0e-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="f0a0e-115">संसाधन उपलब्धता खोजने पर, उस प्रत्येक संसाधन के लिए **ExpandCalendar** को कॉल किया जाता है, जिसके लिए कोई कैलेंडर नियम लागू नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="f0a0e-115">When finding resource availability, **ExpandCalendar** is called for each resource that has no calendar rules applied.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]