---
title: श्रम और व्यय पर स्टैंडर्ड लागत को कन्फीगर करें
description: यह विषय बताता है कि किसी परियोजना के लिए श्रम और व्यय की स्टैंडर्ड लागत कैसे तय की जाती है.
author: Yowelle
manager: AnnBe
ms.date: 08/02/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjCostPriceHour, ProjSalesPriceHour, ProjCostPriceExpense, ProjSalesPriceCost
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: b3eb6b1d4d75b095383689dd53a59a15fe9e884a
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077757"
---
# <a name="configure-standard-costs-for-labor-and-expenses"></a><span data-ttu-id="c1dc9-103">श्रम और व्यय पर स्टैंडर्ड लागत को कन्फीगर करें</span><span class="sxs-lookup"><span data-stu-id="c1dc9-103">Configure standard costs for labor and expenses</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="c1dc9-104">यह विषय बताता है कि किसी परियोजना के लिए श्रम और व्यय की स्टैंडर्ड लागत कैसे तय की जाती है.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-104">This topic explains how to set up standard costs for labor and expenses for a project.</span></span> <span data-ttu-id="c1dc9-105">यह कार्य USSI डेटा सेट का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-105">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="c1dc9-106">नेवीगेशन फलक में, **मॉड्यूल >परियोजना प्रबंधन और लेख विधि > सेट अप > मूल्य > लागत लेखांकन (घंटा)** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-106">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Cost price (hour)**.</span></span>
2. <span data-ttu-id="c1dc9-107">**नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-107">Select **New**.</span></span>
3. <span data-ttu-id="c1dc9-108">**प्रभावी तारीख** फील्ड में, एक तारीख दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-108">In the **Effective date** field, enter a date.</span></span>
4. <span data-ttu-id="c1dc9-109">**लागत मूल्य** फ़ील्ड में, संख्या दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-109">In the **Cost price** field, enter a number.</span></span> <span data-ttu-id="c1dc9-110">आप परियोजना श्रेणी के लिए एक स्टैंडर्ड लागत मूल्य तय कर सकते हैं, या श्रमिकों की संख्या, परियोजना संख्या श्रेणी, तारीख, या इनमें से किसी एक संयोजन के साथ लागत मूल्य तय कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-110">You can set up a standard cost price for the project category, or you can set up a cost price by worker number, project number, category, date, or any combination of these.</span></span> <span data-ttu-id="c1dc9-111">लागत मूल्य वह होती है जो उच्च स्तर वाले ब्यौरे पर लागू होने वाली लागत मूल्य होती है.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-111">The cost price that is applied is the cost price with the highest level of detail.</span></span>  
5. <span data-ttu-id="c1dc9-112">**सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-112">Select **Save**.</span></span>
6. <span data-ttu-id="c1dc9-113">नेवीगेशन फलक में, **मॉड्यूल >परियोजना प्रबंधन और लेख विधि > सेट अप > मूल्य > विक्रय मूल्य (घंटा)** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-113">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Sales price (hour)**.</span></span>
7. <span data-ttu-id="c1dc9-114">**नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-114">Select **New**.</span></span>
8. <span data-ttu-id="c1dc9-115">**प्रभावी तारीख** फील्ड में, एक तारीख दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-115">In the **Effective date** field, enter a date.</span></span>
9. <span data-ttu-id="c1dc9-116">**वैध है** फील्ड, से एक विकल्प को चुनें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-116">In the **Valid for** field, select an option.</span></span>
10. <span data-ttu-id="c1dc9-117">**मूल्य** फ़ील्ड में, संख्या दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-117">In the **Pricing** field, enter a number.</span></span> <span data-ttu-id="c1dc9-118">आप एक घंटा लेनदेन या एक परियोजना श्रेणी के लिए स्टैंडर्ड बिक्री मूल्य तय कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-118">You can set up a standard sales price for hour transactions or for a project category.</span></span> <span data-ttu-id="c1dc9-119">आप श्रमिकों की संख्या, परियोजना संख्या, श्रेणी, लेनदेन की तारीख , या इनमें से किसी एक मेल द्वारा बिक्री का मूल्य तय कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-119">You can also set up sales prices by worker number, project number, category, transaction date, or any combination of these.</span></span> <span data-ttu-id="c1dc9-120">वास्तविक बिक्री मूल्य, उच्च स्तर के ब्यौरे के साथ बिक्री मूल्य होता है, जो तब लागू किया जाता है जब कोई कर्मचारी घंटा बहीखाता में लेनदेन करता है, बिक्री मूल्य के उच्चतम स्तर के साथ होता है.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-120">The actual sales price, which is applied when a worker enters a transaction in the Hour journal, is the sales price with the highest level of detail.</span></span> <span data-ttu-id="c1dc9-121">उदाहरण के लिए, अगर आम बिक्री मूल्य और श्रमिक संबंधित बिक्री मूल्य दोनों को तय किया जाता है, तो श्रमिक संबंधित बिक्री मूल्य का इस्तेमाल किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-121">For example, if both a general sales price and a worker-specific sales price are set up, the worker-specific sales price is used.</span></span>  
11. <span data-ttu-id="c1dc9-122">**सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-122">Select **Save**.</span></span>
12. <span data-ttu-id="c1dc9-123">पृष्ठ बंद करें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-123">Close the page.</span></span>
13. <span data-ttu-id="c1dc9-124">नेवीगेशन फलक में, **मॉड्यूल > परियोजना प्रबंधन और लेख विधि > सेट अप > मूल्य > लागत लेखांकन (व्यय)** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-124">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Cost price (expense)**.</span></span>
14. <span data-ttu-id="c1dc9-125">**नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-125">Select **New**.</span></span>
15. <span data-ttu-id="c1dc9-126">**प्रभावी तारीख** फील्ड में, एक तारीख दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-126">In the **Effective date** field, enter a date.</span></span>
16. <span data-ttu-id="c1dc9-127">**लागत मूल्य** फ़ील्ड में, संख्या दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-127">In the **Cost price** field, enter a number.</span></span> <span data-ttu-id="c1dc9-128">कई फील्ड को भरा जा सकता है, लेकिन रिकॉर्ड को सुरक्षित रखने के लिए इसकी बहुत कम जरूरत होती है.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-128">Multiple fields can be filled in, but this is the minimum needed to save the record.</span></span>  
17. <span data-ttu-id="c1dc9-129">**सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-129">Select **Save**.</span></span>
18. <span data-ttu-id="c1dc9-130">नेवीगेशन फलक में, **मॉड्यूल > परियोजना प्रबंधन और लेख विधि > सेट अप > मूल्य > विक्रय मूल्य (व्यय)** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-130">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Sales price (expense)**.</span></span>
19. <span data-ttu-id="c1dc9-131">**नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-131">Select **New**.</span></span>
20. <span data-ttu-id="c1dc9-132">**प्रभावी तारीख** फील्ड में, एक तारीख दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-132">In the **Effective date** field, enter a date.</span></span>
21. <span data-ttu-id="c1dc9-133">**वैध है** फील्ड, से एक विकल्प को चुनें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-133">In the **Valid for** field, select an option.</span></span>
22. <span data-ttu-id="c1dc9-134">**मूल्य** फ़ील्ड में, संख्या दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-134">In the **Pricing** field, enter a number.</span></span> <span data-ttu-id="c1dc9-135">वास्तविक बिक्री मूल्य, उच्च स्तर के ब्यौरे के साथ बिक्री मूल्य होता है, जो तब लागू किया जाता है जब कोई कर्मचारी व्यय बहीखाता में लेनदेन करता है, बिक्री मूल्य के उच्चतम स्तर के साथ होता है.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-135">The actual sales price, which is applied when a worker enters transactions in an expense journal, is the sales price with the highest level of detail.</span></span> <span data-ttu-id="c1dc9-136">उदाहरण के लिए, अगर आम और श्रमिक संबंधित बिक्री मूल्य दोनों को तय किया जाता है, तो श्रमिक संबंधित बिक्री मूल्य का इस्तेमाल किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-136">For example, if both a general and a worker-specific sales price are set up, the worker-specific sales price is used.</span></span>  
23. <span data-ttu-id="c1dc9-137">**सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c1dc9-137">Select **Save**.</span></span>

