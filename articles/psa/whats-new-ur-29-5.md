---
title: Project Service Automation के अद्यतन रिलीज़ 29.5, हॉटफ़िक्स, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: इस विषय में Project Service Automation अद्यतन रिलीज़ 29.5 हॉटफ़िक्स, V3 में उपलब्ध सुविधाएँ और सुधार सूचीबद्ध किए गए हैं.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 03/26/2021
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
ms.openlocfilehash: 99ba353236ad88b8bdff2c1b25e1247fa4bf3455
ms.sourcegitcommit: 9ebf7dd501898053bfa824f732adabf3f273613b
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/26/2021
ms.locfileid: "5715673"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-295-v3"></a><span data-ttu-id="a62a5-103">Project Service Automation के अपडेट रिलीज़ 29.5, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है</span><span class="sxs-lookup"><span data-stu-id="a62a5-103">What's new or changed in Project Service Automation Update Release 29.5, V3</span></span>

<span data-ttu-id="a62a5-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="a62a5-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="a62a5-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="a62a5-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="a62a5-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="a62a5-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="a62a5-107">इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="a62a5-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="a62a5-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="a62a5-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="a62a5-109">यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 29.5 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="a62a5-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 29.5.</span></span> <span data-ttu-id="a62a5-110">इस वर्ज़न की बिल्ड संख्या V3.10.47.150 है और यह आमतौर पर जनवरी 2021 के सेल्फ-अपडेट के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="a62a5-110">This version has a build number of V3.10.47.150 and is generally available through a self-update in January 2021.</span></span>

## <a name="update-release-295"></a><span data-ttu-id="a62a5-111">अपडेट रिलीज़ 29.5</span><span class="sxs-lookup"><span data-stu-id="a62a5-111">Update Release 29.5</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="a62a5-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="a62a5-112">Bug fixes</span></span>


<span data-ttu-id="a62a5-113">**सेल्स**</span><span class="sxs-lookup"><span data-stu-id="a62a5-113">**Sales**</span></span>

<span data-ttu-id="a62a5-114">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="a62a5-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="a62a5-115">एक संभावित शून्य संदर्भ अपवाद **ContractLineMapHelper.UpdateContractLineDetailPriceListReference** में होता है जब आप एककोटेशन को जीत के रूप में डालते करते हैं और कोटेशन की कोई मूल्य सूची नहीं होती है.</span><span class="sxs-lookup"><span data-stu-id="a62a5-115">A possible null reference exception occurs in **ContractLineMapHelper.UpdateContractLineDetailPriceListReference** when you close a quote as won and the quote has no price list.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
