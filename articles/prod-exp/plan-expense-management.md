---
title: ख़र्च प्रबंधन कॉन्फ़िगर करें
description: यह लेख Microsoft Dynamics 365 Finance में ख़र्च प्रबंधन को कॉन्फ़िगर करने से पहले योजना प्रक्रिया के दौरान किए जाने वाले विचारों और निर्णयों का वर्णन करता है.
author: KimANelson
manager: AnnBe
ms.date: 08/29/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: GlobalCategory, ProjCategory, TrvLocations, TrvParameters, TrvPaymethod, TrvPerDiems
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 23001
ms.assetid: aa3fd14d-7e94-4603-985f-ca26d6f860ea
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: db3529597c662a326730cf6a0b855ae865f0dce5
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960339"
---
# <a name="configure-expense-management"></a><span data-ttu-id="a7a7f-103">ख़र्च प्रबंधन कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="a7a7f-103">Configure expense management</span></span>

<span data-ttu-id="a7a7f-104">यह विषय ख़र्च प्रबंधन को कॉन्फ़िगर करने से पहले योजना प्रक्रिया के दौरान किए जाने वाले विचारों और निर्णयों का वर्णन करता है.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-104">This topic describes the considerations and the decisions that you must make during the planning process before you configure Expense management.</span></span> <span data-ttu-id="a7a7f-105">ख़र्च प्रबंधन में, आप भुगतान विधियों, यात्रा मांगों, ख़र्च रिपोर्ट, नीतियों आदि के बारे में जानकारी संग्रहीत कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-105">In Expense management, you can store information about payment methods, travel requisitions, expense reports, policies, and so on.</span></span>

<span data-ttu-id="a7a7f-106">क्योंकि जब आप ख़र्च प्रबंधन के लिए अपने कॉन्फ़िगरेशन की योजना बनाते हैं तो आपके द्वारा किए गए कई निर्णय आपके संगठन के पदानुक्रम और वित्तीय संरचना पर आधारित होते हैं, आपको उन क्षेत्रों के लिए योजना दस्तावेजों का उल्लेख करना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-106">Because many of the decisions that you make when you plan your configuration for Expense management are based on your organization’s hierarchy and financial structure, you must refer to the planning documents for those areas.</span></span>

## <a name="intercompany-expenses"></a><span data-ttu-id="a7a7f-107">इंटरकंपनी व्यय</span><span class="sxs-lookup"><span data-stu-id="a7a7f-107">Intercompany expenses</span></span>

<span data-ttu-id="a7a7f-108">जब आप इंटरकंपनी ख़र्चों को सक्षम करते हैं, तो आप कानूनी निकायों और कर्मचारियों को किसी अन्य कानूनी निकाय की ओर से ख़र्च उठाने की अनुमति देते हैं, और अपने संगठन के भीतर रोजगार की कानूनी निकाय से भुगतान एकत्रित करते हैं.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-108">When you enable intercompany expenses, you allow legal entities and employees to incur expenses on behalf of another legal entity, and collect payment from the legal entity of employment within your organization.</span></span> <span data-ttu-id="a7a7f-109">उदाहरण के लिए, कानूनी निकाय अ में एक कर्मचारी कानूनी निकाय ब के लिए एक परियोजना को पूरा करता है, और परियोजना यात्रा से संबंधित ख़र्च उठाता है.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-109">For example, an employee in legal entity A completes a project for legal entity B, and the project incurs travel related expenses.</span></span> <span data-ttu-id="a7a7f-110">यदि इंटरकंपनी ख़र्च सक्षम हैं, तो कर्मचारी एक ख़र्च रिपोर्ट दाखिल कर सकता है जो कानूनी निकाय बी को ख़र्च पोस्ट करेगा, और ख़र्च का भुगतान कानूनी निकाय अ द्वारा किया जाना चाहिए. अगर आपके संगठन में कई कानूनी निकायें नहीं हैं, तो आपको इंटरकंपनी ख़र्चों को सक्षम करने की आवश्यकता नहीं है.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-110">If intercompany expenses are enabled, the employee can then file an expense report that will post the expense to legal entity B, and the expense must then be paid by legal entity A. If your organization doesn’t have multiple legal entities, you don’t have to enable intercompany expenses.</span></span>

<span data-ttu-id="a7a7f-111">**निर्णय:** क्या आप इंटरकंपनी ख़र्चों को सक्षम करना चाहते हैं?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-111">**Decision:** Do you want to enable intercompany expenses?</span></span>

## <a name="financial-management"></a><span data-ttu-id="a7a7f-112">वित्तीय प्रबंधन</span><span class="sxs-lookup"><span data-stu-id="a7a7f-112">Financial management</span></span>

<span data-ttu-id="a7a7f-113">ख़र्च प्रबंधन आपके संगठन के वित्तीय प्रबंधन के साथ मज़बूती से एकीकृत है.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-113">Expense management is tightly integrated with the financial management of your organization.</span></span> <span data-ttu-id="a7a7f-114">ख़र्च प्रबंधन के लिए आपके बहुत सारे कॉन्फ़िगरेशन आपके संगठन के वित्त के बारे में आपके द्वारा किए गए निर्णयों पर आधारित होंगे.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-114">Lots of your configuration for Expense management will be based on the decisions that you’ve made about your organization’s finances.</span></span> <span data-ttu-id="a7a7f-115">निम्नलिखित अनुभाग आपके संगठन के वित्तीय निर्णयों और आपकी नेतृत्व टीम के मार्गदर्शन के आधार पर विभिन्न क्षेत्रों का वर्णन करते हैं, जिन्हें योजना और निर्णयों की आवश्यकता होती है.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-115">The following sections describe the various areas that require planning and decisions, based on your organization’s financial decisions and guidance from your leadership team.</span></span>

### <a name="per-diems"></a><span data-ttu-id="a7a7f-116">प्रति भत्ता</span><span class="sxs-lookup"><span data-stu-id="a7a7f-116">Per diems</span></span>

<span data-ttu-id="a7a7f-117">आपको कर्मचारी का दैनिक परिभाषित करना चाहिए जो आपका संगठन प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-117">You must define the employee per diems that your organization provides.</span></span> <span data-ttu-id="a7a7f-118">क्योंकि दैनिक आमतौर पर भोजन, आवास और अन्य आकस्मिक ख़र्चों जैसे ख़र्चों को कवर करने के लिए उपयोग किया जाता है, आप आपके संगठन द्वारा प्रदान किए जाने वाले दैनिक भत्तों के लिए नियम बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-118">Because per diems are typically used to cover expenses such as meals, lodging, and other incidental expenses, you can create rules for the per diem allowances that your organization offers.</span></span> <span data-ttu-id="a7a7f-119">दैनिक दरें वर्ष के समय, यात्रा स्थान या दोनों के आधार पर हो सकती हैं.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-119">per diem rates can be based on the time of year, the travel location, or both.</span></span> <span data-ttu-id="a7a7f-120">जब आप दैनिक नियम को परिभाषित करते हैं, तो आप निर्दिष्ट कर सकते हैं कि यदि किसी श्रमिक को कम्प्लिमेंटरी भोजन या सेवाएं प्राप्त होती हैं तो दैनिक दर का प्रतिशत रोक दिया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-120">When you define a per diem rule, you can specify that a percentage of the per diem rate will be withheld if a worker receives complimentary meals or services.</span></span> <span data-ttu-id="a7a7f-121">आप दैनिक दर स्तरों को भी परिभाषित कर सकते हैं ताकि न्यूनतम और अधिकतम संख्या निर्धारित की जा सके कि दैनिक दर किसी श्रमिक की यात्रा पर लागू की जा सकती है.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-121">You can also define per diem rate tiers to set the minimum and maximum number of hours that the per diem rate can be applied to a worker’s travel.</span></span>

<span data-ttu-id="a7a7f-122">**निर्णय:**</span><span class="sxs-lookup"><span data-stu-id="a7a7f-122">**Decisions:**</span></span>

- <span data-ttu-id="a7a7f-123">पहले और अंतिम दिनों के लिए डिफ़ॉल्ट दैनिक नियम:</span><span class="sxs-lookup"><span data-stu-id="a7a7f-123">Default per diem rules for the first and last days:</span></span>

    - <span data-ttu-id="a7a7f-124">एक दिन के लिए घंटों की न्यूनतम संख्या क्या है जिसका एक कर्मचारी दावा कर सकता है और अभी भी एक दैनिक प्राप्त कर रहा है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-124">What is the minimum number of hours that an employee can claim for a day and still receive a per diem?</span></span>
    - <span data-ttu-id="a7a7f-125">क्या पहले दिन और अंतिम दिन भोजन के लिए दी जाने वाली राशि में कमी आई है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-125">Is there a reduction in the amount that is offered for meals for the first day and last day?</span></span> <span data-ttu-id="a7a7f-126">यदि कोई कमी है, तो कमी का प्रतिशत कितना है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-126">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="a7a7f-127">क्या पहले दिन और आखिरी दिन किसी होटल के लिए ऑफर की जाने वाली राशि में कमी आई है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-127">Is there a reduction in the amount that is offered for a hotel for the first day and last day?</span></span> <span data-ttu-id="a7a7f-128">यदि कोई कमी है, तो कमी का प्रतिशत कितना है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-128">If there is a reduction, what is the percentage of the reduction?</span></span>
    - <span data-ttu-id="a7a7f-129">क्या पहले दिन और अंतिम दिन होने वाले अन्य ख़र्चों के लिए दी जाने वाली राशि में कमी आई है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-129">Is there a reduction in the amount that is offered for other expenses that are incurred on the first day and last day?</span></span> <span data-ttu-id="a7a7f-130">यदि कोई कमी है, तो कमी का प्रतिशत कितना है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-130">If there is a reduction, what is the percentage of the reduction?</span></span>

- <span data-ttu-id="a7a7f-131">डिफ़ॉल्ट दैनिक नियम:</span><span class="sxs-lookup"><span data-stu-id="a7a7f-131">Default per diem rules:</span></span>

    - <span data-ttu-id="a7a7f-132">क्या प्रत्येक भोजन के लिए दैनिक भत्ते में प्रतिशत की कमी है यदि, उदाहरण के लिए, भोजन कम्प्लिमेंटरी है तो?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-132">Is there a percentage reduction in the per diem allowance for each meal if, for example, the meal is complimentary?</span></span> <span data-ttu-id="a7a7f-133">यदि कोई कमी है, तो प्रत्येक भोजन के लिए प्रतिशत कमी क्या है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-133">If there is a reduction, what is the reduction percentage for each meal?</span></span>
    - <span data-ttu-id="a7a7f-134">क्या भोजन में कमी प्रति दिन, प्रति यात्रा, या प्रति दिन भोजन की संख्या से गणना की जाती है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-134">Is the meal reduction calculated per day, per trip, or by the number of meals per day?</span></span>
    - <span data-ttu-id="a7a7f-135">क्या दैनिक राशि को नियमित तरीके से पूर्णांक किया जाना चाहिए या समग्र रूप से?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-135">Should per diem amounts be rounded in the regular manner or rounded up?</span></span>
    - <span data-ttu-id="a7a7f-136">क्या दैनिकों की गणना 24 घंटे की अवधि पर की जाती है या कैलेंडर दिवस पर?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-136">Are per diems calculated on a 24-hour period or on a calendar day?</span></span>

- <span data-ttu-id="a7a7f-137">स्थान पर आधारित दैनिक नियम:</span><span class="sxs-lookup"><span data-stu-id="a7a7f-137">Per diem rules that are based on location:</span></span>

    - <span data-ttu-id="a7a7f-138">क्या दैनिक दरें स्थान के अनुसार बदलती हैं?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-138">Do per diem rates vary according to location?</span></span> <span data-ttu-id="a7a7f-139">किन स्थानों को शामिल किया गया है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-139">What locations are included?</span></span>
    - <span data-ttu-id="a7a7f-140">यदि दैनिक दरें स्थान के अनुसार भिन्न होती हैं, तो प्रत्येक स्थान के लिए, निम्नलिखित प्रकार के ख़र्चों के लिए कितनी प्रतिशत राशि प्रदान की जाती है:</span><span class="sxs-lookup"><span data-stu-id="a7a7f-140">If per diem rates vary according to location, for each location, what percentage amount is provided for the following types of expenses:</span></span>

        - <span data-ttu-id="a7a7f-141">भोजन</span><span class="sxs-lookup"><span data-stu-id="a7a7f-141">Meals</span></span>
        - <span data-ttu-id="a7a7f-142">होटल</span><span class="sxs-lookup"><span data-stu-id="a7a7f-142">Hotel</span></span>
        - <span data-ttu-id="a7a7f-143">अन्‍य ख़र्च</span><span class="sxs-lookup"><span data-stu-id="a7a7f-143">Other expenses</span></span>

### <a name="expense-management-journals-and-accounts"></a><span data-ttu-id="a7a7f-144">ख़र्च प्रबंधन पत्रिकाएं और खाताएं</span><span class="sxs-lookup"><span data-stu-id="a7a7f-144">Expense management journals and accounts</span></span>

<span data-ttu-id="a7a7f-145">ख़र्च प्रबंधन के लिए आवश्यक है कि आप कई पत्रिकाओं और खातों का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-145">Expense management requires that you use multiple journals and accounts.</span></span> <span data-ttu-id="a7a7f-146">उदाहरण के लिए, आपको यह तय करना होगा कि क्या एक ही खाते का उपयोग नकद अग्रिम और क्रेडिट कार्ड विवादों के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-146">You must decide, for example, whether the same account is used for cash advances and credit card disputes.</span></span>

<span data-ttu-id="a7a7f-147">**निर्णय:**</span><span class="sxs-lookup"><span data-stu-id="a7a7f-147">**Decisions:**</span></span>

- <span data-ttu-id="a7a7f-148">कौन सा लेजर जर्नल स्वीकृत ख़र्च रिपोर्ट को पोस्ट कर रहा है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-148">Which ledger journal are approved expense reports posted to?</span></span>
- <span data-ttu-id="a7a7f-149">नकद अग्रिम के लिए किस खाते का उपयोग किया गया है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-149">Which account is used for cash advances?</span></span>
- <span data-ttu-id="a7a7f-150">क्या नकद अग्रिम तुरंत पोस्ट किया जाने चाहिए?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-150">Should cash advances be posted immediately?</span></span>

### <a name="payment-methods"></a><span data-ttu-id="a7a7f-151">भुगतान विधियाँ</span><span class="sxs-lookup"><span data-stu-id="a7a7f-151">Payment methods</span></span>

<span data-ttu-id="a7a7f-152">जब आप कर्मचारियों को अपने व्यवसाय की ओर से ख़र्च उठाने की अनुमति देते हैं, तो आपको भुगतान विधियों को परिभाषित करना होगा जिन्हें कर्मचारियों को उपयोग करने की अनुमति है.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-152">When you allow employees to incur expenses on behalf of your business, you must define the payment methods that employees are allowed to use.</span></span> <span data-ttu-id="a7a7f-153">उदाहरण के लिए, आप कर्मचारियों को नकद या कॉर्पोरेट क्रेडिट कार्ड का उपयोग करने की अनुमति दे सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-153">For example, you might allow employees to use cash or a corporate credit card.</span></span> <span data-ttu-id="a7a7f-154">आप कर्मचारियों को व्यक्तिगत क्रेडिट कार्ड का उपयोग करने की अनुमति भी दे सकते हैं, और फिर कर्मचारियों की प्रतिपूर्ति कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-154">You might also allow employees to use personal credit cards, and then reimburse the employees.</span></span> <span data-ttu-id="a7a7f-155">आपको प्रत्येक भुगतान विधि के लिए निम्नलिखित निर्णय लेने चाहिए, जिसकी आप अनुमति देते हैं.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-155">You must make the following decisions for each payment method that you allow.</span></span>

<span data-ttu-id="a7a7f-156">**निर्णय:**</span><span class="sxs-lookup"><span data-stu-id="a7a7f-156">**Decisions:**</span></span>

- <span data-ttu-id="a7a7f-157">भुगतान के तरीकों की अनुमति क्या है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-157">What payment methods are allowed?</span></span>
- <span data-ttu-id="a7a7f-158">भुगतान विधि के ख़र्चों को कौन स्वीकार करता है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-158">Who owns the payment method expenses?</span></span>
- <span data-ttu-id="a7a7f-159">क्या कोई ऑफसेट खाता जैसा है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-159">Is there an offset account type?</span></span> <span data-ttu-id="a7a7f-160">यदि ऑफसेट खाता जैसा है, तो यह क्या है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-160">If there is an offset account type, what is it?</span></span>
- <span data-ttu-id="a7a7f-161">अगर ऑफसेट खाता है तो खाता क्या है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-161">If there is an offset account, what is the account?</span></span>
- <span data-ttu-id="a7a7f-162">यदि भुगतान विधि क्रेडिट कार्ड है, तो क्या भुगतान विधि का उपयोग केवल आयातित लेनदेन के साथ किया जाना चाहिए?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-162">If the payment method is a credit card, should the payment method be used only with imported transactions?</span></span>

### <a name="expense-categories-and-shared-categories"></a><span data-ttu-id="a7a7f-163">ख़र्च श्रेणियां और साझा श्रेणियां</span><span class="sxs-lookup"><span data-stu-id="a7a7f-163">Expense categories and shared categories</span></span>

<span data-ttu-id="a7a7f-164">जब कर्मचारी ख़र्च रिपोर्ट बनाते हैं, तो प्रत्येक ख़र्च जो वे रिकॉर्ड करते हैं, को एक ख़र्च श्रेणी से जुड़ा होना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-164">When employees create an expense report, each expense that they record must be associated with an expense category.</span></span> <span data-ttu-id="a7a7f-165">व्यय श्रेणियों को साझा की गई श्रेणियों से प्राप्त किया जाता है, जिन्हें आपके संगठन में कानूनी निकायों के बीच साझा किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="a7a7f-165">Expense categories are derived from shared categories that can be shared across the legal entities in your organization.</span></span> <span data-ttu-id="a7a7f-166">इन श्रेणियों को परियोजना प्रबंधन और लेखांकन में भी साझा किया जा सकता है, जो आपके संगठन को परिभाषित करने के तरीके के आधार पर है.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-166">These categories can also be shared in Project management and accounting, depending on the way that your organization is defined.</span></span> <span data-ttu-id="a7a7f-167">अपने संगठन की परिभाषा और कार्यान्वयन टीम से मार्गदर्शन के आधार पर, यह निर्धारित करें कि ख़र्च प्रबंधन में उपयोग की जाने वाली श्रेणियों का उपयोग केवल ख़र्च प्रबंधन में किया जाएगा या क्या उन्हें परियोजना प्रबंधन और लेखांकन और ख़र्च प्रबंधन के बीच साझा किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-167">Based on the definition of your organization and guidance from the implementation team, determine whether the categories that are used in Expense management will be used only in Expense management, or whether they should be shared between Project management and accounting and Expense management.</span></span> <span data-ttu-id="a7a7f-168">ध्यान दें कि इन श्रेणियों को परियोजना और ख़र्च या परियोजना और उत्पादन के बीच साझा किया जा सकता है, लेकिन ख़र्च और उत्पादन के बीच नहीं.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-168">Note that these categories can be shared between Project and Expense or Project and Production, but not between Expense and Production.</span></span> <span data-ttu-id="a7a7f-169">आपको प्रत्येक ख़र्च श्रेणी के लिए निम्नलिखित निर्णय लेने होंगे.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-169">You must make the following decisions for each expense category.</span></span>

<span data-ttu-id="a7a7f-170">**निर्णय:**</span><span class="sxs-lookup"><span data-stu-id="a7a7f-170">**Decisions:**</span></span>

- <span data-ttu-id="a7a7f-171">व्यय श्रेणी क्या है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-171">What is the expense category?</span></span> <span data-ttu-id="a7a7f-172">उदाहरणों में उड़ानों, होटल या माइलेज के लिए श्रेणियां शामिल हैं।</span><span class="sxs-lookup"><span data-stu-id="a7a7f-172">Examples include categories for flights, hotel, or mileage.</span></span>
- <span data-ttu-id="a7a7f-173">क्या व्यय श्रेणी का उपयोग परियोजना प्रबंधन और लेखा में भी किया जा सकता है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-173">Can the expense category also be used in Project management and accounting?</span></span>
- <span data-ttu-id="a7a7f-174">व्यय प्रकार क्या है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-174">What is the expense type?</span></span>
- <span data-ttu-id="a7a7f-175">व्यय श्रेणी के लिए डिफ़ॉल्ट भुगतान विधि क्या है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-175">What is the default payment method for the expense category?</span></span>
- <span data-ttu-id="a7a7f-176">क्या व्यय श्रेणी वाले खर्चों को अलग-अलग करना होगा?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-176">Do expenses in the expense category have to be itemized?</span></span>
- <span data-ttu-id="a7a7f-177">व्यय श्रेणी के लिए मुख्य डिफ़ॉल्ट खाता क्या है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-177">What is the main default account for the expense category?</span></span>
- <span data-ttu-id="a7a7f-178">व्यय श्रेणी के लिए डिफ़ॉल्ट आइटम बिक्री कर समूह क्या है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-178">What is the default item sales tax group for the expense category?</span></span>
- <span data-ttu-id="a7a7f-179">क्या अतिरिक्त भुगतान विधियां व्यय श्रेणी के लिए अनुमत हैं?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-179">Are additional payment methods allowed for the expense category?</span></span> <span data-ttu-id="a7a7f-180">यदि अतिरिक्त भुगतान विधियों की अनुमति है, तो वे क्या हैं?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-180">If additional payment methods are allowed, what are they?</span></span>
- <span data-ttu-id="a7a7f-181">क्या इस व्यय श्रेणी में उपश्रेणियां हैं?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-181">Are there subcategories in this expense category?</span></span> <span data-ttu-id="a7a7f-182">यदि उपश्रेणियां हैं, तो आपको निम्नलिखित निर्णय भी करने होंगे:</span><span class="sxs-lookup"><span data-stu-id="a7a7f-182">If there are subcategories, you must also make the following decisions:</span></span>

    - <span data-ttu-id="a7a7f-183">क्या किसी भी उपश्रेणी को कर वसूली से बाहर रखा गया है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-183">Are any of the subcategories excluded from tax recovery?</span></span>
    - <span data-ttu-id="a7a7f-184">उपश्रेणियों का आइटम विक्रय कर समूह क्या है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-184">What is the item sales tax group of the subcategories?</span></span>

<span data-ttu-id="a7a7f-185">यदि ख़र्च श्रेणी का उपयोग परियोजना प्रबंधन और लेखांकन में भी किया जाता है, तो शेष प्रश्नों का उत्तर दें.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-185">If the expense category is also used in Project management and accounting, answer the remaining questions.</span></span> <span data-ttu-id="a7a7f-186">अन्यथा, अगले खंड पर आगे बढ़ें.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-186">Otherwise, move on to the next section.</span></span>

- <span data-ttu-id="a7a7f-187">निम्नलिखित खर्चों के लिए किन व्यय खातों का उपयोग किया जाएगा?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-187">Which cost accounts will be used for the following expenses?</span></span>

    - <span data-ttu-id="a7a7f-188">लागत</span><span class="sxs-lookup"><span data-stu-id="a7a7f-188">Cost</span></span>
    - <span data-ttu-id="a7a7f-189">पेरोल आवंटन</span><span class="sxs-lookup"><span data-stu-id="a7a7f-189">Payroll allocation</span></span>
    - <span data-ttu-id="a7a7f-190">WIP-लागत मूल्य</span><span class="sxs-lookup"><span data-stu-id="a7a7f-190">WIP-cost value</span></span>
    - <span data-ttu-id="a7a7f-191">लागत-आइटम</span><span class="sxs-lookup"><span data-stu-id="a7a7f-191">Cost-item</span></span>
    - <span data-ttu-id="a7a7f-192">WIP-लागत मूल्य-आइटम</span><span class="sxs-lookup"><span data-stu-id="a7a7f-192">WIP-cost value-item</span></span>
    - <span data-ttu-id="a7a7f-193">उपार्जित नुकसान</span><span class="sxs-lookup"><span data-stu-id="a7a7f-193">Accrued loss</span></span>
    - <span data-ttu-id="a7a7f-194">WIP-उपार्जित नुकसान</span><span class="sxs-lookup"><span data-stu-id="a7a7f-194">WIP-accrued loss</span></span>

- <span data-ttu-id="a7a7f-195">निम्नलिखित के लिए किन राजस्व खातों का उपयोग किया जाएगा?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-195">Which revenue accounts will be used for the following?</span></span>

    - <span data-ttu-id="a7a7f-196">इनवॉइस की गई आमदनी</span><span class="sxs-lookup"><span data-stu-id="a7a7f-196">Invoiced revenue</span></span>
    - <span data-ttu-id="a7a7f-197">उपार्जित राजस्व-बिक्री मूल्य</span><span class="sxs-lookup"><span data-stu-id="a7a7f-197">Accrued revenue-sales value</span></span>
    - <span data-ttu-id="a7a7f-198">WIP-विक्रय मूल्य</span><span class="sxs-lookup"><span data-stu-id="a7a7f-198">WIP-sales value</span></span>
    - <span data-ttu-id="a7a7f-199">उपार्जित राजस्व-उत्पादन</span><span class="sxs-lookup"><span data-stu-id="a7a7f-199">Accrued revenue-production</span></span>
    - <span data-ttu-id="a7a7f-200">WIP-उत्पादन</span><span class="sxs-lookup"><span data-stu-id="a7a7f-200">WIP-production</span></span>
    - <span data-ttu-id="a7a7f-201">उपार्जित राजस्व-लाभ</span><span class="sxs-lookup"><span data-stu-id="a7a7f-201">Accrued revenue-profit</span></span>
    - <span data-ttu-id="a7a7f-202">WIP-लाभ</span><span class="sxs-lookup"><span data-stu-id="a7a7f-202">WIP-profit</span></span>
    - <span data-ttu-id="a7a7f-203">उपार्जित राजस्व-सदस्यता</span><span class="sxs-lookup"><span data-stu-id="a7a7f-203">Accrued revenue-subscription</span></span>
    - <span data-ttu-id="a7a7f-204">WIP-सदस्यता</span><span class="sxs-lookup"><span data-stu-id="a7a7f-204">WIP-subscription</span></span>

### <a name="taxes"></a><span data-ttu-id="a7a7f-205">कर</span><span class="sxs-lookup"><span data-stu-id="a7a7f-205">Taxes</span></span>

<span data-ttu-id="a7a7f-206">ख़र्च से संबंधित करों के लिए, आपको यह निर्धारित करना होगा कि ख़र्च रिपोर्ट पर क्या शामिल या सक्षम है.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-206">For expense-related taxes, you must determine what is included or enabled on expense reports.</span></span>

<span data-ttu-id="a7a7f-207">**निर्णय:**</span><span class="sxs-lookup"><span data-stu-id="a7a7f-207">**Decisions:**</span></span>

- <span data-ttu-id="a7a7f-208">क्या बिक्री कर ख़र्च राशि में शामिल है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-208">Is sales tax included in the expense amounts?</span></span>
- <span data-ttu-id="a7a7f-209">क्या कर वसूली ख़र्चों पर सक्षम होनी चाहिए?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-209">Should tax recovery be enabled on expenses?</span></span>

    > [!NOTE]
    > <span data-ttu-id="a7a7f-210">जब आप सामान्य लेजर की योजना बना रहे थे, यदि आपने अमेरिकी बिक्री कर लागू करने और कर नियमों का उपयोग करने का निर्णय लिया है, तो आप ख़र्चों पर कर वसूली को सक्षम नहीं कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-210">When you were planning the general ledger, if you decided to apply U.S. sales tax and use tax rules, you can’t enable tax recovery on expenses.</span></span> <span data-ttu-id="a7a7f-211">(अमेरिकी बिक्री कर लागू करने और कर नियमों का उपयोग करने के लिए, **बिक्री कर कर-निर्धारण नियम लागू करें** विकल्प को **हाँ** पर सेट करें.)</span><span class="sxs-lookup"><span data-stu-id="a7a7f-211">(To apply U.S. sales tax and use tax rules, set the **Apply sales tax taxations rules** option to **Yes**.)</span></span>

## <a name="policies"></a><span data-ttu-id="a7a7f-212">नीतियाँ</span><span class="sxs-lookup"><span data-stu-id="a7a7f-212">Policies</span></span>

<span data-ttu-id="a7a7f-213">जब कर्मचारी इसकी ओर से ख़र्च उठाते हैं तो ख़र्च रिपोर्ट नीतियां बनाकर, आप अपने संगठन को समय और पैसा बचाने में मदद कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-213">By creating expense report policies, you can help your organization save time and money when employees incur expenses on its behalf.</span></span> <span data-ttu-id="a7a7f-214">नीतियां यह गारंटी देने में मदद करती हैं कि कर्मचारी बजट में रहते हैं, सभी आवश्यक जानकारी प्रदान करते हैं, और केवल पैसे ख़र्च करते हैं क्योंकि उन्हें इसकी आवश्यकता होती है.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-214">Policies help guarantee that employees stay in budget, provide all required information, and spend money only as they require it.</span></span> <span data-ttu-id="a7a7f-215">आपको प्रत्येक ख़र्च रिपोर्ट नीति और आपके द्वारा बनाई गई प्रत्येक ख़र्च रिपोर्ट अनुमोदन नीति के लिए निम्नलिखित निर्णय लेने होंगे.</span><span class="sxs-lookup"><span data-stu-id="a7a7f-215">You must make the following decisions for each expense report policy and each expense report approval policy that you create.</span></span>

<span data-ttu-id="a7a7f-216">**निर्णय:**</span><span class="sxs-lookup"><span data-stu-id="a7a7f-216">**Decisions:**</span></span>

- <span data-ttu-id="a7a7f-217">नीति का नाम क्या है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-217">What is the name of the policy?</span></span>
- <span data-ttu-id="a7a7f-218">ख़र्च नीति किसके लिए है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-218">What is the expense policy for?</span></span>
- <span data-ttu-id="a7a7f-219">यदि आपने पहले इंटरकंपनी ख़र्चों को सक्षम करने का निर्णय लिया है, तो आपके संगठन की कौन सी कंपनियां इस नीति पर लागू होंगी?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-219">If you previously decided to enable intercompany expenses, which companies in your organization will this policy apply to?</span></span>
- <span data-ttu-id="a7a7f-220">नीति कब प्रभावी हो जाती है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-220">When does the policy become effective?</span></span>
- <span data-ttu-id="a7a7f-221">नीति कब समाप्त हो जाती है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-221">When does the policy expire?</span></span>
- <span data-ttu-id="a7a7f-222">नीति नियम क्या है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-222">What is the policy rule?</span></span>
- <span data-ttu-id="a7a7f-223">नीति नियम का परिणाम क्या है?</span><span class="sxs-lookup"><span data-stu-id="a7a7f-223">What is the outcome of the policy rule?</span></span>
