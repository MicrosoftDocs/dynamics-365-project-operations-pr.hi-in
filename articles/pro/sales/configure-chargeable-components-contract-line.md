---
title: परियोजना-आधारित अनुबंध पंक्ति के प्रभार्य घटकों को कॉन्फ़िगर करें
description: यह विषय इस बारे में जानकारी देता है कि परियोजना संचालन में कैसे अनुबंध पंक्तियों को प्रभार्य घटकों से जोड़ना चाहिए.
author: rumant
manager: Annbe
ms.date: 10/08/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: ddada2cb412ba7370fb0a750325a84772937d8d0
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858475"
---
# <a name="configure-chargeable-components-of-a-project-based-contract-line"></a><span data-ttu-id="98d8b-103">परियोजना-आधारित अनुबंध पंक्ति के प्रभार्य घटकों को कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="98d8b-103">Configure chargeable components of a project-based contract line</span></span>

<span data-ttu-id="98d8b-104">लाइट तैनाती _**पर लागू होता है:** प्रोफार्मा इनवॉइस करने के लिए - डील, संसाधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations_</span><span class="sxs-lookup"><span data-stu-id="98d8b-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="98d8b-105">परियोजना-आधारित अनुबंध पंक्ति में *शामिल* घटक और *प्रभार्य* घटक होते हैं.</span><span class="sxs-lookup"><span data-stu-id="98d8b-105">A project-based contract line has *included* components and *chargeable* components.</span></span>

<span data-ttu-id="98d8b-106">शामिल घटक ऐसे घटक हैं जो निम्नलिखित हैं:</span><span class="sxs-lookup"><span data-stu-id="98d8b-106">Included components are components that are subject to:</span></span>

  - <span data-ttu-id="98d8b-107">बिल विधि और ग्राहक विभाजन</span><span class="sxs-lookup"><span data-stu-id="98d8b-107">Billing method and customer splits</span></span>
  - <span data-ttu-id="98d8b-108">सीमा से अधिक नहीं</span><span class="sxs-lookup"><span data-stu-id="98d8b-108">Not-to-exceed limits</span></span> 
  - <span data-ttu-id="98d8b-109">इनवॉइस आवृत्ति सेटिंग को परियोजना-आधारित अनुबंध पंक्ति पर परिभाषित किया जाता है</span><span class="sxs-lookup"><span data-stu-id="98d8b-109">Invoice frequency settings defined on the project-based contract line</span></span>

<span data-ttu-id="98d8b-110">सम्मिलित घटकों के उपसेट को **बिल प्रकार** क्षेत्र का उपयोग करते हुए प्रभार्य चिह्नित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-110">A subset of the included components can be marked as chargeable using the **Billing Type** field.</span></span> <span data-ttu-id="98d8b-111">**बिल प्रकार** क्षेत्र एक ऐसा विकल्प-सेट है, जो अनुबंध पंक्ति के सन्दर्भ में निम्नलिखित मूल्यों की अनुमति देता है:</span><span class="sxs-lookup"><span data-stu-id="98d8b-111">The **Billing Type** field is an option-set that allows the following values in the context of a contract line:</span></span>

  - <span data-ttu-id="98d8b-112">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-112">Chargeable</span></span>
  - <span data-ttu-id="98d8b-113">गैर प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-113">Non-chargeable</span></span>

<span data-ttu-id="98d8b-114">प्रभार्य घटकों को कार्य, भूमिका और लेन-देन श्रेणियों पर परिभाषित किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-114">Chargeable components can be defined on tasks, roles, and transaction categories.</span></span>

<span data-ttu-id="98d8b-115">प्रभार्य को किसी/एक अनुबंध पंक्ति के कार्यों पर परिभाषित किया जाता है और पंक्ति में शामिल सभी लेन-देन वर्गों पर लागू होता है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-115">Chargeability is defined on tasks for a project contract line and applies to all transaction classes included on the line.</span></span> <span data-ttu-id="98d8b-116">यदि किसी अनुबंध पंक्ति पर **सम्मिलित कार्य** फ़ील्ड को रिक्त छोड़ दिया जाए या **संपूर्ण परियोजना** पर सेट कर दिया जाए, तो **प्रभार्य कार्य** टैब उपलब्ध नहीं होगा.</span><span class="sxs-lookup"><span data-stu-id="98d8b-116">If the **Include Tasks** field on a contract line is blank or set to **Entire project**, the **Chargeable tasks** tab will not be available.</span></span>

<span data-ttu-id="98d8b-117">किसी परियोजना अनुबंध पंक्ति के लिए भूमिकाओं पर परिभाषित प्रभार्य केवल **समय** लेन-देन वर्ग पर लागू होता है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-117">Chargeability defined on roles for a project contract line only applies to the **Time** transaction class.</span></span> <span data-ttu-id="98d8b-118">यदि किसी अनुबंध पंक्ति पर **सम्मिलित समय** क्षेत्र को **नहीं** पर सेट किया जाता है, तो **प्रभार्य भूमिकाएं** टैब उपलब्ध नहीं होगा.</span><span class="sxs-lookup"><span data-stu-id="98d8b-118">If the **Include Time** field on a contract line is set to **No**, the **Chargeable roles** tab will not be available.</span></span>

<span data-ttu-id="98d8b-119">किसी परियोजना पंक्ति के लिए लेन-देन श्रेणी पर परिभाषित प्रभार्य केवल **व्यय** लेन-देन वर्ग पर लागू होगा.</span><span class="sxs-lookup"><span data-stu-id="98d8b-119">Chargeability defined on transaction categories for a project contract line only applies to the **Expense** transaction class.</span></span> <span data-ttu-id="98d8b-120">यदि **सम्मिलित खर्च** क्षेत्र को **नहीं** पर सेट किया जाता है, तो **प्रभार्य भूमिकाएं** टैब उपलब्ध नहीं होगा.</span><span class="sxs-lookup"><span data-stu-id="98d8b-120">If the **Include Expenses** field is set to **No**, the **Chargeable Categories** tab will not be available.</span></span>

### <a name="update-a-project-task-as-chargeable-or-non-chargeable"></a><span data-ttu-id="98d8b-121">एक/किसी परियोजना कार्य को प्रभार्य या गैर-प्रभार्य के रूप में अपडेट करें</span><span class="sxs-lookup"><span data-stu-id="98d8b-121">Update a project task as chargeable or non-chargeable</span></span>

<span data-ttu-id="98d8b-122">एक परियोजना कार्य निर्दिष्ट अनुबंध पंक्ति पर प्रभार्य या गैर-प्रभार्य हो सकता है, जो निम्नलिखित संभावित सेटअप को बनाता है:</span><span class="sxs-lookup"><span data-stu-id="98d8b-122">A project task can be chargeable or non-chargeable on a specific contract line, which makes the following setup possible:</span></span>

<span data-ttu-id="98d8b-123">यदि किसी/एक परियोजना-आधारित अनुबंध पंक्ति में **समय** और कोई निश्चित कार्य शामिल है, तो **T1** को प्रभार्य के रूप में इससे जोड़ा जाता है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-123">If a project-based contract line includes **Time** and a certain task, **T1** is associated to it as chargeable.</span></span> <span data-ttu-id="98d8b-124">यदि एक दूसरी अनुबंध पंक्ति है, जिसमें **खर्च** शामिल है, तो आप अनुबंध पंक्ति पर T1 कार्य को गैर-प्रभार्य के रूप में जोड़ सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="98d8b-124">If there is a second contract line that includes **Expense**, you can associate the T1 task on the contract line as non-chargeable.</span></span> <span data-ttu-id="98d8b-125">परिणाम यह है कि कार्य पर रिकॉर्ड/दर्ज किए गए सभी समय प्रभार्य और सभी खर्च गैर-प्रभार्य हैं.</span><span class="sxs-lookup"><span data-stu-id="98d8b-125">The result is that all of the time recorded on the task is chargeable and all expenses are non-chargeable.</span></span>

<span data-ttu-id="98d8b-126">किसी कार्य के बिलिंग प्रकार को अनुबंध पंक्ति के **प्रभार्य कार्य** टैब पर, अनुबंध पंक्ति के कार्य सबग्रिड पर **बिलिंग प्रकार** फ़ील्ड का अद्यतन करके कॉन्फ़िगर किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-126">A task's billing type can be configured on the **Chargeable Tasks** tab of the contract line by updating the **Billing Type** field on the contract line tasks subgrid.</span></span> <span data-ttu-id="98d8b-127">वैकल्पिक रूप से, आप परियोजना के कार्य के बिलिंग सेटअप के सबग्रिड पर **बिलिंग प्रकार** फ़ील्ड का अद्यतन कर सकते हैं, जो कार्य से जुड़ी अनुबंध पंकतियों को दिखाती है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-127">Alternatively, you can update the **Billing Type** field on the subgrid of the task Billing setup of a project that shows the contract lines associated to a task.</span></span>

### <a name="update-a-role-as-chargeable-or-non-chargeable"></a><span data-ttu-id="98d8b-128">प्रभार्य या गैर-प्रभार्य के रूप में भूमिका को अपडेट करें</span><span class="sxs-lookup"><span data-stu-id="98d8b-128">Update a role as chargeable or non-chargeable</span></span>

<span data-ttu-id="98d8b-129">किसी निर्दिष्ट अनुबंध पंक्ति पर एक भूमिका प्रभार्य या गैर- प्रभार्य हो सकती है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-129">A role can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="98d8b-130">किसी/एक भूमिका के बिलिंग प्रकार को अनुबंध पंक्ति के **प्रभार्य भूमिकाएं** टैब पर कॉन्फ़िगर किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-130">A role's billing type can be configured on the **Chargeable Roles** tab of a contract line.</span></span> <span data-ttu-id="98d8b-131">ऐसा करने के लिए, **बिलिंग प्रकार** फ़ील्ड का **प्रभार्य भूमिका** सबग्रिड पर अद्यतन करें.</span><span class="sxs-lookup"><span data-stu-id="98d8b-131">To do this, update the **Billing Type** field on the **Chargeable Roles** subgrid.</span></span>

### <a name="update-a-transaction-category-as-chargeable-or-non-chargeable"></a><span data-ttu-id="98d8b-132">प्रभार्य या गैर-प्रभार्य के रूप में लेन-देन श्रेणी को अपडेट करें</span><span class="sxs-lookup"><span data-stu-id="98d8b-132">Update a transaction category as chargeable or non-chargeable</span></span>

<span data-ttu-id="98d8b-133">किसी निर्दिष्ट अनुबंध पंक्ति पर किसी/एक लेन-देन श्रेणी को प्रभार्य या गैर-प्रभार्य किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-133">A transaction category can be chargeable or non-chargeable on a specific contract line.</span></span>

<span data-ttu-id="98d8b-134">किसी परियोजना-आधारित अनुबंध पंक्ति के **प्रभार्य श्रेणियां** टैब पर लेन-देन के बिलिंग प्रकार को कॉन्फ़िगर किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-134">A transaction's billing type can be configured on the **Chargeable Categories** tab of a project-based contract line.</span></span> <span data-ttu-id="98d8b-135">ऐसा करने के लिए, **बिलिंग प्रकार** फ़ील्ड का **प्रभार्य श्रेणी** सबग्रिड पर अद्यतन करें.</span><span class="sxs-lookup"><span data-stu-id="98d8b-135">To do this, update the **Billing Type** field on the **Chargeable Categories** subgrid.</span></span>

### <a name="resolve-chargeability"></a><span data-ttu-id="98d8b-136">प्रभार्य योग्य को सुलझाएं</span><span class="sxs-lookup"><span data-stu-id="98d8b-136">Resolve chargeability</span></span>

<span data-ttu-id="98d8b-137">समय के लिए बनाया गया अनुमान या वास्तविक केवल आदेय माना जाता है यदि:</span><span class="sxs-lookup"><span data-stu-id="98d8b-137">An estimate or actual created for time is only considered chargeable if:</span></span>

   - <span data-ttu-id="98d8b-138">**समय** अनुबंध पंक्ति में शामिल है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-138">**Time** is included on the contract line.</span></span>
   - <span data-ttu-id="98d8b-139">**भूमिका** को अनुबंध लाइन पर शुल्क लेने योग्य के रूप में कॉन्फ़िगर किया गया है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-139">**Role** is configured as chargeable on the contract line.</span></span>
   - <span data-ttu-id="98d8b-140">**शामिल कार्य** अनुबंध रेखा पर **चयनित कार्यों** के लिए सेट है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-140">**Included Tasks** is set to **Selected tasks** on the contract line.</span></span>
 
 <span data-ttu-id="98d8b-141">यदि ये दोनों चीजें सही हैं, तो कार्य को आदेय के रूप में कॉन्फ़िगर किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-141">If these three things are true, the task is configured as chargeable.</span></span> 

<span data-ttu-id="98d8b-142">व्यय के लिए बनाया गया अनुमान या वास्तविक केवल आदेय माना जाता है यदि:</span><span class="sxs-lookup"><span data-stu-id="98d8b-142">An estimate or actual created for expense is only considered chargeable if:</span></span>

   - <span data-ttu-id="98d8b-143">**व्यय** अनुबंध लाइन में शामिल है</span><span class="sxs-lookup"><span data-stu-id="98d8b-143">**Expense** is included on the contract line</span></span>
   - <span data-ttu-id="98d8b-144">**लेनदेन श्रेणी** को अनुबंध लाइन पर शुल्क लेने योग्य के रूप में कॉन्फ़िगर किया गया है</span><span class="sxs-lookup"><span data-stu-id="98d8b-144">**Transaction category** is configured as chargeable on the contract line</span></span>
   - <span data-ttu-id="98d8b-145">**शामिल कार्य** अनुबंध रेखा पर **चयनित कार्य** के लिए सेट है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-145">**Included Tasks** is set to **Selected task** on the contract line</span></span>
  
 <span data-ttu-id="98d8b-146">यदि ये दोनों चीजें सही हैं, तो **कार्य** को आदेय के रूप में कॉन्फ़िगर किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-146">If these three things are true, the **Task** is configured as chargeable.</span></span> 

<span data-ttu-id="98d8b-147">सामग्री के लिए बनाया गया अनुमान या वास्तविक केवल आदेय माना जाता है यदि:</span><span class="sxs-lookup"><span data-stu-id="98d8b-147">An estimate or actual created for material is only considered chargeable if:</span></span>

   - <span data-ttu-id="98d8b-148">**सामग्री** अनुबंध लाइन में शामिल है</span><span class="sxs-lookup"><span data-stu-id="98d8b-148">**Materials** is included on the contract line</span></span>
   - <span data-ttu-id="98d8b-149">**शामिल कार्य** अनुबंध रेखा पर **चयनित कार्यों** के लिए सेट है</span><span class="sxs-lookup"><span data-stu-id="98d8b-149">**Included Tasks** is set to **Selected tasks** on the contract line</span></span>

<span data-ttu-id="98d8b-150">यदि ये दोनों चीजें सही हैं, तो **कार्य** को आदेय के रूप में कॉन्फ़िगर किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="98d8b-150">If these two things are true, the **Task** is configured as chargeable.</span></span> 

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="98d8b-151">
                    <strong>समय शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-151">
                    <strong>Includes Time</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="98d8b-152">
                    <strong>व्यय शामिल करें</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-152">
                    <strong>Includes Expense</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="98d8b-153">
                    <strong>सामग्री शामिल है</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-153">
                    <strong>Includes Materials</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p><span data-ttu-id="98d8b-154">
                    <strong>शामिल कार्य</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-154">
                    <strong>Included Tasks</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="98d8b-155">
                    <strong>भूमिका</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-155">
                    <strong>Role</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="98d8b-156">
                    <strong>वर्ग</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-156">
                    <strong>Category</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="98d8b-157">
                    <strong>कार्य</strong>
                    <strong></strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-157">
                    <strong>Task</strong>
                    <strong></strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p><span data-ttu-id="98d8b-158">
                    <strong>चार्ज करने की क्षमता का प्रभाव</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-158">
                    <strong>Chargeability impact</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-159">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-159">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="98d8b-160">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-160">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="98d8b-161">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-161">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="98d8b-162">परियोजना संपूर्ण करें</span><span class="sxs-lookup"><span data-stu-id="98d8b-162">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-163">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-163">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-164">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-164">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-165">सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="98d8b-165">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="98d8b-166">वास्तविक समय पर बिलिंग: <strong>प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-166">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-167">वास्तविक खर्च पर बिलिंग प्रकार: <strong>प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-167">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-168">वास्तविक सामग्री पर बिलिंग प्रकार: <strong>प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-168">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-169">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-169">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="98d8b-170">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-170">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="98d8b-171">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-171">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="98d8b-172">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-172">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-173">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-173">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-174">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-174">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-175">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-175">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="98d8b-176">वास्तविक समय पर बिलिंग: <strong>प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-176">Billing on a time actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-177">वास्तविक खर्च पर बिलिंग प्रकार: <strong>प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-177">Billing type on expense actual: <strong>Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-178">वास्तविक सामग्री पर बिलिंग प्रकार: <strong>प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-178">Billing type on material actual: <strong>Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-179">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-179">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="98d8b-180">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-180">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="98d8b-181">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-181">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="98d8b-182">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-182">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="98d8b-183">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-183">
                    <strong>Non - Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-184">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-184">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-185">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-185">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="98d8b-186">वास्तविक समय पर बिलिंग: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-186">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-187">वास्तविक खर्च पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-187">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="98d8b-188">वास्तविक सामग्री पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-188">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-189">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-189">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="98d8b-190">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-190">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="98d8b-191">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-191">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="98d8b-192">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-192">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-193">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-193">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-194">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-194">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="98d8b-195">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-195">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="98d8b-196">वास्तविक समय पर बिलिंग: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-196">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-197">वास्तविक खर्च पर बिलिंग प्रकार: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-197">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-198">वास्तविक सामग्री पर बिलिंग प्रकार: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-198">Billing type on material actual: <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-199">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-199">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="98d8b-200">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-200">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="98d8b-201">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-201">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="98d8b-202">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-202">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="98d8b-203">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-203">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-204">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-204">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="98d8b-205">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-205">
                    <strong>Non- Chargeable</strong>
                </span></span></p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="98d8b-206">वास्तविक समय पर बिलिंग: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-206">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-207">वास्तविक खर्च पर बिलिंग प्रकार: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-207">Billing type on expense actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-208">वास्तविक सामग्री पर बिलिंग प्रकार: <strong> गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-208">Billing type on material actual: <strong> Non-Chargeable</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-209">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-209">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="98d8b-210">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-210">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="98d8b-211">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-211">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="98d8b-212">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-212">Selected tasks only</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="98d8b-213">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-213">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="98d8b-214">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-214">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-215">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-215">Chargeable</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="98d8b-216">वास्तविक समय पर बिलिंग: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-216">Billing on a time actual: <strong>Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-217">वास्तविक खर्च पर बिलिंग प्रकार: <strong> गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-217">Billing type on expense actual: <strong> Non-Chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-218">वास्तविक सामग्री पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-218">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="98d8b-219">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-219">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="98d8b-220">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-220">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="98d8b-221">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-221">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="98d8b-222">परियोजना संपूर्ण करें</span><span class="sxs-lookup"><span data-stu-id="98d8b-222">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-223">सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="98d8b-223">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="98d8b-224">
                    <strong>प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-224">
                    <strong>Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-225">सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="98d8b-225">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="98d8b-226">वास्तविक समय पर बिलिंग: <strong>उपलब्ध नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-226">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-227">वास्तविक खर्च पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-227">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="98d8b-228">वास्तविक सामग्री पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-228">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p><span data-ttu-id="98d8b-229">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-229">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="98d8b-230">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-230">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="98d8b-231">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-231">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="98d8b-232">परियोजना संपूर्ण करें</span><span class="sxs-lookup"><span data-stu-id="98d8b-232">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-233">सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="98d8b-233">Can't be set</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="98d8b-234">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-234">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-235">सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="98d8b-235">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="98d8b-236">वास्तविक समय पर बिलिंग: <strong>उपलब्ध नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-236">Billing on a time actual: <strong>Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-237">वास्तविक खर्च पर बिलिंग प्रकार: <strong> गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-237">Billing type on expense actual: <strong> Non-chargeable</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-238">वास्तविक सामग्री पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-238">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-239">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-239">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="98d8b-240">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-240">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="98d8b-241">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-241">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="98d8b-242">परियोजना संपूर्ण करें</span><span class="sxs-lookup"><span data-stu-id="98d8b-242">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-243">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-243">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-244">सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="98d8b-244">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-245">सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="98d8b-245">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="98d8b-246">वास्तविक समय पर बिलिंग: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-246">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="98d8b-247">वास्तविक खर्च पर बिलिंग प्रकार: <strong>उपलब्ध नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-247">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-248">वास्तविक सामग्री पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-248">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-249">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-249">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p><span data-ttu-id="98d8b-250">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-250">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="63" valign="top">
                <p>
<span data-ttu-id="98d8b-251">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-251">Yes</span></span> </p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="98d8b-252">परियोजना संपूर्ण करें</span><span class="sxs-lookup"><span data-stu-id="98d8b-252">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="98d8b-253">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-253">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-254">सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="98d8b-254">Can't be set</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-255">सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="98d8b-255">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="98d8b-256">वास्तविक समय पर बिलिंग: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-256">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-257">वास्तविक खर्च पर बिलिंग प्रकार: <strong>उपलब्ध नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-257">Billing type on expense actual:<strong> Not available</strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-258">वास्तविक सामग्री पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-258">Billing type on material actual: Chargeable</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-259">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-259">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="98d8b-260">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-260">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="98d8b-261">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-261">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="98d8b-262">परियोजना संपूर्ण करें</span><span class="sxs-lookup"><span data-stu-id="98d8b-262">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-263">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-263">Chargeable</span></span> </p>
            </td>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-264">प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-264">Chargeable</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-265">सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="98d8b-265">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="98d8b-266">वास्तविक समय पर बिलिंग: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-266">Billing on a time actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="98d8b-267">वास्तविक खर्च पर बिलिंग प्रकार: प्रभार्य</span><span class="sxs-lookup"><span data-stu-id="98d8b-267">Billing type on expense actual: Chargeable</span></span> </p>
                <p>
<span data-ttu-id="98d8b-268">वास्तविक सामग्री पर बिलिंग प्रकार: <strong>उपलब्ध नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-268">Billing type on material actual: <strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="70" valign="top">
                <p>
<span data-ttu-id="98d8b-269">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-269">Yes</span></span> </p>
            </td>
            <td width="78" valign="top">
                <p>
<span data-ttu-id="98d8b-270">हाँ</span><span class="sxs-lookup"><span data-stu-id="98d8b-270">Yes</span></span> </p>
            </td>
            <td width="63" valign="top">
                <p><span data-ttu-id="98d8b-271">
                    <strong>No</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-271">
                    <strong>No</strong>
                </span></span></p>
            </td>
            <td width="75" valign="top">
                <p>
<span data-ttu-id="98d8b-272">परियोजना संपूर्ण करें</span><span class="sxs-lookup"><span data-stu-id="98d8b-272">Entire Project</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="98d8b-273">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-273">
                    <strong>Non-Chargeable</strong>
                </span></span></p>
            </td>
            <td width="70" valign="top">
                <p><span data-ttu-id="98d8b-274">
                    <strong>गैर प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-274">
                    <strong>Non-chargeable</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="98d8b-275">सेट नहीं किया जा सकता</span><span class="sxs-lookup"><span data-stu-id="98d8b-275">Can't be set</span></span> </p>
            </td>
            <td width="350" valign="top">
                <p>
<span data-ttu-id="98d8b-276">वास्तविक समय पर बिलिंग: <strong>गैर-प्रभार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-276">Billing on a time actual: <strong>Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-277">वास्तविक खर्च पर बिलिंग प्रकार:<strong> गैर-प्रभार्य </strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-277">Billing type on expense actual:<strong> Non-chargeable </strong>
                </span></span></p>
                <p>
<span data-ttu-id="98d8b-278">वास्तविक सामग्री पर बिलिंग प्रकार:<strong>उपलब्ध नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="98d8b-278">Billing type on material actual:<strong> Not available</strong>
                </span></span></p>
            </td>
        </tr>
    </tbody>
</table>





[!INCLUDE[footer-include](../../includes/footer-banner.md)]
