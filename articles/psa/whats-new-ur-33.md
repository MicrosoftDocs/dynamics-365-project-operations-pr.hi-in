---
title: Project Service Automation के अपडेट रिलीज़ 33, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 33, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 06/30/2021
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
ms.openlocfilehash: 2c96e4abd484bb66285421baaad82ead9589bbe9
ms.sourcegitcommit: be5beba71ee9770c0083b4fe5cc89e7ec6b741b8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334548"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-33-v3"></a><span data-ttu-id="2f11a-103">Project Service Automation के अपडेट रिलीज़ 33, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है</span><span class="sxs-lookup"><span data-stu-id="2f11a-103">What's new or changed in Project Service Automation Update Release 33, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="2f11a-104">हमें Microsoft Dynamics 365 Project Service Automation अनुप्रयोग के लिए नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="2f11a-104">We're pleased to announce the latest update for the Microsoft Dynamics 365 Project Service Automation app.</span></span> <span data-ttu-id="2f11a-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="2f11a-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="2f11a-106">यह Dynamics 365 9.x से मेल के योग्य है.</span><span class="sxs-lookup"><span data-stu-id="2f11a-106">It's compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="2f11a-107">इस रिलीज़ में अद्यतन करने के लिए, Dynamics 365 ऑनलाइन समाधान के लिए व्यवस्थापन केंद्र पृष्ठ पर जाएं और अद्यतन इंस्टॉल करें.</span><span class="sxs-lookup"><span data-stu-id="2f11a-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page, and install the update.</span></span> <span data-ttu-id="2f11a-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="2f11a-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="2f11a-109">यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 33 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="2f11a-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 33.</span></span> <span data-ttu-id="2f11a-110">इस संस्करण में V3.10.54.98 का बिल्ड नंबर है और यह आम तौर पर जुलाई 2021 में स्व-अद्यतन के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="2f11a-110">This version has a build number of V3.10.54.98 and is generally available through a self-update in July 2021.</span></span>

## <a name="update-release-33"></a><span data-ttu-id="2f11a-111">अपडेट रिलीज़ 33</span><span class="sxs-lookup"><span data-stu-id="2f11a-111">Update Release 33</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="2f11a-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="2f11a-112">Bug fixes</span></span>

<span data-ttu-id="2f11a-113">**समय और व्यय**</span><span class="sxs-lookup"><span data-stu-id="2f11a-113">**Time and Expense**</span></span>

<span data-ttu-id="2f11a-114">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="2f11a-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="2f11a-115">दो लॉक फ़ील्ड, **msdyn_description** तथा **msdyn_externaldescription** सबमिट करने के बाद संपादन योग्य हैं.</span><span class="sxs-lookup"><span data-stu-id="2f11a-115">Two locked fields, **msdyn_description** and **msdyn_externaldescription** are editable after submission.</span></span>
- <span data-ttu-id="2f11a-116">एक त्रुटि संदेश तब होता है जब कोई व्यय बनाया जाता है जो किसी प्रोजेक्ट से संबंधित नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="2f11a-116">An error message occurs if an expense is created that isn't related to a project.</span></span>
- <span data-ttu-id="2f11a-117">जब समय प्रविष्टि बनाई जाती है, तो संसाधन भूमिका डिफ़ॉल्ट रूप से निष्क्रिय भूमिका में बदल जाती है.</span><span class="sxs-lookup"><span data-stu-id="2f11a-117">When a time entry is created, the resource role defaults to an inactive role.</span></span>
- <span data-ttu-id="2f11a-118">रीकॉल किए गए और हटाए गए व्यय के साथ जुड़ी जर्नल लाइन नहीं हटाई जाती हैं.</span><span class="sxs-lookup"><span data-stu-id="2f11a-118">Journal lines associated with a recalled and deleted expense aren't deleted.</span></span>
- <span data-ttu-id="2f11a-119">डिफ़ॉल्ट रूप से प्रदर्शित तिथि को कार्य की प्रारंभ तिथि में बदलने के लिए, **समय प्रविष्टि त्वरित प्रपत्र बनाएँ** पर, **प्रोजेक्ट कार्य सूची** दृश्य को अद्यतन करें.</span><span class="sxs-lookup"><span data-stu-id="2f11a-119">On the **Time entry Quick Create Form**, update the **Project Task List** view to change the date displayed by default to the start date of the task.</span></span>
- <span data-ttu-id="2f11a-120">जब आप बुक करने योग्य संसाधन के **सम्बंधित** टैब से समय प्रविष्टि बनाते हैं, तो पैरेंट बुक करने योग्य संसाधन के बजाय साइन-इन किए गए उपयोगकर्ता के लिए समय प्रविष्टि गलत तरीके से बनाई गई है.</span><span class="sxs-lookup"><span data-stu-id="2f11a-120">When you create a time entry from the **Related** tab of the bookable resource, the time entry is incorrectly created for the signed-in user instead of the parent bookable resource.</span></span>
- <span data-ttu-id="2f11a-121">**बल्क अनुमोदन MDD** संवाद बॉक्स में नए फ़ील्ड जोड़े जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="2f11a-121">New fields are added to the **Bulk approval MDD** dialog box.</span></span>

<span data-ttu-id="2f11a-122">**परियोजना नियोजन**</span><span class="sxs-lookup"><span data-stu-id="2f11a-122">**Project planning**</span></span>

<span data-ttu-id="2f11a-123">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="2f11a-123">The following issues have been fixed:</span></span>
- <span data-ttu-id="2f11a-124">जब जटिल कैलेंडर के साथ प्रोजेक्ट कार्य घंटे टेम्प्लेट लागू किए जाते हैं, तो प्रोजेक्ट निर्माण प्रदर्शन धीमा होता है.</span><span class="sxs-lookup"><span data-stu-id="2f11a-124">Slow project creation performance when project work hour templates are applied with complex calendars.</span></span>
- <span data-ttu-id="2f11a-125">जब प्रारंभ तिथि समाप्ति तिथि से अधिक होती है, तो प्रत्येक फ़ील्ड के समय घटक में अंतर के कारण प्रतिलिपि प्रोजेक्ट टेम्प्लेट पर त्रुटि प्रदर्शित होती है.</span><span class="sxs-lookup"><span data-stu-id="2f11a-125">When the start date is greater than the end date, an error displays on the copy project template because of differences in the time component of each field.</span></span>

<span data-ttu-id="2f11a-126">**संसाधन प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="2f11a-126">**Resource management**</span></span>

<span data-ttu-id="2f11a-127">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="2f11a-127">The following issues have been fixed:</span></span>
- <span data-ttu-id="2f11a-128">संसाधन उपयोग क्वेरी में गलत मापदंड का उपयोग किया जाता है और **संसाधन प्रयोग** ग्रिड पर XML गलत फ़िल्टर परिणामों की ओर ले जाता है.</span><span class="sxs-lookup"><span data-stu-id="2f11a-128">An incorrect parameter is used in the resource utilization query and the XML leads to incorrect filter results on the **Resource Utilization** grid.</span></span>
- <span data-ttu-id="2f11a-129">**बुकिंग बढ़ाएँ** पुष्टिकरण बुकिंग के लिए गलत समाप्ति तिथि प्रदर्शित करता है.</span><span class="sxs-lookup"><span data-stu-id="2f11a-129">The **Extend Bookings** confirmation displays incorrect end date for bookings.</span></span>

<span data-ttu-id="2f11a-130">**सेल्स**</span><span class="sxs-lookup"><span data-stu-id="2f11a-130">**Sales**</span></span>

<span data-ttu-id="2f11a-131">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="2f11a-131">The following issues have been fixed:</span></span>
- <span data-ttu-id="2f11a-132">यदि कोई श्रेणी मूल्य अनुपलब्ध मानों के साथ बनाया जाता है, तो त्रुटि संदेश उत्पन्न होता है.</span><span class="sxs-lookup"><span data-stu-id="2f11a-132">An error message occurs if a category price is created with missing values.</span></span>
- <span data-ttu-id="2f11a-133">अनुबंध लाइन माइलस्टोन ऑर्डर लाइन के बिना बनाया जाता है, तो त्रुटि संदेश उत्पन्न होता है.</span><span class="sxs-lookup"><span data-stu-id="2f11a-133">An error message occurs if a contract line milestone is created without an order line.</span></span>
