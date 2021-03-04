---
title: Project Service Automation के अपडेट रिलीज़ 20, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अद्यतन रिलीज़ 20, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 06/12/2020
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
ms.openlocfilehash: ee3be43da401af405ab329b9b5a724a2e95c0219
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/10/2021
ms.locfileid: "5147115"
---
# <a name="project-service-automation-update-release-20-v3"></a><span data-ttu-id="d666a-103">Project Service Automation V3 अद्यतन रिलीज़ 20, V3</span><span class="sxs-lookup"><span data-stu-id="d666a-103">Project Service Automation Update Release 20, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="d666a-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="d666a-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="d666a-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="d666a-105">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="d666a-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="d666a-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="d666a-107">इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="d666a-107">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="d666a-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="d666a-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="d666a-109">यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 20 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="d666a-109">This topic lists the features and fixes that are new or changed for Project Service Automation V3, Update Release 20.</span></span> <span data-ttu-id="d666a-110">इस संस्करण की बिल्ड संख्या V 3.10.31.37 है और यह आमतौर पर जून 2020 में एक स्व-अद्यतन के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="d666a-110">This version has a build number of V 3.10.31.37 and is generally available through a self-update in June 2020.</span></span>

## <a name="update-release-20"></a><span data-ttu-id="d666a-111">अपडेट रिलीज़ 20</span><span class="sxs-lookup"><span data-stu-id="d666a-111">Update Release 20</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="d666a-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="d666a-112">Bug fixes</span></span>

<span data-ttu-id="d666a-113">**परियोजना प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="d666a-113">**Project Management**</span></span>

<span data-ttu-id="d666a-114">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="d666a-114">The following issues have been fixed:</span></span>

- <span data-ttu-id="d666a-115">एक आवंटन विधि के साथ परियोजना टीम के सदस्यों को आयात करना जिसमें घंटे के परिणाम की आवश्यकता होती है, जब निर्दिष्ट घंटे शून्य होते हैं, तो एक अस्पष्ट त्रुटि संदेश होता है.</span><span class="sxs-lookup"><span data-stu-id="d666a-115">Importing project team members with an allocation method that requires hours results in an unclear error message when the specified hours are zero.</span></span>
- <span data-ttu-id="d666a-116">अधिकतम वर्ण किसी परियोजना कार्य के लिए फ़ील्ड **वर्णन** में दर्ज किए जाने पर उपयोगकर्ताओं को एक गलत त्रुटि प्राप्त होती है.</span><span class="sxs-lookup"><span data-stu-id="d666a-116">Users receive an incorrect error when the maximum number of characters have been entered into the **Description** field for a project task.</span></span>
- <span data-ttu-id="d666a-117">**Microsoft Dynamics 365 Project Service Automation ऐड-इन डाउनलोड** जब उपयोगकर्ता की भाषा सेटिंग जापानी में सेट हो जाती है, तो पृष्ठ अंग्रेजी डाउनलोड पृष्ठ पर रीडायरेक्ट करता है.</span><span class="sxs-lookup"><span data-stu-id="d666a-117">The **Microsoft Dynamics 365 Project Service Automation add-in download** page redirects to the English download page when the user’s language settings are set to Japanese.</span></span>
- <span data-ttu-id="d666a-118">जब सर्वर त्रुटि होती है, तो **परियोजना** प्रपत्र के **शेड्यूल** टैब पर सिंक्रनाइज़ेशन लेबल कभी-कभी रहता है.</span><span class="sxs-lookup"><span data-stu-id="d666a-118">When a server error occurs, the synchronization label on the **Schedule** tab of the **Projects** form sometimes remains.</span></span>
- <span data-ttu-id="d666a-119">किसी कार्य के संशोधित होने पर सर्वर पर अनावश्यक कार्य अपडेट भेजे जा रहे हैं.</span><span class="sxs-lookup"><span data-stu-id="d666a-119">Redundant task updates are being sent to the server when a task is modified.</span></span>

<span data-ttu-id="d666a-120">**Sales**</span><span class="sxs-lookup"><span data-stu-id="d666a-120">**Sales**</span></span>

<span data-ttu-id="d666a-121">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="d666a-121">The following issues have been fixed:</span></span>

- <span data-ttu-id="d666a-122">**अनुबंध** प्रपत्र पर, **इनवॉइस बनाएँ** को डबल-क्लिक करने से यह एक वास्तविक रिकॉर्ड के लिए दो इनवॉइस बनाता है.</span><span class="sxs-lookup"><span data-stu-id="d666a-122">On the **Contract** form, double-clicking **Create Invoice** creates two invoices for a single actuals record.</span></span>
- <span data-ttu-id="d666a-123">Internet Explorer 11 में, उपयोगकर्ता व्यय प्रविष्टियाँ बनाने में असमर्थ हैं.</span><span class="sxs-lookup"><span data-stu-id="d666a-123">In Internet Explorer 11, users are unable to create expense entries.</span></span>
- <span data-ttu-id="d666a-124">लागत का रिवर्सल और Unbilled बिक्री वास्तविकता के रिवर्सल जुड़े हुए नहीं होते.</span><span class="sxs-lookup"><span data-stu-id="d666a-124">Reversal of Cost and reversal of Unbilled Sales Actuals are not linked.</span></span>
- <span data-ttu-id="d666a-125">**परियोजना** प्रपत्र पर **रिफ़्रेश वास्तविकता** बटन **कार्य वास्तविक घंटों** को रिफ्रेश नहीं करता.</span><span class="sxs-lookup"><span data-stu-id="d666a-125">The **Refresh Actuals** button on the **Project** form does not refresh **Task Actual Hours**.</span></span>
- <span data-ttu-id="d666a-126">एट्रिब्यूट **msdyn_isgenericresourceprojectscoped** **असत्य** पर सेट होने पर **PreValidateProjectTeamMemberCreate** प्लग-इन डुप्लिकेट जेनेरिक बुक करने योग्य संसाधन बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="d666a-126">The **PreValidateProjectTeamMemberCreate** plug-in can create duplicate generic bookable resources when the attribute **msdyn_isgenericresourceprojectscoped** is set to **False**.</span></span>
- <span data-ttu-id="d666a-127">**पुनर्गणना** उत्पाद-आधारित कोट पंक्ति विवरण और अनुबंध पंक्ति विवरण की प्रभार्य लागत साफ़ करती है.</span><span class="sxs-lookup"><span data-stu-id="d666a-127">**Recalculate** clears chargeable costs of product-based quote line details and contract line details.</span></span>
- <span data-ttu-id="d666a-128">विशिष्ट परिदृश्यों में, **PostEstimateLineUpdate** प्लग-इन एक नल संदर्भ अपवाद त्रुटि प्रदर्शित करता है.</span><span class="sxs-lookup"><span data-stu-id="d666a-128">In specific scenarios, the **PostEstimateLineUpdate** plug-in displays a null teference exception error.</span></span>
- <span data-ttu-id="d666a-129">**लाभप्रदता विश्लेषण चार्ट** पर समय -चरण अवधि कोट की निश्चित-मूल्य कोट पंक्ति विवरण में लागतों की अवधि से मेल नहीं खाती है.</span><span class="sxs-lookup"><span data-stu-id="d666a-129">Time phase duration on the **Profitability Analysis Chart** does not match duration of the costs in the fixed-price quote line detail of the quote.</span></span>
- <span data-ttu-id="d666a-130">इकाई और इकाई समूह के मान **अनुबंध पंक्ति विवरण** और **कोट पंक्ति विवरण** प्रपत्रों पर व्यय श्रेणियों के लिए सही रूप से डिफ़ॉल्ट नहीं हैं.</span><span class="sxs-lookup"><span data-stu-id="d666a-130">Unit and unit group values do not default correctly for expense categories on the **Contract Line Details** and **Quote Line Details** forms.</span></span>
- <span data-ttu-id="d666a-131">**संगठन इकाई लागत मूल्य** सूचियाँ दिनांक प्रभावकारिता में ओवरलैप करती हैं.</span><span class="sxs-lookup"><span data-stu-id="d666a-131">**Org Unit Cost Price** lists permit overlaps in the date effectivity.</span></span>
- <span data-ttu-id="d666a-132">जब आदेश प्रकार कार्य-आधारित न हो, तो उपयोगकर्ताओं को **संगठन-इकाई** बदलने की अनुमति नहीं है क्योंकि यह एक नल संदर्भ अपवाद त्रुटि को जन्म देगा.</span><span class="sxs-lookup"><span data-stu-id="d666a-132">Users are not permitted to change the **OrgUnit** when the order type is not work-based because it will lead to a null reference exception error.</span></span>
- <span data-ttu-id="d666a-133">**कोट पंक्ति विवरण** प्रपत्र से **कोट** टैब पर वापस नेविगेट करने का प्रयास करते समय, प्रपत्र **सारांश** टैब रिफ़्रेश और प्रदर्शित करता है.</span><span class="sxs-lookup"><span data-stu-id="d666a-133">When attempting to navigate from the **Quote Line Details** form, back to the **Quote** tab, the form refreshes and displays the **Summary** tab.</span></span>
