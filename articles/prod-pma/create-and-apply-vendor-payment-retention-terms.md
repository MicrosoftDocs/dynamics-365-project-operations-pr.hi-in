---
title: विक्रेता भुगतान अवधारण शर्तें बनाएँ और लागू करें
description: यह विषय विक्रेता भुगतान के लिए प्रतिधारण शर्तों को सेट करने और बनाए रखने के तरीके के बारे में जानकारी प्रदान करता है.
author: Yowelle
manager: AnnBe
ms.date: 05/26/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 1970a24a5073de6af43db1f1c068332c9ba9c8fe
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077837"
---
# <a name="create-and-apply-vendor-payment-retention-terms"></a><span data-ttu-id="d8302-103">विक्रेता भुगतान अवधारण शर्तें बनाएँ और लागू करें</span><span class="sxs-lookup"><span data-stu-id="d8302-103">Create and apply vendor payment retention terms</span></span>

[!include [banner](../includes/banner.md)] 

<span data-ttu-id="d8302-104">किसी प्रोजेक्ट के लिए विक्रेता भुगतान प्रतिधारण शर्तें सेट करना तब उपयोगी होता है जब आपका संगठन विक्रेता को किए गए भुगतानों का हिस्सा बनाए रखना चाहता है.</span><span class="sxs-lookup"><span data-stu-id="d8302-104">Setting up vendor payment retention terms for a project is useful when your organization wants to retain part of the payments made to a vendor.</span></span> <span data-ttu-id="d8302-105">उदाहरण के लिए, आप तब तक किसी विक्रेता का भुगतान रोके रखना चाहते हैं, जब तक कि डिलीवर किए गए उत्पाद आपकी अपेक्षाओं को पूरा नहीं करते.</span><span class="sxs-lookup"><span data-stu-id="d8302-105">For example, when you want to hold payment to a vendor until the products delivered meet your expectations.</span></span> <span data-ttu-id="d8302-106">जब आप किसी विक्रेता अनुबंध पर बातचीत तय करते हैं तो विक्रेता भुगतान की प्रतिधारण शर्तें निर्दिष्ट की जा सकती हैं.</span><span class="sxs-lookup"><span data-stu-id="d8302-106">Vendor payment retention terms can be specified when you negotiate a vendor contract.</span></span>

## <a name="create-vendor-payment-retention-terms"></a><span data-ttu-id="d8302-107">विक्रेता भुगतान प्रतिधारण शर्तें बनाएं</span><span class="sxs-lookup"><span data-stu-id="d8302-107">Create vendor payment retention terms</span></span>

<span data-ttu-id="d8302-108">आप प्रतिधारण के लिए विक्रेता भुगतान का प्रतिशत और निर्गत होने वाली पहले से रखी गई राशि का प्रतिशत दर्ज कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="d8302-108">You can enter the percentage of vendor payment for retention and the percentage of the previously retained amounts to be released.</span></span> <span data-ttu-id="d8302-109">जब तक अनुबंध पूरा होने की निर्दिष्ट स्थिति तक नहीं पहुंच जाता, तब तक विक्रेता इनवॉइसों पर राशियां स्वचालित रूप से रखी जाती हैं.</span><span class="sxs-lookup"><span data-stu-id="d8302-109">Amounts are automatically retained on vendor invoices until the contract reaches the specified state of completion.</span></span> <span data-ttu-id="d8302-110">प्रतिधारण की शर्तें सेट करने के बाद, आप उन्हें उस विक्रेता के लिए किसी भी प्रोजेक्ट पर लागू कर सकते.</span><span class="sxs-lookup"><span data-stu-id="d8302-110">After you set up the retention terms, you can apply them to any project for that vendor.</span></span>

<span data-ttu-id="d8302-111">विक्रेता भुगतान के लिए प्रतिधारण की शर्तों को सेट करने और बनाए रखने के लिए निम्नलिखित चरणों का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="d8302-111">Use the following steps to set up and maintain retention terms for vendor payments.</span></span> 

1. <span data-ttu-id="d8302-112">**प्रोजेक्ट प्रबंधन और लेखांकन** > **प्रतिधारण** > **विक्रेता भुगतान की प्रतिधारण शर्तें** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="d8302-112">Go to **Project management and accounting** > **Retention** > **Vendor payment retention terms**.</span></span>
2. <span data-ttu-id="d8302-113">एक नई विक्रेता प्रतिधारण शर्त जोड़ने के लिए **नया** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="d8302-113">Select **New** to add a new vendor retention term.</span></span> <span data-ttu-id="d8302-114">नए शर्त के लिए **नियम ID** मान स्वचालित रूप से दर्ज किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d8302-114">The **Rule ID** value for the new term is automatically entered.</span></span> 
3. <span data-ttu-id="d8302-115">**विवरण** फ़ील्ड में एक संक्षिप्त विवरण दर्ज करें, और **शर्त** FastTab पर, निम्नलिखित के लिए शर्त मानों को दर्ज करने के लिए **लाइन जोड़ें** का चयन करें:</span><span class="sxs-lookup"><span data-stu-id="d8302-115">Enter a brief description in the **Description** field, and on the **Terms** FastTab, select **Add line** to enter term values for the following:</span></span>

   - <span data-ttu-id="d8302-116">**डिलीवर की गई इकाईयों का प्रतिशत** : शर्त के लिए पूरा होने का एक प्रतिशत दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="d8302-116">**Percentage of units delivered** : Enter a percentage of completion for the term.</span></span> <span data-ttu-id="d8302-117">जब तक पूरा होने का प्रोजेक्ट चरण निर्दिष्ट प्रतिशत के बराबर नहीं हो जाता तब तक विक्रेता इनवॉइसों पर राशियां स्वचालित रूप से बनी रहती हैं.</span><span class="sxs-lookup"><span data-stu-id="d8302-117">Amounts are automatically retained on vendor invoices until the project stage of completion is equal to the specified percentage.</span></span> <span data-ttu-id="d8302-118">उदाहरण के लिए, यदि आप 50.00 दर्ज करते हैं, तो राशि तब तक बनाई रखी जाती है जब तक कि प्रोजेक्ट 50 प्रतिशत पूरी नहीं हो जाता.</span><span class="sxs-lookup"><span data-stu-id="d8302-118">For example, if you enter 50.00, amounts are retained until the project is 50 percent completed.</span></span>
   - <span data-ttu-id="d8302-119">**प्रतिशत बनाए रखने के लिए** : बनाए रखने के लिए विक्रेता इनवॉइस राशि का एक प्रतिशत दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="d8302-119">**Percentage to retain** : Enter a percentage of the vendor invoice amount to be retained.</span></span> <span data-ttu-id="d8302-120">उदाहरण के लिए, यदि आप 10.00 दर्ज करते हैं, तो विक्रेता इनवॉइस पर राशि का 10 प्रतिशत तब तक बनाए रखा जाता है जब तक कि प्रोजेक्ट **डिलीवर की गई इकाइयों का प्रतिशत** फ़ील्ड में सेट की गई पूरा होने के प्रतिशत तक नहीं पहुंच जाती है.</span><span class="sxs-lookup"><span data-stu-id="d8302-120">For example, if you enter 10.00, then 10 percent of the amount on a vendor invoice is retained until the project reaches the percentage of completion as set in the **Percentage of units delivered field**.</span></span>
   - <span data-ttu-id="d8302-121">**प्रतिशत निर्गत करने के लिए** : प्रोजेक्ट पूरा होने के चयनित स्तर के लिए जारी किए जाने वाले किसी भी पहले से बनाए गए राशि का प्रतिशत दर्ज करने के लिए **लाइन जोड़ें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="d8302-121">**Percentage to release** : Select **Add line** to enter a percentage of any previously retained amounts to be released for the selected level of project completion.</span></span>

> [!NOTE]
> <span data-ttu-id="d8302-122">यदि आपके पास प्रोजेक्ट के पूरा होने के विभिन्न स्तरों के लिए एक से अधिक उपलब्धि है, तो प्रत्येक प्रतिधारण नियम के लिए एक अलग विक्रेता प्रतिधारण शर्त लाइन दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="d8302-122">If you have more than one milestone for different levels of project completion, enter a separate vendor retention term line for each retention rule.</span></span> <span data-ttu-id="d8302-123">प्रत्येक लाइन एक अलग प्रतिधारण प्रतिशत और प्रोजेक्ट पूरा होने के प्रत्येक निर्धारित स्तर के लिए एक अलग निर्गत प्रतिशत निर्दिष्ट कर सकती है.</span><span class="sxs-lookup"><span data-stu-id="d8302-123">Each line can specify a different retention percentage and a different release percentage for each designated level of project completion.</span></span>

<span data-ttu-id="d8302-124">विक्रेता के लिए विक्रेता प्रतिधारण शर्तें बनाने के बाद, आप किसी प्रोजेक्ट पर शर्तें लागू कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="d8302-124">After you create vendor retention terms for a vendor, you can apply the terms to a project.</span></span>

## <a name="apply-vendor-retention-terms-to-a-project"></a><span data-ttu-id="d8302-125">किसी प्रोजेक्ट के लिए विक्रेता प्रतिधारण शर्तें लागू करें</span><span class="sxs-lookup"><span data-stu-id="d8302-125">Apply vendor retention terms to a project</span></span>

1. <span data-ttu-id="d8302-126">**प्रोजेक्ट प्रबंधन और लेखांकन** > **प्रोजेक्ट** > **सभी प्रोजेक्ट** पर जाएं और प्रोजेक्ट सूची पृष्ठ से एक प्रोजेक्ट खोलें.</span><span class="sxs-lookup"><span data-stu-id="d8302-126">Go to **Project management and accounting** > **Projects** > **All projects** and open a project from the project list page.</span></span>
2. <span data-ttu-id="d8302-127">**विक्रेता अनुबंध** फास्ट टैब पर **लाइन जोड़ें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="d8302-127">On the **Vendor agreements** FastTab, select **Add line**.</span></span>
3. <span data-ttu-id="d8302-128">**खाता कोड** फ़ील्ड में, निम्नलिखित विकल्पों में से एक का चयन करें:</span><span class="sxs-lookup"><span data-stu-id="d8302-128">In the **Account code field** , select one of the following options:</span></span> 

   - <span data-ttu-id="d8302-129">**तालिका** : विक्रेता प्रतिधारण शर्तें एक ही विक्रेता पर लागू होती हैं.</span><span class="sxs-lookup"><span data-stu-id="d8302-129">**Table** : The vendor retention terms apply to a single vendor.</span></span>
   - <span data-ttu-id="d8302-130">**समूह** : विक्रेता प्रतिधारण शर्तें विक्रेता समूह के सभी विक्रेताओं पर लागू होती हैं.</span><span class="sxs-lookup"><span data-stu-id="d8302-130">**Group** : The vendor retention terms apply to all vendors in a vendor group.</span></span>
   - <span data-ttu-id="d8302-131">**सभी** : विक्रेता प्रतिधारण शर्तें सभी विक्रेताओं पर लागू होती हैं.</span><span class="sxs-lookup"><span data-stu-id="d8302-131">**All** : The vendor retention terms apply to all vendors.</span></span>

4. <span data-ttu-id="d8302-132">**विक्रेता/विक्रेता समूह** फ़ील्ड में, विक्रेता या विक्रेता समूह का चयन करें जिस पर विक्रेता प्रतिधारण शर्तें लागू होती हैं.</span><span class="sxs-lookup"><span data-stu-id="d8302-132">In the **Vendor/Vendor group field** , select the vendor or vendor group to which the vendor retention terms apply.</span></span> <span data-ttu-id="d8302-133">यदि आपने पिछले चरण में **सभी** का चयन किया है, तो यह फ़ील्ड अनुपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="d8302-133">If you selected **All** in the previous step, this field is unavailable.</span></span>
5. <span data-ttu-id="d8302-134">**विक्रेता प्रतिधारण शर्तें** फ़ील्ड में, पिछली प्रक्रिया में आपके द्वारा बनाए गए प्रतिधारण शर्तों का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="d8302-134">In the **Vendor retention terms** field, select the retention terms that you created in the previous procedure.</span></span>
6. <span data-ttu-id="d8302-135">यदि प्रोजेक्ट में विक्रेता के लिए भुगतान मिलने-पर-भुगतान (PWP) शर्तें भी सेट हैं, तो **PWP सीमा-रेखा प्रतिशत** फ़ील्ड में प्रोजेक्ट के लिए सीमा-रेखा प्रतिशत दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="d8302-135">If the project also has pay-when-paid (PWP) terms set up for the vendor, enter the threshold percentage for the project in the **PWP threshold percentage** field.</span></span>

<span data-ttu-id="d8302-136">विक्रेता प्रतिधारण शर्तें आपके द्वारा विक्रेता के लिए बनाए गए खरीद आदेशों पर भी प्रदर्शित की जाती हैं.</span><span class="sxs-lookup"><span data-stu-id="d8302-136">The vendor retention terms are also displayed on purchase orders that you create for the vendor.</span></span>
