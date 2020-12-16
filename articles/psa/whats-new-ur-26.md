---
title: Project Service Automation के अपडेट रिलीज़ 26, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
ms.openlocfilehash: 849e7288ee91d3e9360c0b03f6b8b37ff29338e7
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/25/2020
ms.locfileid: "4643265"
---
<a name="project-service-automation-update-release-26-v3"></a><span data-ttu-id="b605b-102">Project Service Automation V3 अद्यतन रिलीज़ 26, V3</span><span class="sxs-lookup"><span data-stu-id="b605b-102">Project Service Automation Update Release 26, V3</span></span>
================================================

<span data-ttu-id="b605b-103">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="b605b-103">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="b605b-104">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="b605b-104">This release includes some important improvements to quality, performance, and usability.</span></span> <span data-ttu-id="b605b-105">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="b605b-105">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="b605b-106">इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="b605b-106">To update to this release, visit the Admin Center for Dynamics 365 online solutions page to install the update.</span></span> <span data-ttu-id="b605b-107">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="b605b-107">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="b605b-108">यह विषय Project Service Automation अद्यतन रिलीज़ 26, V3 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="b605b-108">This topic lists the features and fixes that are new or changed for Project Service Automation Update Release 26, V3.</span></span> <span data-ttu-id="b605b-109">इस संस्करण की बिल्ड संख्या V3.10.44.59 है और यह आम तौर पर दिसंबर 2020 में एक स्व-अद्यतन के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="b605b-109">This version has a build number of V3.10.44.59 and is generally available through a self-update in December 2020.</span></span>

<a name="update-release-26"></a><span data-ttu-id="b605b-110">अपडेट रिलीज़ 26</span><span class="sxs-lookup"><span data-stu-id="b605b-110">Update Release 26</span></span>
-----------------

### <a name="bug-fixes"></a><span data-ttu-id="b605b-111">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="b605b-111">Bug fixes</span></span>

<span data-ttu-id="b605b-112">**समय और व्यय**</span><span class="sxs-lookup"><span data-stu-id="b605b-112">**Time and Expense**</span></span>

<span data-ttu-id="b605b-113">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="b605b-113">The following issues have been fixed:</span></span>

-   <span data-ttu-id="b605b-114">उपयोगकर्ता उस समय प्रविष्टि पर कार्य को बदलने में सक्षम हैं, जो स्वीकृत/सबमिट की गई है.</span><span class="sxs-lookup"><span data-stu-id="b605b-114">Users are able to change the task on a time entry that has been approved/submitted.</span></span>

-   <span data-ttu-id="b605b-115">समय प्रविष्टि सहेजते समय "ऑब्जेक्ट संदर्भ सेट नहीं" त्रुटि.</span><span class="sxs-lookup"><span data-stu-id="b605b-115">"Object Reference Not Set" error when saving time entry.</span></span>

-   <span data-ttu-id="b605b-116">संसाधन असाइनमेंट से समय प्रविष्टि आयात, गलत दिनांक समय मानों वाली समय प्रविष्टियाँ बनाता है.</span><span class="sxs-lookup"><span data-stu-id="b605b-116">Time entry import from resource assignments creates time entries with the incorrect DateTime values.</span></span>

-   <span data-ttu-id="b605b-117">Project Service Automation और Field Service ऐप दोनों के स्थापित किए जाने पर, Field Service ऐप में समय प्रविष्टियों के लिए आदेश पट्टी पर **नया** बटन दो बार प्रदर्शित होता है.</span><span class="sxs-lookup"><span data-stu-id="b605b-117">When Project Service Automation and the Field Service app are both installed, the **New** button is displaying twice on the command bar for time entries in the Field Service app.</span></span>

-   <span data-ttu-id="b605b-118">**अनुमति इकाई** और **इकाई समूह** सेल अद्यतन, अब **व्यय अनुमान** ग्रिड पर कार्य करते हैं.</span><span class="sxs-lookup"><span data-stu-id="b605b-118">**Allow Unit** and **Unit group** cells updates now work on the **Expense Estimates** grid.</span></span>

-   <span data-ttu-id="b605b-119">**अद्यतन समय प्रविष्टि संपादन** प्रपत्र **टाइमलाइन** शामिल करते हैं.</span><span class="sxs-lookup"><span data-stu-id="b605b-119">**Update Time Entry Edit** form includes **Timeline**.</span></span>

-   <span data-ttu-id="b605b-120">गैर-परियोजना समय प्रविष्टियों के लिए समय अनुमोदन, परियोजना अनुमोदन भूमिका की खोज करते समय सिस्टम को अवरुद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="b605b-120">Time approval for non-project time entries blocks the system when searching for a project approver role.</span></span>

<span data-ttu-id="b605b-121">**संसाधन प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="b605b-121">**Resource Management**</span></span>

<span data-ttu-id="b605b-122">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="b605b-122">The following issues have been fixed:</span></span>

-   <span data-ttu-id="b605b-123">**PostProjectCreate** प्लग-इन में सत्यापन जोड़ा गया, ताकि नया बनाने से पहले प्राथमिक आवश्यकता की जाँच की जा सके.</span><span class="sxs-lookup"><span data-stu-id="b605b-123">Added validation in the **PostProjectCreate** plug-in to check for a primary requirement before creating one.</span></span>

-   <span data-ttu-id="b605b-124">**परियोजना टीम सदस्य** त्वरित निर्माण प्रपत्र, प्रपत्र से फ़ील्ड निकालने जाने पर नल संदर्भ अपवाद दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="b605b-124">**Project Team Member** quick create form throws a null reference exception if fields are removed from the form.</span></span>

-   <span data-ttu-id="b605b-125">1 वर्ष से अधिक 12 घंटों के लिए आवश्यकता जनरेट करना विफल रहेगा.</span><span class="sxs-lookup"><span data-stu-id="b605b-125">Generate requirements for 12 hours over 1 year will fail.</span></span>

-   <span data-ttu-id="b605b-126">संसाधन आवश्यकता निर्माण के दौरान बेहतर त्रुटि संदेश नल संदर्भ अपवाद.</span><span class="sxs-lookup"><span data-stu-id="b605b-126">Improved error message null reference exception during resource requirement creation.</span></span>

<span data-ttu-id="b605b-127">**परियोजना प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="b605b-127">**Project Management**</span></span>

<span data-ttu-id="b605b-128">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="b605b-128">The following issues have been fixed:</span></span>

-   <span data-ttu-id="b605b-129">नल संदर्भ अपवाद को संबोधित करने के लिए बेहतर सत्यापन **PreProjectUpdate** प्लग-इन में जनरेट हुआ.</span><span class="sxs-lookup"><span data-stu-id="b605b-129">Improved validation to address null reference exception generated in the **PreProjectUpdate** plug-in.</span></span>

-   <span data-ttu-id="b605b-130">Microsoft Project डेस्कटॉप ऐड-इन द्वारा प्रकाशित परियोजनाएँ असाइन न किए गए असाइनमेंट को हटाती हैं.</span><span class="sxs-lookup"><span data-stu-id="b605b-130">Projects published by the Microsoft Project desktop add-in delete unassigned assignments.</span></span>

-   <span data-ttu-id="b605b-131">**PreValidateProjectTaskUpdate** प्लग-इन में नल संदर्भ अपवाद के कारण कार्य का परियोजना संदर्भ अमान्य होने पर नया सत्यापन जोड़ा गया.</span><span class="sxs-lookup"><span data-stu-id="b605b-131">Added new validation when a task’s project reference is invalid due to null reference exception in **PreValidateProjectTaskUpdate** plug-in.</span></span>

-   <span data-ttu-id="b605b-132">टीम सदस्य ग्रिड, टीम सदस्य रिकॉर्ड पर अलग-अलग असाइनमेंट नहीं दिखाती है.</span><span class="sxs-lookup"><span data-stu-id="b605b-132">Team Member grid does not show distinct assignments on the team member record.</span></span>

-   <span data-ttu-id="b605b-133">**PreProjectTaskDelete** प्लग-इन में नल संदर्भ अपवाद होने के कारण नया सत्यापन और त्रुटि संदेश जोड़े गए.</span><span class="sxs-lookup"><span data-stu-id="b605b-133">Added new validation and error messages due to null reference exception in **PreProjectTaskDelete** plug-in.</span></span>

<span data-ttu-id="b605b-134">**Sales**</span><span class="sxs-lookup"><span data-stu-id="b605b-134">**Sales**</span></span>

<span data-ttu-id="b605b-135">निम्नलिखित मुद्दों को ठीक किया गया है:</span><span class="sxs-lookup"><span data-stu-id="b605b-135">The following issues have been fixed:</span></span>

-   <span data-ttu-id="b605b-136">कोट या अनुबंध में परियोजना-आधारित पंक्ति का चयन करते समय, **सुझाव** बटन केवल तब ही दृश्यमान होना चाहिए, जब उत्पाद-आधारित पंक्ति को चुनना मौजूदा उत्पाद से संबद्ध हो.</span><span class="sxs-lookup"><span data-stu-id="b605b-136">When selecting a project-based line in quote or contract, the **Suggestion** button should only be visible when selecting a product-based line associated with an existing product.</span></span>

-   <span data-ttu-id="b605b-137">**Create_ProjectContract** विशेषाधिकार से **Create_Product** विशेषाधिकार विभाजित करें.</span><span class="sxs-lookup"><span data-stu-id="b605b-137">Split **Create_Product** privilege from **Create_ProjectContract** privilege.</span></span>

-   <span data-ttu-id="b605b-138">इनवॉइस पंक्ति को हटाने से **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice** पर नल संदर्भ विफलता होती है.</span><span class="sxs-lookup"><span data-stu-id="b605b-138">Deleting an invoice line causes null reference failure on **MarkReadyToInvoiceForProductContractLineAfterDeletingInvoice**.</span></span>
