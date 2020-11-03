---
title: Project Service Automation के अपडेट रिलीज़ 23, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 23, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 08/25/2020
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
ms.openlocfilehash: eaae9cc62c449695cb2e999be48c57075aadbb21
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077647"
---
# <a name="project-service-automation-update-release-23-v3"></a><span data-ttu-id="5f567-103">Project Service Automation V3 अद्यतन रिलीज़ 23, V3</span><span class="sxs-lookup"><span data-stu-id="5f567-103">Project Service Automation Update Release 23, V3</span></span>

<span data-ttu-id="5f567-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="5f567-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="5f567-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="5f567-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="5f567-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="5f567-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="5f567-107">इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="5f567-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="5f567-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="5f567-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="5f567-109">यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 23 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="5f567-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 23.</span></span> <span data-ttu-id="5f567-110">इस वर्ज़न की बिल्ड संख्या V3.10.34.30 है और यह आमतौर पर अगस्त 2020 के सेल्फ-अपडेट के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="5f567-110">This version has a build number of V 3.10.34.30 and is generally available through a self-update in August 2020.</span></span>

## <a name="update-release-23"></a><span data-ttu-id="5f567-111">अपडेट रिलीज़ 23</span><span class="sxs-lookup"><span data-stu-id="5f567-111">Update Release 23</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="5f567-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="5f567-112">Bug fixes</span></span>

<span data-ttu-id="5f567-113">**समय और व्यय**</span><span class="sxs-lookup"><span data-stu-id="5f567-113">**Time and Expense**</span></span>

<span data-ttu-id="5f567-114">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="5f567-114">The following issues have been fixed:</span></span>
- <span data-ttu-id="5f567-115">एक सार्थक अपवाद प्रदान करने के लिए **परियोजना टीम सदस्य हटाएँ** में बढ़त मामले को संभालें.</span><span class="sxs-lookup"><span data-stu-id="5f567-115">Handle edge case in **Project Team Member Delete** to provide a meaningful exception.</span></span>
- <span data-ttu-id="5f567-116">रिक्त हटाएँ स्क्रीन में असाइनमेंट आयात के परिणाम.</span><span class="sxs-lookup"><span data-stu-id="5f567-116">Assignment import results in a blank remove screen.</span></span>

<span data-ttu-id="5f567-117">**संसाधन प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="5f567-117">**Resource Management**</span></span>

<span data-ttu-id="5f567-118">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="5f567-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="5f567-119">**संसाधन उपयोग ग्रिड संसाधन कार्ड** समय का पैमाना पाँच दिनों से अधिक होने पर गलत डेटा दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="5f567-119">The **Resource utilization grid resource card** shows incorrect data when the time scale is more than five days.</span></span>
- <span data-ttu-id="5f567-120">जब ग्राहक बुक करने योग्य संसाधन बनाते हैं, तो प्लग-इन आंतरायिक रूप से संसाधन को स्वचालित रूप से Microsoft Office 365 समूह में जोड़ने में विफल रहता है.</span><span class="sxs-lookup"><span data-stu-id="5f567-120">When customers create a bookable resource, the plug-in intermittently fails to automatically add the resource to a Microsoft Office 365 group.</span></span>
- <span data-ttu-id="5f567-121">**मिलान** दृशय **सप्ताह** या **महीना** दृश्य में मैनुअल कंटूर गलत तरीके से दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="5f567-121">**Reconciliation** view displays manual contours incorrectly in the **Week** or **Month** view.</span></span>

<span data-ttu-id="5f567-122">**परियोजना प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="5f567-122">**Project Management**</span></span>

<span data-ttu-id="5f567-123">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="5f567-123">The following issues have been fixed:</span></span>

- <span data-ttu-id="5f567-124">**उपयोगकर्ता सेटिंग के लिए एकाधिक पुंरप्राप्त करें** निकाय की अत्यधिक संख्या परियोजना अनुमोदन और अन्य कार्यों के लिए कम प्रदर्शन का कारण बन रही हैं.</span><span class="sxs-lookup"><span data-stu-id="5f567-124">An excessive number of **RetrieveMultiple for usersettings** entities are causing degraded performance for project approvals and other operations.</span></span>
- <span data-ttu-id="5f567-125">**कार्य योजना** ग्रिड संसाधन लुकअप केवल परियोजना टीम के पाँच टीम सदस्यों को दिखाने तक सीमित है.</span><span class="sxs-lookup"><span data-stu-id="5f567-125">The **Task Planning** grid resource lookup is limited to only show up to five team members from the project team.</span></span> 
- <span data-ttu-id="5f567-126">**कार्य योजना** ग्रिड संसाधन लुकअप निष्क्रिय संसाधनों को फ़िल्टर नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="5f567-126">The **Task Planning** grid resource lookup does not filter inactive resources.</span></span>
- <span data-ttu-id="5f567-127">मैनुअल मोड परियोजना नियोजन कार्य वितरण सरंचना में उम्मीद के मुताबिक काम नहीं कर रहा है.</span><span class="sxs-lookup"><span data-stu-id="5f567-127">Manual mode is not working as expected in the project planning work breakdown structure.</span></span>
- <span data-ttu-id="5f567-128">**कार्य योजना** ग्रिड **निष्क्रिय लेनदेन श्रेणियाँ** दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="5f567-128">The **Task Planning** grid shows **Inactive Transaction Categories**.</span></span>
- <span data-ttu-id="5f567-129">किसी कार्य में कई असाइनमेंट होने पर **संसाधन असाइनमेंट** ग्रिड गलत तरीके से ग्रिड राउंड करता है.</span><span class="sxs-lookup"><span data-stu-id="5f567-129">The **Resource Assignment** grid rounds incorrectly when a task has multiple assignments.</span></span>
- <span data-ttu-id="5f567-130">एक कार्य के लिए नियोजित लागत और वास्तविक लागत के बीच राउंडिंग मान भिन्न होते हैं.</span><span class="sxs-lookup"><span data-stu-id="5f567-130">Rounding values are different between planned cost and actual cost for a single task.</span></span>

<span data-ttu-id="5f567-131">**Sales**</span><span class="sxs-lookup"><span data-stu-id="5f567-131">**Sales**</span></span>

<span data-ttu-id="5f567-132">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="5f567-132">The following issues have been fixed:</span></span>

- <span data-ttu-id="5f567-133">**सभी लेनदेन श्रेणियाँ फ़ेच करें** डबल-क्लिक करने से कई लाइनें बनती हैं.</span><span class="sxs-lookup"><span data-stu-id="5f567-133">**Fetch All Transaction Categories** double-click creates multiple lines.</span></span>
