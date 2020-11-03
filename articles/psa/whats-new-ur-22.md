---
title: Project Service Automation के अपडेट रिलीज़ 22, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 22, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 07/28/2020
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
ms.openlocfilehash: badd87a276d68d9959e9cca4220daf61ed570638
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077648"
---
# <a name="project-service-automation-update-release-22-v3"></a><span data-ttu-id="4b7b4-103">Project Service Automation V3 अद्यतन रिलीज़ 22, V3</span><span class="sxs-lookup"><span data-stu-id="4b7b4-103">Project Service Automation Update Release 22, V3</span></span>

<span data-ttu-id="4b7b4-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="4b7b4-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="4b7b4-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="4b7b4-107">इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="4b7b4-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="4b7b4-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="4b7b4-109">यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 22 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 22.</span></span> <span data-ttu-id="4b7b4-110">इस संस्करण की बिल्ड संख्या V 3.10.33.48 है और यह आमतौर पर जून 2020 में एक स्व-अद्यतन के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-110">This version has a build number of V 3.10.33.48 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-22"></a><span data-ttu-id="4b7b4-111">अपडेट रिलीज़ 22</span><span class="sxs-lookup"><span data-stu-id="4b7b4-111">Update Release 22</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="4b7b4-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="4b7b4-112">Bug fixes</span></span>



<span data-ttu-id="4b7b4-113">**समय और व्यय**</span><span class="sxs-lookup"><span data-stu-id="4b7b4-113">**Time and Expense**</span></span>

<span data-ttu-id="4b7b4-114">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="4b7b4-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="4b7b4-115">**समय प्रविष्टियाँ** आयात के बाद समय प्रविष्टि शेड्यूल में स्वचालित रूप से नहीं जोड़ी जाती हैं.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-115">**Time entries** are not automatically added in the Time entries schedule after import.</span></span>
- <span data-ttu-id="4b7b4-116">**समय प्रविष्टि** ग्रिड दिनांक पिकर उपयोगकर्ता की क्षेत्रीय सेटिंग को नहीं पहचानता है.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-116">The **Time Entry** grid date picker does not recognize a user's regional settings.</span></span>

<span data-ttu-id="4b7b4-117">**संसाधन प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="4b7b4-117">**Resource Management**</span></span>

<span data-ttu-id="4b7b4-118">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="4b7b4-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="4b7b4-119">मैनुअल मोड में, **संसाधन असाइनमेंट** रूपरेखा में परिवर्तन, **संसाधन आवश्यकताएं** जनरेट करते समय पहचाने नहीं जाते.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-119">In manual mode, changes to **Resource Assignment** contours are not recognized when generating **Resource Requirements**.</span></span>
- <span data-ttu-id="4b7b4-120">**संसाधन अनुरोध** कस्टम अनुरोध स्थितियों का समर्थन नहीं करते.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-120">**Resource Requests** do not support custom request statuses.</span></span>

<span data-ttu-id="4b7b4-121">**परियोजना प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="4b7b4-121">**Project Management**</span></span>

<span data-ttu-id="4b7b4-122">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="4b7b4-122">The following issues have been fixed:</span></span>

- <span data-ttu-id="4b7b4-123">EstimateGridControl पर डबल-क्लिक का उपयोग डच स्वरूप संख्याओं को सही ढंग से पार्स नहीं करेगा.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-123">Using double-click on EstimateGridControl will not correctly parse Dutch format numbers.</span></span>
- <span data-ttu-id="4b7b4-124">Microsoft परियोजना डेस्कटॉप क्लाइंट ऐड-इन का उपयोग करके असाइनमेंट बदले जाने पर असाइन किए गए घंटे सही ढंग से अद्यतन नहीं होते हैं.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-124">Assigned hours do not update correctly when assignments are changed using the Microsoft Project desktop client add-in.</span></span>
- <span data-ttu-id="4b7b4-125">जब अनुबंध मुद्रा, ग्राहक मुद्रा से भिन्न होती है और संगठन मुद्रा चिह्नों के बजाय मुद्रा कोड प्रदर्शित करने के लिए कॉन्फ़िगर की गई होती है, तो परियोजना ट्रैकिंग और अनुमान ग्रिड गलत विक्रय मुद्रा कोड प्रदर्शित करते हैं.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-125">Project Tracking and Estimates grids display incorrect sales currency code when contract currency is different than customer currency and organization is configured to display currency codes instead of currency symbols.</span></span>
- <span data-ttu-id="4b7b4-126">यदि कार्य समय शेड्यूल 24 घंटे प्रति दिन है, तो टीम सदस्य का समाप्ति दिनांक एक दिन जोड़ देगा.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-126">A Team member's finish date will add one day if the work hour schedule is 24-hours per day.</span></span>
- <span data-ttu-id="4b7b4-127">परियोजना शेड्यूल पर, किसी कार्य के लिए लेन-देन श्रेणी को जोड़ना, स्वतः सहेजें को ट्रिगर नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-127">On the Project Schedule, adding a Transaction Category to a task does not trigger auto save.</span></span>
- <span data-ttu-id="4b7b4-128">परियोजना टेम्पलेट में टीम के सदस्य को जोड़ते समय निम्न त्रुटि प्रदर्शित होती है: "संसाधन आवश्यकताओं को परियोजना टेम्पलेट से संबद्ध नहीं किया जा सकता".</span><span class="sxs-lookup"><span data-stu-id="4b7b4-128">The following error is displayed when adding a team member to the Project Template: "Resource requirements cannot be associated with project templates".</span></span> 
- <span data-ttu-id="4b7b4-129">रिबन नियम स्क्रिप्ट "msdyn.Approval.CanApproveOrReject" एक टाइमआउट त्रुटि प्रदर्शित करती है.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-129">Ribbon rule script "msdyn.Approval.CanApproveOrReject" displays a timeout error.</span></span>

<span data-ttu-id="4b7b4-130">**Sales**</span><span class="sxs-lookup"><span data-stu-id="4b7b4-130">**Sales**</span></span>

<span data-ttu-id="4b7b4-131">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="4b7b4-131">The following issues have been fixed:</span></span>

- <span data-ttu-id="4b7b4-132">'नई कोट परियोजना मूल्य सूची' प्रपत्र/निकाय पर मूल्य सूची लुकअप में लागत मूल्य सूची के चुने जाने पर प्रमाणीकरण त्रुटि संदेश प्रदर्शित नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-132">Validation error message not displayed when a Cost Price List is selected in Price List lookup on 'New Quote Project Price List' form/entity.</span></span>
- <span data-ttu-id="4b7b4-133">यदि कोट से संलग्न BPF अंतिम चरण में है, तो कोट को जीते गए के रूप में बंद करना, बनाए गए अनुबंध पर नेविगेट नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-133">Closing the quote as won does not navigate to the created contract if a BPF attached to the quote is in the final stage.</span></span>
- <span data-ttu-id="4b7b4-134">समय प्रविष्टि को रीकॉल किए जाने पर रीवर्सिंग **बिल न की गई विक्रय** मूल लागत से लिंक की जाती है.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-134">Reversing **Unbilled Sales** is linked to original cost when a time entry is recalled.</span></span>
- <span data-ttu-id="4b7b4-135">**पुष्टि करें** बटन चुने जाने के बाद, इनवॉइस स्थिति तब तक **पुष्टि हुई** में नहीं बदलती है, जब तक इनवॉइस को रीफ़्रेश न किए जाए.</span><span class="sxs-lookup"><span data-stu-id="4b7b4-135">After selecting the **Confirm** button, the invoice status doesn't change to **Confirmed** unless the invoice is refreshed.</span></span>
