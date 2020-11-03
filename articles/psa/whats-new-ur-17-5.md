---
title: Project Service Automation के अपडेट रिलीज़ 17.5, हॉटफ़िक्स, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 17.5, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 03/13/2020
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
ms.openlocfilehash: 359eb8f8ca41d69d4f30dd44497a4deb6a6c4f8d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077655"
---
# <a name="project-service-automation-update-release-175-v3"></a><span data-ttu-id="9351a-103">Project Service Automation V3 अद्यतन रिलीज़ 17.5, V3</span><span class="sxs-lookup"><span data-stu-id="9351a-103">Project Service Automation Update Release 17.5, V3</span></span>

<span data-ttu-id="9351a-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="9351a-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="9351a-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="9351a-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="9351a-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="9351a-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="9351a-107">इस रिलीज़ को अपडेट करने के लिए, Dynamics 365 online के लिए व्यवस्थापन केंद्र पर जाएँ और अपडेट को स्थापित करने के लिए समाधान पृष्ठ पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="9351a-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="9351a-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="9351a-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="9351a-109">यह विषय V3, अपडेट रिलीज़ 17.5 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="9351a-109">This topic lists the features and fixes that are new or changed for V3, Update Release 17.5.</span></span> <span data-ttu-id="9351a-110">इस संस्करण की बिल्ड संख्या V3.10.7.32 है और यह आमतौर पर मार्च 2020 के स्वयं-अपडेट के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="9351a-110">This version has a build number of V3.10.7.32 and is generally available through a self-update in March 2020.</span></span>


## <a name="update-release-175"></a><span data-ttu-id="9351a-111">अपडेट रिलीज़ 17.5</span><span class="sxs-lookup"><span data-stu-id="9351a-111">Update Release 17.5</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="9351a-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="9351a-112">Bug fixes</span></span>


<span data-ttu-id="9351a-113">**परियोजना प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="9351a-113">**Project Management**</span></span>

- <span data-ttu-id="9351a-114">निश्चित: लंबी अवधि के कार्यों के साथ सर्वर साइड सिंक्रनाइज़ेशन समस्याओं के बारे में बताता है.</span><span class="sxs-lookup"><span data-stu-id="9351a-114">Fixed: Addressed server-side synchronization issues that occur with long duration tasks.</span></span>
- <span data-ttu-id="9351a-115">निश्चित: 24-घंटे काम के घंटे के टेम्पलेट को गलत तरीके से कार्यों के दिनों लिए एक अतिरिक्त दिन जोड़ने के बारे में बताता है.</span><span class="sxs-lookup"><span data-stu-id="9351a-115">Fixed: Addressed 24-hour work hour templates inaccurately adding an additional day to tasks.</span></span>
- <span data-ttu-id="9351a-116">निश्चित: +13 GMT काम के घंटे का टेम्प्लेट एक दिन आगे के कार्यों को गलत तरीके से स्थानांतरित करने के बारे में बताता है.</span><span class="sxs-lookup"><span data-stu-id="9351a-116">Fixed: Addressed +13 GMT work hour templates inaccurately shifting tasks one day ahead.</span></span>

