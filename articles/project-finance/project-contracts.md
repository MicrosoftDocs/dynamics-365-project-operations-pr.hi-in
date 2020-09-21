---
title: परियोजना अनुबंध
description: यह विषय उन परियोजना अनुबंधों का उदाहरण प्रदान करता है जिन्हें आप विभिन्न प्रकार की परियोजनाओं और वित्तपोषण स्रोतों के लिए बना सकते हैं, और आप कैसे अनुबंधों का प्रबंधन कर सकते हैं और परियोजना ग्राहकों को इंवॉयस दे सकते हैं.
author: KimANelson
manager: AnnBe
ms.date: 11/03/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectContractsListPage, ProjProjectsListPage
audience: Application User, IT Pro
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 23561
ms.assetid: bfd18d9b-d9a6-4e21-bc95-bf4af45f617f
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 854ddfe6db93b7e93a4ee640268a9c8f254f24e7
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3752046"
---
# <a name="project-contracts"></a><span data-ttu-id="cf194-103">परियोजना अनुबंध</span><span class="sxs-lookup"><span data-stu-id="cf194-103">Project contracts</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="cf194-104">यह लेख परियोजना अनुबंधों का उदाहरण प्रदान करता है जिन्हें आप विभिन्न प्रकार की परियोजनाओं और वित्तपोषण स्रोतों के लिए बना सकते हैं, और आप कैसे अनुबंधों का प्रबंधन कर सकते हैं और परियोजना ग्राहकों को इंवॉयस दे सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-104">This article provides examples of the project contracts that you can create for various types of projects and funding sources, and how you can manage contracts and invoice project customers.</span></span>

<span data-ttu-id="cf194-105">परियोजना अनुबंध के लिए आपके द्वारा बनाई गई परियोजना का प्रकार उस तरीके को निर्धारित करता है, जिसका इस्तेमाल परियोजना ग्राहकों की इनवॉइस बनाने के लिए होता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-105">The type of project that you create for a project contract determines the method that is used to invoice project customers.</span></span> <span data-ttu-id="cf194-106">आप एक परियोजना अनुबंध और संबंधित परियोजना परिवर्तित कर सकते हैं, लेकिन आप परियोजना के प्रकार को परिवर्तित नहीं कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-106">You can change a project contract and the related project, but you can't change the project type.</span></span> 

<span data-ttu-id="cf194-107">एक परियोजना अनुबंध का उपयोग करके, आप एक ही समय में एक या अधिक परियोजनाओं का इंवॉयस बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-107">By using a project contract, you can invoice one or more projects at the same time.</span></span> <span data-ttu-id="cf194-108">परियोजना अनुबंध परियोजना संरचना में हर उपपरियोजना के लिए एक सुसंगत इंवॉयसिंग प्रक्रिया की गारंटी देने में भी मदद करता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-108">The project contract also helps guarantee a consistent invoicing procedure for every subproject in a project structure.</span></span> 

<span data-ttu-id="cf194-109">हर परियोजना जिसका इंवॉयस बनाया जाएगा एक परियोजना अनुबंध के साथ जुड़ा होना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="cf194-109">Every project that will be invoiced must be associated with a project contract.</span></span> <span data-ttu-id="cf194-110">एक परियोजना अनुबंध के लिए सेटिंग्स उन सभी परियोजनाओं और उपपरियोजनाओं पर लागू होती हैं जो उस परियोजना अनुबंध से जुड़ी होती हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-110">The settings for a project contract apply to all projects and subprojects that are associated with that project contract.</span></span> 

<span data-ttu-id="cf194-111">एक परियोजना अनुबंध वित्तपोषण के एक या एक से अधिक स्रोतों को निर्दिष्ट कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-111">A project contract can specify one or more sources of funding.</span></span> <span data-ttu-id="cf194-112">अत:, आप बिलिंग को कई वित्तपोषकों के बीच विभाजित कर सकते हैं, वित्तपोषण की सीमा निर्धारित कर सकते हैं ताकि वित्तपोषण के स्रोतों को एक निर्दिष्ट राशि से अधिक बिल न दिया जा सके, और खर्च वसूलने के लिए वित्तपोषण के नियमों को कॉन्फ़िगर कर सकें.</span><span class="sxs-lookup"><span data-stu-id="cf194-112">Therefore, you can split the billing among multiple funders, set up funding limits so that funding sources are not billed more than a specified amount, and configure funding rules for charging expenditures.</span></span>

## <a name="funding-for-project-contracts"></a><span data-ttu-id="cf194-113">परियोजना अनुबंधों के लिए धन</span><span class="sxs-lookup"><span data-stu-id="cf194-113">Funding for project contracts</span></span>
<span data-ttu-id="cf194-114">कुछ परियोजना अनुबंध निर्दिष्ट करते हैं कि कई पक्ष परियोजना लागत के वित्तपोषण की जिम्मेदारी साझा करती हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-114">Some project contracts specify that multiple parties share the responsibility for funding the project costs.</span></span> <span data-ttu-id="cf194-115">यहाँ कुछ उदाहरण दिए गए हैं:</span><span class="sxs-lookup"><span data-stu-id="cf194-115">Here are some examples:</span></span>

-   <span data-ttu-id="cf194-116">एक बड़ा ग्राहक जिसमें कई डिवीजन हैं, अनुरोध करते हैं कि किसी परियोजना का वित्तपोषण डिवीजन के अनुसार विभाजित हो.</span><span class="sxs-lookup"><span data-stu-id="cf194-116">A large customer that has multiple divisions requests that funding of a project be split by division.</span></span>
-   <span data-ttu-id="cf194-117">आपकी कंपनी किसी बाहरी संगठन के साथ किसी बड़ी परियोजना की लागत साझा करती है.</span><span class="sxs-lookup"><span data-stu-id="cf194-117">Your company shares the costs of a large project with an external organization.</span></span>
-   <span data-ttu-id="cf194-118">एक सड़क परियोजना दो नगर पालिकाओं द्वारा सह-वित्तपोषित है.</span><span class="sxs-lookup"><span data-stu-id="cf194-118">A  road project is co-funded by two municipalities.</span></span>
-   <span data-ttu-id="cf194-119">एक पुल परियोजना एक सरकारी अनुदान और एक निजी निगम द्वारा वित्तपोषित है.</span><span class="sxs-lookup"><span data-stu-id="cf194-119">A bridge project is funded by a government grant and a private corporation.</span></span>

<span data-ttu-id="cf194-120">Dynamics 365 Finance में, आप एक ही लेनदेन के लिए बिलिंग को विभाजित कर सकते हैं या कई ग्राहकों, अनुदानों या संगठनों के बीच एक पूरी परियोजना के लिए बिलिंग को विभाजित कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-120">In Dynamics 365 Finance, you can split the billing for a single transaction or an entire project among multiple customers, grants, or organizations.</span></span> 

<span data-ttu-id="cf194-121">जिन परियोजनाओं में कई वित्तपोषक हैं, उन सभी पक्षों को जो एक उन्नत वित्तपोषण परियोजना के वित्तपोषण में योगदान देते हैं, उन्हें वित्तपोषण स्रोत कहा जाता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-121">In projects that have multiple funders, all parties that contribute to the funding of an advanced funding project are called funding sources.</span></span> <span data-ttu-id="cf194-122">एक ग्राहक, संगठन या अनुदान को वित्तपोषण स्रोत के रूप में परिभाषित करने के बाद, इसे एक या अधिक वित्तपोषण नियमों को सौंपा जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-122">After a customer, organization, or grant is defined as a funding source, it can be assigned to one or more funding rules.</span></span> <span data-ttu-id="cf194-123">वित्तपोषण नियमों में मानदंड होते हैं जो यह निर्धारित करते हैं कि किसी परियोजना के लिए विभिन्न वित्तपोषण स्रोतों को शुल्क कैसे आवंटित किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-123">Funding rules contain the criteria that determines how charges are allocated to the various funding sources for a project.</span></span> 

<span data-ttu-id="cf194-124">क्योंकि स्टॉक किए गए आइटम, जैसे कि वे जो खरीद मांग और खरीद आदेश पर दिखाई देते हैं, विभाजित नहीं किए जा सकते हैं, लागत राशि को वितरण के समय कई वित्तपोषण स्रोतों के बीच विभाजित नहीं किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-124">Because stocked items, such as those that appear on purchase requisitions and purchase orders, can't be split, the cost amount can't be split among multiple funding sources at the time of distribution.</span></span> <span data-ttu-id="cf194-125">इसलिए,जब तक इन्वेंट्री इश्यू पोस्ट नहीं किया जाता तब तक वित्तपोषण के स्रोत का मान 0 (शून्य) रहता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-125">Therefore, the funding source value remains 0 (zero) until the inventory issue is posted.</span></span> <span data-ttu-id="cf194-126">जब इन्वेंट्री इश्यू पोस्ट किया जाता है, तो लागत राशि परियोजना के लिए खाता वितरण नियमों के अनुसार वितरित की जाती है.</span><span class="sxs-lookup"><span data-stu-id="cf194-126">When the inventory issue is posted, the cost amount is distributed according to the account distribution rules for the project.</span></span>

<span data-ttu-id="cf194-127">यहां कुछ कदम दिए गए हैं जिन्हें आप कई वित्तपोषण स्रोतों के बीच बिलिंग को विभाजित करना आसान बनाने के लिए ले सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="cf194-127">Here are some steps that you can take to make it easier to split the billing among multiple funding sources:</span></span>

-   <span data-ttu-id="cf194-128">निर्दिष्ट करें कि किसी परियोजना के लिए दर्ज किए गए सभी लेनदेन परियोजना अनुबंध के रूप में समान बिक्री मुद्रा का उपयोग करते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-128">Specify that all transactions that are entered for a project use the same sales currency as the project contract.</span></span>
-   <span data-ttu-id="cf194-129">वित्तपोषण की सीमाएं सेट करें, ताकि किसी वित्तपोषण स्रोत का किसी परियोजना की ओर किसी निर्दिष्ट राशि से अधिक इंवॉयस न किया जा सके.</span><span class="sxs-lookup"><span data-stu-id="cf194-129">Set up funding limits, so that a funding source isn't invoiced more than a specified amount toward a project.</span></span>
-   <span data-ttu-id="cf194-130">प्रत्येक कार्यकर्ता, आइटम, श्रेणी, श्रेणी समूह और लेनदेन के प्रकार (या सभी लेनदेन के प्रकारों के लिए) के लिए वित्तपोषण के नियमों और वित्तपोषण की सीमाओं को कॉन्फ़िगर करें.</span><span class="sxs-lookup"><span data-stu-id="cf194-130">Configure funding rules and funding limits for each worker, item, category, category group, and transaction type (or for all transaction types).</span></span>
-   <span data-ttu-id="cf194-131">प्रत्येक वित्तपोषण के नियम मान्य होने पर अवधि को परिभाषित करने के लिए वैकल्पिक शुरुआत और अंत तिथियों का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="cf194-131">Select optional start and end dates to define the period when each funding rule is valid.</span></span>
-   <span data-ttu-id="cf194-132">प्रतिशत को निर्दिष्ट करें जिसके लिए प्रत्येक वित्तपोषण के स्रोत जिम्मेदार हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-132">Specify the percentage that each funding source is responsible for.</span></span>
-   <span data-ttu-id="cf194-133">निर्दिष्ट करें कि कौन सा वित्तपोषण का स्रोत वित्तपोषण के आवंटन की गणना के कारण होने वाले मतभेदों को पूर्ण करने के लिए जिम्मेदार है.</span><span class="sxs-lookup"><span data-stu-id="cf194-133">Specify which funding source is responsible for rounding differences that are caused by funding allocation calculations.</span></span>
-   <span data-ttu-id="cf194-134">ऐसे नियम सेट करें जो यह निर्धारित करते हैं कि बाहरी ग्राहकों को परियोजना लागत कैसे इंवॉयस की जाती है और आंतरिक संगठनों से कैसे शुल्क लिया जाता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-134">Set up rules that determine how project costs are invoiced to external customers and charged to internal organizations.</span></span>
-   <span data-ttu-id="cf194-135">जब तक अतिरिक्त धन प्राप्त नहीं किया जा सकता है, तब तक ऑन-होल्ड वित्तपोषण खाते में लेनदेन रिकॉर्ड करें, या जब तक आप आंतरिक रूप से लागत वहन करने का निर्णय नहीं लेते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-135">Record transactions in an on-hold funding account until additional funding can be obtained, or until you decide to bear the costs internally.</span></span>

<span data-ttu-id="cf194-136">यह निर्धारित करने के लिए कि किस कर समूह को लेनदेन के साथ संबद्ध करना है, परियोजना को कर समूह के असाइनमेंट के लिए खोजा जाता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-136">To determine which tax group to associate with a transaction, the project is searched for a tax group assignment.</span></span> <span data-ttu-id="cf194-137">यदि परियोजना स्तर पर किसी कर समूह का असाइनमेंट नहीं किया गया है, तो परियोजना अनुबंध को खोजा जाता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-137">If no tax group assignment has been made at the project level, the project contract is searched.</span></span>

### <a name="example-multiple-funding-sources-simple"></a><span data-ttu-id="cf194-138">उदाहरण: कई वित्तपोषण के स्रोत (सरल)</span><span class="sxs-lookup"><span data-stu-id="cf194-138">Example: Multiple funding sources (simple)</span></span>

<span data-ttu-id="cf194-139">निम्नलिखित तालिका कई वित्तपोषण स्रोतों के बीच वित्तपोषण आवंटन के प्रबंधन के लिए परिदृश्य प्रदान करती है.</span><span class="sxs-lookup"><span data-stu-id="cf194-139">The following table provides scenarios for managing funding allocation among multiple funding sources.</span></span> <span data-ttu-id="cf194-140">ये परिदृश्य निम्नलिखित अवधारणाओं पर आधारित हैं:</span><span class="sxs-lookup"><span data-stu-id="cf194-140">These scenarios are based on the following assumptions:</span></span>

-   <span data-ttu-id="cf194-141">अन्य वित्तपोषण नियम मानदंडों को लागू करने से पहले प्राथमिकता सेटिंग्स को पूंजी के आवंटन में प्रतिनिधित्व दिया जाता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-141">Priority settings are factored into the allocation of funds before other funding rule criteria are applied.</span></span>
-   <span data-ttu-id="cf194-142">जब वित्तपोषण नियम मान्य होती है तब अवधि को परिभाषित करने के लिए कोई तिथि सीमा निर्दिष्ट नहीं की गई है.</span><span class="sxs-lookup"><span data-stu-id="cf194-142">No date range has been specified to define the period d when the funding rule is valid.</span></span>

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="cf194-143"><strong>परिदृश्य</strong></span><span class="sxs-lookup"><span data-stu-id="cf194-143"><strong>Scenario</strong></span></span></td>
<td><span data-ttu-id="cf194-144"><strong>वित्तपोषण का स्रोत</strong></span><span class="sxs-lookup"><span data-stu-id="cf194-144"><strong>Funding source</strong></span></span></td>
<td><span data-ttu-id="cf194-145"><strong>आवंटन प्रतिशत</strong></span><span class="sxs-lookup"><span data-stu-id="cf194-145"><strong>Allocation percentage</strong></span></span></td>
<td><span data-ttu-id="cf194-146"><strong>आवंटन प्राथमिकता </strong></span><span class="sxs-lookup"><span data-stu-id="cf194-146"><strong>Allocation priority</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cf194-147">आप तब तक एक वित्तपोषण के स्रोत के लिए लागत आवंटित करना चाहते है जब तक इसकी पूंजी समाप्त नहीं हो गई हो, तब तक एक दूसरे वित्तपोषण के स्रोत के लिए लागत आवंटित करें जब तक इसकी पूंजी समाप्त नहीं हो गई हो, और अंतत: एक तीसरे वित्तपोषण के स्रोत के लिए शेष लागत आवंटित करें.</span><span class="sxs-lookup"><span data-stu-id="cf194-147">You want to allocate costs to one funding source until its funds are exhausted, allocate costs to a second funding source until its funds are exhausted, and finally allocate the remaining costs to a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="cf194-148">वित्तपोषण　का स्रोत　1</span><span class="sxs-lookup"><span data-stu-id="cf194-148">Funding　source　1</span></span></li>
<li><span data-ttu-id="cf194-149">वित्तपोषण　का स्रोत　2</span><span class="sxs-lookup"><span data-stu-id="cf194-149">Funding　source　2</span></span></li>
<li><span data-ttu-id="cf194-150">वित्तपोषण　का स्रोत　3</span><span class="sxs-lookup"><span data-stu-id="cf194-150">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="cf194-151">100%</span><span class="sxs-lookup"><span data-stu-id="cf194-151">100%</span></span></li>
<li><span data-ttu-id="cf194-152">100%</span><span class="sxs-lookup"><span data-stu-id="cf194-152">100%</span></span></li>
<li><span data-ttu-id="cf194-153">100%</span><span class="sxs-lookup"><span data-stu-id="cf194-153">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="cf194-154">1</span><span class="sxs-lookup"><span data-stu-id="cf194-154">1</span></span></li>
<li><span data-ttu-id="cf194-155">2</span><span class="sxs-lookup"><span data-stu-id="cf194-155">2</span></span></li>
<li><span data-ttu-id="cf194-156">3</span><span class="sxs-lookup"><span data-stu-id="cf194-156">3</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cf194-157">आप एक वित्तपोषण के स्रोत के लिए लागत का 75 प्रतिशत और एक दूसरे वित्तपोषण के स्रोत के लिए 25 प्रतिशत आवंटित करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-157">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="cf194-158">जब उन वित्तपोषण के स्रोतों में से कोई एक समाप्त हो जाता है, तो आप एक तीसरे वित्तपोषण के स्रोत से शेष लागत का भुगतान करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-158">When either of those funding sources is exhausted, you want to pay the remaining costs from a third funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="cf194-159">वित्तपोषण　का स्रोत　1</span><span class="sxs-lookup"><span data-stu-id="cf194-159">Funding　source　1</span></span></li>
<li><span data-ttu-id="cf194-160">वित्तपोषण　का स्रोत　2</span><span class="sxs-lookup"><span data-stu-id="cf194-160">Funding　source　2</span></span></li>
<li><span data-ttu-id="cf194-161">वित्तपोषण　का स्रोत　3</span><span class="sxs-lookup"><span data-stu-id="cf194-161">Funding　source　3</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="cf194-162">75%</span><span class="sxs-lookup"><span data-stu-id="cf194-162">75%</span></span></li>
<li><span data-ttu-id="cf194-163">25%</span><span class="sxs-lookup"><span data-stu-id="cf194-163">25%</span></span></li>
<li><span data-ttu-id="cf194-164">100%</span><span class="sxs-lookup"><span data-stu-id="cf194-164">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="cf194-165">1</span><span class="sxs-lookup"><span data-stu-id="cf194-165">1</span></span></li>
<li><span data-ttu-id="cf194-166">1</span><span class="sxs-lookup"><span data-stu-id="cf194-166">1</span></span></li>
<li><span data-ttu-id="cf194-167">2</span><span class="sxs-lookup"><span data-stu-id="cf194-167">2</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cf194-168">आप एक वित्तपोषण के स्रोत के लिए लागत का 75 प्रतिशत और एक दूसरे वित्तपोषण के स्रोत के लिए 25 प्रतिशत आवंटित करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-168">You want to allocate 75 percent of costs to one funding source and 25 percent to a second funding source.</span></span> <span data-ttu-id="cf194-169">जब उन वित्तपोषण के स्रोतों में से कोई एक समाप्त हो जाता है, तो आप एक तीसरे वित्तपोषण के स्रोत और एक चौथे वित्तपोषण के स्रोत के बीच शेष लागत विभाजित करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-169">When either of those funding sources is exhausted, you want to split the remaining costs between a third funding source and a fourth funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="cf194-170">वित्तपोषण　का स्रोत　1</span><span class="sxs-lookup"><span data-stu-id="cf194-170">Funding　source　1</span></span></li>
<li><span data-ttu-id="cf194-171">वित्तपोषण　का स्रोत　2</span><span class="sxs-lookup"><span data-stu-id="cf194-171">Funding　source　2</span></span></li>
<li><span data-ttu-id="cf194-172">वित्तपोषण　का स्रोत　3</span><span class="sxs-lookup"><span data-stu-id="cf194-172">Funding　source　3</span></span></li>
<li><span data-ttu-id="cf194-173">Funding　source　4</span><span class="sxs-lookup"><span data-stu-id="cf194-173">Funding　source　4</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="cf194-174">75%</span><span class="sxs-lookup"><span data-stu-id="cf194-174">75%</span></span></li>
<li><span data-ttu-id="cf194-175">25%</span><span class="sxs-lookup"><span data-stu-id="cf194-175">25%</span></span></li>
<li><span data-ttu-id="cf194-176">50%</span><span class="sxs-lookup"><span data-stu-id="cf194-176">50%</span></span></li>
<li><span data-ttu-id="cf194-177">50%</span><span class="sxs-lookup"><span data-stu-id="cf194-177">50%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="cf194-178">1</span><span class="sxs-lookup"><span data-stu-id="cf194-178">1</span></span></li>
<li><span data-ttu-id="cf194-179">1</span><span class="sxs-lookup"><span data-stu-id="cf194-179">1</span></span></li>
<li><span data-ttu-id="cf194-180">2</span><span class="sxs-lookup"><span data-stu-id="cf194-180">2</span></span></li>
<li><span data-ttu-id="cf194-181">2</span><span class="sxs-lookup"><span data-stu-id="cf194-181">2</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cf194-182">आप लागत का पहला 25 प्रतिशत एक वित्तपोषण के स्रोत को आवंटित करना चाहते है और बाकी एक दूसरे वित्तपोषण के स्रोत को.</span><span class="sxs-lookup"><span data-stu-id="cf194-182">You want to allocate the first 25 percent of costs to one funding source and the rest to a second funding source.</span></span></td>
<td><ul>
<li><span data-ttu-id="cf194-183">वित्तपोषण　का स्रोत　1</span><span class="sxs-lookup"><span data-stu-id="cf194-183">Funding　source　1</span></span></li>
<li><span data-ttu-id="cf194-184">वित्तपोषण　का स्रोत　2</span><span class="sxs-lookup"><span data-stu-id="cf194-184">Funding　source　2</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="cf194-185">25%</span><span class="sxs-lookup"><span data-stu-id="cf194-185">25%</span></span></li>
<li><span data-ttu-id="cf194-186">100%</span><span class="sxs-lookup"><span data-stu-id="cf194-186">100%</span></span></li>
</ul></td>
<td><ul>
<li><span data-ttu-id="cf194-187">1</span><span class="sxs-lookup"><span data-stu-id="cf194-187">1</span></span></li>
<li><span data-ttu-id="cf194-188">2</span><span class="sxs-lookup"><span data-stu-id="cf194-188">2</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

### <a name="example-multiple-funding-sources-complex"></a><span data-ttu-id="cf194-189">उदाहरण: कई वित्तपोषण के स्रोत (जटिल)</span><span class="sxs-lookup"><span data-stu-id="cf194-189">Example: Multiple funding sources (complex)</span></span>

<span data-ttu-id="cf194-190">आपके पास तीन वित्तपोषण के स्रोत हैं जिन्हें आप निम्नलिखित क्रम में उपयोग करना चाहते हैं:</span><span class="sxs-lookup"><span data-stu-id="cf194-190">You have three funding sources that you want to use in the following order:</span></span>

1.  <span data-ttu-id="cf194-191">वित्तपोषण के स्रोत 2 और वित्तपोषण के स्रोत 3 का इस्तेमाल समान रूप से तब तक करें जब तक कि वित्तपोषण का स्रोत 2 खत्म न हो जाए.</span><span class="sxs-lookup"><span data-stu-id="cf194-191">Use funding source 2 and funding source 3 equally until funding source 2 is exhausted.</span></span>
2.  <span data-ttu-id="cf194-192">वित्तपोषण के स्रोत 3 का इस्तेमाल तब तक जारी रखें, जब तक कि यह खत्म न हो जाए.</span><span class="sxs-lookup"><span data-stu-id="cf194-192">Continue to use funding source 3 until it is exhausted.</span></span>
3.  <span data-ttu-id="cf194-193">वित्तपोषण के स्रोत 3 के खत्म होने के बाद वित्तपोषण के स्रोत 1 का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="cf194-193">Use funding source 1 after funding source 3 is exhausted.</span></span>

<span data-ttu-id="cf194-194">इस लक्ष्य को पूरा करने के लिए, आपको निम्नलिखित करना होगा:</span><span class="sxs-lookup"><span data-stu-id="cf194-194">To accomplish this goal, you must do the following:</span></span>

-   <span data-ttu-id="cf194-195">वित्तपोषण के स्रोत 2 और वित्तपोषण के स्रोत 3 के लिए वित्तपोषण की सीमा सेट करें, उनके संबंधित राशियों के लिए.</span><span class="sxs-lookup"><span data-stu-id="cf194-195">Set up funding limits for funding source 2 and funding source 3, for their respective amounts.</span></span>
-   <span data-ttu-id="cf194-196">निम्न फंडिंग नियम बनाएँ:</span><span class="sxs-lookup"><span data-stu-id="cf194-196">Create the following funding rules:</span></span>
    -   <span data-ttu-id="cf194-197">नियम 1 (प्राथमिकता 1): वित्तपोषण के स्रोत 2 को लेनदेन का 50 प्रतिशत आवंटित करें और 50 प्रतिशत वित्तपोषण के स्रोत 3 को.</span><span class="sxs-lookup"><span data-stu-id="cf194-197">Rule 1 (Priority 1): Allocate 50 percent of transactions to funding source 2 and 50 percent to funding source 3.</span></span>
    -   <span data-ttu-id="cf194-198">नियम 2 (प्राथमिकता 2): वित्तपोषण के स्रोत 3 को लेनदेन का 100 प्रतिशत आवंटित करें.</span><span class="sxs-lookup"><span data-stu-id="cf194-198">Rule 2 (Priority 2): Allocate 100 percent of transactions to funding source 3.</span></span>
    -   <span data-ttu-id="cf194-199">नियम 3 (प्राथमिकता 3): वित्तपोषण के स्रोत 1 को लेनदेन का 100 प्रतिशत आवंटित करें.</span><span class="sxs-lookup"><span data-stu-id="cf194-199">Rule 3 (Priority 3): Allocate 100 percent of transactions to funding source 1.</span></span>

<span data-ttu-id="cf194-200">यह सेटअप इसलिए काम करता है क्योंकि लेनदेन की नियमों और सीमाओं के खिलाफ जांच की जाती है ताकि यह निर्धारित किया जा सके कि उनमें से कोई भी लेनदेन पर लागू होता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-200">This setup works because transactions are checked against rules and limits to determine whether any of them apply to the transaction.</span></span> <span data-ttu-id="cf194-201">यदि लेन-देन पर कोई विशिष्ट नियम या सीमा लागू नहीं होती है, तो सभी लेनदेन के नियम लागू होते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-201">If no specific rules or limits apply to the transaction, the All transactions rule applies.</span></span> <span data-ttu-id="cf194-202">सभी लेनदेन के नियम सभी लेनदेन से मेल खाते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-202">The All transactions rule matches all transactions.</span></span> 

<span data-ttu-id="cf194-203">यदि कोई नियम पाया जाता है जो किसी लेन-देन से मेल खाता हो, तो उस नियम में आवंटित प्रतिशत पहले लागू किया जाता है, लेकिन केवल स्थापित की गई किसी भी सीमा के खिलाफ मिलानों के जाँच करने के बाद.</span><span class="sxs-lookup"><span data-stu-id="cf194-203">If a rule is found that matches a transaction, the percentage that has been allocated in that rule is applied first, but only after the matches are checked against any limits that have been set up.</span></span> <span data-ttu-id="cf194-204">यदि एक सीमा पूरी हो गई है, और एक वित्तपोषण के स्रोत की पूंजी समाप्त हो गई हो, तो वित्तपोषण का नियम की जो वित्तपोषण की सीमा के साथ जुड़ा हुआ है उपेक्षा की जाती है, और प्रोग्राम लागू होते अगले नियम की जांच करता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-204">If a limit has been met, and a funding source’s funds are exhausted, the funding rule that is associated with the funding limit is disregarded, and the program checks for the next rule that applies.</span></span> 

<span data-ttu-id="cf194-205">कुछ मामलों में, एक नियम के तहत लेनदेन का केवल एक हिस्सा आवंटित किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-205">In some cases, only part of a transaction can be allocated under a rule.</span></span> <span data-ttu-id="cf194-206">ऐसा इसलिए हो सकता है क्योंकि लेन-देन आवंटित होने पर एक सीमा पूरी हो जाती है.</span><span class="sxs-lookup"><span data-stu-id="cf194-206">This might happen because a limit is reached when the transaction is allocated.</span></span> <span data-ttu-id="cf194-207">इस मामले में, उस नियम के अनुसार केवल एक निश्चित राशि आवंटित की जाती है, जैसे कि प्रत्येक वित्तपोषण के स्रोत के लिए 50 प्रतिशत.</span><span class="sxs-lookup"><span data-stu-id="cf194-207">In this case, only a certain amount is allocated according to that rule, such as 50 percent to each funding source.</span></span> <span data-ttu-id="cf194-208">नियम 1 में यह उदाहरण है, जो इस अनुभाग में पहले बताया जाता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-208">This is the case in rule 1, which is described earlier in this section.</span></span> <span data-ttu-id="cf194-209">क्रम में आए अगले नियम के अनुसार शेष आवंटित की जाती है.</span><span class="sxs-lookup"><span data-stu-id="cf194-209">The remainder is allocated according to the next rule in the sequence.</span></span> 

<span data-ttu-id="cf194-210">निम्नलिखित तालिका इस परिदृश्य की अधिक विस्तार से जांच करती है.</span><span class="sxs-lookup"><span data-stu-id="cf194-210">The following table examines this scenario in more detail.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="cf194-211"><strong>फ़ोकस</strong></span><span class="sxs-lookup"><span data-stu-id="cf194-211"><strong>Focus</strong></span></span></td>
<td><span data-ttu-id="cf194-212"><strong>विवरण</strong></span><span class="sxs-lookup"><span data-stu-id="cf194-212"><strong>Details</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cf194-213">फंडिंग नियम</span><span class="sxs-lookup"><span data-stu-id="cf194-213">Funding rules</span></span></td>
<td><ul>
<li><span data-ttu-id="cf194-214">नियम 1 (प्राथमिकता 1): सभी लेनदेन.</span><span class="sxs-lookup"><span data-stu-id="cf194-214">Rule 1 (Priority 1): All transactions.</span></span> <span data-ttu-id="cf194-215">50% पर वित्तपोषण के स्रोत 2 और 50% पर वित्तपोषण के स्रोत 3 को आवंटित करें.</span><span class="sxs-lookup"><span data-stu-id="cf194-215">Allocate funding source 2 at 50% and funding source 3 at 50%.</span></span></li>
<li><span data-ttu-id="cf194-216">नियम 2 (प्राथमिकता 2): सभी लेनदेन.</span><span class="sxs-lookup"><span data-stu-id="cf194-216">Rule 2 (Priority 2): All transactions.</span></span> <span data-ttu-id="cf194-217">100% पर फंडिंग सोर्स 3 आवंटित करें.</span><span class="sxs-lookup"><span data-stu-id="cf194-217">Allocate funding source 3 at 100%.</span></span></li>
<li><span data-ttu-id="cf194-218">नियम 3 (प्राथमिकता 2): सभी लेनदेन.</span><span class="sxs-lookup"><span data-stu-id="cf194-218">Rule 3 (Priority 2): All transactions.</span></span> <span data-ttu-id="cf194-219">100% पर फंडिंग सोर्स 1 आवंटित करें.</span><span class="sxs-lookup"><span data-stu-id="cf194-219">Allocate funding source 1 at 100%.</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cf194-220">धन की सीमा</span><span class="sxs-lookup"><span data-stu-id="cf194-220">Funding limits</span></span></td>
<td><ul>
<li><span data-ttu-id="cf194-221">निधि स्रोत 1 सीमा = 10,000.00</span><span class="sxs-lookup"><span data-stu-id="cf194-221">Funding source 1 limit = 10,000.00</span></span></li>
<li><span data-ttu-id="cf194-222">निधि स्रोत 2 सीमा = 500.00</span><span class="sxs-lookup"><span data-stu-id="cf194-222">Funding source 2 limit = 500.00</span></span></li>
<li><span data-ttu-id="cf194-223">निधि स्रोत 3 सीमा = 750.00</span><span class="sxs-lookup"><span data-stu-id="cf194-223">Funding source 3 limit = 750.00</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cf194-224">लेनदेन 1</span><span class="sxs-lookup"><span data-stu-id="cf194-224">Transaction 1</span></span></td>
<td><span data-ttu-id="cf194-225"><strong>लेन-देन की राशि:</strong> 100.00<strong>वित्तपोषण:</strong> लेनदेन का भुगतान केवल नियम 1 के अनुसार किया जाता है, क्योंकि नियम 1 लागू होने के बाद लेनदेन का पूरी तरह से भुगतान किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-225"><strong>Transaction amount:</strong> 100.00<strong>Funding:</strong> The transaction is paid according to rule 1 only, because the transaction is fully paid after rule 1 is applied.</span></span> <span data-ttu-id="cf194-226">लेनदेन को वित्तपोषण के स्रोत 2 और वित्तपोषण के स्रोत 3 के बीच समान रूप से वित्तपोषित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-226">The transaction is funded equally between funding source 2 and funding source 3.</span></span>
<ul>
<li><span data-ttu-id="cf194-227">वित्तपोषण का स्रोत 2: 50.00</span><span class="sxs-lookup"><span data-stu-id="cf194-227">Funding source 2: 50.00</span></span></li>
<li><span data-ttu-id="cf194-228">वित्तपोषण का स्रोत 3: 50.00</span><span class="sxs-lookup"><span data-stu-id="cf194-228">Funding source 3: 50.00</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="cf194-229">लेनदेन 2</span><span class="sxs-lookup"><span data-stu-id="cf194-229">Transaction 2</span></span></td>
<td><span data-ttu-id="cf194-230"><strong>लेन-देन की राशि:</strong> 5,000.00<strong>वित्तपोषण:</strong> लेन-देन का भुगतान तीनों नियमों के अनुसार किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-230"><strong>Transaction amount:</strong> 5,000.00<strong>Funding:</strong> The transaction is paid according to all three rules.</span></span> <span data-ttu-id="cf194-231"><strong>नियम 1</strong>
</span><span class="sxs-lookup"><span data-stu-id="cf194-231"><strong>Rule 1</strong>
</span></span><ul>
<li><span data-ttu-id="cf194-232">वित्तपोषण का स्रोत 2: 450.00</span><span class="sxs-lookup"><span data-stu-id="cf194-232">Funding source 2: 450.00</span></span></li>
<li><span data-ttu-id="cf194-233">वित्तपोषण का स्रोत 3: 450.00</span><span class="sxs-lookup"><span data-stu-id="cf194-233">Funding source 3: 450.00</span></span></li>
</ul><span data-ttu-id="cf194-234">
<strong>नियम 2</strong>
</span><span class="sxs-lookup"><span data-stu-id="cf194-234">
<strong>Rule 2</strong>
</span></span><ul>
<li><span data-ttu-id="cf194-235">वित्तपोषण का स्रोत 3: 250.00 (= 750.00 – 50.00 – 450.00)</span><span class="sxs-lookup"><span data-stu-id="cf194-235">Funding source 3: 250.00 (= 750.00 – 50.00 – 450.00)</span></span></li>
</ul><span data-ttu-id="cf194-236">
<strong>नियम 3</strong>
</span><span class="sxs-lookup"><span data-stu-id="cf194-236">
<strong>Rule 3</strong>
</span></span><ul>
<li><span data-ttu-id="cf194-237">वित्तपोषण का स्रोत 1: 3,850.00 (= 5,000.00 – 450.00 – 450.00 – 250.00)</span><span class="sxs-lookup"><span data-stu-id="cf194-237">Funding source 1: 3,850.00 (= 5,000.00 – 450.00 – 450.00 – 250.00)</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="cf194-238">प्रत्येक वित्तपोषण के स्रोत के लिए वितरित की जाने वाली कुल पूंजी</span><span class="sxs-lookup"><span data-stu-id="cf194-238">Total funds that are distributed for each funding source</span></span></td>
<td><ul>
<li><span data-ttu-id="cf194-239">वित्तपोषण का स्रोत 1: 3,850.00</span><span class="sxs-lookup"><span data-stu-id="cf194-239">Funding source 1: 3,850.00</span></span></li>
<li><span data-ttu-id="cf194-240">वित्तपोषण का स्रोत 2: 500.00</span><span class="sxs-lookup"><span data-stu-id="cf194-240">Funding source 2: 500.00</span></span></li>
<li><span data-ttu-id="cf194-241">वित्तपोषण का स्रोत 3: 750.00</span><span class="sxs-lookup"><span data-stu-id="cf194-241">Funding source 3: 750.00</span></span></li>
</ul></td>
</tr>
</tbody>
</table>

## <a name="billing-rules"></a><span data-ttu-id="cf194-242">बिलिंग नियम</span><span class="sxs-lookup"><span data-stu-id="cf194-242">Billing rules</span></span>
<span data-ttu-id="cf194-243">जब आप किसी ग्राहक के साथ परियोजना अनुबंध पर बातचीत करते हैं, तो आप परिभाषित करते हैं कि आप किसी परियोजना पर काम के लिए ग्राहक को इंवॉयस कैसे और कब दे सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-243">When you negotiate a project contract with a customer, you define how and when you can invoice the customer for work on a project.</span></span> <span data-ttu-id="cf194-244">आपके परियोजना अनुबंध और परियोजना सेट करने के बाद, आप परियोजना के लिए बिलिंग के नियम सेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-244">After you set up the project contract and the project, you can set up billing rules for the project.</span></span> <span data-ttu-id="cf194-245">बिलिंग के नियम परियोजना की शर्तों पर आधारित होते हैं जो परियोजना अनुबंध में निर्दिष्ट होते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-245">Billing rules are based on the project terms that are specified in the project contract.</span></span> <span data-ttu-id="cf194-246">बिलिंग नियम जो आप बना सकते हैं, वे परियोजना अनुबंध और परियोजना के प्रकार की शर्तों जैसे समय और सामग्री या निश्चित-मूल्य पर निर्भर करते हैं, जिसे आप बिलिंग के नियम से संबद्ध करते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-246">The billing rules that you can create depend on the terms of the project contract and the project type, such as Time and material or Fixed-price, that you associate with the billing rule.</span></span> <span data-ttu-id="cf194-247">आप परियोजना अनुबंध के लिए एक से अधिक बिलिंग के नियम बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-247">You can create more than one billing rule for a project contract.</span></span> <span data-ttu-id="cf194-248">आप एक ही परियोजना अनुबंध से जुड़ी कई परियोजनाओं के लिए समान बिलिंग शर्तों वाली एक बिलिंग के नियम भी नियत कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-248">You can also assign a billing rule to multiple projects that are associated with the same project contract and have similar billing terms.</span></span> 

<span data-ttu-id="cf194-249">आप निम्नलिखित प्रकार के बिलिंग के नियमों को सेट कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="cf194-249">You can set up the following types of billing rules:</span></span>

-   <span data-ttu-id="cf194-250">**डिलीवरी की इकाई** - डिलीवरी की एक यूनिट पूरी होने पर ग्राहक को इंवॉयस दें..</span><span class="sxs-lookup"><span data-stu-id="cf194-250">**Unit of delivery** – Invoice a customer when you complete a unit of delivery.</span></span> <span data-ttu-id="cf194-251">आप अनुबंध में वितरण की इकाईयों को परिभाषित करते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-251">You define the units of delivery in the contract.</span></span>
-   <span data-ttu-id="cf194-252">**प्रगति** - जब आप परियोजना का एक निर्दिष्ट प्रतिशत पूरा करते हैं तो ग्राहक को इंवॉयस दें.</span><span class="sxs-lookup"><span data-stu-id="cf194-252">**Progress** – Invoice a customer when you complete a specified percentage of the project.</span></span> <span data-ttu-id="cf194-253">आप पूरा किए गए कार्य के प्रतिशत की स्वचालित रूप से गणना करने के लिए एक बिलिंग के नियम स्थापित कर सकते हैं, या आप मैन्युअल रूप से पूरा किए गए कार्य के प्रतिशत और ग्राहक को इंवॉयस देने के लिए राशि की गणना कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-253">You can set up a billing rule to automatically calculate the percentage of work completed, or you can manually calculate the percentage of work completed and the amount to invoice the customer.</span></span>
-   <span data-ttu-id="cf194-254">**उपलब्धि** - उपलब्धि पहुंचने पर एक परियोजना के उपलब्धि की पूरी राशि के लिए एक ग्राहक को इंवॉयस दें.</span><span class="sxs-lookup"><span data-stu-id="cf194-254">**Milestone** – Invoice a customer for the full amount of a project milestone when the milestone is reached.</span></span>
-   <span data-ttu-id="cf194-255">**शुल्क** - अपनी सेवाओं के साथ-साथ एक प्रबंधन शुल्क के लिए ग्राहक को इंवॉयस दें, जो आमतौर पर सेवाओं की लागत का प्रतिशत होता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-255">**Fee** – Invoice a customer for your services plus a management fee, which is typically a percentage of the cost of services.</span></span>
-   <span data-ttu-id="cf194-256">**समय और सामग्री** - किसी परियोजना पर उपयोग किए जाने वाले समय और सामग्रीयों के मूल्य के लिए ग्राहक को इंवॉयस दें.</span><span class="sxs-lookup"><span data-stu-id="cf194-256">**Time and material** – Invoice a customer for the value of time and materials that are used on a project.</span></span>

<span data-ttu-id="cf194-257">सभी प्रकार के बिलिंग के नियमों के लिए, आप एक याद रखी गई प्रतिशत निर्दिष्ट कर सकते हैं जो ग्राहक इंवॉयस से तब तक काटी जाती है जब तक कि कोई परियोजना एक सहमत चरण तक नहीं पहुंच जाती है.</span><span class="sxs-lookup"><span data-stu-id="cf194-257">For all types of billing rules, you can specify a retention percentage that is deducted from customer invoices until a project reaches an agreed-upon stage.</span></span> <span data-ttu-id="cf194-258">परियोजना अनुबंध में याद रखी गई भुगतान प्रतिशत निर्दिष्ट है.</span><span class="sxs-lookup"><span data-stu-id="cf194-258">The payment retention percentage is specified in the project contract.</span></span> <span data-ttu-id="cf194-259">राशि की गणना एक ग्राहक इंवॉयस में लाइनों के कुल मूल्य के आधार पर की जाती है, और उससे घटाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-259">The amount is calculated based on, and subtracted from, the total value of the lines in a customer invoice.</span></span> 

<span data-ttu-id="cf194-260">**समय और सामग्री** और **प्रगति** बिलिंग के नियमों के लिए, आप शुल्क लगाने योग्य श्रेणियां नियत कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-260">For **Time and material** and **Progress** billing rules, you can assign chargeable categories.</span></span> <span data-ttu-id="cf194-261">शुल्क लगाने योग्य श्रेणियां ग्राहक इंवॉयस में शामिल किए जाने वाले लेनदेन को इंगित करती हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-261">Chargeable categories indicate the transactions that should be included in customer invoices.</span></span> 

<span data-ttu-id="cf194-262">जब आप ग्राहक को इंवॉयस देने के लिए तैयार होते हैं, तो परियोजना के लिए इंवॉयस की राशि की गणना बिलिंग के नियमों के आधार पर की जाती है, और एक परियोजना का इंवॉयस प्रस्ताव उत्पन्न होता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-262">When you are ready to invoice the customer, the amount to invoice for the project is calculated based on the billing rules, and a project invoice proposal is generated.</span></span> 

<span data-ttu-id="cf194-263">निम्नलिखित अनुभाग ऐसे उदाहरण प्रदान करते हैं जो प्रदर्शित करते हैं कि कैसे किसी परियोजना के लिए बिलिंग के नियमों को सेट और प्रबंधित करें.</span><span class="sxs-lookup"><span data-stu-id="cf194-263">The following sections provide examples that show how to set up and manage billing rules for a project.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-the-number-of-units-delivered"></a><span data-ttu-id="cf194-264">उदाहरण: एक बिलिंग का नियम बनाएं जो डिलीवर की गई इकाईयों की संख्या पर आधारित हो</span><span class="sxs-lookup"><span data-stu-id="cf194-264">Example: Create a billing rule that is based on the number of units delivered</span></span>

<span data-ttu-id="cf194-265">आपका संगठन प्रति प्रशिक्षण सत्र 10,000 की लागत से ग्राहक के कर्मचारियों को कुल पांच प्रशिक्षण सत्र प्रदान करने के लिए एक समझौते में प्रवेश करता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-265">Your organization enters into an agreement to provide a total of five training sessions to a customer’s employees at a cost of 10,000 per training session.</span></span> <span data-ttu-id="cf194-266">आप प्रत्येक प्रशिक्षण सत्र के बाद ग्राहक को इंवॉयस देते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-266">You invoice the customer after each training session.</span></span> 

<span data-ttu-id="cf194-267">जब आप अनुबंध के लिए बिलिंग के नियम सेट करते हैं, तो आप निम्नलिखित मूल्यों का उपयोग करते हैं:</span><span class="sxs-lookup"><span data-stu-id="cf194-267">When you set up the billing rules for the contract, you use the following values:</span></span>

-   <span data-ttu-id="cf194-268">डिलीवरी की इकाई एक प्रशिक्षण सत्र है.</span><span class="sxs-lookup"><span data-stu-id="cf194-268">The unit of delivery is one training session.</span></span>
-   <span data-ttu-id="cf194-269">प्रति प्रशिक्षण सत्र 10,000 इकाई मूल्य है.</span><span class="sxs-lookup"><span data-stu-id="cf194-269">The unit price is 10,000 per training session.</span></span>
-   <span data-ttu-id="cf194-270">इकाईयों की कुल संख्या पांच प्रशिक्षण सत्र है.</span><span class="sxs-lookup"><span data-stu-id="cf194-270">The total number of units is five training sessions.</span></span>

<span data-ttu-id="cf194-271">जब आप एक प्रशिक्षण सत्र पूरा कर लेते हैं, तो आप डिलीवर की गई पहली इकाई के लिए 10,000 की इंवॉयस बना सकते हैं, और ग्राहक को इंवॉयस भेज सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-271">When you have completed one training session, you can create an invoice for 10,000, for the first unit that was delivered, and send the invoice to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-manual-calculation"></a><span data-ttu-id="cf194-272">उदाहरण: एक बिलिंग का नियम बनाएं जो परियोजना पूरा होने के निर्दिष्ट प्रतिशत (मैन्युअल गणना) के आधार पर हो</span><span class="sxs-lookup"><span data-stu-id="cf194-272">Example: Create a billing rule that is based on a specified percentage of project completion (manual calculation)</span></span>

<span data-ttu-id="cf194-273">आपका संगठन, एक सॉफ्टवेयर पर परामर्श देने वाला फर्म, ग्राहक द्वारा विकसित किए जा रहे उत्पाद का हिस्सा विकसित करने के लिए ग्राहक के साथ एक समझौते में प्रवेश करती है.</span><span class="sxs-lookup"><span data-stu-id="cf194-273">Your organization, a software consulting firm, enters into an agreement with a customer to develop part of a product that the customer is developing.</span></span> <span data-ttu-id="cf194-274">आपका संगठन छह महीने की अवधि में सॉफ्टवेयर कोड देने के लिए सहमत होता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-274">Your organization agrees to deliver the software code over a period of six months.</span></span> <span data-ttu-id="cf194-275">ग्राहक आपके संगठन को काम के लिए कुल 100,000 का भुगतान करने के लिए सहमत होता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-275">The customer agrees to pay your organization a total of 100,000 for the work.</span></span> <span data-ttu-id="cf194-276">जैसा कि अनुबंध में निर्दिष्ट है आप परियोजना पर पूरा किए गए कार्य के प्रतिशत के आधार पर ग्राहक को इंवॉयस देने के लिए एक बिलिंग का नियम बनाते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-276">You create a billing rule to invoice the customer based on the percentage of work that is completed on the project, as specified in the contract.</span></span>

-   <span data-ttu-id="cf194-277">पहले महीने के अंत में, आप पूरा किए गए काम का प्रतिशत निर्धारित करने के लिए ग्राहक से मिलते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-277">At the end of the first month, you meet with the customer to determine the percentage of work completed.</span></span> <span data-ttu-id="cf194-278">आपके और ग्राहक द्वारा परियोजना की समीक्षा करने के बाद, आप तय करते हैं कि परियोजना 15 प्रतिशत पूरी हो गई है.</span><span class="sxs-lookup"><span data-stu-id="cf194-278">After you and the customer review the project, you decide that the project is 15 percent completed.</span></span>
-   <span data-ttu-id="cf194-279">आप 15,000 (100,000 का 15 प्रतिशत) के लिए इंवॉयस बनाते हैं और इसे ग्राहक को भेजते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-279">You create an invoice for 15,000 (15 percent of 100,000) and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-a-specified-percentage-of-project-completion-automatic-calculation"></a><span data-ttu-id="cf194-280">उदाहरण: एक बिलिंग का नियम बनाएं जो परियोजना पूरा होने के निर्दिष्ट प्रतिशत (स्वचालित गणना) के आधार पर हो</span><span class="sxs-lookup"><span data-stu-id="cf194-280">Example: Create a billing rule that is based on a specified percentage of project completion (automatic calculation)</span></span>

<span data-ttu-id="cf194-281">आपका संगठन, एक सॉफ्टवेयर का विकास करने वाला फर्म, 30,000 के लिए एक ग्राहक के लिए पेरोल लेखांकन पैकेज विकसित करने के लिए सहमत होता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-281">Your organization, a software development firm, agrees to develop a payroll accounting package for a customer for 30,000.</span></span> <span data-ttu-id="cf194-282">ग्राहक पूरा किए गए कार्य के प्रतिशत के आधार पर आपके संगठन को भुगतान करने के लिए सहमत होता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-282">The customer agrees to pay your organization based on the percentage of work completed.</span></span> <span data-ttu-id="cf194-283">आप अनुमान लगाते हैं कि परियोजना की लागत 20,000 है.</span><span class="sxs-lookup"><span data-stu-id="cf194-283">You estimate that the project costs are 20,000.</span></span> <span data-ttu-id="cf194-284">परियोजना अनुबंध बिलिंग की प्रक्रिया में आपके द्वारा उपयोग किए जाने वाले कार्य की श्रेणियों को निर्दिष्ट करता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-284">The project contract specifies the categories of work that you use in the billing process.</span></span> <span data-ttu-id="cf194-285">आप बिलिंग के नियम सेट करते हैं जो प्रत्येक श्रेणी के लिए पूरा किए गए कार्य के प्रतिशत के लिए इंवॉयस की राशियों की गणना स्वचालित रूप से करते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-285">You set up billing rules that automatically calculate the invoice amounts for the percentage of work that is completed for each category.</span></span> <span data-ttu-id="cf194-286">आप प्रत्येक श्रेणी के लिए एक बजट सेट करते हैं:</span><span class="sxs-lookup"><span data-stu-id="cf194-286">You set up a budget for each category:</span></span>

-   <span data-ttu-id="cf194-287">**विकास** - 15,000 की लागत और 20,000 का राजस्व</span><span class="sxs-lookup"><span data-stu-id="cf194-287">**Development** – Cost of 15,000 and revenue of 20,000</span></span>
-   <span data-ttu-id="cf194-288">**इंस्टॉलेशन** - 5,000 की लागत और 10,000 का राजस्व</span><span class="sxs-lookup"><span data-stu-id="cf194-288">**Installation** – Cost of 5,000 and revenue of 10,000</span></span>

<span data-ttu-id="cf194-289">जब आप पहली बार ग्राहक का इंवॉयस बनाते हैं, तो निम्नलिखित जानकारी के आधार पर इंवॉयस की राशि की गणना स्वचालित रूप से की जाती है:</span><span class="sxs-lookup"><span data-stu-id="cf194-289">When you create a customer invoice for the first time, the invoice amount is automatically calculated based on the following information:</span></span>

-   <span data-ttu-id="cf194-290">एक महीने के बाद, परियोजना पर कार्यरत कर्मचारी परियोजना के लिए एक टाइमशीट प्रस्तुत करता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-290">After a month, the worker on the project submits a timesheet for the project.</span></span> <span data-ttu-id="cf194-291">कर्मचारी के घंटे की लागत विकास के लिए 5,000 है और इंस्टॉलेशन के लिए 1,000 है.</span><span class="sxs-lookup"><span data-stu-id="cf194-291">The cost of the worker’s hours is 5,000 for development and 1,000 for installation.</span></span> <span data-ttu-id="cf194-292">विकास कार्य 33 प्रतिशत पूरा (5,000 वास्तविक लागत/15,000 बजट लागत) हो गया है, और इंस्टॉलेशन कार्य 20 प्रतिशत पूरा (1,000 वास्तविक लागत/5,000 बजट लागत) हो गया है.</span><span class="sxs-lookup"><span data-stu-id="cf194-292">The development work is 33 percent completed (5,000 actual cost/15,000 budget cost), and the installation work is 20 percent completed (1,000 actual cost/5,000 budget cost).</span></span>
-   <span data-ttu-id="cf194-293">8,667 की इंवॉयस की राशि की स्वचालित रूप से गणना की गई है (20,000 का 33 प्रतिशत + 10,000 का 20 प्रतिशत).</span><span class="sxs-lookup"><span data-stu-id="cf194-293">The invoice amount of 8,667 is automatically calculated (33 percent of 20,000 + 20 percent of 10,000).</span></span>
-   <span data-ttu-id="cf194-294">आप 8,667 के लिए एक इंवॉयस बनाते हैं और इसे ग्राहक को भेजते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-294">You create an invoice for 8,667 and send it to the customer.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-agreed-upon-milestones"></a><span data-ttu-id="cf194-295">उदाहरण: एक बिलिंग के नियम बनाएं जो तयशुदा उपलब्धियों पर आधारित है</span><span class="sxs-lookup"><span data-stu-id="cf194-295">Example: Create a billing rule that is based on agreed-upon milestones</span></span>

<span data-ttu-id="cf194-296">आपका संगठन, एक प्रबंधन का परामर्श देने वाला फर्म, एक उपभोक्ता उत्पाद के लिए बाजार अनुसंधान का संचालन करने के लिए सहमत होता है जिसे ग्राहक को बेचने की योजना बना रहा है.</span><span class="sxs-lookup"><span data-stu-id="cf194-296">Your organization, a management consulting firm, agrees to conduct market research for a consumer product that the customer plans to sell.</span></span> <span data-ttu-id="cf194-297">ग्राहक, मार्च में शुरू होने वाले तीन महीनों की अवधि के लिए आपकी सेवाओं का उपयोग करने के लिए सहमत होता है, और आपके संगठन को 50,000 का भुगतान करने के लिए सहमत होता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-297">The customer agrees to use your services for a period of three months, starting in March, and agrees to pay your organization 50,000.</span></span> <span data-ttu-id="cf194-298">परियोजना के तीन मील के पत्थर हैं:</span><span class="sxs-lookup"><span data-stu-id="cf194-298">The project has three milestones:</span></span>

-   <span data-ttu-id="cf194-299">उपलब्धि 1: उपभोक्ता डेटा एकत्र करें - 31 मार्च</span><span class="sxs-lookup"><span data-stu-id="cf194-299">Milestone 1: Collect consumer data – March 31</span></span>
-   <span data-ttu-id="cf194-300">उपलब्धि 2: उपभोक्ता डेटा का विश्लेषण करें - 30 अप्रैल</span><span class="sxs-lookup"><span data-stu-id="cf194-300">Milestone 2: Analyze consumer data – April 30</span></span>
-   <span data-ttu-id="cf194-301">उपलब्धि 3: एक उत्पाद व्यावहारिकता प्रस्ताव प्रस्तुत करें - 31 मई</span><span class="sxs-lookup"><span data-stu-id="cf194-301">Milestone 3: Present a product viability proposal – May 31</span></span>

<span data-ttu-id="cf194-302">ग्राहक आपके संगठन को पहली उपलब्धि के लिए 10,000, दूसरी उपलब्धि के लिए 20,000 और तीसरी उपलब्धि के लिए 20,000 का भुगतान करने के लिए सहमत होता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-302">The customer agrees to pay your organization 10,000 for the first milestone, 20,000 for the second milestone, and 20,000 for the third milestone.</span></span> 

<span data-ttu-id="cf194-303">जब आप परियोजना अनुबंध स्थापित करते हैं, तो आप पूरी की गई उपलब्धि के आधार पर ग्राहक को बिल देने के लिए सहमत होते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-303">When you set up the project contract, you agree to bill the customer based on the milestone that has been completed.</span></span> <span data-ttu-id="cf194-304">बिलिंग के नियम के सेटअप में निम्नलिखित चरण शामिल हैं:</span><span class="sxs-lookup"><span data-stu-id="cf194-304">The billing rule setup includes the following steps:</span></span>

-   <span data-ttu-id="cf194-305">प्रोजेक्ट मील के पत्थर को परिभाषित करें.</span><span class="sxs-lookup"><span data-stu-id="cf194-305">Define the project milestones.</span></span>
-   <span data-ttu-id="cf194-306">प्रत्येक उपलब्धि पूरी होने पर ग्राहक को इंवॉयस देने के लिए राशि को परिभाषित करें.</span><span class="sxs-lookup"><span data-stu-id="cf194-306">Define the amount to invoice the customer when each milestone is completed.</span></span>

<span data-ttu-id="cf194-307">जब पहली उपलब्धि 31 मार्च को पूरी हो जाती है, तो आप उपलब्धि को पूरी हुई के रूप में चिह्नित करते हैं, और फिर 10,000 के लिए एक इंवॉयस बनाते हैं और इसे ग्राहक को भेजते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-307">When the first milestone is completed on March 31, you mark the milestone as completed, and then create an invoice for 10,000 and send it to the customer.</span></span> <span data-ttu-id="cf194-308">जब तक आप उपलब्धि को पूरी हुई के रूप में चिह्नित नहीं करते हैं, तब तक आप किसी उपलब्धि के लिए इंवॉयस नहीं बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-308">You can’t create an invoice for a milestone until you have marked the milestone as completed.</span></span>

### <a name="example-create-a-billing-rule-that-is-based-on-services-plus-a-management-fee"></a><span data-ttu-id="cf194-309">उदाहरण: एक बिलिंग का नियम बनाएं जो सेवाओं के साथ-साथ प्रबंधन शुल्क पर आधारित हो</span><span class="sxs-lookup"><span data-stu-id="cf194-309">Example: Create a billing rule that is based on services plus a management fee</span></span>

<span data-ttu-id="cf194-310">आपका संगठन, एक प्रबंधन का परामर्श देने वाला फर्म, एक उत्पाद की व्यावहारिकता का मूल्यांकन करने के लिए बाजार अनुसंधान का संचालन करने के लिए सहमत होता है जो ग्राहक, एक खुदरा कंपनी, विकसित कर रहा है.</span><span class="sxs-lookup"><span data-stu-id="cf194-310">Your organization, a management consulting firm, agrees to conduct market research to evaluate the viability of a product that the customer, a retail company, is developing.</span></span> <span data-ttu-id="cf194-311">समझौते की शर्तें निर्दिष्ट करती हैं कि आप अपने शीर्ष तीन प्रबंधन सलाहकारों की सेवाएं प्रदान करेंगे, जो समय-और-सामग्रीयों के आधार पर अनुसंधान का संचालन करेंगे.</span><span class="sxs-lookup"><span data-stu-id="cf194-311">The terms of the agreement specify that you will provide the services of your top three management consultants, who will conduct the research on a time-and-materials basis.</span></span> <span data-ttu-id="cf194-312">ग्राहक प्रति घंटे 100 का भुगतान करने के लिए सहमत होते हैं, साथ ही साथ परामर्श के घंटों के लिए 10 प्रतिशत प्रबंधन शुल्क जो परियोजना को चार्ज किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-312">The customer agrees to pay 100 per hour, plus a 10 percent management fee for the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="cf194-313">जब आप परियोजना अनुबंध स्थापित करते हैं, तो परामर्श के घंटों में 10 प्रतिशत प्रबंधन शुल्क जोड़ने के लिए एक बिलिंग का नियम बनाएं जो परियोजना को चार्ज किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-313">When you set up the project contract, create a billing rule to add a 10 percent management fee to the consulting hours that are charged to the project.</span></span> 

<span data-ttu-id="cf194-314">जब आप ग्राहक के लिए एक इंवॉयस बनाते हैं, तो ग्राहक को 10 प्रतिशत प्रबंधन शुल्क के साथ-साथ परामर्श के घंटों की लागत का बिल दिया जाता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-314">When you create an invoice for the customer, the customer is billed a 10 percent management fee plus the cost of the consulting hours.</span></span> <span data-ttu-id="cf194-315">उदाहरण के लिए, यदि तीनों सलाहकारों ने परियोजना पर कुल 200 घंटे काम किया, तो निम्नलिखित गणना के आधार पर 22,000 के लिए इंवॉयस बनाया जाता है:</span><span class="sxs-lookup"><span data-stu-id="cf194-315">For example, if the three consultants worked a total of 200 hours on the project, an invoice for 22,000 is created based on the following calculation:</span></span>

-   <span data-ttu-id="cf194-316">200 प्रति घंटे 100 प्रति घंटे = 20,000</span><span class="sxs-lookup"><span data-stu-id="cf194-316">200 hours at 100 per hour = 20,000</span></span>
-   <span data-ttu-id="cf194-317">10 प्रतिशत प्रबंधन शुल्क = 2,000</span><span class="sxs-lookup"><span data-stu-id="cf194-317">10 percent management fee = 2,000</span></span>
-   <span data-ttu-id="cf194-318">कुल इनवॉइस राशि = 22,000</span><span class="sxs-lookup"><span data-stu-id="cf194-318">Total invoice amount = 22,000</span></span>

<span data-ttu-id="cf194-319">यदि शुल्क किसी ग्राहक के लिए कर लगने योग्य हैं, और आप परियोजना अनुबंध में बिक्री कर समूह का चयन करते हैं, तो बिक्री कर समूह स्वचालित रूप से शुल्क के लिए बिलिंग के नियम में दर्ज होता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-319">If fees are taxable to a customer, and you select a sales tax group in the project contract, the sales tax group is automatically entered in a billing rule for fees.</span></span>

### <a name="example-create-a-billing-rule-for-the-value-of-time-and-materials"></a><span data-ttu-id="cf194-320">उदाहरण: समय और सामग्रीयों के मूल्य के लिए एक बिलिंग का नियम बनाएं</span><span class="sxs-lookup"><span data-stu-id="cf194-320">Example: Create a billing rule for the value of time and materials</span></span>

<span data-ttu-id="cf194-321">आपका संगठन, एक सॉफ्टवेयर के लिए परामर्श देने वाला फर्म, अगले छह महीनों के लिए एक ग्राहक के लिए एक सॉफ्टवेयर के विकास परियोजना पर काम करने के लिए पांच तकनीकी सलाहकारों को प्रदान करने के लिए सहमत होता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-321">Your organization, a software consulting firm, agrees to provide five technical consultants to work on a software development project for a customer for the next six months.</span></span> <span data-ttu-id="cf194-322">ग्राहक प्रत्येक परामर्श के घंटे के लिए 150 का भुगतान करने के लिए, साथ ही कार्यालय की आपूर्ति की लागत के लिए सहमत होता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-322">The customer agrees to pay 150 for each consulting hour, plus the cost of office supplies.</span></span> <span data-ttu-id="cf194-323">आपका संगठन प्रत्येक महीने के अंत में ग्राहक को इंवॉयस भेजता है.</span><span class="sxs-lookup"><span data-stu-id="cf194-323">Your organization sends an invoice to the customer at the end of each month.</span></span> 

<span data-ttu-id="cf194-324">जब आप परियोजना अनुबंध स्थापित करते हैं, तो आप परियोजना पर समय और सामग्रीयों के लिए प्रत्येक महीने ग्राहक को बिल देने के लिए सहमत होते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-324">When you set up the project contract, you agree to bill the customer each month for time and materials on the project.</span></span> <span data-ttu-id="cf194-325">आप एक बिलिंग का नियम बनाते हैं जिसमें निम्नलिखित जानकारी शामिल है:</span><span class="sxs-lookup"><span data-stu-id="cf194-325">You create a billing rule that includes the following information:</span></span>

-   <span data-ttu-id="cf194-326">अनुबंध की अवधि छह महीने है.</span><span class="sxs-lookup"><span data-stu-id="cf194-326">The contract period is six months.</span></span>
-   <span data-ttu-id="cf194-327">परामर्श के समय की गणना 150 प्रति घंटे की दर से की जाती है.</span><span class="sxs-lookup"><span data-stu-id="cf194-327">Consulting time is calculated at a rate of 150 per hour.</span></span>
-   <span data-ttu-id="cf194-328">कार्यालय की आपूर्तियाँ लागत पर इंवॉयस की जाती हैं, और परियोजना के लिए कुल लागत 10,000 से अधिक नहीं होनी चाहिए.</span><span class="sxs-lookup"><span data-stu-id="cf194-328">Office supplies are invoiced at cost, and the total cost for the project must not exceed 10,000.</span></span>
-   <span data-ttu-id="cf194-329">आप परियोजना के दौरान प्रत्येक कैलेंडर महीने के अंत में एक ग्राहक इंवॉयस बनाते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-329">You create a customer invoice at the end of each calendar month during the project.</span></span>

<span data-ttu-id="cf194-330">पहले महीने के दौरान, परियोजना पर सलाहकारों द्वारा कुल 800 घंटे रिकॉर्ड किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf194-330">During the first month, a total of 800 hours are recorded by the consultants on the project.</span></span> <span data-ttu-id="cf194-331">परियोजना के लिए चार्ज किए जाने वाले कार्यालय आपूर्तियों की लागत 2,000 है.</span><span class="sxs-lookup"><span data-stu-id="cf194-331">The cost of office supplies that are charged to the project is 2,000.</span></span> <span data-ttu-id="cf194-332">इसलिए, महीने के अंत में, आप 122,000 के लिए एक इंवॉयस बनाते हैं, जिसकी गणना 150 प्रति घंटे पर 800 घंटे के रूप में, साथ ही साथ कार्यालय की आपूर्तियों के लिए 2,000 की जाती है.</span><span class="sxs-lookup"><span data-stu-id="cf194-332">Therefore, at the end of the month, you create an invoice for 122,000, which is calculated as 800 hours at 150 per hour, plus 2,000 for office supplies.</span></span>



