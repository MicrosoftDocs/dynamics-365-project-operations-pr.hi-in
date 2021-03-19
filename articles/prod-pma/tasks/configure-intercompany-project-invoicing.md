---
title: इंटरकंपनी परियोजना इनवॉइस को कन्फीगर करता है
description: यह विषय दिखाता है कि आपके संगठन में दो कंपनियों के बीच प्रोजेक्ट इनवॉइस कैसे सेट करें.
author: Yowelle
manager: AnnBe
ms.date: 07/29/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: VendTable, InterCompanyTradingRelationSetupVendor, SysDataAreaSelectLookup, ProjParameters, ProjPosting, ProjTransferPrice
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 9df15cb3712356a164de3507f5dbc17a9ff9a652
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288381"
---
# <a name="configure-intercompany-project-invoicing"></a><span data-ttu-id="b4f9d-103">इंटरकंपनी परियोजना इनवॉइस को कन्फीगर करता है</span><span class="sxs-lookup"><span data-stu-id="b4f9d-103">Configure intercompany project invoicing</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="b4f9d-104">यह विषय दिखाता है कि आपके संगठन में दो कंपनियों के बीच प्रोजेक्ट इनवॉइस कैसे सेट करें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-104">This topic shows how to set up project invoicing between two companies in your organization.</span></span> <span data-ttu-id="b4f9d-105">यह कार्य USSI डेटा सेट का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-105">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="b4f9d-106">नेविगेशन फलक में **मॉड्यूल > देनदारी लेखे > विक्रेता > सभी विक्रेता** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-106">In the navigation pane, go to **Modules > Accounts payable > Vendors > All vendors**.</span></span>
2. <span data-ttu-id="b4f9d-107">**सभी विक्रेता** सूची में, वांछित रिकॉर्ड को पाएं या चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-107">In the **All vendors** list, find and select the desired record.</span></span>
3. <span data-ttu-id="b4f9d-108">क्रिया फलक पर, **सामान्य** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-108">On the Action Pane, select **General**.</span></span>
4. <span data-ttu-id="b4f9d-109">चुनते हैं **इंटरकंपनी** ।</span><span class="sxs-lookup"><span data-stu-id="b4f9d-109">Select **Intercompany**.</span></span>
5. <span data-ttu-id="b4f9d-110">इंटरकंपनी व्यापार को सक्रिय करने के लिए **सक्रिय** को **हां** करें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-110">Set **Active** to **Yes** to enable intercompany trading.</span></span>
6. <span data-ttu-id="b4f9d-111">**कस्टमर कंपनी** फील्ड में, एक मूल्य को दर्ज करें या चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-111">In the **Customer company** field, enter or select a value.</span></span>
7. <span data-ttu-id="b4f9d-112">**मेरा खाता** फील्ड में मूल्य को दर्ज करें या चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-112">In the **My account** field, enter or select a value.</span></span>
8. <span data-ttu-id="b4f9d-113">**सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-113">Select **Save**.</span></span>
9. <span data-ttu-id="b4f9d-114">होमपेज पर लौटने के लिए पेज को बंद करें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-114">Close the pages to return to the home page.</span></span>
10. <span data-ttu-id="b4f9d-115">नेविगेशन फलक में, **मॉड्यूल > परियोजना प्रबंधन और लेखांकन > सेटअप > परियोजना प्रबंधन और लेखांकन मापदंड** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-115">In the navigation pane, go to **Modules > Project management and accounting > Setup > Project management and accounting parameters**.</span></span>
11. <span data-ttu-id="b4f9d-116">**Intercompany** टैब का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-116">Select the **Intercompany** tab.</span></span>
12. <span data-ttu-id="b4f9d-117">इंटरकंपनी संसाधन शेड्युलिंग और टाइमशीट को सक्रिय करने के लिए स्लाइडर को **हां** में बदलें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-117">Move the slider to **Yes** to enable intercompany resource scheduling and timesheets.</span></span>
13. <span data-ttu-id="b4f9d-118">सूची में, चयनित पंक्ति को चिह्नित करें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-118">In the list, mark the selected row.</span></span>
14. <span data-ttu-id="b4f9d-119">**नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-119">Select **New**.</span></span>
15. <span data-ttu-id="b4f9d-120">**कानूनी इकाई उधार लेना** फील्ड में, एक मूल्य दर्ज करें या चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-120">In the **Borrowing legal entity** field, enter or select a value.</span></span>
16. <span data-ttu-id="b4f9d-121">**राजस्व आय** चेक बॉक्स को चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-121">Select the **Accrue revenue** check box.</span></span>
17. <span data-ttu-id="b4f9d-122">**डिफॉल्ट टाइमशीट श्रेणी** फील्ड में, एक मूल्य दर्ज करें या चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-122">In the **Default timesheet category** field, enter or select a value.</span></span>
18. <span data-ttu-id="b4f9d-123">**डिफॉल्ट व्यय श्रेणी** फील्ड में, एक मूल्य दर्ज करें या चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-123">In the **Default expense category** field, enter or select a value.</span></span>
19. <span data-ttu-id="b4f9d-124">**सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-124">Select **Save**.</span></span>
20. <span data-ttu-id="b4f9d-125">पृष्ठ बंद करें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-125">Close the page.</span></span>
21. <span data-ttu-id="b4f9d-126">नेवीगेशन फलक में, **मॉड्यूल >परियोजना प्रबंधन और लेख विधि > सेट अप >पोस्टिंग > लेजर पोस्टिंग सेट अप** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-126">In the navigation pane, go to **Modules > Project management and accounting > Setup > Posting > Ledger posting setup**.</span></span>
22. <span data-ttu-id="b4f9d-127">**लेजर खाता प्रकार** प्रकार में एक विकल्प चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-127">In the **Ledger account types** field, select an option.</span></span>
23. <span data-ttu-id="b4f9d-128">**नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-128">Select **New**.</span></span>
24. <span data-ttu-id="b4f9d-129">नई पंक्ति के **मुख्य खाता** फील्ड में, वांछित मूल्य दर्शाएं.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-129">In the **Main account** field of the new row, specify the desired values.</span></span>
25. <span data-ttu-id="b4f9d-130">**सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-130">Select **Save**.</span></span>
26. <span data-ttu-id="b4f9d-131">पृष्ठ बंद करें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-131">Close the page.</span></span>
27. <span data-ttu-id="b4f9d-132">नेवीगेशन फलक में, **मॉड्यूल >परियोजना प्रबंधन और लेख विधि > सेट अप > मूल्य > स्थानांतरण मूल्य** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-132">In the navigation pane, go to **Modules > Project management and accounting > Setup > Prices > Transfer price**.</span></span>
28. <span data-ttu-id="b4f9d-133">**नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-133">Select **New**.</span></span>
29. <span data-ttu-id="b4f9d-134">**प्रभावी तारीख** फील्ड में, एक तारीख दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-134">In the **Effective date** field, enter a date.</span></span>
30. <span data-ttu-id="b4f9d-135">**कानूनी इकाई उधार लेना** फील्ड में, एक मूल्य दर्ज करें या चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-135">In the **Borrowing legal entity** field, enter or select a value.</span></span>
31. <span data-ttu-id="b4f9d-136">**हस्तांतरण मूल्य मॉडल** फील्ड, में एक विकल्प को चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-136">In the **Transfer price model** field, select an option.</span></span>
32. <span data-ttu-id="b4f9d-137">**मूल्य** फ़ील्ड में, संख्या दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-137">In the **Pricing** field, enter a number.</span></span>
33. <span data-ttu-id="b4f9d-138">**सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="b4f9d-138">Select **Save**.</span></span>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]