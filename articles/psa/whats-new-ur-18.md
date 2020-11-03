---
title: Project Service Automation के अपडेट रिलीज़ 18, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 18, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 04/27/2020
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
ms.openlocfilehash: 1d7ea200531dd24d56a829f879e3a2532a9b38dc
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077654"
---
# <a name="project-service-automation-update-release-18-v3"></a><span data-ttu-id="c81de-103">Project Service Automation V3 अद्यतन रिलीज़ 18, V3</span><span class="sxs-lookup"><span data-stu-id="c81de-103">Project Service Automation Update Release 18, V3</span></span>

<span data-ttu-id="c81de-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="c81de-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="c81de-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="c81de-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="c81de-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="c81de-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="c81de-107">इस रिलीज़ को अपडेट करने के लिए, Dynamics 365 online के लिए व्यवस्थापन केंद्र पर जाएँ और अपडेट को स्थापित करने के लिए समाधान पृष्ठ पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="c81de-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="c81de-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="c81de-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="c81de-109">यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 18 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="c81de-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 18.</span></span> <span data-ttu-id="c81de-110">इस संस्करण की बिल्ड संख्या V3.10.8.12 है और यह आमतौर पर अप्रैल 2020 में एक स्व-अद्यतन के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="c81de-110">This version has a build number of V3.10.8.12 and is generally available through a self-update in April 2020.</span></span>

## <a name="update-release-18"></a><span data-ttu-id="c81de-111">अपडेट रिलीज़ 18</span><span class="sxs-lookup"><span data-stu-id="c81de-111">Update Release 18</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="c81de-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="c81de-112">Bug fixes</span></span>

<span data-ttu-id="c81de-113">**समय और व्यय**</span><span class="sxs-lookup"><span data-stu-id="c81de-113">**Time and Expense**</span></span>

- <span data-ttu-id="c81de-114">सुधार किया गया: **रिकॉल करें** , **अनुरोध करें** और **अनुमोदन रद्द करें** प्रवाह अस्पष्ट त्रुटि संदेशों के साथ अपवाद दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="c81de-114">Fixed: **Recall** , **Request** , and **Cancel Approval** flows throw exceptions with unclear error messages.</span></span>
- <span data-ttu-id="c81de-115">सुधार किया गया: जब **अनुमोदन रद्द करें** किसी व्यय के लिए विफल हो जाता है, तो एक प्रासंगिक अपवाद त्रुटि नहीं दिखाई जाती है.</span><span class="sxs-lookup"><span data-stu-id="c81de-115">Fixed: When **Cancel Approval** fails for an expense, a relevant exception error is not thrown.</span></span>
- <span data-ttu-id="c81de-116">सुधार किया गया: टाइम एंट्री ग्रिड अक्टूबर में डेलाइट सेविंग टाइम (DST) स्विच के बाद ऑस्ट्रेलिया में गैर-कार्य दिवसों को गलत तरीके से संभालती है.</span><span class="sxs-lookup"><span data-stu-id="c81de-116">Fixed: The Time Entry grid incorrectly handles non-working days in Australia after the daylight savings time (DST) switch in October.</span></span>
- <span data-ttu-id="c81de-117">सुधार किया गया: गलत डिफ़ॉल्टिंग लॉजिक व्ययों के सबमिशन को रोकता है.</span><span class="sxs-lookup"><span data-stu-id="c81de-117">Fixed: Incorrect defaulting logic prevents submission of expenses.</span></span>
- <span data-ttu-id="c81de-118">सुधार किया गया: जब समय प्रविष्टि स्वीकृति विफल हो जाती है, तो अनुमोदन **लंबित** की स्थिति में बना रहता है.</span><span class="sxs-lookup"><span data-stu-id="c81de-118">Fixed: When time entry approval fails, the approval remains in a state of **Pending**.</span></span>
- <span data-ttu-id="c81de-119">सुधार किया गया: बल्क अनुमोदन पर SQL त्रुटियाँ (डेडलॉक/टाइमआउट).</span><span class="sxs-lookup"><span data-stu-id="c81de-119">Fixed: SQL Errors on bulk approvals (deadlock/timeout).</span></span>
- <span data-ttu-id="c81de-120">सुधार किया गया: समय प्रविष्टियों को अनुमोदन देते समय टीम के सदस्यों को अपडेट करने के कारण उपयोगकर्ता अनुभव में महत्वपूर्ण प्रदर्शन समस्याएँ.</span><span class="sxs-lookup"><span data-stu-id="c81de-120">Fixed: Significant performance issues in the user experience caused by updating team members while approving time entries.</span></span>

<span data-ttu-id="c81de-121">**परियोजना प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="c81de-121">**Project Management**</span></span>

- <span data-ttu-id="c81de-122">सुधार किया गया: टाइम ज़ोन अधिसूचना **समायोजन** दृश्य से **प्रोजेक्ट** मुख्य प्रपत्र में स्थानांतरित हो गया.</span><span class="sxs-lookup"><span data-stu-id="c81de-122">Fixed: Time zone notification moved from the **Reconciliation** view to the **Project** main form.</span></span>
- <span data-ttu-id="c81de-123">सुधार किया गया: नया प्रोजेक्ट प्रपत्र खुलने पर कैलेंडर टेम्पलेट सही तरीके से डिफ़ॉल्ट नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="c81de-123">Fixed: Calendar template is not correctly defaulting when a new project form opens.</span></span>
- <span data-ttu-id="c81de-124">सुधार किया गया: क्रोमियम-आधारित ब्राउज़रों के लिए, उपयोगकर्ता हटाने के लिए पूर्ववर्ती कार्यों का आसानी से चयन करने में असमर्थ हैं.</span><span class="sxs-lookup"><span data-stu-id="c81de-124">Fixed: For chromium-based browsers, users are unable to easily select predecessor tasks to delete.</span></span>
- <span data-ttu-id="c81de-125">सुधार किया गया: **खाली टेम्पलेट से प्रोजेक्ट** बनाने या कॉपी करने से असंबंधित असाइनमेंट फ़ेच होता है.</span><span class="sxs-lookup"><span data-stu-id="c81de-125">Fixed: Creating or copying **Project from Empty template** fetches unrelated assignments.</span></span>
- <span data-ttu-id="c81de-126">सुधार किया गया: विशिष्ट Edge मामलों में, टास्क ग्रिड से एक नया असाइनमेंट बनाने से डुप्लिकेट रिकॉर्ड बन रहा है.</span><span class="sxs-lookup"><span data-stu-id="c81de-126">Fixed: In specific edge cases, creating a new assignment from the task grid results in duplicate records being created.</span></span>
- <span data-ttu-id="c81de-127">सुधार किया गया: मैनुअल मोड में, उपयोगकर्ता कार्य के प्रारंभ होने की तिथि को वर्तमान में सहेजी गई तिथि के बाद की तिथि में अपडेट करने में असमर्थ हैं.</span><span class="sxs-lookup"><span data-stu-id="c81de-127">Fixed: In manual mode, users are unable to update task start dates to be later than the current date saved.</span></span>

<span data-ttu-id="c81de-128">**संसाधन प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="c81de-128">**Resource Management**</span></span>

- <span data-ttu-id="c81de-129">सुधार किया गया: **समायोजन** दृश्य उपयोग पंक्ति बुकिंग बढ़ाने के बाद बुकिंग भिन्नता की गलत तरीके से गणना करता है.</span><span class="sxs-lookup"><span data-stu-id="c81de-129">Fixed: **Reconciliation** view subtotal row incorrectly calculates bookings variance after extending bookings.</span></span>
- <span data-ttu-id="c81de-130">सुधार किया गया: जब बुक करने योग्य संसाधन में ऐसा कैलेंडर होता है, जो प्रोजेक्ट कैलेंडर से मेल नहीं खाता है, तो **समायोजन** दृश्य संसाधन असाइनमेंट को गलत तरीके से प्रदर्शित करता है.</span><span class="sxs-lookup"><span data-stu-id="c81de-130">Fixed: **Reconciliation** view incorrectly displays resource assignments when the bookable resource has a calendar that does not match the project calendar.</span></span>

<span data-ttu-id="c81de-131">**Sales**</span><span class="sxs-lookup"><span data-stu-id="c81de-131">**Sales**</span></span>

- <span data-ttu-id="c81de-132">सुधार किया गया: जब समय प्रविष्टियों का फिर से अनुमोदन ( **अनुमोदन करें > रद्द करें >** फिर से अनुमोदन करें) किया जाता है, तो एक डुप्लिकेट नॉन-चार्जिएबल एक्चुअल बन जाता है.</span><span class="sxs-lookup"><span data-stu-id="c81de-132">Fixed: When time entries are re-approved ( **Approve > Cancel >** approve again), a duplicate non-chargeable actual is created.</span></span>
