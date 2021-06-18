---
title: Project Service Automation के अपडेट रिलीज़ 24, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 24, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 10/02/2020
ms.topic: article
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: c95a9dcada4fbf6c462df29d450aaafab4e73aa5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000258"
---
# <a name="project-service-automation-update-release-24-v3"></a><span data-ttu-id="fdd81-103">Project Service Automation V3 अद्यतन रिलीज़ 24, V3</span><span class="sxs-lookup"><span data-stu-id="fdd81-103">Project Service Automation Update Release 24, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="fdd81-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="fdd81-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="fdd81-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="fdd81-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="fdd81-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="fdd81-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="fdd81-107">इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="fdd81-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="fdd81-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="fdd81-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="fdd81-109">यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 24 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="fdd81-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 24.</span></span> <span data-ttu-id="fdd81-110">इस वर्ज़न की बिल्ड संख्या V 3.10.42.43 है और यह आमतौर पर अक्तूबर 2020 के सेल्फ-अपडेट के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="fdd81-110">This version has a build number of V 3.10.42.43 and is generally available through a self-update in October 2020.</span></span>

## <a name="update-release-24"></a><span data-ttu-id="fdd81-111">अपडेट रिलीज़ 24</span><span class="sxs-lookup"><span data-stu-id="fdd81-111">Update Release 24</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="fdd81-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="fdd81-112">Bug fixes</span></span>

<span data-ttu-id="fdd81-113">**Sales**</span><span class="sxs-lookup"><span data-stu-id="fdd81-113">**Sales**</span></span>

<span data-ttu-id="fdd81-114">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="fdd81-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="fdd81-115">उत्पादों की डिफ़ॉल्ट मूल्य सूची सेट करते समय समस्या.</span><span class="sxs-lookup"><span data-stu-id="fdd81-115">Problem while setting default price list of products.</span></span>
- <span data-ttu-id="fdd81-116">एम्बेडे की गई मूल्य सूची और भूमिका मूल्य रिकॉर्ड प्रतिलिपि के कारण कोट जीत का प्रदर्शन धीमा है.</span><span class="sxs-lookup"><span data-stu-id="fdd81-116">Performance of Quote win is slow due to the embedded price list and role price records copy.</span></span>
- <span data-ttu-id="fdd81-117">**परियोजना अनुबंध/विक्रय हब** > **उत्पाद लाइन आइटम/ऑर्डर लाइन मात्रा** को स्वचालित रूप से निकटतम पूर्णांक पर राउंड कर दिया जाता है.</span><span class="sxs-lookup"><span data-stu-id="fdd81-117">**Project Contract/Sales Hub** > **Product Line Item/Order Line Quantity** is automatically rounded to the nearest integer.</span></span>
- <span data-ttu-id="fdd81-118">मूल्य सूचियाँ पढ़ते समय सिस्टम विशेषाधिकारों को बढ़ाएँ.</span><span class="sxs-lookup"><span data-stu-id="fdd81-118">Elevate to system privileges when reading price lists.</span></span>
- <span data-ttu-id="fdd81-119">ग्राहक पता फ़ील्ड **address1_freighttermscode** और **address1_shippingmethodcode** की प्रतिलिपि कोट/ऑर्डर में बनाएँ.</span><span class="sxs-lookup"><span data-stu-id="fdd81-119">Copy customer address fields **address1_freighttermscode** and **address1_shippingmethodcode** to Quote/Order.</span></span> 


<span data-ttu-id="fdd81-120">**समय और व्यय**</span><span class="sxs-lookup"><span data-stu-id="fdd81-120">**Time and Expense**</span></span>

<span data-ttu-id="fdd81-121">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="fdd81-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="fdd81-122">**समय प्रविष्टि ग्रिड** **केवल दिनांक** समय व्यवहार का समर्थन नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="fdd81-122">The **Time Entry Grid** doesn't support **Date Only** time behavior.</span></span>
- <span data-ttu-id="fdd81-123">**समय प्रविष्टि** स्वचालित रूप से ताज़ा नहीं होती है.</span><span class="sxs-lookup"><span data-stu-id="fdd81-123">**Time Entry** is not refreshing automatically.</span></span> <span data-ttu-id="fdd81-124">खुद से ताज़ा करना पड़ता है.</span><span class="sxs-lookup"><span data-stu-id="fdd81-124">A manual refresh is required.</span></span>
- <span data-ttu-id="fdd81-125">किसी संसाधन के असाइनमेंट में कोई ब्रेक (0 घंटे) होने पर असाइनमेंट से समय प्रविष्टियों को आयात करने में असमर्थ.</span><span class="sxs-lookup"><span data-stu-id="fdd81-125">Unable to import the time entries from an assignment when there is a break (0 hours) in a resource's assignments.</span></span>
- <span data-ttu-id="fdd81-126">समय प्रविष्टि बनाते समय, प्रारंभ को **msdyn_date** पर ही सेट करें.</span><span class="sxs-lookup"><span data-stu-id="fdd81-126">When creating a time entry, set the start to the same as **msdyn_date**.</span></span>
- <span data-ttu-id="fdd81-127">समय प्रविष्टि के लिए बल्क संपादन को पुनः सक्षम करें.</span><span class="sxs-lookup"><span data-stu-id="fdd81-127">Re-enable bulk edit for time entry.</span></span>

<span data-ttu-id="fdd81-128">**संसाधन प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="fdd81-128">**Resource Management**</span></span>

<span data-ttu-id="fdd81-129">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="fdd81-129">The following issues have been fixed:</span></span>

- <span data-ttu-id="fdd81-130">आवश्यकता के बिना इंटर-डे बुकिंग की स्थिति को अपडेट करने की कोशिश करने से अशक्तता-संदर्भ अपवाद आएगा.</span><span class="sxs-lookup"><span data-stu-id="fdd81-130">Trying to update the status of an inter-day booking without a requirement will throw a null-ref exception.</span></span>
- <span data-ttu-id="fdd81-131">**मिलान दृश्य** को लोड करने में त्रुटि.</span><span class="sxs-lookup"><span data-stu-id="fdd81-131">Error loading the **Reconciliation View**.</span></span>


<span data-ttu-id="fdd81-132">**परियोजना प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="fdd81-132">**Project Management**</span></span>

<span data-ttu-id="fdd81-133">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="fdd81-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="fdd81-134">**परियोजना शेड्यूल** में, **मैनुअल** को **ऑटो** में बदलते समय, सव सहेजें पूरा नहीं हो रहा है.</span><span class="sxs-lookup"><span data-stu-id="fdd81-134">In the **Project Schedule**, when changing from **Manual** to **Auto**, auto save is not completing.</span></span>
- <span data-ttu-id="fdd81-135">व्यय लागतों को **परियोजना ट्रैकिंग ग्रिड** पर भिन्नता की ओर गणना नहीं करनी चाहिए.</span><span class="sxs-lookup"><span data-stu-id="fdd81-135">Expense costs should not calculate toward variance on the **Project Tracking Grid**.</span></span>
- <span data-ttu-id="fdd81-136">लोड करने के दौरान **अनुमान टैग** स्तंभ के लिए असंगत व्यवहार बनाम **समय-चरण** प्रकार को बदलना.</span><span class="sxs-lookup"><span data-stu-id="fdd81-136">Inconsistent behavior for **Estimates tag** columns during load versus changing the **Time-Phase** type.</span></span>
- <span data-ttu-id="fdd81-137">हो सकता है कि किसी परियोजना की वास्तविक लागत **वास्तविक** से योग को न दर्शाए.</span><span class="sxs-lookup"><span data-stu-id="fdd81-137">The actual cost on a project may not reflect the totals from **Actuals**.</span></span>
- <span data-ttu-id="fdd81-138">**सारांश** टैब पर **अनुमानित समाप्ति दिनांक** **WBS शेड्यूल** से मेल नहीं खाती है.</span><span class="sxs-lookup"><span data-stu-id="fdd81-138">**Estimated Finish Date** on the **Summary** tab does not match the **WBS Schedule**.</span></span>
- <span data-ttu-id="fdd81-139">आउटडेंट पर **वास्तविक कार्य अपडेट करें** सही ढंग से काम नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="fdd81-139">**Update Actual Hours** on outdent does not work correctly.</span></span>
- <span data-ttu-id="fdd81-140">रूट **BU** के बाहर का कोई परियोजना प्रबंधक एक परियोजना नहीं बना सकता है.</span><span class="sxs-lookup"><span data-stu-id="fdd81-140">A Project manager outside of root **BU** can't create a project.</span></span>
- <span data-ttu-id="fdd81-141">**व्यय अनुमान** पर कार्य या श्रेणी में परिवर्तन कायम नहीं हैं.</span><span class="sxs-lookup"><span data-stu-id="fdd81-141">Changes to task or category on **Expense Estimates** are not persisted.</span></span>
- <span data-ttu-id="fdd81-142">**अनुबंध की प्रतिलिपि** इनवॉइस शेड्यूल और रन स्थिति की प्रतिलिपि बनाता है.</span><span class="sxs-lookup"><span data-stu-id="fdd81-142">**Copy of contract** copies the invoice schedules and the run status.</span></span>
- <span data-ttu-id="fdd81-143">**वास्तविक को ताज़ा करें** बटन सारांश कार्यों की गलत तरीके से गणना करता है.</span><span class="sxs-lookup"><span data-stu-id="fdd81-143">**Refresh Actuals** button incorrectly calculates summary tasks.</span></span>
- <span data-ttu-id="fdd81-144">Microsoft परियोजना ऐड-इन: यदि किसी टीम सदस्य के पास रिक्त संसाधन इकाई है, तो अशक्त संदर्भ त्रुटि को ठीक करें.</span><span class="sxs-lookup"><span data-stu-id="fdd81-144">Microsoft Project Add-in: Fix null reference error if any team member has an empty resourcing unit.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]