---
title: इकाईयाँ और इकाई समूह
description: यह विषय Dynamics 365 Project Operations में इकाईयाँ एयर इकाई समूह बनाने के तरीके के बारे में जानकारी प्रदान करता है.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 162366f4b7aa678b4e39d9745a657037bf36cbe0
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5277340"
---
# <a name="units-and-unit-groups"></a><span data-ttu-id="ce76e-103">इकाईयाँ और इकाई समूह</span><span class="sxs-lookup"><span data-stu-id="ce76e-103">Units and unit groups</span></span>

<span data-ttu-id="ce76e-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="ce76e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ce76e-105">इकाइयाँ वे मात्राएँ या माप होती हैं जिनमें आप अपने उत्पाद या सेवाएँ बेचते हैं.</span><span class="sxs-lookup"><span data-stu-id="ce76e-105">Units are the quantities or measurements that you sell your products or services in.</span></span> <span data-ttu-id="ce76e-106">उदाहरण के लिए, अगर आप बागान संबंधी आपूर्तियों का विक्रय करते हैं, तो हो सकता है कि आप पैकेट, बॉक्स और पैलेट में बीजों को बेचते हों.</span><span class="sxs-lookup"><span data-stu-id="ce76e-106">For example, if you sell gardening supplies, you might sell seeds in units of packets, boxes, and pallets.</span></span> <span data-ttu-id="ce76e-107">एक इकाई समूह, इन विभिन्न इकाइयों का संकलन होता है.</span><span class="sxs-lookup"><span data-stu-id="ce76e-107">A unit group is a collection of these different units.</span></span>

<span data-ttu-id="ce76e-108">इस विषय के चरणों को पूरा करने के लिए, सुनिश्चित करें कि आपको सिस्टम व्यवस्थापक या Sales Professional प्रंधक की भूमिका सौंपी गई है या समतुल्य अनुमति है.</span><span class="sxs-lookup"><span data-stu-id="ce76e-108">To complete the steps in this topic, make sure that you have been assigned to the System Administrator or Sales Professional Manager role or have equivalent permissions.</span></span>

## <a name="create-a-unit-group"></a><span data-ttu-id="ce76e-109">एक इकाई समूह बनाएँ</span><span class="sxs-lookup"><span data-stu-id="ce76e-109">Create a unit group</span></span>

1. <span data-ttu-id="ce76e-110">साइट मानचित्र में, **इकाइयाँ** चुनें.</span><span class="sxs-lookup"><span data-stu-id="ce76e-110">In the site map, select **Units**.</span></span>
2. <span data-ttu-id="ce76e-111">**नया** चुनें और **इकाई समूह बनाएं** संवाद बॉक्स में, इकाई का नाम दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="ce76e-111">Select **New**, and in the **Create Unit Group** dialog box, enter the unit name.</span></span>
3. <span data-ttu-id="ce76e-112">**प्राथमिक इकाई** फ़ील्ड में, उस उत्पाद की न्यूनतम सामान्य इकाई दर्ज करें जिस पर उत्पाद बेचा जाएगा.</span><span class="sxs-lookup"><span data-stu-id="ce76e-112">In the **Primary unit** field, enter the lowest common unit of measure that the product will be sold in.</span></span> <span data-ttu-id="ce76e-113">उदाहरण के लिए आप "सेट" या "औंस" दर्ज कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="ce76e-113">For example, you might enter "piece" or "ounce".</span></span>
4. <span data-ttu-id="ce76e-114">**ठीक** चुनें।</span><span class="sxs-lookup"><span data-stu-id="ce76e-114">Select **OK**.</span></span>

## <a name="add-units-to-a-unit-group"></a><span data-ttu-id="ce76e-115">इकाई समूह में इकाई जोड़ें</span><span class="sxs-lookup"><span data-stu-id="ce76e-115">Add units to a unit group</span></span>

1. <span data-ttu-id="ce76e-116">इकाई समूह खोलें, और **संबंधित** टैब पर, **इकाई** चुनें.</span><span class="sxs-lookup"><span data-stu-id="ce76e-116">Open a unit group, and on the **Related** tab, select **Units**.</span></span> <span data-ttu-id="ce76e-117">आप देखेंगे कि प्राथमिक इकाई पहले से ही जोड़ी गई है.</span><span class="sxs-lookup"><span data-stu-id="ce76e-117">You will see that the primary unit is already added.</span></span>
2. <span data-ttu-id="ce76e-118">**नई इकाई जोड़ें** चुनें, और **त्वरित इकाई बनाएं** पृष्ठ पर **नाम** फ़ील्ड में, इकाई का नाम लिखें.</span><span class="sxs-lookup"><span data-stu-id="ce76e-118">Select **Add New Unit**, and on the **Quick Create: Unit** page, in the **Name** field, enter the nanem of the unit.</span></span>
3. <span data-ttu-id="ce76e-119">**मात्रा** फ़ील्ड में, वह मात्रा दर्ज करें जो इकाई में होगी.</span><span class="sxs-lookup"><span data-stu-id="ce76e-119">In the **QUantity** field, enter the quantity that the unit will contain.</span></span> <span data-ttu-id="ce76e-120">उदाहरण के लिए, यदि किसी बॉक्स में दो सेट हैं, तो "2" दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="ce76e-120">For example, if a box contains two pieces, enter "2".</span></span> 
4. <span data-ttu-id="ce76e-121">**आधार इकाई** फ़ील्ड में, इकाई के लिए माप की निम्नतम इकाई स्थापित करने के लिए आधार इकाई चुनें.</span><span class="sxs-lookup"><span data-stu-id="ce76e-121">In the **Base unit** field, select a base unit to establish the lowest unit of measurement for the unit.</span></span> <span data-ttu-id="ce76e-122">उदाहरण के लिए, आप "सेट" चुन सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="ce76e-122">For example, you might select "Piece".</span></span>
5. <span data-ttu-id="ce76e-123">**सहेजें** चुनें:</span><span class="sxs-lookup"><span data-stu-id="ce76e-123">Select **Save**:</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]