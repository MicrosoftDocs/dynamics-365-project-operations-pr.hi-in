---
title: एक उद्धरण पंक्ति के प्रभार्य घटकों को कॉन्फ़िगर करें
description: यह विषय किसी परियोजना-आधारित उद्धरण पंक्ति पर प्रभार्य और गैर-प्रभार्य घटकों को सेट/स्थापित करने के बारे में जानकारी प्रदान करता है.
author: rumant
ms.date: 03/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: c933a3800aae72624dbcbe3f06df20e5981d74d4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003768"
---
# <a name="configure-the-chargeable-components-of-a-quote-line"></a><span data-ttu-id="b8381-103">एक कोट पंक्ति के सशुल्क घटकों को कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="b8381-103">Configure the chargeable components of a quote line</span></span> 

<span data-ttu-id="b8381-104">लाइट तैनाती _**पर लागू होता है:** प्रोफार्मा इनवॉइस करने के लिए - डील, संसाधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations_</span><span class="sxs-lookup"><span data-stu-id="b8381-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="b8381-105">एक/किसी परियोजना-आधारित उद्धरण पंक्ति में *सम्मिलित* घटक और *प्रभार्य* घटकों की अवधारणा होती है.</span><span class="sxs-lookup"><span data-stu-id="b8381-105">A project-based quote line has the concept of *included* components and *chargeable* components.</span></span>

<span data-ttu-id="b8381-106">शामिल घटकों के अधीन है:</span><span class="sxs-lookup"><span data-stu-id="b8381-106">Included components are subject to:</span></span>

  - <span data-ttu-id="b8381-107">बिल विधि और ग्राहक विभाजन</span><span class="sxs-lookup"><span data-stu-id="b8381-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="b8381-108">सीमा से अधिक नहीं</span><span class="sxs-lookup"><span data-stu-id="b8381-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="b8381-109">परियोजना-आधारित उद्धरण पंक्ति पर इनवॉइस आवृत्ति सेटिंग को परिभाषित किया जाता है</span><span class="sxs-lookup"><span data-stu-id="b8381-109">Invoice frequency settings defined on the project-based quote line</span></span>

<span data-ttu-id="b8381-110">सम्मिलित घटकों के उपसेट को **बिल प्रकार** क्षेत्र का उपयोग करते हुए प्रभार्य चिह्नित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="b8381-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="b8381-111">**बिलिंग प्रकार** क्षेत्र एक ऐसा विकल्प-सेट है, जो किसी उद्धरण पंक्ति के सन्दर्भ में निम्नलिखित मूल्यों की अनुमति देता है:</span><span class="sxs-lookup"><span data-stu-id="b8381-111">The **Billing Type** field is an option-set that allows the following values in the context of a quote line:</span></span>

  - <span data-ttu-id="b8381-112">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-112">Chargeable</span></span>
  - <span data-ttu-id="b8381-113">गैर प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-113">Non-chargeable</span></span>

<span data-ttu-id="b8381-114">प्रभार्य घटकों को कार्य, भूमिका और लेन-देन श्रेणियों पर परिभाषित किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b8381-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="b8381-115">किसी/एक उद्धरण पंक्ति के कार्यों पर प्रभार्य को परिभाषित किया जाता है और यह उस पंक्ति में शामिल सभी लेन-देन पर लागू होता है.</span><span class="sxs-lookup"><span data-stu-id="b8381-115">Chargeability is defined on the tasks for a quote line and applies to all transaction classes included on that line.</span></span> <span data-ttu-id="b8381-116">यदि **सम्मिलित कार्य** क्षेत्र को **संपूर्ण परियोजना** पर सेट/स्थापित किया जाता है या रिक्त छोड़ दिया जाता है, तो **प्रभार्य भूमिकाएं** टैब उपलब्ध नहीं होगा.</span><span class="sxs-lookup"><span data-stu-id="b8381-116">If the **Include Tasks** field is set to **Entire project** or left blank, the **Chargeable Tasks** tab isn't available.</span></span>

<span data-ttu-id="b8381-117">किसी/एक उद्धरण पंक्ति की भूमिकाओं पर प्रभार्य को परिभाषित किया जाता है और यह केवल **समय** लेन-देन वर्ग पर लागू होता है.</span><span class="sxs-lookup"><span data-stu-id="b8381-117">Chargeability is defined on roles for a quote line and only applies to the **Time** transaction class.</span></span> <span data-ttu-id="b8381-118">यदि किसी/एक परियोजना उद्धरण पंक्ति पर **समय को शामिल करें** क्षेत्र को **नहीं** पर सेट कर दिया जाता है, तो **प्रभार्य भूमिकाएं** टैब उपलब्ध नहीं होगा.</span><span class="sxs-lookup"><span data-stu-id="b8381-118">If the field, **Include Time** is set to **No** on a project quote line, the **Chargeable Roles** tab isn't available.</span></span>

<span data-ttu-id="b8381-119">किसी/एक उद्धरण पंक्ति के लिए लेन-देन श्रेणियों पर प्रभार्य को परिभाषित किया जाता है, और यह केवल **खर्च** लेन-देन वर्ग पर लागू होता है.</span><span class="sxs-lookup"><span data-stu-id="b8381-119">Chargeability is defined on transaction categories for a  quote line and only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="b8381-120">यदि किसी/एक परियोजना उद्धरण पंक्ति पर **खर्च को शामिल करें** क्षेत्र को **नहीं** पर सेट किया जाता है, तो **प्रभार्य श्रेणियां** टैब उपलब्ध नहीं होगा.</span><span class="sxs-lookup"><span data-stu-id="b8381-120">If the field, **Include Expenses** is set to **No** on a project quote line, the **Chargeable Categories** tab isn't available.</span></span>

### <a name="update-a-project-task-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="b8381-121">प्रभार्य या गैर-प्रभार्य के रूप में परियोजना कार्य को अपडेट करें</span><span class="sxs-lookup"><span data-stu-id="b8381-121">Update a project task to be chargeable or non-chargeable</span></span>

<span data-ttu-id="b8381-122">किसी निर्दिष्ट परियोजना-आधारित उद्धरण पंक्ति के सन्दर्भ में एक परियोजना कार्य को प्रभार्य या गैर- प्रभार्य किया जा सकता है, जो निम्नलिखित सेटअप को संभव बनाता है.</span><span class="sxs-lookup"><span data-stu-id="b8381-122">A project task can be chargeable or non-chargeable in the context of a specific project-based quote line, which makes the following setup possible.</span></span>

<span data-ttu-id="b8381-123">यदि किसी परियोजना-आधारित उद्धरण पंक्ति में **समय** और कार्य **T1** शामिल है, तो कार्य उद्धरण पंक्ति से प्रभार्य के रूप में संबद्ध है.</span><span class="sxs-lookup"><span data-stu-id="b8381-123">If a project-based quote line includes **Time** and the task **T1**, the task is associated to the quote line as chargeable.</span></span> <span data-ttu-id="b8381-124">यदि एक दूसरी उद्धरण पंक्ति है, जिसमें **खर्च** शामिल है, तो आप **T1** कार्य को उद्धरण पंक्ति पर गैर-प्रभार्य के रूप में जोड़ सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="b8381-124">If there is a second quote line that includes **Expenses**, you can associate the **T1** task on the quote line as non-chargeable.</span></span> <span data-ttu-id="b8381-125">परिणाम यह है कि कार्य पर रिकॉर्ड किए गए सभी समय प्रभार्य और कार्य पर रिकॉर्ड किए गए सभी खर्च गैर-प्रभार्य हैं.</span><span class="sxs-lookup"><span data-stu-id="b8381-125">The result is that all time recorded on the task is chargeable and all expenses recorded on the task are non-chargeable.</span></span>

<span data-ttu-id="b8381-126">**कोट पंक्ति कार्य** सब-ग्रिड पर **बिलिंग प्रकार** को अद्यतन करके परियोजना-आधारित कोट पंक्ति के **प्रभार्य कार्य** टैब पर कार्य के बिलिंग प्रकार को कॉन्फ़िगर किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b8381-126">A task's billing type can be configured on the **Chargeable Tasks** tab of a project-based quote line by updating the **Billing Type** field on the **Quote Line Tasks** subgrid.</span></span> <span data-ttu-id="b8381-127">वैकल्पिक रूप से, आप परियोजना कार्य के लिए बिलिंग प्रकार को उस परियोजना के कार्य बिलिंग सेटअप की सबग्रिड पर **बिलिंग प्रकार** फ़ील्ड में अद्यतन कर सकते हैं, जो दिखाती है कि कोट पंक्तियाँ कार्य से संबद्ध हैं.</span><span class="sxs-lookup"><span data-stu-id="b8381-127">Alternatively, you can update the billing type for a project task in the **Billing Type** field on the subgrid on the task billing setup of a project that shows the quote lines associated to a task.</span></span>

### <a name="update-a-role-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="b8381-128">प्रभार्य या गैर-प्रभार्य के रूप में भूमिका को अपडेट करें</span><span class="sxs-lookup"><span data-stu-id="b8381-128">Update a role to be chargeable or non-chargeable</span></span>

<span data-ttu-id="b8381-129">किसी निर्दिष्ट परियोजना-आधारित उद्धरण पंक्ति के सन्दर्भ में एक भूमिका प्रभार्य या गैर- प्रभार्य हो सकती है.</span><span class="sxs-lookup"><span data-stu-id="b8381-129">A role can be chargeable or non-chargeable in the context of a specific project-based quote line.</span></span>

<span data-ttu-id="b8381-130">**प्रभार्य भूमिका** टैब पर **बिलिंग प्रकार** को अद्यतन करके **प्रभार्य भूमिकाएँ** टैब पर भूमिका के बिलिंग प्रकार को कॉन्फ़िगर किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b8381-130">A role's billing type can be configured on the **Chargeable Roles** tab of a quote line by updating the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-to-be-chargeable-or-non-chargeable"></a><span data-ttu-id="b8381-131">लेन-देन श्रेणी को प्रभार्य या गैर-प्रभार्य के रूप में अपडेट करें</span><span class="sxs-lookup"><span data-stu-id="b8381-131">Update a transaction category to be chargeable or non-chargeable</span></span>

<span data-ttu-id="b8381-132">एक/किसी निर्दिष्ट उद्धरण पंक्ति पर एक लेन-देन श्रेणी को प्रभार्य या गैर-प्रभार्य किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b8381-132">A transaction category can be chargeable or non-chargeable on a specific quote line.</span></span>

<span data-ttu-id="b8381-133">**प्रभार्य श्रेणियाँ** सबग्रिड पर **बिलिंग प्रकार** फ़ील्ड को अद्यतन करके ट्रांज़ैक्शन के बिलिंग प्रकार को कोट पंक्ति के **प्रभार्य श्रेणियाँ** टैब पर कॉन्फ़िगर किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b8381-133">A transaction's billing type can be configured on the **Chargeable Categories** tab of a quote line by updating the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="b8381-134">प्रभार्य योग्य को सुलझाएं</span><span class="sxs-lookup"><span data-stu-id="b8381-134">Resolve chargeability</span></span>
<span data-ttu-id="b8381-135">समय के लिए बनाया गया अनुमान या एक्चुअल (वास्तविक आंकड़ा) केवल तभी चार्जेबल माना जाएगा यदि:</span><span class="sxs-lookup"><span data-stu-id="b8381-135">An estimate or actual created for time will only be considered chargeable if:</span></span>

   - <span data-ttu-id="b8381-136">**समय** कोट लाइन में शामिल है.</span><span class="sxs-lookup"><span data-stu-id="b8381-136">**Time** is included on the quote line.</span></span>
   - <span data-ttu-id="b8381-137">**भूमिका** को कोट लाइन पर चार्जेबल के रूप में कॉन्फ़िगर किया गया है.</span><span class="sxs-lookup"><span data-stu-id="b8381-137">**Role** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="b8381-138">**शामिल कार्य** कोट रेखा पर **चयनित कार्यों** के लिए सेट है.</span><span class="sxs-lookup"><span data-stu-id="b8381-138">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span> 

<span data-ttu-id="b8381-139">यदि ये तीन बातें सच हैं, तो **टास्क** को भी चार्जेबल के रूप में कॉन्फ़िगर किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="b8381-139">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="b8381-140">व्यय के लिए बनाया गया अनुमान या वास्तविक केवल आदेय माना जाता है यदि:</span><span class="sxs-lookup"><span data-stu-id="b8381-140">An estimate or actual created for expense is only considered chargeable if:</span></span> 

   - <span data-ttu-id="b8381-141">**व्यय** कोट लाइन में शामिल है.</span><span class="sxs-lookup"><span data-stu-id="b8381-141">**Expense** is included on the quote line.</span></span>
   - <span data-ttu-id="b8381-142">**लेनदेन श्रेणी** को अनुबंध लाइन पर शुल्क लेने योग्य के रूप में कॉन्फ़िगर किया गया है.</span><span class="sxs-lookup"><span data-stu-id="b8381-142">**Transaction category** is configured as chargeable on the quote line.</span></span>
   - <span data-ttu-id="b8381-143">**शामिल कार्य** कोट रेखा पर **चयनित कार्यों** के लिए सेट है.</span><span class="sxs-lookup"><span data-stu-id="b8381-143">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="b8381-144">यदि ये तीन बातें सच हैं, तो **टास्क** को भी चार्जेबल के रूप में कॉन्फ़िगर किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="b8381-144">If these three things are true, the **Task** is also configured as chargeable.</span></span> 

<span data-ttu-id="b8381-145">मटिरियल के लिए बनाया गया अनुमान या एक्चुअल (वास्तविक आंकड़ा) केवल तभी चार्जेबल माना जाएगा यदि:</span><span class="sxs-lookup"><span data-stu-id="b8381-145">An estimate or actual created for material will only be considered chargeable if:</span></span>

   - <span data-ttu-id="b8381-146">**सामग्रियाँ** कोट लाइन में शामिल है.</span><span class="sxs-lookup"><span data-stu-id="b8381-146">**Materials** is included on the quote line.</span></span>
   - <span data-ttu-id="b8381-147">**शामिल कार्य** कोट रेखा पर **चयनित कार्यों** के लिए सेट है.</span><span class="sxs-lookup"><span data-stu-id="b8381-147">**Included Tasks** is set to **Selected tasks** on the quote line.</span></span>

<span data-ttu-id="b8381-148">यदि ये दोनों चीजें सच हैं, तो **टास्क** को भी चार्जेबल के रूप में कॉन्फ़िगर किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="b8381-148">If these two things are true, the **Task** should also be configured as chargeable.</span></span> 


<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="b8381-149">
                    <strong>समय शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-149">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="b8381-150">
                    <strong>व्यय शामिल करें</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-150">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="b8381-151">
                    <strong>सामग्री शामिल है</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-151">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="b8381-152">
                    <strong>शामिल कार्य</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-152">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b8381-153">
                    <strong>भूमिका</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-153">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="b8381-154">
                    <strong>वर्ग</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-154">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b8381-155">
                    <strong>कार्य</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-155">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="b8381-156">
                    <strong>चार्ज करने की क्षमता का प्रभाव</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-156">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-157">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-157">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b8381-158">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-158">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b8381-159">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-159">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b8381-160">परियोजना संपूर्ण करें</span><span class="sxs-lookup"><span data-stu-id="b8381-160">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-161">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-161">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-162">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-162">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-163"> सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="b8381-163">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b8381-164">वास्तविक समय पर बिलिंग: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-164">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="b8381-165">वास्तविक खर्च पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-165">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="b8381-166">वास्तविक सामग्री पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-166">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-167">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-167">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b8381-168">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-168">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b8381-169">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-169">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b8381-170">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-170">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-171">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-171">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-172">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-172">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-173">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-173">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b8381-174">वास्तविक समय पर बिलिंग: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-174">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="b8381-175">वास्तविक खर्च पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-175">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="b8381-176">वास्तविक सामग्री पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-176">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-177">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-177">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b8381-178">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-178">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b8381-179">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-179">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b8381-180">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-180">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b8381-181">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-181">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-182">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-182">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-183">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-183">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b8381-184">वास्तविक समय पर बिलिंग: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-184">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b8381-185">वास्तविक खर्च पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-185">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="b8381-186">वास्तविक सामग्री पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-186">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-187">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-187">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b8381-188">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-188">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b8381-189">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-189">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b8381-190">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-190">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-191">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-191">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-192">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-192">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b8381-193">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-193">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b8381-194">वास्तविक समय पर बिलिंग: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-194">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b8381-195">वास्तविक खर्च पर बिलिंग प्रकार: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-195">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b8381-196">वास्तविक सामग्री पर बिलिंग प्रकार: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-196">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-197">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-197">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b8381-198">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-198">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b8381-199">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-199">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b8381-200">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-200">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b8381-201">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-201">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-202">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-202">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b8381-203">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-203">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b8381-204">वास्तविक समय पर बिलिंग: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-204">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b8381-205">वास्तविक खर्च पर बिलिंग प्रकार: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-205">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b8381-206">वास्तविक सामग्री पर बिलिंग प्रकार: <strong> गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-206">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-207">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-207">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b8381-208">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-208">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b8381-209">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-209">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b8381-210">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-210">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b8381-211">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-211">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="b8381-212">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-212">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-213">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-213">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b8381-214">वास्तविक समय पर बिलिंग: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-214">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b8381-215">वास्तविक खर्च पर बिलिंग प्रकार: <strong> गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-215">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b8381-216">वास्तविक सामग्री पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-216">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="b8381-217">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-217">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b8381-218">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-218">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b8381-219">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-219">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b8381-220">परियोजना संपूर्ण करें</span><span class="sxs-lookup"><span data-stu-id="b8381-220">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-221"> सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="b8381-221">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="b8381-222">
                    <strong>प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-222">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-223"> सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="b8381-223">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b8381-224">वास्तविक समय पर बिलिंग: <strong>उपलब्ध नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-224">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b8381-225">वास्तविक खर्च पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-225">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="b8381-226">वास्तविक सामग्री पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-226">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="b8381-227">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-227">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b8381-228">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-228">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b8381-229">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-229">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b8381-230">परियोजना संपूर्ण करें</span><span class="sxs-lookup"><span data-stu-id="b8381-230">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-231"> सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="b8381-231">Cannot be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="b8381-232">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-232">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-233"> सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="b8381-233">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b8381-234">वास्तविक समय पर बिलिंग: <strong>उपलब्ध नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-234">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b8381-235">वास्तविक खर्च पर बिलिंग प्रकार: <strong> गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-235">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b8381-236">वास्तविक सामग्री पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-236">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-237">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-237">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="b8381-238">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-238">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b8381-239">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-239">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b8381-240">परियोजना संपूर्ण करें</span><span class="sxs-lookup"><span data-stu-id="b8381-240">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-241">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-241">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-242"> सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="b8381-242">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-243"> सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="b8381-243">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b8381-244">वास्तविक समय पर बिलिंग: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-244">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="b8381-245">वास्तविक खर्च पर बिलिंग प्रकार: <strong>उपलब्ध नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-245">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b8381-246">वास्तविक सामग्री पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-246">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-247">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-247">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="b8381-248">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-248">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="b8381-249">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-249">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b8381-250">परियोजना संपूर्ण करें</span><span class="sxs-lookup"><span data-stu-id="b8381-250">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b8381-251">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-251">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-252"> सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="b8381-252">Cannot be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-253"> सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="b8381-253">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b8381-254">वास्तविक समय पर बिलिंग: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-254">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="b8381-255">वास्तविक खर्च पर बिलिंग प्रकार: <strong>उपलब्ध नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-255">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="b8381-256">वास्तविक सामग्री पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-256">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-257">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-257">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b8381-258">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-258">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="b8381-259">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-259">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b8381-260">परियोजना संपूर्ण करें</span><span class="sxs-lookup"><span data-stu-id="b8381-260">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-261">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-261">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-262">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-262">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-263"> सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="b8381-263">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b8381-264">वास्तविक समय पर बिलिंग: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-264">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="b8381-265">वास्तविक खर्च पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="b8381-265">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="b8381-266">वास्तविक सामग्री पर बिलिंग प्रकार: <strong>उपलब्ध नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-266">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="b8381-267">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-267">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="b8381-268">हाँ</span><span class="sxs-lookup"><span data-stu-id="b8381-268">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="b8381-269">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-269">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="b8381-270">परियोजना संपूर्ण करें</span><span class="sxs-lookup"><span data-stu-id="b8381-270">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="b8381-271">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-271">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="b8381-272">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-272">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="b8381-273"> सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="b8381-273">Cannot be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="b8381-274">वास्तविक समय पर बिलिंग: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-274">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="b8381-275">वास्तविक खर्च पर बिलिंग प्रकार:<strong> गैर-प्रभार्य </strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-275">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="b8381-276">वास्तविक सामग्री पर बिलिंग प्रकार:<strong>उपलब्ध नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="b8381-276">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../../includes/footer-banner.md)]
