---
title: मूल्य निर्धारण आयाम अवलोकन
description: इस विषय में Dynamics 365 Project Operations में मूल्य निर्धारण के पैमाने की जानकारी दी गई है.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: fe2ab3a1b12c00e346e27709d66b5a0cb81a3b56
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898218"
---
# <a name="pricing-dimensions-overview"></a><span data-ttu-id="d0013-103">मूल्य निर्धारण आयाम अवलोकन</span><span class="sxs-lookup"><span data-stu-id="d0013-103">Pricing dimensions overview</span></span>

<span data-ttu-id="d0013-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="d0013-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="d0013-105">मानव संसाधन में कीमत और लागत निर्धारित करने में प्रयुक्त डायमेंशन दो वर्गों में आते हैं:</span><span class="sxs-lookup"><span data-stu-id="d0013-105">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="d0013-106">लोग</span><span class="sxs-lookup"><span data-stu-id="d0013-106">People</span></span>
- <span data-ttu-id="d0013-107">नियोजित कार्य</span><span class="sxs-lookup"><span data-stu-id="d0013-107">Planned work</span></span>

<span data-ttu-id="d0013-108">इसके कारण, मूल्य निर्धारण पैमाने के दो प्रकार के मान उपलब्ध हैं:</span><span class="sxs-lookup"><span data-stu-id="d0013-108">Because of this, there are two types of pricing dimension values available:</span></span>

- <span data-ttu-id="d0013-109">**विकल्प सेट**: ऐसे पैमाने जो मानों के समूह के लिए निश्चित गणना होते हैं.</span><span class="sxs-lookup"><span data-stu-id="d0013-109">**Option sets**: Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="d0013-110">**निकाय-आधारित मान**: ऐसे पैमाने जो अलग-अलग मानों के समूह के हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="d0013-110">**Entity-based values**: Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="d0013-111">मूल्य निर्धारण आयाम</span><span class="sxs-lookup"><span data-stu-id="d0013-111">Pricing dimensions</span></span>

<span data-ttu-id="d0013-112">Dynamics 365 Project Operations मूल्य निर्धारण आयामों के डिफ़ॉल्ट सेट के साथ भेजा जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0013-112">Dynamics 365 Project Operations ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="d0013-113">आप इन मूल्य निर्धारण आयामों को **Project Operations** > **मापदंड**.</span><span class="sxs-lookup"><span data-stu-id="d0013-113">You can view these pricing dimensions by going to **Project Operations** > **Parameters**.</span></span> <span data-ttu-id="d0013-114">पैरामीटर रिकार्ड में, **राशि आधारित मूल्य निर्धारण आयाम** टैब पर, इसका सत्यापन करें कि भूमिका, **msdyn_resourcecategory** और रिसोर्सिंग ऑर्गेनाइज़ेशन यूनिट, **msdyn_organizationalunit** में **विक्रय पर लागू** और **लागत पर लागू** फील्ड **हाँ** पर सेट हैं।</span><span class="sxs-lookup"><span data-stu-id="d0013-114">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="d0013-115">इन फ़ील्ड को सक्षम करने के साथ, आप प्रत्येक भूमिका और संगठनात्मक इकाई संयोजन के लिए मूल्य और लागत सेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="d0013-115">With these fields enabled, you can set up the price and cost for each role and organizational unit combination.</span></span>

<span data-ttu-id="d0013-116">यदि आपको अतिरिक्त गुणों का इस्तेमाल करते हुए अपने संसाधनों की कीमत और लागत निर्धारण करना हो तो आप अपनी ज़रूरत के अनुसार फील्ड, एंटिटी और डायमेंशन बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="d0013-116">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span>

## <a name="pricing-human-resource-time"></a><span data-ttu-id="d0013-117">मानव संसाधन समय का कीमत निर्धारण</span><span class="sxs-lookup"><span data-stu-id="d0013-117">Pricing human resource time</span></span>
<span data-ttu-id="d0013-118">संगठनों में मानव संसाधन के समय का कीमत निर्धारण कैसे किया जाता है यह अक्सर एक महत्वपूर्ण और रणनीतिक निर्णय होता है जो संगठन की लाभप्रदता को प्रत्यक्ष रूप से प्रभावित करता है।</span><span class="sxs-lookup"><span data-stu-id="d0013-118">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="d0013-119">जब आपका संगठन इसकी पहचान करने के लिए तैयार होता है कि वह मानव संसाधन समय के लिए बिल और लागत दरों को किस प्रकार तय करना चाहता है, वित्त की टीमों और प्रैक्टिस प्रमुखों के साथ काम करें।</span><span class="sxs-lookup"><span data-stu-id="d0013-119">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="d0013-120">मूल्य निर्धारण करते समय ध्यान देने वाली अन्य बातों में ऐसे फील्ड और एंटिटी का दोबारा इस्तेमाल करना शामिल होता है जो वर्तमान में तो मूल्य निर्धारण के आयाम नहीं है लेकिन आपके संगठन के मूल्य निर्धारण आयाम के रूप में लागू होते हैं।</span><span class="sxs-lookup"><span data-stu-id="d0013-120">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="d0013-121">**लेनदेन श्रेणी** (**msdyn_transactioncategory**) और **बुक करने योग्य संसाधन** (**bookableresource**) जैसे फील्ड केंडीडेट डायमेंशन के उदाहरण हैं।</span><span class="sxs-lookup"><span data-stu-id="d0013-121">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="d0013-122">ध्यान रखें कि आपके मूल्य निर्धारण का आयाम तालिका या विकल्प सेट हो.</span><span class="sxs-lookup"><span data-stu-id="d0013-122">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="d0013-123">यदि आपको लगता है कि डायमेंशन के मूल्य में परिवर्तन हो सकता है जो 10 या 12 से अधिक होगा और आपको इन मूल्यों पर अतिरिक्त गुण की ज़रूरत होगी, तो आप ऑप्शन सेट के बजाय एंटिटी बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="d0013-123">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="d0013-124">ऑप्शन सेट बनाए रखना जैसे मूल्य को शामिल करना या हटाना, के लिए एक एडमिन या डेवलपर की ज़रूरत होगी जबकि टेबल में नई पंक्तियाँ जोड़ना ज्यादातर यूज़र द्वारा किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="d0013-124">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="d0013-125">निम्नलिखित उदाहरण ऐसी बिल दरों को दर्शाता है जो भूमिका और रिसोर्सिंग ऑर्गेनाइज़ेशनल यूनिट के आधार पर तय किए गए हैं जिससे रिसोर्स संबंधित है।</span><span class="sxs-lookup"><span data-stu-id="d0013-125">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="d0013-126">लागत दरें आम तौर पर कर्मचारी के वेतन स्तर और ऑर्गेनाइज़ेशनल यूनिट, जिससे वे संबंधित हैं, पर आधारित होती हैं।</span><span class="sxs-lookup"><span data-stu-id="d0013-126">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="d0013-127">इस उदाहरण में, बिल की दर और लागत की दर टेबल इस प्रकार दिखेंगे।</span><span class="sxs-lookup"><span data-stu-id="d0013-127">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="d0013-128">**नमूना बिल दरें**</span><span class="sxs-lookup"><span data-stu-id="d0013-128">**Sample bill rates**</span></span>

| <span data-ttu-id="d0013-129">भूमिका</span><span class="sxs-lookup"><span data-stu-id="d0013-129">Role</span></span>        | <span data-ttu-id="d0013-130">संगठन इकाई</span><span class="sxs-lookup"><span data-stu-id="d0013-130">Org Unit</span></span>    |<span data-ttu-id="d0013-131">इकाई</span><span class="sxs-lookup"><span data-stu-id="d0013-131">Unit</span></span>      |<span data-ttu-id="d0013-132">मूल्य</span><span class="sxs-lookup"><span data-stu-id="d0013-132">Price</span></span>      |<span data-ttu-id="d0013-133">मुद्रा</span><span class="sxs-lookup"><span data-stu-id="d0013-133">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="d0013-134">डेवलपर</span><span class="sxs-lookup"><span data-stu-id="d0013-134">Developer</span></span>   | <span data-ttu-id="d0013-135">Contoso US</span><span class="sxs-lookup"><span data-stu-id="d0013-135">Contoso US</span></span>  |<span data-ttu-id="d0013-136">Hour</span><span class="sxs-lookup"><span data-stu-id="d0013-136">Hour</span></span> | <span data-ttu-id="d0013-137">200</span><span class="sxs-lookup"><span data-stu-id="d0013-137">200</span></span>|<span data-ttu-id="d0013-138">USD</span><span class="sxs-lookup"><span data-stu-id="d0013-138">USD</span></span>     |
| <span data-ttu-id="d0013-139">डेवलपर</span><span class="sxs-lookup"><span data-stu-id="d0013-139">Developer</span></span>   | <span data-ttu-id="d0013-140">रैना इंडिया</span><span class="sxs-lookup"><span data-stu-id="d0013-140">Contoso India</span></span> |<span data-ttu-id="d0013-141">Hour</span><span class="sxs-lookup"><span data-stu-id="d0013-141">Hour</span></span>|   <span data-ttu-id="d0013-142">112</span><span class="sxs-lookup"><span data-stu-id="d0013-142">112</span></span>|<span data-ttu-id="d0013-143">USD</span><span class="sxs-lookup"><span data-stu-id="d0013-143">USD</span></span>     |


<span data-ttu-id="d0013-144">**नमूना लागत दरें**</span><span class="sxs-lookup"><span data-stu-id="d0013-144">**Sample cost rates**</span></span>

| <span data-ttu-id="d0013-145">वेतन बैंड</span><span class="sxs-lookup"><span data-stu-id="d0013-145">Salary Band</span></span>     | <span data-ttu-id="d0013-146">संगठन इकाई</span><span class="sxs-lookup"><span data-stu-id="d0013-146">Org Unit</span></span>    |<span data-ttu-id="d0013-147">इकाई</span><span class="sxs-lookup"><span data-stu-id="d0013-147">Unit</span></span>      |<span data-ttu-id="d0013-148">मूल्य</span><span class="sxs-lookup"><span data-stu-id="d0013-148">Price</span></span>      |<span data-ttu-id="d0013-149">मुद्रा</span><span class="sxs-lookup"><span data-stu-id="d0013-149">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="d0013-150">मेरा company_Band1</span><span class="sxs-lookup"><span data-stu-id="d0013-150">My company_Band1</span></span> | <span data-ttu-id="d0013-151">रैना US</span><span class="sxs-lookup"><span data-stu-id="d0013-151">Contoso US</span></span>  |<span data-ttu-id="d0013-152">Hour</span><span class="sxs-lookup"><span data-stu-id="d0013-152">Hour</span></span> | <span data-ttu-id="d0013-153">145</span><span class="sxs-lookup"><span data-stu-id="d0013-153">145</span></span>|<span data-ttu-id="d0013-154">USD</span><span class="sxs-lookup"><span data-stu-id="d0013-154">USD</span></span>     |
| <span data-ttu-id="d0013-155">मेरा company_Band2</span><span class="sxs-lookup"><span data-stu-id="d0013-155">My company_Band2</span></span> | <span data-ttu-id="d0013-156">रैना इंडिया</span><span class="sxs-lookup"><span data-stu-id="d0013-156">Contoso India</span></span> |<span data-ttu-id="d0013-157">Hour</span><span class="sxs-lookup"><span data-stu-id="d0013-157">Hour</span></span>|   <span data-ttu-id="d0013-158">67</span><span class="sxs-lookup"><span data-stu-id="d0013-158">67</span></span>|<span data-ttu-id="d0013-159">USD</span><span class="sxs-lookup"><span data-stu-id="d0013-159">USD</span></span>     |
