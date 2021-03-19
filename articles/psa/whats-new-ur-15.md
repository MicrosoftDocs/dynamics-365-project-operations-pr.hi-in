---
title: Project Service Automation के अपडेट रिलीज़ 15, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह टॉपिक Project Service Automation अपडेट रिलीज़ 15, V3 में क्या नया है, इसके बारे में जानकारी प्रदान करता है.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/27/2020
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
ms.openlocfilehash: 189b99c6a4bf18b6063c7b6020dbf1ac372b41e9
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280940"
---
# <a name="project-service-automation-update-release-15-v3"></a><span data-ttu-id="7c6c7-103">Project Service Automation V3 अद्यतन रिलीज़ 15, V3</span><span class="sxs-lookup"><span data-stu-id="7c6c7-103">Project Service Automation Update Release 15, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="7c6c7-104">हमें Dynamics 365 Project Service Automation (PSA) अनुप्रयोग के लिए नवीनतम अपडेट की घोषणा करते हुए बेहद खुशी है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="7c6c7-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="7c6c7-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="7c6c7-107">इस रिलीज़ पर अपडेट करने के लिए, Dynamics 365 online के लिए व्यवस्थापन केंद्र पर जाएँ, और अपडेट को स्थापित करने के लिए समाधान पृष्ठ पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="7c6c7-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="7c6c7-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="7c6c7-109">यह टॉपिक PSA V3, अपडेट रिलीज़ 15 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 15.</span></span> <span data-ttu-id="7c6c7-110">इस वर्ज़न की बिल्ड संख्या V3.10.5.28 है और यह आमतौर पर जनवरी 2020 के सेल्फ-अपडेट के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-110">This version has a build number of V3.10.5.28 and is generally available through a self-update in January 2020.</span></span>

## <a name="update-release-15"></a><span data-ttu-id="7c6c7-111">अपडेट रिलीज़ 15</span><span class="sxs-lookup"><span data-stu-id="7c6c7-111">Update Release 15</span></span> 

### <a name="enhancements"></a><span data-ttu-id="7c6c7-112">एन्हांसमेंट</span><span class="sxs-lookup"><span data-stu-id="7c6c7-112">Enhancements</span></span>

- <span data-ttu-id="7c6c7-113">परियोजना प्रबंधन</span><span class="sxs-lookup"><span data-stu-id="7c6c7-113">Project Management</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="7c6c7-114">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="7c6c7-114">Bug fixes</span></span>

- <span data-ttu-id="7c6c7-115">समय और व्यय</span><span class="sxs-lookup"><span data-stu-id="7c6c7-115">Time and Expense</span></span>

  - <span data-ttu-id="7c6c7-116">फिक्स्ड: समायोजन दृश्य में ऑन-लोड त्रुटि हैंडलिंग जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-116">Fixed: Add on-load error handling in the reconciliation view.</span></span>
  - <span data-ttu-id="7c6c7-117">फिक्स्ड: परियोजना संसाधन हब: अस्पष्टता को कम करने के लिए **राशि** का नाम बदलें.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-117">Fixed: Project Resource Hub: Rename **Amount** to reduce ambiguity.</span></span>
  - <span data-ttu-id="7c6c7-118">फिक्स्ड: प्रकार को शामिल करने के लिए **कॉपी समय पृविष्टि कॉलम** दृशय को एडजस्ट करें.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-118">Fixed: Adjust the view **Copy Time Entry Columns** to include the type.</span></span>
  - <span data-ttu-id="7c6c7-119">फिक्स्ड: दशमलव संख्या का उपयोग करके ग्रिड दृश्य में समय प्रविष्टि अवधि को संपादित करने का परिणाम कुछ संख्या के लिए अज्ञात त्रुटि आता है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-119">Fixed: Editing time entry duration in the grid view using decimal numbers results in unknown error for some numbers.</span></span>

- <span data-ttu-id="7c6c7-120">परियोजना प्रबंधन</span><span class="sxs-lookup"><span data-stu-id="7c6c7-120">Project Management</span></span>

  - <span data-ttu-id="7c6c7-121">फिक्स्ड: **ट्रैकिंग दृश्य में उपयोग करें** के लिए ड्रॉप-डाउन मेनू अब विकल्पों की चौड़ाई के आधार पर विस्तार करता है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-121">Fixed: The drop-down menu for **Use in Tracking View** now expands based on the width of the options.</span></span>
  - <span data-ttu-id="7c6c7-122">फिक्स्ड: +13 समय क्षेत्र में परियोजनाओं का प्रबंधन करते समय, कार्य गणना गलत परिणाम प्रदर्शित कर सकती है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-122">Fixed: When managing projects in the +13 time zone, tasks calculations can display inaccurate results.</span></span>
  - <span data-ttu-id="7c6c7-123">फिक्स्ड: 24-घंटे के कैलेंडर का उपयोग करते समय **टीम सदस्य समाप्ति समय** को सही किया गया है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-123">Fixed: **Team Member End Time** has been corrected when using a 24-hour calendar.</span></span>
  - <span data-ttu-id="7c6c7-124">फिक्स्ड: **BPF** को **msdyn_project** मुख्य प्रपत्र में फिर से सक्रिय किया गया है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-124">Fixed: Re-activated the **BPF** in **msdyn_project** main form.</span></span>
  - <span data-ttu-id="7c6c7-125">फिक्स्ड: असाइनमेंट गणना में अब एक दिन की उपेक्षा नहीं की जाती है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-125">Fixed: Assignments calculation no longer ignores one day.</span></span>
  - <span data-ttu-id="7c6c7-126">फ़िक्स्ड: उपयोगकर्ता और परियोजना के बीच समय क्षेत्र अलग होने पर परियोजना प्रपत्र में एक नया सूचना बैनर जोड़ा गया है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-126">Fixed: A new notification banner has been added to the project form when the time zone differs between user and project.</span></span>

- <span data-ttu-id="7c6c7-127">Sales</span><span class="sxs-lookup"><span data-stu-id="7c6c7-127">Sales</span></span>

  - <span data-ttu-id="7c6c7-128">फ़िक्स्ड: डुप्लिकेट को फ़िल्टर करने के लिए व्यय अनुमान श्रेणी लुकअप का उपयोग किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-128">Fixed: Expense estimate category lookup can be used to filter duplicates.</span></span>
  - <span data-ttu-id="7c6c7-129">फ़िक्स्ड: **PluginDomain.ExecuteInTryCatchBlock (..)** में कोड अब अपवाद के मूल को छुपाता नहीं है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-129">Fixed: Code in **PluginDomain.ExecuteInTryCatchBlock(..)** no longer hides the origin of the exception.</span></span>
  - <span data-ttu-id="7c6c7-130">फ़िक्स्ड: 1000 से अधिक परियोजनाएं होने पर अब **उद्धरण पंक्ति** में **परियोजना लुकअप** में कोई त्रुटि संदेश नहीं आता है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-130">Fixed: No longer get an error message in **Project lookup** in the **Quote Line** form when there are more than 1000 projects.</span></span>
  - <span data-ttu-id="7c6c7-131">फ़िक्स्ड: श्रम अनुमान और व्यय अनुमान के लिए **अनुमान** ग्रिड अब सही मुद्रा चिह्न दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-131">Fixed: **Estimates** grid for labor estimates and expense estimates now displays the correct currency symbol.</span></span>
  - <span data-ttu-id="7c6c7-132">फ़िक्स्ड: किसी भी संगठन द्वारा PSA को अपडेट रिलीज़ 14 से अपडेट रिलीज़ 15 पर अपडेट करने के बाद, अब **परियोजना** प्रपत्र पर **शेड्यूल** टैब रिक्त नहीं आती है.</span><span class="sxs-lookup"><span data-stu-id="7c6c7-132">Fixed: After an organization updates PSA from Update Release 14 to Update Release 15, the **Schedule** tab no longer appears as blank on the **Project** form.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]