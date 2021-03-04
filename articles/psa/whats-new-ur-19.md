---
title: Project Service Automation के अपडेट रिलीज़ 19, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 19, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 05/05/2020
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
ms.openlocfilehash: 8a73a6acd4ce4c9559cdf4591ede735a613f4d52
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/10/2021
ms.locfileid: "5143608"
---
# <a name="project-service-automation-update-release-19-v3"></a><span data-ttu-id="ffd5b-103">Project Service Automation V3 अद्यतन रिलीज़ 19, V3</span><span class="sxs-lookup"><span data-stu-id="ffd5b-103">Project Service Automation Update Release 19, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="ffd5b-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="ffd5b-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="ffd5b-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="ffd5b-107">इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="ffd5b-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="ffd5b-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="ffd5b-109">यह टॉपिक PSA V3, अपडेट रिलीज़ 19 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 19.</span></span> <span data-ttu-id="ffd5b-110">इस संस्करण की बिल्ड संख्या V3.10.30.41 है और यह आमतौर पर मई 2020 में एक स्व-अद्यतन के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-110">This version has a build number of V3.10.30.41 and is generally available through a self-update in May 2020.</span></span>

## <a name="update-release-19"></a><span data-ttu-id="ffd5b-111">अपडेट रिलीज़ 19</span><span class="sxs-lookup"><span data-stu-id="ffd5b-111">Update Release 19</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="ffd5b-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="ffd5b-112">Bug fixes</span></span>

<span data-ttu-id="ffd5b-113">**समय और व्यय**</span><span class="sxs-lookup"><span data-stu-id="ffd5b-113">**Time and Expense**</span></span>

<span data-ttu-id="ffd5b-114">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="ffd5b-114">The following issues have been fixed:</span></span> 

- <span data-ttu-id="ffd5b-115">समय प्रविष्टि आयात से प्राप्त त्रुटियाँ सही ढंग से सामने नहीं आई हैं.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-115">Errors derived from time entry imports are not surfaced correctly.</span></span>
- <span data-ttu-id="ffd5b-116">समय प्रविष्टि ग्रिड **केवल दिनांक** फ़ील्ड व्यवहार का समर्थन नहीं करती है.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-116">Time Entry Grid does not support **Date Only** field behavior.</span></span>
- <span data-ttu-id="ffd5b-117">परियोजना संसाधन किसी परियोजना के साथ एक व्यय बनाने में असमर्थ हैं.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-117">Project Resources are unable to create an expense with a project.</span></span>

<span data-ttu-id="ffd5b-118">**परियोजना प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="ffd5b-118">**Project Management**</span></span>

<span data-ttu-id="ffd5b-119">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="ffd5b-119">The following issues have been fixed:</span></span> 

-  <span data-ttu-id="ffd5b-120">ग्रैंडचाइल्ड कार्य पूर्णता (EAC) गणना के दौरान एक गलत प्रयास का अनुमान लगाता है.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-120">Grandchild task causes an incorrect effort estimate during the Completion (EAC) Calculation.</span></span>

<span data-ttu-id="ffd5b-121">**Sales**</span><span class="sxs-lookup"><span data-stu-id="ffd5b-121">**Sales**</span></span>

<span data-ttu-id="ffd5b-122">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="ffd5b-122">The following issues have been fixed:</span></span> 

- <span data-ttu-id="ffd5b-123">**पुनर्गणना** कार्रवाई व्यय अनुबंध पंक्ति विवरण या कोट पंक्ति विवरण के साथ काम नहीं करती है.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-123">The **Recalculate** action does not work with expense contract line details or quote line details.</span></span>
- <span data-ttu-id="ffd5b-124">**अद्यतन मूल्य** व्यय अनुमानों के लिए गायब है.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-124">**Update Prices** is missing for expense estimates.</span></span>
-  <span data-ttu-id="ffd5b-125">ग्राहक **परियोजना अनुबंध** पृष्ठ से कस्टम अनुबंध स्थिति कारणों को चयन करने में असमर्थ हैं.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-125">Customers are unable to select custom contract status reasons from the **Project Contract** page.</span></span>
- <span data-ttu-id="ffd5b-126">किसी कोट से कस्टम मूल्य सूची बनाते समय ग्राहकों को अपमानजनक प्रदर्शन का अनुभव होता है.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-126">Customers experience degraded performance when creating a custom price list from a quote.</span></span>
- <span data-ttu-id="ffd5b-127">ग्राहकों को **कोट पंक्ति विवरण** और **अनुबंध पंक्ति विवरण** पृष्ठों पर डिफ़ॉल्ट **इकाई** के साथ असंगतता का अनुभव होता है.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-127">Customers experience inconsistency with **unit** defaults on **Quote Line Details** and **Contract Line Details** pages.</span></span>
- <span data-ttu-id="ffd5b-128">किसी प्रभार्य अनुबंध पंक्ति में गैर-प्रभार्य लेन-देन श्रेणी आइटम जोड़ने से यह लेन-देन श्रेणी के **गैर प्रभार्य** बिलिंग प्रकार का सम्मान नहीं होगा.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-128">Adding non-chargeable transaction category items to a chargeable contract line will not respect the **Non-chargeable** billing type of the transaction category.</span></span>
- <span data-ttu-id="ffd5b-129">ग्राहक पहले बनाए गए अनुबंधों पर नए रूप से जोड़ी गई भूमिकाओं और श्रेणी का उपयोग नहीं कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-129">Customers can't use the newly added roles and category on previously created contracts.</span></span>
- <span data-ttu-id="ffd5b-130">ग्राहकों को अनावश्यक रूप से PreValidateProjectTeamMemberUpdate.cs में अपमानित प्रदर्शन का अनुभव प्राप्त होता है</span><span class="sxs-lookup"><span data-stu-id="ffd5b-130">Customers experience degraded performance Unnecessary retrieve in PreValidateProjectTeamMemberUpdate.cs</span></span>
- <span data-ttu-id="ffd5b-131">**संसाधन श्रेणियाँ** सूची में गैर-प्रभार्य के रूप में सेट अप की गई भूमिकाओं को परियोजना के लिए अनुबंध पंक्ति पर **प्रभार्य भूमिकाएँ** टैब में **गैर-प्रभार्य** के रूप में जोड़ा जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-131">Roles set up as non-chargeable in the **Resource Categories** list should be added to the **Chargeable Roles** tab as **Non0chargeable** on the contract line for a project.</span></span>
- <span data-ttu-id="ffd5b-132">ग्राहक एक परियोजना बनाते समय अपमानित प्रदर्शन का अनुभव कर सकते हैं क्योंकि **GetBookableResourceIdFromUser** केवल प्राथमिक आईडी के बजाय बुक करने योग्य संसाधनों के सभी स्तंभों को पुनर्प्राप्त करता है.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-132">Customers may experience degraded performance when creating a project because **GetBookableResourceIdFromUser** retrieves all columns of bookable resources instead of just the primary ID.</span></span>
- <span data-ttu-id="ffd5b-133">**लेनदेन प्रकार** निकाय में उपयोगकर्ताओं को **इकाइयों** और **UnitGroups** से प्रवेश करने से रोकने के लिए पूर्व-सत्यापन अद्यतन प्लग-इन गुम होता है, जो लेनदेन प्रकारों के लिए मान्य नहीं होता.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-133">**TransactionType** entity missing the pre-validation update plug-in to prevent users from entering **Units** and **UnitGroups** that are not valid for transaction types.</span></span>
- <span data-ttu-id="ffd5b-134">**हटाना** चरण समय प्रविष्टि आयात के लिए कार्य नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="ffd5b-134">The **Remove** step does not work for time entry import.</span></span>
