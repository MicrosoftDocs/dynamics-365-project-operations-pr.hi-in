---
title: सुरक्षा मॉडल
description: यह विषय Dynamics 365 Project Operations सुरक्षा मॉडल के बारे में जानकारी प्रदान करता है.
author: stsporen
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 3f65d13809fef342be8bec682c11d95c4d9e9b19
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276800"
---
# <a name="security-model"></a><span data-ttu-id="98b09-103">सुरक्षा मॉडल</span><span class="sxs-lookup"><span data-stu-id="98b09-103">Security Model</span></span>

<span data-ttu-id="98b09-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="98b09-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="98b09-105">Microsoft Dynamics 365 Project Operations में एक अद्वितीय सुरक्षा मॉडल है, जो भूमिका-आधारित व्यावसायिक सुरक्षा मॉडल की अनुमति देता है, जो सहयोग Microsoft Office समूह के साथ सहयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="98b09-105">Microsoft Dynamics 365 Project Operations contains a unique security model that allows for a role-based business security model that collaborates with Microsoft Office Groups.</span></span> 


## <a name="security-roles"></a><span data-ttu-id="98b09-106">सुरक्षा भूमिकाएँ</span><span class="sxs-lookup"><span data-stu-id="98b09-106">Security roles</span></span>
<span data-ttu-id="98b09-107">परियोजना संचालन फ्रंट-एंड क्षमताओं में निम्नलिखित भूमिकाएं शामिल हैं:</span><span class="sxs-lookup"><span data-stu-id="98b09-107">Project Operations front-end capabilities include the following roles:</span></span>

| <span data-ttu-id="98b09-108">भूमिका</span><span class="sxs-lookup"><span data-stu-id="98b09-108">Role</span></span>                          | <span data-ttu-id="98b09-109">विवरण</span><span class="sxs-lookup"><span data-stu-id="98b09-109">Description</span></span>                                                                                                                                                                 | <span data-ttu-id="98b09-110">Scope</span><span class="sxs-lookup"><span data-stu-id="98b09-110">Scope</span></span> |
|-------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|
| <span data-ttu-id="98b09-111">अभ्यास प्रबंधक</span><span class="sxs-lookup"><span data-stu-id="98b09-111">Practice manager</span></span>              | <span data-ttu-id="98b09-112">क्रॉस-परियोजना रिपोर्टिंग का समर्थन करता है।</span><span class="sxs-lookup"><span data-stu-id="98b09-112">Supports cross-project reporting.</span></span>                                                                                                            | <span data-ttu-id="98b09-113">व्यवसाय इकाई</span><span class="sxs-lookup"><span data-stu-id="98b09-113">Business unit</span></span>              |
| <span data-ttu-id="98b09-114">परियोजना अनुमोदक</span><span class="sxs-lookup"><span data-stu-id="98b09-114">Project approver</span></span>              | <span data-ttu-id="98b09-115">किसी परियोजना के लिए समय और खर्च को मंजूरी देता है।</span><span class="sxs-lookup"><span data-stu-id="98b09-115">Approves time and expenses against a project.</span></span>                                                                                                                              | <span data-ttu-id="98b09-116">व्यवसाय इकाई</span><span class="sxs-lookup"><span data-stu-id="98b09-116">Business unit</span></span> |
| <span data-ttu-id="98b09-117">परियोजना बिलिंग व्यवस्थापक</span><span class="sxs-lookup"><span data-stu-id="98b09-117">Project billing administrator</span></span> | <span data-ttu-id="98b09-118">इनवॉइस प्रस्ताव बनाता है.</span><span class="sxs-lookup"><span data-stu-id="98b09-118">Creates the invoice proposal.</span></span>                                                                                                                                                 | <span data-ttu-id="98b09-119">व्यवसाय इकाई</span><span class="sxs-lookup"><span data-stu-id="98b09-119">Business unit</span></span> |
| <span data-ttu-id="98b09-120">परियोजना प्रबंधक</span><span class="sxs-lookup"><span data-stu-id="98b09-120">Project manager</span></span>               | <span data-ttu-id="98b09-121">परियोजना की योजना बनाता है और संसाधनों का अनुरोध करता है।</span><span class="sxs-lookup"><span data-stu-id="98b09-121">Creates the project plan and requests resources.</span></span>                                                                                                                              | <span data-ttu-id="98b09-122">व्यवसाय इकाई</span><span class="sxs-lookup"><span data-stu-id="98b09-122">Business unit</span></span> |
| <span data-ttu-id="98b09-123">परियोजना संसाधन</span><span class="sxs-lookup"><span data-stu-id="98b09-123">Project resource</span></span>              | <span data-ttu-id="98b09-124">टीम के सदस्य जिन्हें बुक किया जा सकता है और टाइम रिपोर्ट।</span><span class="sxs-lookup"><span data-stu-id="98b09-124">Team members who can be booked and report time.</span></span>                                                                                                          | <span data-ttu-id="98b09-125">व्यवसाय इकाई</span><span class="sxs-lookup"><span data-stu-id="98b09-125">Business unit</span></span>|
| <span data-ttu-id="98b09-126">संसाधन प्रबंधक</span><span class="sxs-lookup"><span data-stu-id="98b09-126">Resource manager</span></span>              | <span data-ttu-id="98b09-127">सभी संसाधन प्रबंधन कार्य, जैसे कि संसाधन अनुरोध और बुकिंग को पूरा करें, हाइब्रिड परियोजना प्रबंधक + संसाधन प्रबंधक कॉन्फ़िगरेशन और एकल और केंद्रीकृत संसाधन प्रबंधक भूमिका का समर्थन करने से अलग है।</span><span class="sxs-lookup"><span data-stu-id="98b09-127">All resource management functions, such as fulfill resource requests and bookings, separated to support a hybrid Project manager + Resource manager configuration and a single and centralized Resource manager role.</span></span> | <span data-ttu-id="98b09-128">व्यवसाय इकाई</span><span class="sxs-lookup"><span data-stu-id="98b09-128">Business unit</span></span> |


<span data-ttu-id="98b09-129">वेब के लिए Microsoft परियोजना में निम्नलिखित भूमिकाएं शामिल हैं:</span><span class="sxs-lookup"><span data-stu-id="98b09-129">Microsoft Project for the Web includes the following roles:</span></span>

| <span data-ttu-id="98b09-130">भूमिका</span><span class="sxs-lookup"><span data-stu-id="98b09-130">Role</span></span>           | <span data-ttu-id="98b09-131">विवरण</span><span class="sxs-lookup"><span data-stu-id="98b09-131">Description</span></span>                                                                                                        | <span data-ttu-id="98b09-132">Scope</span><span class="sxs-lookup"><span data-stu-id="98b09-132">Scope</span></span>  |
|----------------|--------------------------------------------------------------------------------------------------------------------|--------|
| <span data-ttu-id="98b09-133">परियोजना उपयोगकर्ता</span><span class="sxs-lookup"><span data-stu-id="98b09-133">Project user</span></span>   | <span data-ttu-id="98b09-134">परियोजना के सहयोगी उपयोगकर्ता जो अपनी परियोजनाएं बना सकते हैं और उनके साथ साझा की गई किसी भी परियोजना को देख सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="98b09-134">Collaborative user of Project   who is able to create their own projects and view any projects shared with   them.</span></span> | <span data-ttu-id="98b09-135">उपयोगकर्ता</span><span class="sxs-lookup"><span data-stu-id="98b09-135">User</span></span>   |
| <span data-ttu-id="98b09-136">परियोजना प्रणाली</span><span class="sxs-lookup"><span data-stu-id="98b09-136">Project system</span></span> | <span data-ttu-id="98b09-137">प्रयोग के संदर्भ के लिए प्रयुक्त भूमिका.</span><span class="sxs-lookup"><span data-stu-id="98b09-137">Role used for application   context.</span></span> <span data-ttu-id="98b09-138">ग्राहकों को इस सिस्टम भूमिका का उपयोग नहीं करना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="98b09-138">Customers should not use this system role.</span></span>                                    | <span data-ttu-id="98b09-139">ग्लोबल</span><span class="sxs-lookup"><span data-stu-id="98b09-139">Global</span></span> |

## <a name="security-enforcement"></a><span data-ttu-id="98b09-140">सुरक्षा प्रवर्तन</span><span class="sxs-lookup"><span data-stu-id="98b09-140">Security enforcement</span></span>
<span data-ttu-id="98b09-141">परियोजना स्तर पर किए जाने वाले कार्य लॉग इन उपयोगकर्ता के संदर्भ में किए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="98b09-141">Actions that are performed at the project level are performed in the context of the logged in user.</span></span> <span data-ttu-id="98b09-142">इसका मतलब है कि किसी परियोजना को बनाने, खोलने या हटाने के लिए, उपयोगकर्ता को CDS में पहुंच उपलब्ध होना आवश्यक है।</span><span class="sxs-lookup"><span data-stu-id="98b09-142">This means that in order to create, open, or delete a project, the user is required to have access available in CDS.</span></span> <span data-ttu-id="98b09-143">CDS में पहुंच प्लेटफार्म में शामिल किसी भी संभावित तंत्र के माध्यम से दिया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="98b09-143">Access in CDS may be granted through any of the possible mechanisms included in the platform.</span></span> <span data-ttu-id="98b09-144">उदाहरण के लिए, बड़े दायरे वाला उपयोगकर्ता परियोजना तक पहुंच सकता है या यदि उपयोगकर्ता की पहुंच को अनुमति देने वाली स्पष्ट परियोजना साझा कार्रवाई की गई है।</span><span class="sxs-lookup"><span data-stu-id="98b09-144">For example, a user with a larger scope may access the project or if an explicit project share action has been performed which grants the user access.</span></span>

<span data-ttu-id="98b09-145">परियोजना संचालन में प्रोजेक्ट बनाते समय इस पर विचार करना महत्वपूर्ण है।</span><span class="sxs-lookup"><span data-stu-id="98b09-145">It's important to consider this when creating projects in Project Operations.</span></span>

## <a name="modern-group-collaboration-with-project-operations"></a><span data-ttu-id="98b09-146">परियोजना संचालन के साथ आधुनिक समूह सहयोग</span><span class="sxs-lookup"><span data-stu-id="98b09-146">Modern group collaboration with Project Operations</span></span>
<span data-ttu-id="98b09-147">वेब और परियोजना संचालन के लिए परियोजना सहयोग के लिए आधुनिक समूहों का समर्थन करते हैं।</span><span class="sxs-lookup"><span data-stu-id="98b09-147">Project for the Web and Project Operations support modern groups for collaboration.</span></span> <span data-ttu-id="98b09-148">समूह के माध्यम से परियोजना में जोड़े गए उपयोगकर्ता परियोजना योजना को संपादित कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="98b09-148">Users added to the project through a group are able to edit the project plan.</span></span>

<span data-ttu-id="98b09-149">वेब के लिए परियोजना असाइन किए जाने पर समूह में उपयोगकर्ताओं को अपने आप जोड़ता है।</span><span class="sxs-lookup"><span data-stu-id="98b09-149">Project for the Web adds users to the group automatically upon assignment.</span></span>

<span data-ttu-id="98b09-150">समूह परियोजना और सहायक सहभागिता वाली शिल्पकृति की अनुमति देते हैं जिन पर मिलकर काम करना है।</span><span class="sxs-lookup"><span data-stu-id="98b09-150">Groups allow the permissions of the project and supporting collaboration artifacts to be worked on collaboratively.</span></span> <span data-ttu-id="98b09-151">निम्न आरेख में समूह असाइनमेंट प्रक्रिया के दौरान होने वाली घटनाओं और स्थिति में बदलावों को दर्शाया गया है।</span><span class="sxs-lookup"><span data-stu-id="98b09-151">The following diagram depicts the events and state changes that happen during the group assignment process.</span></span>

<span data-ttu-id="98b09-152">परियोजना संचालन अंतर्निहित कार्रवाई के माध्यम से समूह नहीं बनाता और केवल दबाव समूहों की स्पष्ट कार्रवाई के माध्यम से ऐसा करता है।</span><span class="sxs-lookup"><span data-stu-id="98b09-152">Project Operations does not create a group through implicit action and only does so through the explicit action of pressing groups.</span></span>

<span data-ttu-id="98b09-153">**समूह प्रबंधन** संवाद में समूह सदस्य खोज, उन लोगों तक सीमित है जो परिवेश के सुरक्षा समूह के हिस्से के रूप में सेट हैं।</span><span class="sxs-lookup"><span data-stu-id="98b09-153">Group member search in the **Group management** dialog, is limited to those who are set as part of the environment's security group.</span></span> <span data-ttu-id="98b09-154">अधिक जानकारी के लिए, [परिवेशों तक उपयोगकर्ताओं की पहुँच नियंत्रित करें: सुरक्षा समूह और लाइसेंस](https://docs.microsoft.com/power-platform/admin/control-user-access) देखें.</span><span class="sxs-lookup"><span data-stu-id="98b09-154">For more information, see [Control user access to environments: security groups and licenses](https://docs.microsoft.com/power-platform/admin/control-user-access).</span></span>

![समूह मोड](./media/groupsmode.png)

1. <span data-ttu-id="98b09-156">परियोजना को बनाया गया है और बनाने वाले उपयोगकर्ता के स्वामित्व में है।</span><span class="sxs-lookup"><span data-stu-id="98b09-156">The Project is created and owned by the creating User.</span></span>
2. <span data-ttu-id="98b09-157">परियोजना के मालिक को टीम में अपडेट किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="98b09-157">The Project owner is updated to the team.</span></span>
3. <span data-ttu-id="98b09-158">मालिक टीम को निर्दिष्ट या बनाए गए Office समूह में मैप किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="98b09-158">The Owner team is mapped to the specified or created Office Group.</span></span>
4. <span data-ttu-id="98b09-159">परियोजना का असली स्वामी Office समूह में जोड़ा जाता है।</span><span class="sxs-lookup"><span data-stu-id="98b09-159">The original owner of the Project is added to the Office Group.</span></span>

## <a name="deployment-recommendation"></a><span data-ttu-id="98b09-160">परिनियोजन सुझाव</span><span class="sxs-lookup"><span data-stu-id="98b09-160">Deployment recommendation</span></span>
<span data-ttu-id="98b09-161">जैसे-जैसे Office समूह सहयोग मॉडल विकसित होता है, समय के साथ अधिक विस्तृत नियंत्रण प्रदान करने के लिए कार्यक्षमता को जोड़ा जाएगा।</span><span class="sxs-lookup"><span data-stu-id="98b09-161">As the Office group collaboration model evolves, functionality will be added to provide more detailed control over time.</span></span> <span data-ttu-id="98b09-162">ग्राहक जो आज परियोजना संचालन नियोजित करते हैं, उन्हें पारंपरिक Microsoft Dynamics 365 सुरक्षा मॉडल पर ध्यान केंद्रित करने के लिए प्रोत्साहित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="98b09-162">Customers that deploy Project Operations today are encouraged to focus on a traditional Microsoft Dynamics 365 security model.</span></span>

<span data-ttu-id="98b09-163">अधिक जानकारी के लिए, [Common Data Service में सुरक्षा](https://docs.microsoft.com/power-platform/admin/wp-security) देखें.</span><span class="sxs-lookup"><span data-stu-id="98b09-163">For more information, see [Security in Common Data Service](https://docs.microsoft.com/power-platform/admin/wp-security).</span></span>

## <a name="project-operations-and-microsoft-dynamics-365-finance-security"></a><span data-ttu-id="98b09-164">परियोजना संचालन और Microsoft Dynamics 365 Finance सुरक्षा</span><span class="sxs-lookup"><span data-stu-id="98b09-164">Project Operations and Microsoft Dynamics 365 Finance security</span></span>
<span data-ttu-id="98b09-165">परियोजना संचालन में निम्नलिखित भूमिकाएं शामिल हैं:</span><span class="sxs-lookup"><span data-stu-id="98b09-165">Project Operations includes the following roles:</span></span>

- <span data-ttu-id="98b09-166">परियोजना प्रबंधक</span><span class="sxs-lookup"><span data-stu-id="98b09-166">Project manager</span></span>
- <span data-ttu-id="98b09-167">परियोजना अकाउंटेंट</span><span class="sxs-lookup"><span data-stu-id="98b09-167">Project accountant</span></span>

<span data-ttu-id="98b09-168">वित्त में सुरक्षा के बारे में अधिक जानकारी के लिए, [भूमिका-आधारित सुरक्षा](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security) देखें.</span><span class="sxs-lookup"><span data-stu-id="98b09-168">For more information about security in Finance, see [Role-based security](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/sysadmin/role-based-security).</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]