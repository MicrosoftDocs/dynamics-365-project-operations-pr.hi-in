---
title: मूल्य निर्धारण आयाम अवलोकन
description: यह विषय Dynamics 365 Project Operations में मूल्य निर्धारण आयामों के बारे में जानकारी प्रदान करता है.
author: rumant
ms.date: 11/30/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 01ba11e34e7d8a59716fa9d8c8be3389ab380048
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6004983"
---
# <a name="pricing-dimensions-overview"></a><span data-ttu-id="2492b-103">मूल्य निर्धारण आयाम ओवरव्यू</span><span class="sxs-lookup"><span data-stu-id="2492b-103">Pricing dimensions overview</span></span>

<span data-ttu-id="2492b-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="2492b-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="2492b-105">मानव संसाधन में कीमत और लागत निर्धारित करने में प्रयुक्त डायमेंशन दो वर्गों में आते हैं:</span><span class="sxs-lookup"><span data-stu-id="2492b-105">The dimensions that are used in human resources to set up pricing and costs fall into two categories:</span></span>

- <span data-ttu-id="2492b-106">लोग</span><span class="sxs-lookup"><span data-stu-id="2492b-106">People</span></span>
- <span data-ttu-id="2492b-107">नियोजित कार्य</span><span class="sxs-lookup"><span data-stu-id="2492b-107">Planned work</span></span>

<span data-ttu-id="2492b-108">इसके कारण, मूल्य निर्धारण पैमाने के दो प्रकार के मान उपलब्ध हैं:</span><span class="sxs-lookup"><span data-stu-id="2492b-108">Because of this, there are two types of pricing dimension values available:</span></span>

- <span data-ttu-id="2492b-109">**विकल्प सेट**: ऐसे पैमाने जो मानों के समूह के लिए निश्चित गणना होते हैं.</span><span class="sxs-lookup"><span data-stu-id="2492b-109">**Option sets**: Dimensions that are fixed enumerations for a set of values.</span></span>
- <span data-ttu-id="2492b-110">**निकाय-आधारित मान**: ऐसे पैमाने जो अलग-अलग मानों के समूह के हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="2492b-110">**Entity-based values**: Dimensions that can be a varied set of values.</span></span>

## <a name="pricing-dimensions"></a><span data-ttu-id="2492b-111">मूल्य निर्धारण आयाम</span><span class="sxs-lookup"><span data-stu-id="2492b-111">Pricing dimensions</span></span>

<span data-ttu-id="2492b-112">Dynamics 365 Project Operations मूल्य निर्धारण आयामों के डिफ़ॉल्ट सेट के साथ भेजा जाता है.</span><span class="sxs-lookup"><span data-stu-id="2492b-112">Dynamics 365 Project Operations ships with a default set of pricing dimensions.</span></span> <span data-ttu-id="2492b-113">आप इन मूल्य निर्धारण आयामों को **Project Operations** > **मापदंड**.</span><span class="sxs-lookup"><span data-stu-id="2492b-113">You can view these pricing dimensions by going to **Project Operations** > **Parameters**.</span></span> <span data-ttu-id="2492b-114">पैरामीटर रिकार्ड में, **राशि आधारित मूल्य निर्धारण आयाम** टैब पर, इसका सत्यापन करें कि भूमिका, **msdyn_resourcecategory** और रिसोर्सिंग ऑर्गेनाइज़ेशन यूनिट, **msdyn_organizationalunit** में **विक्रय पर लागू** और **लागत पर लागू** फील्ड **हाँ** पर सेट हैं।</span><span class="sxs-lookup"><span data-stu-id="2492b-114">In the parameter record, on the **Amount-based pricing dimensions** tab, verify that the role, **msdyn_resourcecategory** and resourcing organizational unit, **msdyn_organizationalunit** have the fields **Applicable to sales** and **Applicable to cost** set to **Yes**.</span></span> <span data-ttu-id="2492b-115">इन फ़ील्ड को सक्षम करने के साथ, आप प्रत्येक भूमिका और संगठनात्मक इकाई संयोजन के लिए मूल्य और लागत सेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="2492b-115">With these fields enabled, you can set up the price and cost for each role and organizational unit combination.</span></span>

!["विक्रय पर लागू" के साथ Project Service पैरामीटर का स्क्रीनशॉट](media/PS-OOB-parameters.png)

<span data-ttu-id="2492b-117">यदि आपको अतिरिक्त गुणों का इस्तेमाल करते हुए अपने संसाधनों की कीमत और लागत निर्धारण करना हो तो आप अपनी ज़रूरत के अनुसार फील्ड, एंटिटी और डायमेंशन बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="2492b-117">If you need to price or cost for your resources using additional attributes, you can create customized fields, entities, and dimensions.</span></span> <span data-ttu-id="2492b-118">अधिक जानकारी के लिए, निम्न विषय देखें.</span><span class="sxs-lookup"><span data-stu-id="2492b-118">For more information, see the following topics.</span></span> 
  
  > [!NOTE]
  > <span data-ttu-id="2492b-119">ये प्रक्रियाओं सूचीबद्ध क्रम में पूरी की जानी चाहिए.</span><span class="sxs-lookup"><span data-stu-id="2492b-119">The procedures must be completed in the order they are listed.</span></span>

1. [<span data-ttu-id="2492b-120">कस्टम मूल्य निर्धारण आयामों के लिए एक समाधान बनाएँ</span><span class="sxs-lookup"><span data-stu-id="2492b-120">Create a solution for custom pricing dimensions</span></span>](../sales/create-solution-custompd.md)
2. [<span data-ttu-id="2492b-121">कस्टम फ़ील्ड और निकाय बनाएँ</span><span class="sxs-lookup"><span data-stu-id="2492b-121">Create custom fields and entities</span></span>](create-custom-fields-entities-pricing-dimensions.md)
3. [<span data-ttu-id="2492b-122">कस्टम फ़ील्ड को मूल्य सेटअप और लेन-देन वाली निकाय में जोड़ें </span><span class="sxs-lookup"><span data-stu-id="2492b-122">Add custom fields to price setup and transactional entities</span></span>](add-custom-fields-price-setup-transactional-entities.md)
4. [<span data-ttu-id="2492b-123">मूल्य निर्धारण आयामों के रूप में कस्टम फ़ील्ड सेटअप</span><span class="sxs-lookup"><span data-stu-id="2492b-123">Set up custom fields as pricing dimensions</span></span>](set-up-custom-fields-pricing-dimensions.md)
5. [<span data-ttu-id="2492b-124">नए मूल्य निर्धारण आयामों को शामिल करने के लिए प्लग-इन विशेषताओं को अपडेट करें</span><span class="sxs-lookup"><span data-stu-id="2492b-124">Update plug-in attributes to include new pricing dimensions</span></span>](update-plugin-attributes-pd.md)


## <a name="pricing-human-resource-time"></a><span data-ttu-id="2492b-125">मानव संसाधन समय का कीमत निर्धारण</span><span class="sxs-lookup"><span data-stu-id="2492b-125">Pricing human resource time</span></span>
<span data-ttu-id="2492b-126">संगठनों में मानव संसाधन के समय का कीमत निर्धारण कैसे किया जाता है यह अक्सर एक महत्वपूर्ण और रणनीतिक निर्णय होता है जो संगठन की लाभप्रदता को प्रत्यक्ष रूप से प्रभावित करता है।</span><span class="sxs-lookup"><span data-stu-id="2492b-126">How an organization prices human resource time is often an important strategic consideration that directly affects the organization's profitability.</span></span> <span data-ttu-id="2492b-127">जब आपका संगठन इसकी पहचान करने के लिए तैयार होता है कि वह मानव संसाधन समय के लिए बिल और लागत दरों को किस प्रकार तय करना चाहता है, वित्त की टीमों और प्रैक्टिस प्रमुखों के साथ काम करें।</span><span class="sxs-lookup"><span data-stu-id="2492b-127">Work with the finance teams and practice heads when your organization is ready to identify how it wants to set up bill and cost rates for human resource time.</span></span>

<span data-ttu-id="2492b-128">मूल्य निर्धारण करते समय ध्यान देने वाली अन्य बातों में ऐसे फील्ड और एंटिटी का दोबारा इस्तेमाल करना शामिल होता है जो वर्तमान में तो मूल्य निर्धारण के आयाम नहीं है लेकिन आपके संगठन के मूल्य निर्धारण आयाम के रूप में लागू होते हैं।</span><span class="sxs-lookup"><span data-stu-id="2492b-128">Other considerations for pricing include whether to re-use fields or entities that are not currently pricing dimensions but apply as a pricing dimension for your organization.</span></span> <span data-ttu-id="2492b-129">**लेनदेन श्रेणी** (**msdyn_transactioncategory**) और **बुक करने योग्य संसाधन** (**bookableresource**) जैसे फील्ड केंडीडेट डायमेंशन के उदाहरण हैं।</span><span class="sxs-lookup"><span data-stu-id="2492b-129">Fields like **Transaction Category** (**msdyn_transactioncategory**) and **Bookable Resource** (**bookableresource**) are examples of candidate dimensions.</span></span> 

<span data-ttu-id="2492b-130">ध्यान रखें कि आपके मूल्य निर्धारण का आयाम तालिका या विकल्प सेट हो.</span><span class="sxs-lookup"><span data-stu-id="2492b-130">Consider whether your pricing dimension should be a table or an option set.</span></span> <span data-ttu-id="2492b-131">यदि आपको लगता है कि डायमेंशन के मूल्य में परिवर्तन हो सकता है जो 10 या 12 से अधिक होगा और आपको इन मूल्यों पर अतिरिक्त गुण की ज़रूरत होगी, तो आप ऑप्शन सेट के बजाय एंटिटी बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="2492b-131">If you foresee changes to the values of a dimension which will exceed 10 or 12 and you need additional attributes on these values, you could create an entity rather than an option set.</span></span> <span data-ttu-id="2492b-132">ऑप्शन सेट बनाए रखना जैसे मूल्य को शामिल करना या हटाना, के लिए एक एडमिन या डेवलपर की ज़रूरत होगी जबकि टेबल में नई पंक्तियाँ जोड़ना ज्यादातर यूज़र द्वारा किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="2492b-132">Maintaining an option set, such as adding or removing values, requires an admin or developer whereas adding new rows to a table can be done by most users.</span></span>

<span data-ttu-id="2492b-133">निम्नलिखित उदाहरण ऐसी बिल दरों को दर्शाता है जो भूमिका और रिसोर्सिंग ऑर्गेनाइज़ेशनल यूनिट के आधार पर तय किए गए हैं जिससे रिसोर्स संबंधित है।</span><span class="sxs-lookup"><span data-stu-id="2492b-133">The following example shows bill rates that are set up based on the role and the resourcing org unit to which the resource belongs.</span></span> <span data-ttu-id="2492b-134">लागत दरें आम तौर पर कर्मचारी के वेतन स्तर और ऑर्गेनाइज़ेशनल यूनिट, जिससे वे संबंधित हैं, पर आधारित होती हैं।</span><span class="sxs-lookup"><span data-stu-id="2492b-134">Cost rates are typically based on the salary band of the employee and the org unit that they belong to.</span></span> <span data-ttu-id="2492b-135">इस उदाहरण में, बिल की दर और लागत की दर टेबल इस प्रकार दिखेंगे।</span><span class="sxs-lookup"><span data-stu-id="2492b-135">In this example, the bill rate and cost rate tables will look like the following.</span></span>

<span data-ttu-id="2492b-136">**नमूना बिल दरें**</span><span class="sxs-lookup"><span data-stu-id="2492b-136">**Sample bill rates**</span></span>

| <span data-ttu-id="2492b-137">भूमिका</span><span class="sxs-lookup"><span data-stu-id="2492b-137">Role</span></span>        | <span data-ttu-id="2492b-138">संगठन इकाई</span><span class="sxs-lookup"><span data-stu-id="2492b-138">Org Unit</span></span>    |<span data-ttu-id="2492b-139">इकाई</span><span class="sxs-lookup"><span data-stu-id="2492b-139">Unit</span></span>      |<span data-ttu-id="2492b-140">कीमत</span><span class="sxs-lookup"><span data-stu-id="2492b-140">Price</span></span>      |<span data-ttu-id="2492b-141">मुद्रा</span><span class="sxs-lookup"><span data-stu-id="2492b-141">Currency</span></span>  |
| ------------|-------------|----------|----------:|----------|
| <span data-ttu-id="2492b-142">डेवलपर</span><span class="sxs-lookup"><span data-stu-id="2492b-142">Developer</span></span>   | <span data-ttu-id="2492b-143">Contoso अमेरिका</span><span class="sxs-lookup"><span data-stu-id="2492b-143">Contoso US</span></span>  |<span data-ttu-id="2492b-144">घंटा</span><span class="sxs-lookup"><span data-stu-id="2492b-144">Hour</span></span> | <span data-ttu-id="2492b-145">200</span><span class="sxs-lookup"><span data-stu-id="2492b-145">200</span></span>|<span data-ttu-id="2492b-146">USD</span><span class="sxs-lookup"><span data-stu-id="2492b-146">USD</span></span>     |
| <span data-ttu-id="2492b-147">डेवलपर</span><span class="sxs-lookup"><span data-stu-id="2492b-147">Developer</span></span>   | <span data-ttu-id="2492b-148">Contoso भारत</span><span class="sxs-lookup"><span data-stu-id="2492b-148">Contoso India</span></span> |<span data-ttu-id="2492b-149">घंटा</span><span class="sxs-lookup"><span data-stu-id="2492b-149">Hour</span></span>|   <span data-ttu-id="2492b-150">112</span><span class="sxs-lookup"><span data-stu-id="2492b-150">112</span></span>|<span data-ttu-id="2492b-151">USD</span><span class="sxs-lookup"><span data-stu-id="2492b-151">USD</span></span>     |


<span data-ttu-id="2492b-152">**नमूना लागत दरें**</span><span class="sxs-lookup"><span data-stu-id="2492b-152">**Sample cost rates**</span></span>

| <span data-ttu-id="2492b-153">वेतन बैंड</span><span class="sxs-lookup"><span data-stu-id="2492b-153">Salary Band</span></span>     | <span data-ttu-id="2492b-154">संगठन इकाई</span><span class="sxs-lookup"><span data-stu-id="2492b-154">Org Unit</span></span>    |<span data-ttu-id="2492b-155">इकाई</span><span class="sxs-lookup"><span data-stu-id="2492b-155">Unit</span></span>      |<span data-ttu-id="2492b-156">कीमत</span><span class="sxs-lookup"><span data-stu-id="2492b-156">Price</span></span>      |<span data-ttu-id="2492b-157">मुद्रा</span><span class="sxs-lookup"><span data-stu-id="2492b-157">Currency</span></span>  |
| ----------------|-------------|----------|----------:|----------|
| <span data-ttu-id="2492b-158">मेरा company_Band1</span><span class="sxs-lookup"><span data-stu-id="2492b-158">My company_Band1</span></span> | <span data-ttu-id="2492b-159">Contoso अमेरिका</span><span class="sxs-lookup"><span data-stu-id="2492b-159">Contoso US</span></span>  |<span data-ttu-id="2492b-160">घंटा</span><span class="sxs-lookup"><span data-stu-id="2492b-160">Hour</span></span> | <span data-ttu-id="2492b-161">145</span><span class="sxs-lookup"><span data-stu-id="2492b-161">145</span></span>|<span data-ttu-id="2492b-162">USD</span><span class="sxs-lookup"><span data-stu-id="2492b-162">USD</span></span>     |
| <span data-ttu-id="2492b-163">मेरा company_Band2</span><span class="sxs-lookup"><span data-stu-id="2492b-163">My company_Band2</span></span> | <span data-ttu-id="2492b-164">Contoso भारत</span><span class="sxs-lookup"><span data-stu-id="2492b-164">Contoso India</span></span> |<span data-ttu-id="2492b-165">घंटा</span><span class="sxs-lookup"><span data-stu-id="2492b-165">Hour</span></span>|   <span data-ttu-id="2492b-166">67</span><span class="sxs-lookup"><span data-stu-id="2492b-166">67</span></span>|<span data-ttu-id="2492b-167">USD</span><span class="sxs-lookup"><span data-stu-id="2492b-167">USD</span></span>     |


[!INCLUDE[footer-include](../includes/footer-banner.md)]