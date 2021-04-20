---
title: उत्पाद-आधारित अनुबंध पंक्तियाँ ओवरव्यू
description: यह विषय परियोजना-आधारित अनुबंध पंक्तियों के साथ कार्य करने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/28/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 824fdd54d7b513b49afd1a6d76d3387df81418e2
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858160"
---
# <a name="project-based-contract-lines-overview"></a><span data-ttu-id="8de79-103">उत्पाद-आधारित अनुबंध पंक्तियाँ ओवरव्यू</span><span class="sxs-lookup"><span data-stu-id="8de79-103">Project-based contract lines overview</span></span>

<span data-ttu-id="8de79-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="8de79-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8de79-105">Dynamics 365 Project Operations में परियोजना-आधारित अनुबंध पंक्तियाँ किसी सहभागिता पर परियोजना कार्य के विशिष्ट घटकों के लिए अनुमान और बिलिंग समझौतों को होल्ड करने के लिए डिज़ाइन की गई हैं.</span><span class="sxs-lookup"><span data-stu-id="8de79-105">Project-based contract lines in Dynamics 365 Project Operations are designed to hold the estimate and billing agreements for specific components of project work on an engagement.</span></span> <span data-ttu-id="8de79-106">निम्न अवधारणाओं के साथ परियोजना अनुमानों और बिलिंग परिदृश्यों के लिए परियोजना-आधारित अनुबंध पंक्ति की संरचना को विस्तृत किया गया है:</span><span class="sxs-lookup"><span data-stu-id="8de79-106">The structure of a project–based contract line is extended for project estimates and billing scenarios with the following concepts:</span></span>

- <span data-ttu-id="8de79-107">बिलिंग विधि</span><span class="sxs-lookup"><span data-stu-id="8de79-107">Billing method</span></span>
- <span data-ttu-id="8de79-108">परियोजना और कार्य मैपिंग</span><span class="sxs-lookup"><span data-stu-id="8de79-108">Project and task mapping</span></span>
- <span data-ttu-id="8de79-109">शामिल ट्रांज़ैक्शन श्रेणियाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-109">Included transaction classes</span></span>
- <span data-ttu-id="8de79-110">सीमा-में रखें सीमा</span><span class="sxs-lookup"><span data-stu-id="8de79-110">Not-to-exceed limit</span></span>
- <span data-ttu-id="8de79-111">प्रभार्यता सेटअप</span><span class="sxs-lookup"><span data-stu-id="8de79-111">Chargeability setup</span></span>
- <span data-ttu-id="8de79-112">अनुबंध पंक्ति विवरण का उपयोग करके अनुमान लगाता है</span><span class="sxs-lookup"><span data-stu-id="8de79-112">Estimates using contract line details</span></span>
- <span data-ttu-id="8de79-113">अनुबंध पंक्ति ग्राहक</span><span class="sxs-lookup"><span data-stu-id="8de79-113">Contract line customers</span></span>

<span data-ttu-id="8de79-114">निम्न तालिका में परियोजना आधारित अनुबंध पंक्तियों के **समान्य** टैब पर फ़ील्ड शामिल हैं, जो परियोजना-आधारित कार्य के लिए विस्तृत, जमीनी अनुमान और बिलिंग व्यवस्था के लिए आधार सेट करने में मदद करती हैं.</span><span class="sxs-lookup"><span data-stu-id="8de79-114">The following table includes the fields on the **General** tab of project–based contract lines that help set up the basis for a detailed, ground–up estimate and billing arrangements for project–based work.</span></span>

| <span data-ttu-id="8de79-115">क्षेत्र</span><span class="sxs-lookup"><span data-stu-id="8de79-115">Field</span></span> | <span data-ttu-id="8de79-116">विवरण</span><span class="sxs-lookup"><span data-stu-id="8de79-116">Description</span></span> | <span data-ttu-id="8de79-117">डाउनस्ट्रीम प्रभाव</span><span class="sxs-lookup"><span data-stu-id="8de79-117">Downstream impact</span></span> |
| --- | --- | --- |
| <span data-ttu-id="8de79-118">**नाम**</span><span class="sxs-lookup"><span data-stu-id="8de79-118">**Name**</span></span> | <span data-ttu-id="8de79-119">अनुबंध पंक्ति का नाम.</span><span class="sxs-lookup"><span data-stu-id="8de79-119">Name of the contract line.</span></span> <span data-ttu-id="8de79-120">यह उस अनुबंध के असतत घटक की पहचान करता है, जिसका अनुमान लगाया जा रहा है.</span><span class="sxs-lookup"><span data-stu-id="8de79-120">This identifies the discrete component of the contract that is being estimated.</span></span> <span data-ttu-id="8de79-121">किसी कोट से बनाए गए परियोजना अनुबंध के लिए, यह मान परियोजना-आधारित कोट पंक्ति के संगत मान से कॉपी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-121">For a project contract created from a quote, this value is copied from a corresponding value of the project-based quote line.</span></span> | <span data-ttu-id="8de79-122">उस परियोजना इनवॉइस पंक्ति पर कॉपी किया गया नाम, जो इनवॉइस के बनाए जाने पर इस अनुबंध पंक्ति से बनाई गई थी.</span><span class="sxs-lookup"><span data-stu-id="8de79-122">The name copied over to the project invoice line that is created from this contract line when the invoice is created.</span></span> |
| <span data-ttu-id="8de79-123">**बिलिंग विधि**</span><span class="sxs-lookup"><span data-stu-id="8de79-123">**Billing Method**</span></span> | <span data-ttu-id="8de79-124">किसी कोट से बनाए गए परियोजना अनुबंध पर, यह मान संगत फ़ील्ड से कोट पंक्ति पर कॉपी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-124">On a project contract created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="8de79-125">यह एक विकल्प सेट है, जो Project Operations द्वारा समर्थित दो मुख्य अनुबंध मॉडल का प्रतिनिधित्व करता है:</span><span class="sxs-lookup"><span data-stu-id="8de79-125">This is an option set that represents the two main contracting models supported by Project Operations:</span></span></br><span data-ttu-id="8de79-126">- **निश्चित मूल्य**</span><span class="sxs-lookup"><span data-stu-id="8de79-126">- **Fixed Price**</span></span></br><span data-ttu-id="8de79-127">- **समय और सामग्री**</span><span class="sxs-lookup"><span data-stu-id="8de79-127">- **Time and Material**</span></span> | <span data-ttu-id="8de79-128">संदर्भित अनुबंध पंक्ति की बिलिंग पद्धति के आधार पर, वास्तविक ट्रांज़ैक्शन संसाधित किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="8de79-128">Based on the billing method of the referenced contract line, the actual transaction will be processed.</span></span> <span data-ttu-id="8de79-129">यदि वास्तविक द्वारा संदर्भित अनुबंध पंक्ति में समय और सामग्री बिलिंग विधि होती है, तो लागत और बिल न किए गए विक्रय वास्तविक रिकॉर्ड बनाए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="8de79-129">If the contract line referenced by the actual has a time and material billing method, cost and unbilled sales actual records are created.</span></span> <span data-ttu-id="8de79-130">यदि वास्तविक द्वारा संदर्भित अनुबंध पंक्ति में एक निश्चित मूल्य बिलिंग विधि होती है, तो केवल वास्तविक लागत बनाई जाती है.</span><span class="sxs-lookup"><span data-stu-id="8de79-130">If the contract line referenced by the actual has a fixed price billing method, only a cost actual is created.</span></span> |
| <span data-ttu-id="8de79-131">**Project**</span><span class="sxs-lookup"><span data-stu-id="8de79-131">**Project**</span></span> | <span data-ttu-id="8de79-132">इस फ़ील्ड का उपयोग उस परियोजना की पहचान करने के लिए करें, जिसका उपयोग इस सहभागिता पर कार्य वितरित करने के लिए किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="8de79-132">Use this field to identify the project that will be used to deliver the work on this engagement.</span></span> | <span data-ttu-id="8de79-133">इस मान का उपयोग वास्तविक या अनुमानित लाइन रिकॉर्ड पर कॉन्ट्रैक्ट लाइन के संदर्भ को हल करने के लिए **शामिल कार्य** और **शामिल लेनदेन श्रेणियां** के साथ मिलकर किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="8de79-133">This value will be used in conjunction with **Included Tasks** and **Included Transaction Classes** to resolve the contract line reference on an actual or estimate line record.</span></span> |
| <span data-ttu-id="8de79-134">**शामिल कार्य**</span><span class="sxs-lookup"><span data-stu-id="8de79-134">**Included Tasks**</span></span> | <span data-ttu-id="8de79-135">इंगित करता है कि यह अनुबंध पंक्ति चयनित परियोजना के लिए सभी परियोजना कार्य शामिल करती है या केवल कार्यों का एक सबसेट शामिल करती है.</span><span class="sxs-lookup"><span data-stu-id="8de79-135">Indicates if this contract line includes all project tasks for the selected project or only a subset of the tasks.</span></span> <span data-ttu-id="8de79-136">यह एक विकल्प सेट है जिसमें निम्न संभावित मान हैं:</span><span class="sxs-lookup"><span data-stu-id="8de79-136">This is an option set that has the following possible values:</span></span></br><span data-ttu-id="8de79-137">- **सभी परियोजना कार्य**</span><span class="sxs-lookup"><span data-stu-id="8de79-137">- **All Project Tasks**</span></span></br><span data-ttu-id="8de79-138">- **केवल चयनित परियोजना कार्य**.</span><span class="sxs-lookup"><span data-stu-id="8de79-138">- **Selected Project Tasks Only**.</span></span> <span data-ttu-id="8de79-139">इस फ़ील्ड में एक रिक्त मान **सभी परियोजना कार्य** चुनने के बराबर है.</span><span class="sxs-lookup"><span data-stu-id="8de79-139">A blank value in this field is equal to selecting **All Project Tasks**.</span></span> | <span data-ttu-id="8de79-140">यदि **केवल चयनित कार्य** चुना जाता है, तो आप विशिष्ट कार्य चुन सकते हैं और उन्हें **परियोजना** पृष्ठ पर **कार्य बिलिंग सेटअप** टैब पर इस अनुबंध पंक्ति से संबद्ध कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="8de79-140">If **Selected Tasks Only** is selected, you can select specific tasks and associate them to this contract line on the **Task Billing Setup** tab on the **Project** page.</span></span> <span data-ttu-id="8de79-141">वास्तविक या अनुमान पंक्ति रिकॉर्ड पर अनुबंध पंक्ति संदर्भ को हल करने के लिए इस मान का उपयोग **परियोजना** और **शामिल ट्रांज़ैक्शन** श्रेणियों के संयोजन में किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="8de79-141">The value will be used in conjunction with **Project** and **Included Transaction** classes to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="8de79-142">**समय शामिल करें**</span><span class="sxs-lookup"><span data-stu-id="8de79-142">**Include Time**</span></span> | <span data-ttu-id="8de79-143">यदि इस कॉन्ट्रैक्ट लाइन पर चयनित परियोजना में समय ट्रांज़ेक्शनों को या श्रम लागत शामिल किया जाएगा तो एक **हां**/**नहीं** मान इंगित करता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-143">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="8de79-144">**नहीं** मान इंगित करता है कि इस अनुबंध पंक्ति पर समय ट्रांज़ैक्शन या लेबर लागत शामिल नहीं होगी.</span><span class="sxs-lookup"><span data-stu-id="8de79-144">A **No** value indicates that the time transactions or labor cost will not be included on this contract line.</span></span> <span data-ttu-id="8de79-145">**हाँ** मान इंगित करता है कि वह शामिल होगी.</span><span class="sxs-lookup"><span data-stu-id="8de79-145">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="8de79-146">इस मान का उपयोग परियोजना के साथ मिलकर एक्चुअल या अनुमानित लाइन रिकॉर्ड पर कॉन्ट्रैक्ट लाइन के संदर्भ को हल करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-146">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="8de79-147">**व्यय शामिल करें**</span><span class="sxs-lookup"><span data-stu-id="8de79-147">**Include Expense**</span></span> | <span data-ttu-id="8de79-148">यदि इस कॉन्ट्रैक्ट लाइन पर चयनित परियोजना में खर्च लागत शामिल किया जाएगा तो एक **हां**/**नहीं** मान इंगित करता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-148">A **Yes**/**No** value indicates if expense costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="8de79-149">**नहीं** मान इंगित करता है कि इस अनुबंध पंक्ति पर व्यय लागत शामिल नहीं होगी.</span><span class="sxs-lookup"><span data-stu-id="8de79-149">A **No** value indicates that the expense cost will not be included on this contract line.</span></span> <span data-ttu-id="8de79-150">**हाँ** मान इंगित करता है कि वह शामिल होगी.</span><span class="sxs-lookup"><span data-stu-id="8de79-150">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="8de79-151">इस मान का उपयोग परियोजना के साथ मिलकर एक्चुअल या अनुमानित लाइन रिकॉर्ड पर कॉन्ट्रैक्ट लाइन के संदर्भ को हल करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-151">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="8de79-152">**सामग्री शामिल करें**</span><span class="sxs-lookup"><span data-stu-id="8de79-152">**Include Materials**</span></span> | <span data-ttu-id="8de79-153">यदि इस कॉन्ट्रैक्ट लाइन पर चयनित परियोजना में सामग्री लागत शामिल किया जाएगा तो एक **हां**/**नहीं** मान इंगित करता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-153">A **Yes**/**No** value indicates if material costs on the selected project will be included on this contract line.</span></span> <span data-ttu-id="8de79-154">एक **नहीं** मान इंगित करता है कि सामग्री की लागत को इस कॉन्ट्रैक्ट लाइन पर शामिल नहीं किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="8de79-154">A **No** value indicates that the material costs will not be included on this contract line.</span></span> <span data-ttu-id="8de79-155">**हाँ** मान इंगित करता है कि वह शामिल होगी.</span><span class="sxs-lookup"><span data-stu-id="8de79-155">A **Yes** value indicates that it will.</span></span> | <span data-ttu-id="8de79-156">इस मान का उपयोग परियोजना के साथ मिलकर एक्चुअल या अनुमानित लाइन रिकॉर्ड पर कॉन्ट्रैक्ट लाइन के संदर्भ को हल करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-156">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="8de79-157">**शुल्क शामिल करें**</span><span class="sxs-lookup"><span data-stu-id="8de79-157">**Include Fee**</span></span> | <span data-ttu-id="8de79-158">यदि इस कॉन्ट्रैक्ट लाइन पर चयनित परियोजना में शुल्क शामिल किया जाएगा तो एक **हां**/**नहीं** मान इंगित करता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-158">A **Yes**/**No** value indicates if fees on the selected project will be included on this contract line.</span></span> <span data-ttu-id="8de79-159">**नहीं** मान इंगित करता है कि इस अनुबंध पंक्ति पर शुल्क शामिल नहीं होगा.</span><span class="sxs-lookup"><span data-stu-id="8de79-159">A **No** value indicates that the fees will not be included on this contract line.</span></span> <span data-ttu-id="8de79-160">**हाँ** मान इंगित करता है कि वह शामिल होगी.</span><span class="sxs-lookup"><span data-stu-id="8de79-160">A **Yes** value indicates that they will.</span></span> | <span data-ttu-id="8de79-161">इस मान का उपयोग परियोजना के साथ मिलकर एक्चुअल या अनुमानित लाइन रिकॉर्ड पर कॉन्ट्रैक्ट लाइन के संदर्भ को हल करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-161">This value is used in conjunction with the project to resolve the contract line reference on an actual or an estimate line record.</span></span> |
| <span data-ttu-id="8de79-162">**अनुबंधित राशि**</span><span class="sxs-lookup"><span data-stu-id="8de79-162">**Contracted Amount**</span></span> | <span data-ttu-id="8de79-163">एक निश्चित मूल्य अनुबंध पंक्ति पर, यह राशि वह सहमत मूल्य है, जो ग्राहक को इस अनुबंध पंक्ति से संबद्ध सभी कार्य घटकों के लिए इनवॉइस किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="8de79-163">On a fixed price contract line, this amount is the agreed-on value that will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="8de79-164">समय और सामग्री अनुबंध पंक्ति पर, यह राशि वह अनुमानित मूल्य है, जो ग्राहक को इस अनुबंध पंक्ति से संबद्ध सभी कार्य घटकों के लिए इनवॉइस किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="8de79-164">On a time and material contract line, this amount is an estimated value of what will be invoiced to the customer for all the work components associated to this contract line.</span></span> <span data-ttu-id="8de79-165">किसी कोट से बनाए गए परियोजना अनुबंध पर, यह मान संगत फ़ील्ड से कोट पंक्ति पर कॉपी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-165">On a project contract that is created from a quote, this value is copied from the corresponding field on the quote line.</span></span> <span data-ttu-id="8de79-166">जब किसी परियोजना-आधारित अनुबंध पंक्ति में पंक्ति विवरण होता है, तो यह फ़ील्ड संपादन के लिए लॉक हो जाती है और अनुबंध पंक्ति विवरण पर राशि से सारांशित होती है.</span><span class="sxs-lookup"><span data-stu-id="8de79-166">When a project–based contract line has line details, this field is locked for editing and is summarized from the amount on the contract line details.</span></span> | <span data-ttu-id="8de79-167">जब अनुबंध पंक्ति में पंक्ति विवरण होता है, तो यह मान पंक्ति विवरण पर राशि को बदलकर संशोधित किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-167">When the contract line has line details, this value can be modified by changing the amounts on the line details.</span></span> <span data-ttu-id="8de79-168">एक निश्चित मूल्य अनुबंध पंक्ति पर, इस मान का उपयोग आवधिक बिलिंग माइलस्टोन पर कर से पहले राशि जनरेट करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-168">On a fixed price contract line, this value is used to generate the amount before tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="8de79-169">**अनुमानित कर**</span><span class="sxs-lookup"><span data-stu-id="8de79-169">**Estimated Tax**</span></span> | <span data-ttu-id="8de79-170">उपयोगकर्ता अनुबंध पंक्ति पर अनुमानित कर राशि इनपुट करने के लिए इस फ़ील्ड को संपादित कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-170">The user can edit this field to input the estimated tax amount on the contract line.</span></span> <span data-ttu-id="8de79-171">जब किसी परियोजना-आधारित अनुबंध पंक्ति में पंक्ति विवरण होता है, तो यह फ़ील्ड संपादन के लिए लॉक हो जाती है और अनुबंध पंक्ति विवरण पर कर राशि से सारांशित होती है.</span><span class="sxs-lookup"><span data-stu-id="8de79-171">When a project–based contract line has line details, this field is locked for editing and is summarized from the tax amount on the contract line details.</span></span> | <span data-ttu-id="8de79-172">जब अनुबंध पंक्ति में पंक्ति विवरण होता है, तो यह मान पंक्ति विवरण पर कर राशि को बदलकर संशोधित किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-172">When the contract line has line details, this value can be modified by changing the tax amounts on the line details.</span></span> <span data-ttu-id="8de79-173">एक निश्चित मूल्य अनुबंध पंक्ति पर, इस मान का उपयोग आवधिक बिलिंग माइलस्टोन पर कर को जनरेट करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-173">On a fixed price contract line, this value is used to generate the tax on periodic billing milestones.</span></span> |
| <span data-ttu-id="8de79-174">**कर के बाद अनुबंधित राशि**</span><span class="sxs-lookup"><span data-stu-id="8de79-174">**Contracted Amount after Tax**</span></span> | <span data-ttu-id="8de79-175">कर के बाद अनुबंध पंक्ति राशि.</span><span class="sxs-lookup"><span data-stu-id="8de79-175">The contract line amount after tax.</span></span> <span data-ttu-id="8de79-176">यह फ़ील्ड केवल पढ़ने के लिए है और इसकी गणना **अनुबंधित राशि + कर** के रूप में की जाती है.</span><span class="sxs-lookup"><span data-stu-id="8de79-176">This field is read only and is calculated as **Contracted Amount + Tax**.</span></span> | <span data-ttu-id="8de79-177">एक निश्चित मूल्य अनुबंध पंक्ति पर, इस मान का उपयोग आवधिक बिलिंग माइलस्टोन को जनरेट करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-177">On a fixed price contract line, this value is used to generate periodic billing milestones.</span></span> |
| <span data-ttu-id="8de79-178">**सीमा-में-रखें सीमा**</span><span class="sxs-lookup"><span data-stu-id="8de79-178">**Not-to-Exceed Limit**</span></span> | <span data-ttu-id="8de79-179">उपयोगकर्ता इस फ़ील्ड को संपादित कर सकता है और यह केवल उन परियोजना-आधारित अनुबंध पंक्तियों पर उपलब्ध है, जिनमें समय और सामग्री के रूप में बिलिंग पद्धति सेट होती है.</span><span class="sxs-lookup"><span data-stu-id="8de79-179">The user can edit this field and it is only available on project-based contract lines that have the billing method set as time and material.</span></span> | <span data-ttu-id="8de79-180">उपयोगकर्ता इस फ़ील्ड को संपादित कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-180">The user can edit this field.</span></span> <span data-ttu-id="8de79-181">जब समय और सामग्री के लिए कोई वास्तविक समय और सामग्री हेतु इस अनुबंध पंक्ति को संदर्भित करता है, तो वास्तविक पर राशि का मूल्यांकन अनुबंध रेखा पर सीमा-में-रखें सीमा के विरुद्ध किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-181">When an actual for time and material references this contract line for time and material, the amount on the actual is evaluated against the not-to-exceed limit on the contract line.</span></span> <span data-ttu-id="8de79-182">यह मूल्यांकन पहले से खर्च की गई और प्रतिबद्ध राशि पर ध्यान दिए जाने के बाद पूर्ण होता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-182">This evaluation is completed after  the already spent and committed amounts are accounted for.</span></span> |
| <span data-ttu-id="8de79-183">**ग्राहक बजट**</span><span class="sxs-lookup"><span data-stu-id="8de79-183">**Customer Budget**</span></span> | <span data-ttu-id="8de79-184">यह फ़ील्ड संपादन योग्य है और यदि अनुबंध को कोट से बनाया गया था, तो उसे संगत फ़ील्ड से कोट पंक्ति पर कॉपी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-184">This field is editable and is copied from the corresponding field on the quote line if the contract was created from a quote.</span></span> | <span data-ttu-id="8de79-185">इस फ़ील्ड का उपयोग केवल जानकारी के लिए किया जाता है और इसका कोई महत्व नहीं है.</span><span class="sxs-lookup"><span data-stu-id="8de79-185">This field is only used for information and does not have any downstream significance.</span></span> |

## <a name="validation-rules-for-the-options-on-the-general-tab-of-project-based-contract-lines"></a><span data-ttu-id="8de79-186">परियोजना-आधारित अनुबंध पंक्तियों के सामान्य टैब पर विकल्पों के लिए सत्यापन नियम</span><span class="sxs-lookup"><span data-stu-id="8de79-186">Validation rules for the options on the General tab of project-based contract lines</span></span>

<span data-ttu-id="8de79-187">नियम 1: यदि **शामिल कार्य** फ़ील्ड रिक्त है या **सभी परियोजना कार्य** पर सेट है, तो परियोजना के सभी कार्य अनुबंध पंक्ति में शामिल किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="8de79-187">Rule 1: If the **Included Tasks** field is blank or set to **All Project Tasks**, all tasks of the project are included on the contract line.</span></span>

<span data-ttu-id="8de79-188">नियम 2: जब **शामिल कार्य** फ़ील्ड रिक्त होती है या स्पष्ट रूप से **सभी परियोजना कार्य** पर सेट होती है, तो परियोजना और निश्चित ट्रांज़ैक्शन श्रेणी को केवल अनुबंध की एक परियोजना-आधारित अनुबंध पंक्ति पर शामिल किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-188">Rule 2: When the **Included Tasks** field is blank or explicitly set to **All Project Tasks**, a project and a certain transaction class can only be included on one project-based contract line of a contract.</span></span>

<span data-ttu-id="8de79-189">नियम 3: जब **शामिल कार्य** फ़ील्ड **केवल चयनित परियोजना कार्य** पर सेट होती है, तो परियोजना और निश्चित ट्रांज़ैक्शन श्रेणी को अनुबंध की एकाधिक परियोजना-आधारित अनुबंध पंक्तियों पर शामिल किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-189">Rule 3: When the **Included Tasks** field is set to **Selected Project Tasks Only**, a project and a certain transaction class can be included on multiple project-based contract lines of a contract.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="43" valign="top">
                <p><span data-ttu-id="8de79-190">
                    <strong>संविदा</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8de79-190">
                    <strong>Contract</strong>
                </span></span></p>
            </td>
            <td width="65" valign="top">
                <p><span data-ttu-id="8de79-191">
                    <strong>अनुबंध पंक्ति</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8de79-191">
                    <strong>Contract line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="8de79-192">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8de79-192">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="67" valign="top">
                <p><span data-ttu-id="8de79-193">
                    <strong>शामिल कार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8de79-193">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="8de79-194">
                    <strong>समय शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8de79-194">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="8de79-195">
                    <strong>व्यय शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8de79-195">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="8de79-196">
                    <strong>सामग्री शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8de79-196">
                    <strong>Include Materials</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="8de79-197">
                    <strong>शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8de79-197">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="8de79-198">
                    <strong>शुल्क</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8de79-198">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="53" valign="top">
                <p><span data-ttu-id="8de79-199">
                    <strong>मान्य/ मान्य नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8de79-199">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="250" valign="top">
                <p><span data-ttu-id="8de79-200">
                    <strong>कारण</strong>
                </span><span class="sxs-lookup"><span data-stu-id="8de79-200">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="8de79-201">C1</span><span class="sxs-lookup"><span data-stu-id="8de79-201">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="8de79-202">CL1</span><span class="sxs-lookup"><span data-stu-id="8de79-202">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-203">P1</span><span class="sxs-lookup"><span data-stu-id="8de79-203">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="8de79-204">रिक्त</span><span class="sxs-lookup"><span data-stu-id="8de79-204">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-205">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-205">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-206">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-206">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-207">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-207">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-208">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-208">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8de79-209">मान्य नहीं है</span><span class="sxs-lookup"><span data-stu-id="8de79-209">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8de79-210">नियम #2 का उल्लंघन.</span><span class="sxs-lookup"><span data-stu-id="8de79-210">Violation of Rule #2.</span></span> <span data-ttu-id="8de79-211">P1 परियोजना पर समय, व्यय, सामग्री और शुल्क दोनों कॉन्ट्रैक्ट लाइन CL1 और CL2 पर शामिल किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="8de79-211">Time, Expense, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="8de79-212">C1</span><span class="sxs-lookup"><span data-stu-id="8de79-212">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="8de79-213">CL2</span><span class="sxs-lookup"><span data-stu-id="8de79-213">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-214">P1</span><span class="sxs-lookup"><span data-stu-id="8de79-214">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="8de79-215">रिक्त</span><span class="sxs-lookup"><span data-stu-id="8de79-215">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-216">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-216">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-217">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-217">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-218">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-218">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-219">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-219">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="8de79-220">C1</span><span class="sxs-lookup"><span data-stu-id="8de79-220">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="8de79-221">CL1</span><span class="sxs-lookup"><span data-stu-id="8de79-221">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-222">P1</span><span class="sxs-lookup"><span data-stu-id="8de79-222">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="8de79-223">रिक्त</span><span class="sxs-lookup"><span data-stu-id="8de79-223">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-224">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-224">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-225">No</span><span class="sxs-lookup"><span data-stu-id="8de79-225">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-226">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-226">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-227">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-227">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8de79-228">मान्य नहीं है</span><span class="sxs-lookup"><span data-stu-id="8de79-228">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8de79-229">नियम #2 का उल्लंघन.</span><span class="sxs-lookup"><span data-stu-id="8de79-229">Violation of Rule #2.</span></span> <span data-ttu-id="8de79-230">P1 परियोजना पर समय, सामग्री और शुल्क दोनों कॉन्ट्रैक्ट लाइन CL1 और CL2 पर शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="8de79-230">Time, Materials, and Fees on P1 project are included on both Contract lines CL1 and CL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="8de79-231">C1</span><span class="sxs-lookup"><span data-stu-id="8de79-231">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="8de79-232">CL2</span><span class="sxs-lookup"><span data-stu-id="8de79-232">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-233">P1</span><span class="sxs-lookup"><span data-stu-id="8de79-233">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="8de79-234">रिक्त</span><span class="sxs-lookup"><span data-stu-id="8de79-234">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-235">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-235">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-236">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-236">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-237">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-237">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-238">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-238">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="8de79-239">C1</span><span class="sxs-lookup"><span data-stu-id="8de79-239">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="8de79-240">CL1</span><span class="sxs-lookup"><span data-stu-id="8de79-240">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-241">P1</span><span class="sxs-lookup"><span data-stu-id="8de79-241">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="8de79-242">रिक्त</span><span class="sxs-lookup"><span data-stu-id="8de79-242">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-243">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-243">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-244">No</span><span class="sxs-lookup"><span data-stu-id="8de79-244">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-245">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-245">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-246">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-246">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8de79-247">मान्य</span><span class="sxs-lookup"><span data-stu-id="8de79-247">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8de79-248">P1 प्रोजेक्ट पर समय, सामग्री और शुल्क CL1 पर शामिल किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="8de79-248">Time, Materials, and Fees on P1 project are included on CL1.</span></span>
                </p>
                <ul>
                    <li>
<span data-ttu-id="8de79-249">P1 परियोजना पर ख़र्च CL2 पर शामिल है.</span><span class="sxs-lookup"><span data-stu-id="8de79-249">Expense on P1 project is included on CL2.</span></span>
                    </li>
                </ul>
                <p>
<span data-ttu-id="8de79-250">प्रत्येक कॉन्ट्रैक्ट लाइन पर जो शामिल किया जा रहा है उनमें ओवरलैप नहीं होता है इसलिए मान्य है.</span><span class="sxs-lookup"><span data-stu-id="8de79-250">No overlap in what is being included on each Contract line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="8de79-251">C1</span><span class="sxs-lookup"><span data-stu-id="8de79-251">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="8de79-252">CL2</span><span class="sxs-lookup"><span data-stu-id="8de79-252">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-253">P1</span><span class="sxs-lookup"><span data-stu-id="8de79-253">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="8de79-254">रिक्त</span><span class="sxs-lookup"><span data-stu-id="8de79-254">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-255">No</span><span class="sxs-lookup"><span data-stu-id="8de79-255">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-256">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-257">No</span><span class="sxs-lookup"><span data-stu-id="8de79-257">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-258">No</span><span class="sxs-lookup"><span data-stu-id="8de79-258">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="8de79-259">C1</span><span class="sxs-lookup"><span data-stu-id="8de79-259">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="8de79-260">CL1</span><span class="sxs-lookup"><span data-stu-id="8de79-260">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-261">P1</span><span class="sxs-lookup"><span data-stu-id="8de79-261">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="8de79-262">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="8de79-262">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-263">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-263">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-264">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-264">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-265">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-266">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-266">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8de79-267">मान्य नहीं है</span><span class="sxs-lookup"><span data-stu-id="8de79-267">Not valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8de79-268">नियम #2 का उल्लंघन</span><span class="sxs-lookup"><span data-stu-id="8de79-268">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="8de79-269">C1 परियोजना P1 पर कार्यों के सबसेट पर समय, सामग्री, व्यय और शुल्क को शामिल करता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-269">C1 includes Time, Materials, Expenses and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="8de79-270">CL2 पूरी परियोजना P1 के लिए समय, सामग्री, व्यय और शुल्क को शामिल करता है और इसलिए C1 पर जो भी शामिल किए जाते हैं उससे ओवरलैप करता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-270">CL2 includes Time, Materials, Expenses and Fees for the whole project P1 and therefore overlaps with what is included on C1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="8de79-271">C1</span><span class="sxs-lookup"><span data-stu-id="8de79-271">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="8de79-272">CL2</span><span class="sxs-lookup"><span data-stu-id="8de79-272">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-273">P1</span><span class="sxs-lookup"><span data-stu-id="8de79-273">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="8de79-274">रिक्त</span><span class="sxs-lookup"><span data-stu-id="8de79-274">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-275">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-275">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-276">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-276">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-277">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-278">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-278">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
            </td>
            <td width="65" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="67" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="53" valign="top">
            </td>
            <td width="250" valign="top">
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="8de79-279">C1</span><span class="sxs-lookup"><span data-stu-id="8de79-279">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="8de79-280">CL1</span><span class="sxs-lookup"><span data-stu-id="8de79-280">CL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-281">P1</span><span class="sxs-lookup"><span data-stu-id="8de79-281">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="8de79-282">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="8de79-282">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-283">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-283">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-284">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-284">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-285">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-285">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-286">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-286">Yes</span></span> </p>
            </td>
            <td width="53" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8de79-287">मान्य</span><span class="sxs-lookup"><span data-stu-id="8de79-287">Valid</span></span> </p>
            </td>
            <td width="250" rowspan="2" valign="top">
                <p>
<span data-ttu-id="8de79-288">प्रति नियम #3</span><span class="sxs-lookup"><span data-stu-id="8de79-288">Per Rule #3</span></span> </p>
                <p>
<span data-ttu-id="8de79-289">C1 परियोजना P1 पर कार्यों के सबसेट के लिए समय, व्यय, सामग्री और शुल्क को शामिल करता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-289">C1 includes Time, Expenses, Materials, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="8de79-290">CL2 परियोजना P1 पर कार्यों के सबसेट के लिए समय, व्यय, सामग्री, और शुल्क को शामिल करता है.</span><span class="sxs-lookup"><span data-stu-id="8de79-290">CL2 includes Time, Expenses, Materials, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="8de79-291">CL1 पर कार्यों के सबसेट के आसपास एकमात्र अतिरिक्त सत्यापन CL2 पर कार्यों के सबसेट से अलग है ताकि यह सुनिश्चित हो सके कि वहां कोई ओवरलैप नहीं हैं.</span><span class="sxs-lookup"><span data-stu-id="8de79-291">The only additional validation is around the subset of tasks on CL1 is different from the subset of tasks on CL2 to ensure that there are no overlaps there.</span></span> <span data-ttu-id="8de79-292">यह सिस्टम द्वारा किया जाता है जब कार्य संबध्द होते हैं.</span><span class="sxs-lookup"><span data-stu-id="8de79-292">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="8de79-293">C1</span><span class="sxs-lookup"><span data-stu-id="8de79-293">C1</span></span> </p>
            </td>
            <td width="65" valign="top">
                <p>
<span data-ttu-id="8de79-294">CL2</span><span class="sxs-lookup"><span data-stu-id="8de79-294">CL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-295">P1</span><span class="sxs-lookup"><span data-stu-id="8de79-295">P1</span></span> </p>
            </td>
            <td width="67" valign="top">
                <p>
<span data-ttu-id="8de79-296">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="8de79-296">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-297">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-297">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="8de79-298">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-298">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-299">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-299">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="8de79-300">हाँ</span><span class="sxs-lookup"><span data-stu-id="8de79-300">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
