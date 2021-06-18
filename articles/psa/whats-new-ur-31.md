---
title: Project Service Automation के अपडेट रिलीज़ 31, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 31, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/26/2021
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
ms.openlocfilehash: 160187ba7b96547e85a7a4ec4bf84c86d8fd8257
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999133"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-31-v3"></a><span data-ttu-id="287fb-103">Project Service Automation के अपडेट रिलीज़ 31, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है</span><span class="sxs-lookup"><span data-stu-id="287fb-103">What's new or changed in Project Service Automation Update Release 31, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="287fb-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="287fb-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="287fb-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="287fb-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="287fb-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="287fb-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="287fb-107">इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="287fb-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="287fb-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="287fb-108">For more information, see [Install, update, or remove a preferred solution](/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="287fb-109">यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 31 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="287fb-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 31.</span></span> <span data-ttu-id="287fb-110">इस संस्करण की बिल्ड संख्या V3.10.52.77 है और यह आमतौर पर मई 2021 में एक स्व-अद्यतन के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="287fb-110">This version has a build number of V3.10.52.77 and is generally available through a self-update in May 2021.</span></span>

## <a name="update-release-31"></a><span data-ttu-id="287fb-111">अपडेट रिलीज़ 31</span><span class="sxs-lookup"><span data-stu-id="287fb-111">Update Release 31</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="287fb-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="287fb-112">Bug fixes</span></span>

<span data-ttu-id="287fb-113">**समय और व्यय**</span><span class="sxs-lookup"><span data-stu-id="287fb-113">**Time and Expense**</span></span>

<span data-ttu-id="287fb-114">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="287fb-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="287fb-115">**बुक करने योग्य संसाधन** पृष्ठ पर समय प्रविष्टि नियंत्रण कमांड बटन भ्रमित कर रहे थे.</span><span class="sxs-lookup"><span data-stu-id="287fb-115">Time entry control command buttons on the **Bookable Resource** page were confusing.</span></span>
- <span data-ttu-id="287fb-116">एक शून्य संदर्भ अपवाद **Project.SetTrackingFields** में एक समय प्रविष्टि को मंजूरी देते समय उत्पन्न किया गया था.</span><span class="sxs-lookup"><span data-stu-id="287fb-116">A null reference exception was generated in **Project.SetTrackingFields** when approving a time entry.</span></span>

<span data-ttu-id="287fb-117">**संसाधन प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="287fb-117">**Resource Management**</span></span>

<span data-ttu-id="287fb-118">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="287fb-118">The following issues have been fixed:</span></span>

- <span data-ttu-id="287fb-119">**Team सदस्य बनाएं** बुकिंग सेटअप मेटाडेटा सेटिंग को **डिफॉल्ट बुकिंग प्रतिबद्ध स्थिति** के लिए सही ढंग से प्रदर्शित नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="287fb-119">**Create Team Member** doesn't correctly display the booking setup metadata setting for **Default Booking Committed Status**.</span></span>
- <span data-ttu-id="287fb-120">PSA 1.X से 3.X में अपग्रेड करते समय, अपग्रेड प्रक्रिया **UpgradResourceRequirements** पर विफल हो जाती है.</span><span class="sxs-lookup"><span data-stu-id="287fb-120">When upgrading from PSA 1.X to 3.X, the upgrade process fails at **UpgradeResourceRequirements**.</span></span>


<span data-ttu-id="287fb-121">**सेल्स**</span><span class="sxs-lookup"><span data-stu-id="287fb-121">**Sales**</span></span>

<span data-ttu-id="287fb-122">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="287fb-122">The following issues have been fixed:</span></span>

- <span data-ttu-id="287fb-123">वास्तविक राजस्व ट्रैकिंग ग्रिड में परियोजना मुद्रा के लिए राशियाँ परिवर्तित करता है.</span><span class="sxs-lookup"><span data-stu-id="287fb-123">Actual revenue converts the amounts to the project currency in the tracking grid.</span></span>
- <span data-ttu-id="287fb-124">किसी संगठन की आधार मुद्रा प्रोजेक्ट मुद्रा से भिन्न होने पर, जर्नल लाइनों, उद्धरण लाइनों और अनुबंध लाइनों को बनाते समय मुद्रा डिफ़ॉल्ट स्पष्ट नहीं होती है.</span><span class="sxs-lookup"><span data-stu-id="287fb-124">The currency default is unclear when creating journal lines, quote lines, and contract lines in scenarios where an organization's base currency differs from the project currency.</span></span>
- <span data-ttu-id="287fb-125">**लंबित सुधार पत्रिका सत्यापन** क्वेरी परियोजना द्वारा फ़िल्टर नहीं होती है.</span><span class="sxs-lookup"><span data-stu-id="287fb-125">**Pending correction journal validation** query doesn't filter by project.</span></span>
- <span data-ttu-id="287fb-126">शेष बिक्री की गणना एक परियोजना पर गलत तरीके से की जाती है.</span><span class="sxs-lookup"><span data-stu-id="287fb-126">Remaining sales are calculated incorrectly on a project.</span></span>
- <span data-ttu-id="287fb-127">संपर्क के आधार पर उद्धरण मूल्य सूची के बिना बनाए जाने पर विफल हो जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="287fb-127">Quotes based on a contact fail when they are created without a price list.</span></span>
- <span data-ttu-id="287fb-128">जब आप **चालान की पुष्टि करें** का चयन करते हैं, तो कोई प्रसंस्करण स्पिनर नहीं दिखाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="287fb-128">No processing spinner is shown when you select **Confirm Invoice**.</span></span>
- <span data-ttu-id="287fb-129">जब आप **इनवॉइस बनाएं** का चयन करते हैं, तो कोई प्रोसेसिंग स्पिनर नहीं दिखाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="287fb-129">No processing spinner is shown when you select **Create Invoice**.</span></span>
- <span data-ttu-id="287fb-130">खो के रूप में एक उद्धरण बंद बुकिंग रद्द नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="287fb-130">Closing a quote as lost doesn't cancel the bookings.</span></span>







