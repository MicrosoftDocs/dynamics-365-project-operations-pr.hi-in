---
title: Project Service Automation के अपडेट रिलीज़ 21, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 21, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 06/19/2020
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
ms.openlocfilehash: 69b592db7456bf11c2e933256569d726056d1a32
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280625"
---
# <a name="project-service-automation-update-release-21-v3"></a><span data-ttu-id="a3f02-103">Project Service Automation V3 अद्यतन रिलीज़ 21, V3</span><span class="sxs-lookup"><span data-stu-id="a3f02-103">Project Service Automation Update Release 21, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="a3f02-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="a3f02-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="a3f02-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="a3f02-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="a3f02-107">इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="a3f02-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="a3f02-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="a3f02-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="a3f02-109">यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 21 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 21.</span></span> <span data-ttu-id="a3f02-110">इस संस्करण की बिल्ड संख्या V 3.10.32.50 है और यह आमतौर पर जून 2020 में एक स्व-अद्यतन के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-110">This version has a build number of V 3.10.32.50 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-21"></a><span data-ttu-id="a3f02-111">अपडेट रिलीज़ 21</span><span class="sxs-lookup"><span data-stu-id="a3f02-111">Update Release 21</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="a3f02-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="a3f02-112">Bug fixes</span></span>

<span data-ttu-id="a3f02-113">**समय और व्यय**</span><span class="sxs-lookup"><span data-stu-id="a3f02-113">**Time and Expense**</span></span>

<span data-ttu-id="a3f02-114">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="a3f02-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="a3f02-115">डैशबोर्ड में **समय प्रविष्टि ग्रिड नियंत्रण** होस्ट करने के दौरान ग्रिड, डैशबोर्ड ग्रिड कंटेनर की पूरी चौड़ाई का उपयोग नहीं करती है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-115">When hosting the **Time Entry Grid Control** in Dashboards, the grid does not utilize the full width of the dashboard grid container.</span></span>
- <span data-ttu-id="a3f02-116">विशिष्ट समय क्षेत्रों के लिए, **समय प्रविष्टि** ग्रिड नियंत्रण, रिकॉर्ड प्रदर्शित नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-116">For specific time zones, the **Time Entry** grid control does not display records.</span></span>
- <span data-ttu-id="a3f02-117">9:00 PM के बाद की समय प्रविष्टियाँ गलत दिन दिखाई देती हैं.</span><span class="sxs-lookup"><span data-stu-id="a3f02-117">Time entries that are after 9:00 PM appear on the wrong day.</span></span>
- <span data-ttu-id="a3f02-118">यदि व्यय श्रेणी, **व्यय प्राप्ति आवश्यक** का कोई मान नहीं होता है, तो उपयोगकर्ता व्यय सबमिट नहीं कर पाते हैं.</span><span class="sxs-lookup"><span data-stu-id="a3f02-118">Users are unable to submit expenses if the expense category, **Expense receipt required** has no value.</span></span>

<span data-ttu-id="a3f02-119">**संसाधन प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="a3f02-119">**Resource Management**</span></span>

<span data-ttu-id="a3f02-120">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="a3f02-120">The following issues have been fixed:</span></span>

- <span data-ttu-id="a3f02-121">निष्क्रिय बुकिंग **समायोजन** दृश्य में प्रदर्शित की जाती हैं.</span><span class="sxs-lookup"><span data-stu-id="a3f02-121">Inactive bookings are displayed in the **Reconciliation** view.</span></span>
- <span data-ttu-id="a3f02-122">यह सुनिश्चित करने के लिए कि एक मान्य बुकिंग स्थिति मौजूद है, जेनेरिक संसाधन पूर्ति में प्रमाणीकरण मौजूद नहीं था.</span><span class="sxs-lookup"><span data-stu-id="a3f02-122">Generic resource fulfillment was missing validation to ensure that a valid booking status exists.</span></span>

<span data-ttu-id="a3f02-123">**परियोजना प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="a3f02-123">**Project Management**</span></span>

<span data-ttu-id="a3f02-124">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="a3f02-124">The following issues have been fixed:</span></span>

- <span data-ttu-id="a3f02-125">**परियोजना** प्रपत्र ग्रिड (**संसाधन असाइनमेंट**, **कार्य**, **समायोजन** दृश्य, **व्यय अनुमान**) परियोजना के सक्रिय न होने पर भी संपादन योग्य बने रहते हैं.</span><span class="sxs-lookup"><span data-stu-id="a3f02-125">The **Project** form grids (**Resource Assignment**, **Task**, **Reconciliation** view, **Expense Estimates**) remain editable even when a project is not active.</span></span>
- <span data-ttu-id="a3f02-126">डुप्लिकेट ग्राहकों को उन ग्राहकों के साथ मर्ज नहीं किया जा सकता, जो पुष्टि किए गए परियोजना अनुबंधों से लिंक हैं.</span><span class="sxs-lookup"><span data-stu-id="a3f02-126">Duplicate customers can't be merged with customers that are linked to confirmed project contracts.</span></span>
- <span data-ttu-id="a3f02-127">जब एक संसाधन, जिसके पास वैध कैलेंडर नहीं है, को जोड़ा जाता है, तो सिस्टम उपयोगकर्ता के अनुकूल-त्रुटि संदेश नहीं देता है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-127">When a resource who does not have a valid calendar is added, the system does not return a user friendly-error message.</span></span>
- <span data-ttu-id="a3f02-128">परियोजना के **Microsoft परियोजना ऐड-इन** से लिंक होने पर, कार्य ग्रिड पर मौजूद **कार्य जोड़ें** बटन सक्षम होता है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-128">The **Add Task** button on the task grid is enabled when the project is linked to **Microsoft Project add-in**.</span></span>
- <span data-ttu-id="a3f02-129">जब श्रेणी वाले कार्य को किसी ऐसे संसाधन को असाइन किया जाता है, जिसकी ऐसी भूमिका होती है, जिसके लिए कोई लागत मूल्य परिभाषित नहीं होता है, तो प्रयास अनियंत्रित रूप से बढ़ता है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-129">Effort grows uncontrollably when a task with a category is assigned to a resource with a role for which there is a cost price defined.</span></span>

<span data-ttu-id="a3f02-130">**Sales**</span><span class="sxs-lookup"><span data-stu-id="a3f02-130">**Sales**</span></span>

<span data-ttu-id="a3f02-131">निम्न एन्हांसमेंट किए गए हैं:</span><span class="sxs-lookup"><span data-stu-id="a3f02-131">The following enhancements have been made:</span></span>

- <span data-ttu-id="a3f02-132">**इनवॉइस आवृत्ति** और **बिलिंग प्रारंभ** को **इनवॉइस शेड्यूल** टैब पर स्थानांतरित किया गया है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-132">**Invoice Frequency** and **Billing Start** have been moved to the **Invoice Schedule** tab.</span></span>

<span data-ttu-id="a3f02-133">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="a3f02-133">The following issues have been fixed:</span></span>

- <span data-ttu-id="a3f02-134">**श्रेणी** के लिए **कुल विक्रय मूल्य** शून्य (0) है, भले ही **भूमिका** का कुल विक्रय मूल्य शून्य नहीं है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-134">**Total Sales Price** is zero (0) for **Category** even though **Role** has a total sales price that is not zero.</span></span>
- <span data-ttu-id="a3f02-135">जब कोई अन्य अनुकूलित प्रक्रिया किसी अतिरिक्त फ़ील्ड को अद्यतन कर रही हो, तो ग्राहक **इनवॉइस स्थिति** फ़ील्ड के मान को **इनवॉइसिंग के लिए तैयार** में नहीं बदल सकते.</span><span class="sxs-lookup"><span data-stu-id="a3f02-135">Customers can't change the value of the **Invoice Status** field to **Ready for invoicing** when another customized process is updating an additional field.</span></span>
- <span data-ttu-id="a3f02-136">**इनवॉइस पंक्तियाँ रीफ़्रेश करें** बटन को यदि बार-बार चुना जाता है, तो वह कई डुप्लिकेट पंक्तियाँ बना सकता है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-136">The **Refresh Invoice Lines** button can create multiple duplicated lines if it is repeatedly selected.</span></span>
- <span data-ttu-id="a3f02-137">**त्वरित दृश्य** प्रपत्र में **भूमिका मूल्य** सबग्रिड पर **मूल्यों का अद्यतन करें** बटन काम नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-137">The **Update Prices** button doesn't work on the **Role Prices** subgrid in the **Quick View** form.</span></span>
- <span data-ttu-id="a3f02-138">**विक्रय मूल्य सूची समाधान** तर्क अनुचित रूप से समय क्षेत्र को हैंडल करता है, जिसके परिणामस्वरूप मूल्य सूचियों का गलत चयन होता है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-138">The **Sales Price List Resolution** logic improperly handles time zones, resulting in the incorrect selection of price lists.</span></span>
- <span data-ttu-id="a3f02-139">परियोजना की **कुल वास्तविक लागत**, एकल समय प्रविष्टि के स्वीकृत होने के बाद एक भिन्नात्मक राशि द्वारा बंद की जा सकती है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-139">A project’s **Total Actual Cost** can be off by a fractional amount after a single time entry is approved.</span></span>
- <span data-ttu-id="a3f02-140">**मूल्य समाधान** तर्क तब उपयोगकर्ता के अनुकूल त्रुटि संदेश प्रदान नहीं करता है, जब **पुनर्प्राप्त RolePrice** का **'प्राथमिक इकाई'** और **'प्राथमिक इकाई में मूल्य'** फ़ील्ड में कोई मान नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="a3f02-140">The **Price Resolution** logic does not provide a user-friendly error message if **Retrieved RolePrice** doesn't have values in **'Primary Unit'** and **'Price In Primary Unit'** fields.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]