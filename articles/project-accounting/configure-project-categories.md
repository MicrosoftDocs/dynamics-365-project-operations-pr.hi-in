---
title: परियोजना श्रेणियाँ कॉन्फ़िगर करें
description: यह विषय परियोजना श्रेणियों की स्थापना के बारे में जानकारी देता है.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b7adf61a82714a0148d9c8b1d2b2b37fd611c1cf
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287510"
---
# <a name="configure-project-categories"></a><span data-ttu-id="32d8e-103">परियोजना श्रेणियाँ कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="32d8e-103">Configure project categories</span></span>

<span data-ttu-id="32d8e-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="32d8e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="32d8e-105">Project Operations राजस्व और परियोजनाओं पर खर्च को वर्गीकृत करने के लिए मजबूत क्षमता प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="32d8e-105">Project Operations offers robust capabilities for categorizing revenue and expenses on projects.</span></span> <span data-ttu-id="32d8e-106">श्रेणियां परियोजना लेन-देन की रिपोर्ट करने और विश्लेषण करने और सामान्य बही खाते में ड्राइव पोस्टिंग करने की क्षमता प्रदान करती हैं.</span><span class="sxs-lookup"><span data-stu-id="32d8e-106">Categories provide the ability to report on and analyze project transactions, and drive posting to the general ledger.</span></span>

<span data-ttu-id="32d8e-107">निम्नलिखित रेखा चित्र लेनदेन श्रेणियों, साझा श्रेणियों और परियोजना श्रेणियों के बीच के संबंध को दर्शाता है.</span><span class="sxs-lookup"><span data-stu-id="32d8e-107">The following diagram illustrates the correlation between transaction categories, shared categories, and project categories.</span></span> 

<span data-ttu-id="32d8e-108">लेन-देन श्रेणियां परियोजना लेनदेन के लिए मूल ग्रुपिंग है.</span><span class="sxs-lookup"><span data-stu-id="32d8e-108">Transaction categories are the basic grouping for project transactions.</span></span> <span data-ttu-id="32d8e-109">उस ग्रुपिंग में साझा श्रेणियों का एक सेट होता है जिसे अनुप्रयोगों और मॉड्यूल में साझा किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="32d8e-109">Within that grouping, there is a set of shared categories that can be shared across applications and modules.</span></span> <span data-ttu-id="32d8e-110">विशिष्टताओं में और भी आगे बढ़ते हुए, परियोजना श्रेणियां श्रेणियों का सबसे स्पष्ट स्तर हैं.</span><span class="sxs-lookup"><span data-stu-id="32d8e-110">Getting even further into specifics, project categories are the most granular level of categories.</span></span> <span data-ttu-id="32d8e-111">परियोजना श्रेणियां कानूनी इकाई, मॉड्यूल और अनुप्रयोग के लिए विशिष्ट हैं.</span><span class="sxs-lookup"><span data-stu-id="32d8e-111">Project categories are specific to legal entity, module, and application.</span></span>

![लेनदेन श्रेणियों, साझा श्रेणियों और परियोजना श्रेणियों के बीच परस्पर संबंध](media/project-categories.png)

## <a name="transaction-categories"></a><span data-ttu-id="32d8e-113">लेन-देन श्रेणियाँ</span><span class="sxs-lookup"><span data-stu-id="32d8e-113">Transaction categories</span></span>

<span data-ttu-id="32d8e-114">लेनदेन श्रेणियां परियोजना लेनदेन के लिए मूल समूह का प्रतिनिधित्व करती हैं और यह कंपनी या प्रकार-विशिष्ट लेनदेन नहीं होती हैं.</span><span class="sxs-lookup"><span data-stu-id="32d8e-114">Transaction categories represent the basic grouping for project transactions and are not company or transaction type-specific.</span></span> <span data-ttu-id="32d8e-115">उदाहरण के लिए, Contoso Robotics समूह परियोजना लेनदेन के लिए डिजाइन, यात्रा, इंस्टॉलेशन और सेवा लेनदेन श्रेणियों का इस्तेमाल करता है.</span><span class="sxs-lookup"><span data-stu-id="32d8e-115">For example, Contoso Robotics uses Design, Travel, Installation, and Service Transaction categories to group Project transactions.</span></span>

<span data-ttu-id="32d8e-116">Project Operations मॉड्यूल में लेनदेन श्रेणियों को परिभाषित किया गया है.</span><span class="sxs-lookup"><span data-stu-id="32d8e-116">Transaction categories are defined in the Project Operations module.</span></span> 
1. <span data-ttu-id="32d8e-117">प्रपत्र खोलने के लिए **सेटिंग्स** \> **लेनदेन श्रेणियाँ** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="32d8e-117">Go to **Settings** \> **Transaction Categories** to open the form.</span></span> 
2. <span data-ttu-id="32d8e-118">नई लेनदेन श्रेणी बनाएं या तो **नया** चुनें या **Excel से आयात** चुनें.</span><span class="sxs-lookup"><span data-stu-id="32d8e-118">Create a new transaction category either by selecting **New** or by selecting **Import from Excel**.</span></span>

## <a name="shared-categories"></a><span data-ttu-id="32d8e-119">साझा श्रेणियां</span><span class="sxs-lookup"><span data-stu-id="32d8e-119">Shared categories</span></span>

<span data-ttu-id="32d8e-120">Dynamics 365 विभिन्न अनुप्रयोगों में खर्चों को वर्गीकृत करने के लिए साझा श्रेणियों की अवधारणा का उपयोग करता है, जैसे कि Dynamics 365 Finance, Dynamics 365 Supply Chain, और Dynamics 365 Project Operations.</span><span class="sxs-lookup"><span data-stu-id="32d8e-120">Dynamics 365 uses the Shared categories concept to categorize expenses in different applications, such as Dynamics 365 Finance, Dynamics 365 Supply Chain, and Dynamics 365 Project Operations.</span></span> <span data-ttu-id="32d8e-121">बनाई गई प्रत्येक लेन-देन श्रेणी के लिए, Project Operations स्वचालित रूप से चार संबंधित साझा श्रेणियां बनाता है: घंटे, व्यय, शुल्क, और आइटम.</span><span class="sxs-lookup"><span data-stu-id="32d8e-121">For each Transaction category created, Project Operations automatically creates four related Shared categories: Hours, Expense, Fees, and Item.</span></span> <span data-ttu-id="32d8e-122">आप **परियोजना प्रबंधन और लेखांकन** \> **सेटअप** \> **श्रेणियां** \> **साझा श्रेणियां** पर जाकर साझा श्रेणियों की समीक्षा और समायोजन कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="32d8e-122">You can review and adjust the shared categories by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Shared Categories**.</span></span>

## <a name="project-categories"></a><span data-ttu-id="32d8e-123">परियोजना श्रेणियाँ</span><span class="sxs-lookup"><span data-stu-id="32d8e-123">Project categories</span></span>

<span data-ttu-id="32d8e-124">परियोजना श्रेणियां श्रेणी कॉन्फ़िगरेशन के अधिकतम ग्रैन्युलर स्तर का प्रतिनिधित्व करती हैं और परियोजना अकाउंटेंट द्वारा अलग-अलग और प्रत्येक कंपनी के लिए कॉन्फ़िगर की जानी चाहिए.</span><span class="sxs-lookup"><span data-stu-id="32d8e-124">Project categories represent most granular level of category configuration and must be configured separately, and for each company, by a Project accountant.</span></span>

1. <span data-ttu-id="32d8e-125">**परियोजना प्रबंधन और लेखांकन** \> **सेटअप करें** \> **श्रेणियाँ** \> **परियोजना श्रेणियाँ** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="32d8e-125">Go to **Project Management and Accounting** \> **Setup** \> **Categories** \> **Project categories**.</span></span>
2. <span data-ttu-id="32d8e-126">**नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="32d8e-126">Select **New**.</span></span>
3. <span data-ttu-id="32d8e-127">आपके द्वारा पिछले अनुभाग में बनाई गई साझा श्रेणी की **श्रेणी ID** चुनें.</span><span class="sxs-lookup"><span data-stu-id="32d8e-127">Select the **Category ID** of the Shared category you created in the previous section.</span></span> <span data-ttu-id="32d8e-128">Project Operations केवल उन साझा श्रेणियों का इस्तेमाल करने की अनुमति देता है जो लेनदेन श्रेणियों से जुड़ी हैं.</span><span class="sxs-lookup"><span data-stu-id="32d8e-128">Project Operations allows using only those shared categories that are associated with transaction categories.</span></span>
4. <span data-ttu-id="32d8e-129">श्रेणी समूह चुनें.</span><span class="sxs-lookup"><span data-stu-id="32d8e-129">Select a category group.</span></span>

## <a name="category-groups"></a><span data-ttu-id="32d8e-130">श्रेणी समूह</span><span class="sxs-lookup"><span data-stu-id="32d8e-130">Category groups</span></span>

<span data-ttu-id="32d8e-131">श्रेणी समूह का उपयोग गुणों को साझा करने, मुख्य रूप से संबंधित परियोजना श्रेणियों के बीच प्रोफाइल दर्ज करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="32d8e-131">Category groups are used to share properties, primarily posting profiles, between related Project categories.</span></span> <span data-ttu-id="32d8e-132">प्रत्येक लेनदेन प्रकार के लिए कम से कम एक श्रेणी समूह होना चाहिए और प्रत्येक परियोजना श्रेणी को समूह सौंपा गया है.</span><span class="sxs-lookup"><span data-stu-id="32d8e-132">There must be at least one category group for each transaction type and each project category is assigned a group.</span></span>

<span data-ttu-id="32d8e-133">Project Operations में पोस्टिंग विनिर्देश को परियोजना लागत और आय प्रोफ़ाइल नियमों, परियोजना श्रेणियों और श्रेणी समूहों से स्पष्ट किया गया है.</span><span class="sxs-lookup"><span data-stu-id="32d8e-133">The posting specifications in Project Operations are defined by the project cost and revenue profile rules, project categories, and category groups.</span></span> <span data-ttu-id="32d8e-134">आप **परियोजना प्रबंधन और लेखांकन** \> **सेटअप**\> **श्रेणी** \> **श्रेणी समूह** पर जाकर श्रेणी समूह सेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="32d8e-134">You can set up category groups by going to **Project management and accounting** \> **Setup** \> **Categories** \> **Category groups**.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]