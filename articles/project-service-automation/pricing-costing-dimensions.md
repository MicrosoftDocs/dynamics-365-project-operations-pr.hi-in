---
title: कीमत और लागत निर्धारण डायमेंशन का होम पेज
description: इस विषय में कीमत निर्धारण डायमेंशन की सामान्य जानकारी दी गई है।
author: rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/19/2018
ms.topic: article
ms.prod: Project Service
ms.service: business-applications
ms.assetid: 425d7bb8-9015-4f67-b9c9-cf3602e9afe8
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
ms.openlocfilehash: 2379d0d2e038f28a1a8df87a851e9bf7db7fe33f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751997"
---
# <a name="pricing-and-costing-dimensions-home-page"></a><span data-ttu-id="1dce3-103">कीमत और लागत निर्धारण डायमेंशन का होम पेज</span><span class="sxs-lookup"><span data-stu-id="1dce3-103">Pricing and costing dimensions home page</span></span>

<span data-ttu-id="1dce3-104">मानव संसाधन में कीमत और लागत निर्धारित करने में प्रयुक्त डायमेंशन दो वर्गों में आते हैं:</span><span class="sxs-lookup"><span data-stu-id="1dce3-104">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="1dce3-105">लोग</span><span class="sxs-lookup"><span data-stu-id="1dce3-105">People</span></span>
- <span data-ttu-id="1dce3-106">नियोजित कार्य</span><span class="sxs-lookup"><span data-stu-id="1dce3-106">Planned work</span></span>

<span data-ttu-id="1dce3-107">इसके कारण, Project Service Automation (PSA) में उपलब्ध दो प्रकार के कीमत निर्धारण डायमेंशन मूल्य आते हैं:</span><span class="sxs-lookup"><span data-stu-id="1dce3-107">Because of this, there are two types of pricing dimension values available in Project Service Automation (PSA):</span></span> 

- <span data-ttu-id="1dce3-108">**विकल्प सेट** - ऐसे डायमेंशन जो मूल्य समूह के लिए निश्चित गणना होते हैं।</span><span class="sxs-lookup"><span data-stu-id="1dce3-108">**Option sets** - Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="1dce3-109">**निकाय-आधारित मान** - ऐसे डायमेंसन जो अलग-अलग मूल्य समूह के हो सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="1dce3-109">**Entity-based values** - Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="1dce3-110">कीमत निर्धारण के डायमेंशन</span><span class="sxs-lookup"><span data-stu-id="1dce3-110">Pricing dimensions</span></span>

<span data-ttu-id="1dce3-111">PSA कीमत निर्धारण डायमेंश के डिफाल्ट सेट भेजती है।</span><span class="sxs-lookup"><span data-stu-id="1dce3-111">PSA ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="1dce3-112">आप इन्हें **Project Service** > **पैरामीटर्स** में देख सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="1dce3-112">You can view these by going to **Project Service** > **Parameters**.</span></span> <span data-ttu-id="1dce3-113">पैरामीटर रिकार्ड में, **राशि आधारित मूल्य निर्धारण आयाम** टैब पर, इसका सत्यापन करें कि भूमिका, **msdyn_resourcecategory** और रिसोर्सिंग ऑर्गेनाइज़ेशन यूनिट, **msdyn_organizationalunit** में **विक्रय पर लागू** और **लागत पर लागू** फील्ड **हाँ** पर सेट हैं।</span><span class="sxs-lookup"><span data-stu-id="1dce3-113">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="1dce3-114">इससे आप प्रत्येक भूमिका और ऑर्गेनाइज़ेशनल यूनिट के संयोजन के लिए कीमत और लागत निर्धारित कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="1dce3-114">This will allow you to set up the price and cost for each role and organizational unit combination.</span></span>

!["विक्रय पर लागू" के साथ Project Service पैरामीटर का स्क्रीनशॉट](media/PS-OOB-parameters.png)

> [!IMPORTANT]
> <span data-ttu-id="1dce3-116">यदि आप PSA के वर्शन 3 से पहले कीमत निर्धारण के डायमेंशन के लिए भूमिका और ऑर्गेनाइज़ेशन यूनिट के अलग फील्ड का इस्तेमाल करते आ रहे थे तो कोई बड़ा परिवर्तन नहीं होगा।</span><span class="sxs-lookup"><span data-stu-id="1dce3-116">If you have been the using out-of-the box fields of role and organizational unit as pricing dimensions prior to version 3 of PSA, there will not be any observable change.</span></span> <span data-ttu-id="1dce3-117">आप सामान्य ढंग से Project Service का इस्तेमाल करना जारी रख सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="1dce3-117">You can continue to use Project Service as usual.</span></span> 

<span data-ttu-id="1dce3-118">यदि आपको अतिरिक्त गुणों का इस्तेमाल करते हुए अपने संसाधनों की कीमत और लागत निर्धारण करना हो तो आप अपनी ज़रूरत के अनुसार फील्ड, एंटिटी और डायमेंशन बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="1dce3-118">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="1dce3-119">अधिक जानकारी के लिए, निम्नलिखित विषय देखें, बहरहाल यह नोट करें कि आपको नीचे दिए गए क्रम में प्रक्रियाएँ पूरी करनी होंगी:</span><span class="sxs-lookup"><span data-stu-id="1dce3-119">For more information, see the following topics, however note that you must complete the procedures in the order listed below:</span></span>

- [<span data-ttu-id="1dce3-120">कस्टम फ़ील्ड और एंटिटी बनाएँ</span><span class="sxs-lookup"><span data-stu-id="1dce3-120">Create custom fields and entities</span></span>](create-custom-fields-entities.md)
- [<span data-ttu-id="1dce3-121">कस्टम फ़ील्ड को मूल्य सेटअप और लेन-देन वाली एंटिटी में जोड़ें</span><span class="sxs-lookup"><span data-stu-id="1dce3-121">Add custom fields to price setup and transactional entities</span></span>](field-references.md)
- [<span data-ttu-id="1dce3-122">कस्टम फ़ील्ड को मूल्य निर्धारण आयामों के रूप में सेट अप करें</span><span class="sxs-lookup"><span data-stu-id="1dce3-122">Set up custom fields as pricing dimensions</span></span>](set-up-pricing-dimensions.md)
- [<span data-ttu-id="1dce3-123">नए मूल्य निर्धारण आयामों को शामिल करने के लिए प्लग-इन विशेषताओं को अपडेट करें</span><span class="sxs-lookup"><span data-stu-id="1dce3-123">Update plug-in attributes to include new pricing dimensions</span></span>](update-plug-in-attributes.md)

## <a name="pricing-human-resource-time"></a><span data-ttu-id="1dce3-124">मानव संसाधन समय का कीमत निर्धारण</span><span class="sxs-lookup"><span data-stu-id="1dce3-124">Pricing human resource time</span></span>
<span data-ttu-id="1dce3-125">संगठनों में मानव संसाधन के समय का कीमत निर्धारण कैसे किया जाता है यह अक्सर एक महत्वपूर्ण और रणनीतिक निर्णय होता है जो संगठन की लाभप्रदता को प्रत्यक्ष रूप से प्रभावित करता है।</span><span class="sxs-lookup"><span data-stu-id="1dce3-125">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="1dce3-126">जब आपका संगठन इसकी पहचान करने के लिए तैयार होता है कि वह मानव संसाधन समय के लिए बिल और लागत दरों को किस प्रकार तय करना चाहता है, वित्त की टीमों और प्रैक्टिस प्रमुखों के साथ काम करें।</span><span class="sxs-lookup"><span data-stu-id="1dce3-126">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="1dce3-127">मूल्य निर्धारण करते समय ध्यान देने वाली अन्य बातों में ऐसे फील्ड और एंटिटी का दोबारा इस्तेमाल करना शामिल होता है जो वर्तमान में तो मूल्य निर्धारण के आयाम नहीं है लेकिन आपके संगठन के मूल्य निर्धारण आयाम के रूप में लागू होते हैं।</span><span class="sxs-lookup"><span data-stu-id="1dce3-127">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="1dce3-128">**लेनदेन श्रेणी** (**msdyn_transactioncategory**) और **बुक करने योग्य संसाधन** (**bookableresource**) जैसे फील्ड केंडीडेट डायमेंशन के उदाहरण हैं।</span><span class="sxs-lookup"><span data-stu-id="1dce3-128">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="1dce3-129">आपको इस बात पर भी विचार करना चाहिए कि क्या आपका कीमत निर्धारण डायमेंशन टेबल होना चाहिए या ऑप्शन सेट।</span><span class="sxs-lookup"><span data-stu-id="1dce3-129">You should also consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="1dce3-130">यदि आपको लगता है कि डायमेंशन के मूल्य में परिवर्तन हो सकता है जो 10 या 12 से अधिक होगा और आपको इन मूल्यों पर अतिरिक्त गुण की ज़रूरत होगी, तो आप ऑप्शन सेट के बजाय एंटिटी बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="1dce3-130">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="1dce3-131">ऑप्शन सेट बनाए रखना जैसे मूल्य को शामिल करना या हटाना, के लिए एक एडमिन या डेवलपर की ज़रूरत होगी जबकि टेबल में नई पंक्तियाँ जोड़ना ज्यादातर यूज़र द्वारा किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="1dce3-131">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="1dce3-132">निम्नलिखित उदाहरण ऐसी बिल दरों को दर्शाता है जो भूमिका और रिसोर्सिंग ऑर्गेनाइज़ेशनल यूनिट के आधार पर तय किए गए हैं जिससे रिसोर्स संबंधित है।</span><span class="sxs-lookup"><span data-stu-id="1dce3-132">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="1dce3-133">लागत दरें आम तौर पर कर्मचारी के वेतन स्तर और ऑर्गेनाइज़ेशनल यूनिट, जिससे वे संबंधित हैं, पर आधारित होती हैं।</span><span class="sxs-lookup"><span data-stu-id="1dce3-133">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="1dce3-134">इस उदाहरण में, बिल की दर और लागत की दर टेबल इस प्रकार दिखेंगे।</span><span class="sxs-lookup"><span data-stu-id="1dce3-134">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="1dce3-135">**नमूना बिल दरें**</span><span class="sxs-lookup"><span data-stu-id="1dce3-135">**Sample bill rates**</span></span>

| <span data-ttu-id="1dce3-136">भूमिका</span><span class="sxs-lookup"><span data-stu-id="1dce3-136">Role</span></span>        | <span data-ttu-id="1dce3-137">संगठन इकाई</span><span class="sxs-lookup"><span data-stu-id="1dce3-137">Org Unit</span></span>    |<span data-ttu-id="1dce3-138">इकाई</span><span class="sxs-lookup"><span data-stu-id="1dce3-138">Unit</span></span>      |<span data-ttu-id="1dce3-139">मूल्य</span><span class="sxs-lookup"><span data-stu-id="1dce3-139">Price</span></span>      |<span data-ttu-id="1dce3-140">मुद्रा</span><span class="sxs-lookup"><span data-stu-id="1dce3-140">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="1dce3-141">डेवलपर</span><span class="sxs-lookup"><span data-stu-id="1dce3-141">Developer</span></span>   | <span data-ttu-id="1dce3-142">Contoso US</span><span class="sxs-lookup"><span data-stu-id="1dce3-142">Contoso US</span></span>  |<span data-ttu-id="1dce3-143">Hour</span><span class="sxs-lookup"><span data-stu-id="1dce3-143">Hour</span></span> | <span data-ttu-id="1dce3-144">200</span><span class="sxs-lookup"><span data-stu-id="1dce3-144">200</span></span>|<span data-ttu-id="1dce3-145">USD</span><span class="sxs-lookup"><span data-stu-id="1dce3-145">USD</span></span>     |
| <span data-ttu-id="1dce3-146">डेवलपर</span><span class="sxs-lookup"><span data-stu-id="1dce3-146">Developer</span></span>   | <span data-ttu-id="1dce3-147">रैना इंडिया</span><span class="sxs-lookup"><span data-stu-id="1dce3-147">Contoso India</span></span> |<span data-ttu-id="1dce3-148">Hour</span><span class="sxs-lookup"><span data-stu-id="1dce3-148">Hour</span></span>|   <span data-ttu-id="1dce3-149">112</span><span class="sxs-lookup"><span data-stu-id="1dce3-149">112</span></span>|<span data-ttu-id="1dce3-150">USD</span><span class="sxs-lookup"><span data-stu-id="1dce3-150">USD</span></span>     |


<span data-ttu-id="1dce3-151">**नमूना लागत दरें**</span><span class="sxs-lookup"><span data-stu-id="1dce3-151">**Sample cost rates**</span></span>

| <span data-ttu-id="1dce3-152">वेतन बैंड</span><span class="sxs-lookup"><span data-stu-id="1dce3-152">Salary Band</span></span>     | <span data-ttu-id="1dce3-153">संगठन इकाई</span><span class="sxs-lookup"><span data-stu-id="1dce3-153">Org Unit</span></span>    |<span data-ttu-id="1dce3-154">इकाई</span><span class="sxs-lookup"><span data-stu-id="1dce3-154">Unit</span></span>      |<span data-ttu-id="1dce3-155">मूल्य</span><span class="sxs-lookup"><span data-stu-id="1dce3-155">Price</span></span>      |<span data-ttu-id="1dce3-156">मुद्रा</span><span class="sxs-lookup"><span data-stu-id="1dce3-156">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="1dce3-157">मेरा company_Band1</span><span class="sxs-lookup"><span data-stu-id="1dce3-157">My company_Band1</span></span> | <span data-ttu-id="1dce3-158">रैना US</span><span class="sxs-lookup"><span data-stu-id="1dce3-158">Contoso US</span></span>  |<span data-ttu-id="1dce3-159">Hour</span><span class="sxs-lookup"><span data-stu-id="1dce3-159">Hour</span></span> | <span data-ttu-id="1dce3-160">145</span><span class="sxs-lookup"><span data-stu-id="1dce3-160">145</span></span>|<span data-ttu-id="1dce3-161">USD</span><span class="sxs-lookup"><span data-stu-id="1dce3-161">USD</span></span>     |
| <span data-ttu-id="1dce3-162">मेरा company_Band2</span><span class="sxs-lookup"><span data-stu-id="1dce3-162">My company_Band2</span></span> | <span data-ttu-id="1dce3-163">रैना इंडिया</span><span class="sxs-lookup"><span data-stu-id="1dce3-163">Contoso India</span></span> |<span data-ttu-id="1dce3-164">Hour</span><span class="sxs-lookup"><span data-stu-id="1dce3-164">Hour</span></span>|   <span data-ttu-id="1dce3-165">67</span><span class="sxs-lookup"><span data-stu-id="1dce3-165">67</span></span>|<span data-ttu-id="1dce3-166">USD</span><span class="sxs-lookup"><span data-stu-id="1dce3-166">USD</span></span>     |
