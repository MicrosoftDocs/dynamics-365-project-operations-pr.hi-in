---
title: Project Service Automation के अपडेट रिलीज़ 13, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह टॉपिक Project Service Automation अपडेट रिलीज़ 13, V3 में क्या नया है, इसके बारे में जानकारी प्रदान करता है.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: c328821064065e19938406856d327f690f577e7a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000303"
---
# <a name="project-service-automation-update-release-13-v3"></a><span data-ttu-id="7c4c3-103">Project Service Automation V3 अद्यतन रिलीज़ 13, V3</span><span class="sxs-lookup"><span data-stu-id="7c4c3-103">Project Service Automation Update Release 13, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="7c4c3-104">हमें Dynamics 365 Project Service Automation (PSA) अनुप्रयोग के लिए नवीनतम अपडेट की घोषणा करते हुए बेहद खुशी है.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="7c4c3-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="7c4c3-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="7c4c3-107">इस रिलीज़ पर अपडेट करने के लिए, Dynamics 365 online के लिए व्यवस्थापन केंद्र पर जाएँ, और अपडेट को स्थापित करने के लिए समाधान पृष्ठ पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="7c4c3-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="7c4c3-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="7c4c3-109">यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 13 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 13.</span></span> <span data-ttu-id="7c4c3-110">इस वर्ज़न की बिल्ड संख्या V3.10.3.18 है और यह निम्नलिखित शेड्यूल पर उपलब्ध है:</span><span class="sxs-lookup"><span data-stu-id="7c4c3-110">This version has a build number of V3.10.3.18 and is available on the following schedule:</span></span>

- <span data-ttu-id="7c4c3-111">**सामान्य उपलब्धता (सेल्फ-अपडेट):** नवंबर 2019</span><span class="sxs-lookup"><span data-stu-id="7c4c3-111">**General availability (self-update):** November 2019</span></span>
- <span data-ttu-id="7c4c3-112">**ऑटो-अपडेट:** दिसंबर 2019</span><span class="sxs-lookup"><span data-stu-id="7c4c3-112">**Auto-update:** December 2019</span></span>


## <a name="update-release-13"></a><span data-ttu-id="7c4c3-113">अपडेट रिलीज़ 13</span><span class="sxs-lookup"><span data-stu-id="7c4c3-113">Update Release 13</span></span> 

### <a name="bug-fixes"></a><span data-ttu-id="7c4c3-114">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="7c4c3-114">Bug fixes</span></span>

- <span data-ttu-id="7c4c3-115">समय और व्यय</span><span class="sxs-lookup"><span data-stu-id="7c4c3-115">Time and Expense</span></span>

     - <span data-ttu-id="7c4c3-116">फ़िक्स्ड: व्यय उद्देश्य से खोज करने पर **व्यय अनुमोदन** पृष्ठ पर खोज कार्यक्षमता काम नहीं करती है.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-116">Fixed: Search functionality on the **Expense approval** page does not work when searching by expense purpose.</span></span>

- <span data-ttu-id="7c4c3-117">संसाधन प्रबंधन</span><span class="sxs-lookup"><span data-stu-id="7c4c3-117">Resource Management</span></span>

     - <span data-ttu-id="7c4c3-118">फ़िक्स्ड: समायोजन में संख्याओ को दाहिनी ओर जस्टिफ़ाई पर अपडेट किया गया है.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-118">Fixed: Numbers in the reconciliation have been updated to be right justified.</span></span>
     - <span data-ttu-id="7c4c3-119">फ़िक्स्ड: नामित संसाधनों को **शेड्यूल** टैब के माध्यम से कार्यों को असाइन नहीं किया जा सकता.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-119">Fixed: Named Resources can't be assigned to tasks through the **Schedule** tab.</span></span>

- <span data-ttu-id="7c4c3-120">परियोजना प्रबंधन</span><span class="sxs-lookup"><span data-stu-id="7c4c3-120">Project Management</span></span>

     - <span data-ttu-id="7c4c3-121">फ़िक्स्ड: टीम सदस्य को असाइन करते समय नल संदर्भ अपवाद, जब **TransactionType**, **इकाई** और **DefaultGroup** के लिए सेटअप जानकारी उपलब्ध न हो.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-121">Fixed: Null reference exception when assigning team member when the **TransactionType** is missing setup information for **Unit** and **DefaultGroup**.</span></span>

- <span data-ttu-id="7c4c3-122">Sales</span><span class="sxs-lookup"><span data-stu-id="7c4c3-122">Sales</span></span>

     - <span data-ttu-id="7c4c3-123">फ़िक्स्ड: डुप्लिकेट ट्रांजेक्शन टाइप रिकॉर्ड एक त्रुटि लौटाते हैं जब भूमिका मूल्य रिकॉर्ड बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-123">Fixed: Duplicate transaction type records return an error when role price records are created.</span></span>
     - <span data-ttu-id="7c4c3-124">ठीक किया गया: **नया अवसर**, **कोट**, **ऑर्डर पंक्ति**, और **उत्पाद जोड़ें** के लिए अतिरिक्त बटन, अवसर, कोट, उत्पाद ऑर्डर और परियोजना-आधारित पंक्ति सबग्रिड के आदेशों में दिखाई देते हैं.</span><span class="sxs-lookup"><span data-stu-id="7c4c3-124">Fixed: Extra buttons for **New Opportunity**, **Quote**, **Order Line**, and **Add Product** are visible in commands for Opportunities, Quotes, Order Products, and the project-based Lines subgrid.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]