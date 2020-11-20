---
title: Project Service Automation के अपडेट रिलीज़ 14, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह टॉपिक Project Service Automation अपडेट रिलीज़ 14 V3 में क्या नया है, इसके बारे में जानकारी प्रदान करता है.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 01/29/2020
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
ms.openlocfilehash: b811bf7ccfb626e6944801dffa943d2afab0c5e8
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4124820"
---
# <a name="project-service-automation-update-release-14-v3"></a><span data-ttu-id="a1398-103">Project Service Automation V3 अद्यतन रिलीज़ 14, V3</span><span class="sxs-lookup"><span data-stu-id="a1398-103">Project Service Automation Update Release 14, V3</span></span>
<span data-ttu-id="a1398-104">हमें Dynamics 365 Project Service Automation (PSA) अनुप्रयोग के लिए नवीनतम अपडेट की घोषणा करते हुए बेहद खुशी है.</span><span class="sxs-lookup"><span data-stu-id="a1398-104">We’re pleased to announce the latest update for the Dynamics 365 Project Service Automation (PSA) application.</span></span> <span data-ttu-id="a1398-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="a1398-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="a1398-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="a1398-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="a1398-107">इस रिलीज़ पर अपडेट करने के लिए, Dynamics 365 online के लिए व्यवस्थापन केंद्र पर जाएँ, और अपडेट को स्थापित करने के लिए समाधान पृष्ठ पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="a1398-107">To update to this release, visit the Admin Center for Dynamics 365 online, and go to the solutions page to install the update.</span></span> <span data-ttu-id="a1398-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="a1398-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="a1398-109">यह टॉपिक PSA V3, अपडेट रिलीज़ 14 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="a1398-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 14.</span></span> <span data-ttu-id="a1398-110">इस वर्ज़न की बिल्ड संख्या V3.10.4.21 है और यह निम्नलिखित शेड्यूल पर उपलब्ध है:</span><span class="sxs-lookup"><span data-stu-id="a1398-110">This version has a build number of V3.10.4.21 and is available on the following schedule:</span></span>

- <span data-ttu-id="a1398-111">**सामान्य उपलब्धता (सेल्फ-अपडेट):** जनवरी 2020</span><span class="sxs-lookup"><span data-stu-id="a1398-111">**General availability (self-update):** January 2020</span></span>
- <span data-ttu-id="a1398-112">**ऑटो-अपडेट:** फरवरी 2020</span><span class="sxs-lookup"><span data-stu-id="a1398-112">**Auto-update:** February 2020</span></span>

## <a name="update-release-14"></a><span data-ttu-id="a1398-113">अपडेट रिलीज़ 14</span><span class="sxs-lookup"><span data-stu-id="a1398-113">Update Release 14</span></span>

### <a name="enhancements"></a><span data-ttu-id="a1398-114">एन्हांसमेंट</span><span class="sxs-lookup"><span data-stu-id="a1398-114">Enhancements</span></span>

- <span data-ttu-id="a1398-115">Sales</span><span class="sxs-lookup"><span data-stu-id="a1398-115">Sales</span></span>

     - <span data-ttu-id="a1398-116">**उद्धरण पंक्ति विवरण** से कस्टम फील्ड मानों को **परियोजना अनुबंध पंक्ति विवरण** में कॉपी किया जाता है, जब किसी उद्धरण को **जीत के रूप में बंद** पर अपडेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="a1398-116">Custom field values from **Quote Line Details** are copied to **Project Contract Line Details** when a quote is updated to **Closed as won**.</span></span>
     - <span data-ttu-id="a1398-117">पुष्टि की गई परियोजनाओं को **खो जाने के रूप में बंद** किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="a1398-117">Confirmed projects can be **Closed as lost**.</span></span>

- <span data-ttu-id="a1398-118">संसाधन प्रबंधन</span><span class="sxs-lookup"><span data-stu-id="a1398-118">Resource Management</span></span>

     - <span data-ttu-id="a1398-119">बुकिंग का विस्तार करते समय, उपयोगकर्ताओं को पुष्टिकरण संवाद बॉक्स के साथ बुकिंग परिणामों को सारांशित करने के लिए और बुकिंग को बनाए रखने के लिए एक लिंक प्रदान करने के लिए पूछा जाएगा.</span><span class="sxs-lookup"><span data-stu-id="a1398-119">When extending bookings, users will be prompted with a confirmation dialog box to summarize booking results and provide a link to Maintain Bookings.</span></span>


### <a name="bug-fixes"></a><span data-ttu-id="a1398-120">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="a1398-120">Bug fixes</span></span>

- <span data-ttu-id="a1398-121">समय और व्यय</span><span class="sxs-lookup"><span data-stu-id="a1398-121">Time and Expense</span></span>

     - <span data-ttu-id="a1398-122">फ़िक्स्ड: किसी उपयोगकर्ता द्वारा किसी भी प्रविष्टि को सही करने के लिए न चुनने पर बेहतर उपयोगकर्ता अनुभव.</span><span class="sxs-lookup"><span data-stu-id="a1398-122">Fixed: Improved the user experience when the user has not selected any entries to be corrected.</span></span>

- <span data-ttu-id="a1398-123">संसाधन प्रबंधन</span><span class="sxs-lookup"><span data-stu-id="a1398-123">Resource Management</span></span>

     - <span data-ttu-id="a1398-124">फ़िक्स्ड: किसी भी संसाधन को कई बार बुक करने से बुक करने योग्य संसाधन का नाम ओवरफ़्लो हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="a1398-124">Fixed: Booking a resource multiple times overflows the name of the bookable resource.</span></span>

- <span data-ttu-id="a1398-125">Sales</span><span class="sxs-lookup"><span data-stu-id="a1398-125">Sales</span></span>

     - <span data-ttu-id="a1398-126">फ़िक्स्ड: कुल विक्रय मूल्य की गणना तब तक नहीं की जाती है जब तक उपयोगकर्ता किसी परियोजना पर व्यय अनुमानों के लिए लागत मूल्य इनपुट नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="a1398-126">Fixed: The total sales price is not calculated until the user also inputs a cost price for expense estimates on a project.</span></span>
     - <span data-ttu-id="a1398-127">फ़िक्स्ड: किसी उद्धरण को **जीत** के रूप में बंद करना विफल हो जाता है, यदि संबद्ध परियोजना अनुबंध **ड्राफ्ट** स्थिति में नहीं है.</span><span class="sxs-lookup"><span data-stu-id="a1398-127">Fixed: Closing a quote as **Won** fails if the associated project contract is not in a **Draft** state.</span></span>

