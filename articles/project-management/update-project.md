---
title: परियोजना अपडेट करें
description: यह विषय परियोजना संचालन परियोजनाओं को अपडेट करने के बारे में जानकारी प्रदान करता है।
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 5c9cd0c7c6886bd454c5f2ef2ae7f20d1707293f
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897814"
---
# <a name="update-a-project"></a><span data-ttu-id="ff57c-103">परियोजना अपडेट करें</span><span class="sxs-lookup"><span data-stu-id="ff57c-103">Update a project</span></span>

<span data-ttu-id="ff57c-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="ff57c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="ff57c-105">नीचे उन क्षेत्रों का सारांश है, जिन्हें बनाए जाने और अपडेट के किसी भी लागू निहितार्थ किसी परियोजना पर अपडेट किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="ff57c-105">Below is a summary of the fields that can be updated on a project after it has been created and any applicable implications of the updates.</span></span>

## <a name="project-detail-fields"></a><span data-ttu-id="ff57c-106">परियोजना विस्तार क्षेत्र</span><span class="sxs-lookup"><span data-stu-id="ff57c-106">Project detail fields</span></span>

- <span data-ttu-id="ff57c-107">**नाम**: परियोजना का शीर्षक।</span><span class="sxs-lookup"><span data-stu-id="ff57c-107">**Name**: The title of the project.</span></span>
- <span data-ttu-id="ff57c-108">**विवरण**: परियोजना का संक्षिप्त विवरण।</span><span class="sxs-lookup"><span data-stu-id="ff57c-108">**Description**: An overview of the project.</span></span>
- <span data-ttu-id="ff57c-109">**ग्राहक**: जिस कंपनी को परियोजना दी जाएगी।</span><span class="sxs-lookup"><span data-stu-id="ff57c-109">**Customer**: The company the project will be delivered to.</span></span>
- <span data-ttu-id="ff57c-110">**कैलेंडर टेम्प्लेट**: परियोजना के काम के घंटे।</span><span class="sxs-lookup"><span data-stu-id="ff57c-110">**Calendar template**: The working hours of the project.</span></span> <span data-ttu-id="ff57c-111">जब क्षेत्र को बदला जाता है, तो पूरा शेड्यूल पुनर्गणित होता है.</span><span class="sxs-lookup"><span data-stu-id="ff57c-111">When the field is changed, the entire schedule is recalculated.</span></span>
- <span data-ttu-id="ff57c-112">**मुद्रा**: परियोजना के लिए मुद्रा।</span><span class="sxs-lookup"><span data-stu-id="ff57c-112">**Currency**: The currency for the project.</span></span> <span data-ttu-id="ff57c-113">यह क्षेत्र अनुबंध इकाई में परिभाषित मुद्रा के आधार पर डिफॉल्ट करता है.</span><span class="sxs-lookup"><span data-stu-id="ff57c-113">This field defaults based on the currency defined in the contracting unit.</span></span> <span data-ttu-id="ff57c-114">जब अनुबंध इकाई को अपडेट किया जाता है, तो क्षेत्र को भी अपडेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="ff57c-114">When the contracting unit is updated, the field is also updated.</span></span>
- <span data-ttu-id="ff57c-115">**अनुबंध इकाई**: वह संगठनात्मक इकाई जो कंपनी समूह या विभाग का प्रतिनिधित्व करती है, जो मुख्य रूप से बिक्री को पाने और ग्राहक को कार्य और सेवाओं के वितरण का प्रबंधन करने के लिए जिम्मेदार है।</span><span class="sxs-lookup"><span data-stu-id="ff57c-115">**Contracting Unit**: The organizational unit that represents the company group or division that is primarily responsible for winning the sale and managing the delivery of work and services to the customer.</span></span> 
- <span data-ttu-id="ff57c-116">**परियोजना प्रबंधक**: परियोजना टीम का वह सदस्य जिसके पास समय प्रविष्टियों और खर्च की समीक्षा करने और स्वीकृत करने का अधिकार है.</span><span class="sxs-lookup"><span data-stu-id="ff57c-116">**Project Manager**: The project team member who has the authority to review and approve time entries and expenses.</span></span>

## <a name="estimate-fields"></a><span data-ttu-id="ff57c-117">खेतों का अनुमान लगाएं</span><span class="sxs-lookup"><span data-stu-id="ff57c-117">Estimate fields</span></span>

- <span data-ttu-id="ff57c-118">**अनुमानित आरंभ तिथि**: वह तिथि जब परियोजना शुरू होगी।</span><span class="sxs-lookup"><span data-stu-id="ff57c-118">**Estimated Start Date**: The date that the project will begin.</span></span> <span data-ttu-id="ff57c-119">जब इस क्षेत्र को अपडेट किया जाता है, तो परियोजना पर कोई भी कार्य नई प्रारंभ तिथि प्रारंभ करें के साथ आनुपातिक रूप से आगे बढ़ेगा.</span><span class="sxs-lookup"><span data-stu-id="ff57c-119">When this field is updated, any tasks on the project will move proportionately with the start new start date.</span></span>
- <span data-ttu-id="ff57c-120">**समाप्ति तिथि**: वह तिथि जब परियोजना समाप्त होने का शेड्यूल है।</span><span class="sxs-lookup"><span data-stu-id="ff57c-120">**Finish Date**: The date that the project is scheduled to end.</span></span>
- <span data-ttu-id="ff57c-121">**प्रयास**: परियोजना का अनुमानित प्रयास।</span><span class="sxs-lookup"><span data-stu-id="ff57c-121">**Effort**: The estimated effort of the project.</span></span> <span data-ttu-id="ff57c-122">जब कार्यों को परियोजना में जोड़ा जाता है, तो यह क्षेत्र तब संपादन योग्य नहीं रहता.</span><span class="sxs-lookup"><span data-stu-id="ff57c-122">When tasks are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="ff57c-123">**अनुमानित श्रम लागत**: परियोजना की अनुमानित श्रम लागत।</span><span class="sxs-lookup"><span data-stu-id="ff57c-123">**Estimated Labor Cost**: The estimated labor cost of the project.</span></span> <span data-ttu-id="ff57c-124">जब श्रम लागत को परियोजना में जोड़ा जाता है, तो यह क्षेत्र तब संपादन योग्य नहीं रहता.</span><span class="sxs-lookup"><span data-stu-id="ff57c-124">When labor costs are added to the project, this field is no longer editable.</span></span>
- <span data-ttu-id="ff57c-125">**अनुमानित व्यय**: परियोजना का अनुमानित खर्च।</span><span class="sxs-lookup"><span data-stu-id="ff57c-125">**Estimated Expenses**: The estimated expenses of the project.</span></span> <span data-ttu-id="ff57c-126">जब व्यय प्रोजेक्ट में जोड़े जाते हैं, तो यह फ़ील्ड अब संपादन योग्य नहीं है।</span><span class="sxs-lookup"><span data-stu-id="ff57c-126">When expenses are added to the project, this field is no longer editable.</span></span>

## <a name="project-actual-fields"></a><span data-ttu-id="ff57c-127">परियोजना का वास्तविक क्षेत्र</span><span class="sxs-lookup"><span data-stu-id="ff57c-127">Project actual fields</span></span>
- <span data-ttu-id="ff57c-128">**वास्तविक शुरुआत**: परियोजना शुरू होने की तिथि।</span><span class="sxs-lookup"><span data-stu-id="ff57c-128">**Actual Start**: The date that the project started.</span></span>
- <span data-ttu-id="ff57c-129">**वास्तविक समाप्ति**: परियोजना के पूरा होने पर अपडेट किया जाना है।</span><span class="sxs-lookup"><span data-stu-id="ff57c-129">**Actual Finish**: To be updated when a project has been completed.</span></span>

## <a name="project-status-fields"></a><span data-ttu-id="ff57c-130">परियोजना स्थिति क्षेत्र</span><span class="sxs-lookup"><span data-stu-id="ff57c-130">Project status fields</span></span>

- <span data-ttu-id="ff57c-131">**समग्र परियोजना स्थिति**: परियोजना प्रबंधक द्वारा प्रदान किया गया समग्र परियोजना स्वास्थ्य.</span><span class="sxs-lookup"><span data-stu-id="ff57c-131">**Overall Project Status**: The overall project health provided by the Project manager.</span></span>
- <span data-ttu-id="ff57c-132">**टिप्पणियां**: परियोजना के वर्तमान स्वास्थ्य के बारे में परियोजना प्रबंधक द्वारा प्रदान किया गया विवरण।</span><span class="sxs-lookup"><span data-stu-id="ff57c-132">**Comments**: A narrative regarding the current health of the project provided by the Project manager.</span></span>

