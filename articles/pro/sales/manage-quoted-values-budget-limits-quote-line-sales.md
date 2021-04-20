---
title: परियोजना-आधारित कोट पंक्तियाँ ओवरव्यू
description: यह विषय परियोजना कार्य के लिए परियोजना-आधारित कोटेशन लाइनों का उपयोग करने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 03/30/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: cfe98fc89130c93dd0a36af8583881fdcb4550c0
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/06/2021
ms.locfileid: "5858700"
---
# <a name="project-based-quote-lines-overview"></a><span data-ttu-id="02f43-103">परियोजना-आधारित कोट पंक्तियाँ ओवरव्यू</span><span class="sxs-lookup"><span data-stu-id="02f43-103">Project-based quote lines overview</span></span> 

<span data-ttu-id="02f43-104">लाइट तैनाती _**पर लागू होता है:** प्रोफार्मा इनवॉइस करने के लिए - डील, संसाधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations_</span><span class="sxs-lookup"><span data-stu-id="02f43-104">_**Applies To:** Lite deployment - deal to proforma invoicing, Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="02f43-105">परियोजना-आधारित कोटेशन लाइनों को एक सगाई पर परियोजना के काम का अनुमान लगाने में मदद करने के लिए डिज़ाइन कर रहे हैं.</span><span class="sxs-lookup"><span data-stu-id="02f43-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="02f43-106">परियोजना-आधारित कोटेशन लाइन की संरचना को निम्नलिखित अवधारणाओं के साथ परियोजना अनुमानों के लिए बढ़ाया गया है:</span><span class="sxs-lookup"><span data-stu-id="02f43-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="02f43-107">बिलिंग विधि</span><span class="sxs-lookup"><span data-stu-id="02f43-107">Billing Method</span></span>
- <span data-ttu-id="02f43-108">प्रोजेक्ट और टास्क मैपिंग</span><span class="sxs-lookup"><span data-stu-id="02f43-108">Project and Task Mapping</span></span>
- <span data-ttu-id="02f43-109">शामिल लेनदेन कक्षाएं</span><span class="sxs-lookup"><span data-stu-id="02f43-109">Included Transaction classes</span></span>
- <span data-ttu-id="02f43-110">सीमा-में रखें सीमा</span><span class="sxs-lookup"><span data-stu-id="02f43-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="02f43-111">प्रभार्यता सेटअप</span><span class="sxs-lookup"><span data-stu-id="02f43-111">Chargeability setup</span></span>
- <span data-ttu-id="02f43-112">कोटेशन लाइन विवरणों का उपयोग करके अनुमान लगाना</span><span class="sxs-lookup"><span data-stu-id="02f43-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="02f43-113">कोट पंक्ति ग्राहक</span><span class="sxs-lookup"><span data-stu-id="02f43-113">Quote line Customers</span></span>

<span data-ttu-id="02f43-114">निम्नलिखित तालिका परियोजना-आधारित कोटेशन लाइन के **सामान्य** टैब पर फ़ील्ड के बारे में जानकारी प्रदान करती है.</span><span class="sxs-lookup"><span data-stu-id="02f43-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="02f43-115">ये फ़ील्ड परियोजना कार्य के लिए विस्तृत, बुनियादी अनुमान के आधार सेट करने में मदद करते हैं.</span><span class="sxs-lookup"><span data-stu-id="02f43-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="02f43-116">**फ़ील्ड**</span><span class="sxs-lookup"><span data-stu-id="02f43-116">**Field**</span></span> | <span data-ttu-id="02f43-117">**विवरण**</span><span class="sxs-lookup"><span data-stu-id="02f43-117">**Description**</span></span> | <span data-ttu-id="02f43-118">**डाउनस्ट्रीम प्रभाव**</span><span class="sxs-lookup"><span data-stu-id="02f43-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="02f43-119">नाम</span><span class="sxs-lookup"><span data-stu-id="02f43-119">Name</span></span> | <span data-ttu-id="02f43-120">कोट लाइन का नाम जो आपको अनुमान लगाए गए कोट के अलग घटक की पहचान करने में मदद करता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-120">The name of quote line that helps you to identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="02f43-121">कोटेशन जीतने के बाद इस कोटेशन लाइन से बनाए गए परियोजना अनुबंध लाइन में कॉपी किया गया.</span><span class="sxs-lookup"><span data-stu-id="02f43-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="02f43-122">बिलिंग विधि</span><span class="sxs-lookup"><span data-stu-id="02f43-122">Billing Method</span></span> | <span data-ttu-id="02f43-123">एक अवसर से बनाई गई कोटेशन पर, इस मूल्य को अवसर लाइन पर संबंधित फ़ील्ड से कॉपी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="02f43-124">इस फ़ील्ड में Dynamics 365 Project Operations समर्थित दो मुख्य अनुबंध मॉडल शामिल हैं:</span><span class="sxs-lookup"><span data-stu-id="02f43-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="02f43-125">- निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="02f43-125">- Fixed price</span></span></br><span data-ttu-id="02f43-126">- समय और सामग्री.</span><span class="sxs-lookup"><span data-stu-id="02f43-126">- Time and material.</span></span>| <span data-ttu-id="02f43-127">इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-127">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="02f43-128">Project</span><span class="sxs-lookup"><span data-stu-id="02f43-128">Project</span></span> | <span data-ttu-id="02f43-129">इस वैकल्पिक फ़ील्ड का उपयोग परियोजना की पहचान करने में करें जिसका उपयोग इस अनुबंध पर कार्य निष्पादन के लिए किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="02f43-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="02f43-130">जब किसी परियोजना का कोटेशन लाइन में मानचित्रण किया जाता है, तो यह देय योग्य कार्यों को सेट करने और कोटेशन लाइन विवरणों के रूप में कोटेशन लाइन पर परियोजना-आधारित अनुमान को उत्पन्न करने में भी मदद करता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="02f43-131">जब किसी परियोजना का परियोजना-आधारित कोटेशन लाइन पर मानचित्रण नहीं किया जाता है, तो प्रत्येक कोटेशन लाइन विवरण बनाकर मैन्युअल रूप से अनुमान बनाया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="02f43-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="02f43-132">इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-132">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="02f43-133">शामिल कार्य</span><span class="sxs-lookup"><span data-stu-id="02f43-133">Included Tasks</span></span> | <span data-ttu-id="02f43-134">इंगित करता है कि क्या इस कोटेशन लाइन का उपयोग चयनित परियोजना के लिए सभी या कुछ परियोजना कार्यों के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-134">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="02f43-135">इस फ़ील्ड में निम्नलिखित संभावित मान हैं:</span><span class="sxs-lookup"><span data-stu-id="02f43-135">This field has the following possible values:</span></span></br><span data-ttu-id="02f43-136">- सभी परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="02f43-136">- All project tasks</span></span></br><span data-ttu-id="02f43-137">- केवल चयनित परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="02f43-137">- Selected project tasks only</span></span></br><span data-ttu-id="02f43-138">इस फ़ील्ड में एक खाली मान **सभी परियोजना कार्य** विकल्प के समान है.</span><span class="sxs-lookup"><span data-stu-id="02f43-138">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="02f43-139">जब **केवल चयनित परियोजना कार्य** को परियोजना पेज पर चुना जाता है, तो **कार्य बिलिंग सेटअप** टैब आपको इस कोट लाइन से संबद्ध करने के लिए विशिष्ट कार्यों का चयन करने की अनुमति देता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-139">When **Selected project tasks only** is selected on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="02f43-140">इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-140">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="02f43-141">समय शामिल करें</span><span class="sxs-lookup"><span data-stu-id="02f43-141">Include Time</span></span> | <span data-ttu-id="02f43-142">यदि इस कोट लाइन पर अनुमान में लेन-देन या श्रम की लागत को चुनी गई परियोजना में शामिल किया जाएगा तो **हां**/**नहीं** मान इंगित होता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-142">A **Yes**/**No** value indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="02f43-143">एक **नहीं** मान इंगित करता है कि समय की लेनदेन या श्रम लागत इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="02f43-143">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="02f43-144">एक **हाँ** मान इंगित करता है कि समय की लेनदेन या श्रम लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="02f43-144">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="02f43-145">इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-145">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="02f43-146">व्यय शामिल करें</span><span class="sxs-lookup"><span data-stu-id="02f43-146">Include Expense</span></span> | <span data-ttu-id="02f43-147">यदि इस कोट लाइन पर अनुमान में लेन-देन या व्यय की लागत को चुनी गई परियोजना में शामिल किया जाएगा तो **हां**/**नहीं** मान इंगित होता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-147">A **Yes**/**No** value indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="02f43-148">एक **नहीं** मान इंगित करता है कि ख़र्च लागत इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="02f43-148">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="02f43-149">एक **हाँ** मान इंगित करता है कि ख़र्च लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="02f43-149">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="02f43-150">इस मान को परियोजना कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-150">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="02f43-151">सामग्री शामिल करें</span><span class="sxs-lookup"><span data-stu-id="02f43-151">Include Material</span></span> | <span data-ttu-id="02f43-152">यदि इस कोट लाइन पर अनुमान में लेन-देन या सामग्री लागत को चुनी गई परियोजना में शामिल किया जाएगा तो **हां**/**नहीं** मान इंगित होता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-152">A **Yes**/**No** value indicates if material costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="02f43-153">**नहीं** मान इंगित करता है कि सामग्री की लागत को इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="02f43-153">A **No** value indicates that the material costs will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="02f43-154">एक **हां** मान इंगित करता है कि सामग्री की लागत को इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="02f43-154">A **Yes** value indicates that the material costs will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="02f43-155">इस मान को परियोजना कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-155">This value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="02f43-156">शुल्क शामिल करें</span><span class="sxs-lookup"><span data-stu-id="02f43-156">Include Fee</span></span> | <span data-ttu-id="02f43-157">यदि इस कोट लाइन पर अनुमान में लेन-देन या शुल्क को चुनी गई परियोजना में शामिल किया जाएगा तो **हां**/**नहीं** मान इंगित होता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-157">A **Yes**/**No** value indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="02f43-158">एक **नहीं** मान इंगित करता है कि शुल्क को इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="02f43-158">A **No** value indicates that the fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="02f43-159">एक **हाँ** मान इंगित करता है कि शुल्क को इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="02f43-159">A **Yes** value indicates that the fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="02f43-160">इस मान को परियोजना कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-160">This value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="02f43-161">कोट की गई राशि</span><span class="sxs-lookup"><span data-stu-id="02f43-161">Quoted Amount</span></span> | <span data-ttu-id="02f43-162">यह वह राशि है जिसे इस परियोजना-आधारित कोट लाइन पर पूर्वानुमानित सभी कार्यों के लिए ग्राहक को कोट किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="02f43-162">This is the amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="02f43-163">एक अवसर से बनाई गई कोटेशन पर, इस मान को अवसर लाइन पर **ग्राहक बजट** फ़ील्ड से कॉपी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-163">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="02f43-164">जब परियोजना-आधारित कोटेशन लाइन में लाइन विवरण होते हैं, तो इस फ़ील्ड को संपादन के लिए लॉक कर दिया जाता है और कोटेशन लाइन विवरणों पर दर्ज राशि से संक्षेपित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-164">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="02f43-165">इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-165">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="02f43-166">अनुमानित कर</span><span class="sxs-lookup"><span data-stu-id="02f43-166">Estimated Tax</span></span> | <span data-ttu-id="02f43-167">यह उपयोगकर्ता के लिए कोटेशन लाइन पर अनुमानित कर राशि जोड़ने के लिए एक संपादन योग्य फ़ील्ड है.</span><span class="sxs-lookup"><span data-stu-id="02f43-167">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="02f43-168">जब किसी परियोजना-आधारित कोटेशन लाइन में लाइन विवरण होते हैं, तो इस फ़ील्ड को संपादन के लिए लॉक कर दिया जाता है और कोटेशन लाइन विवरणों पर दर्ज कर राशि से संक्षेपित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-168">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="02f43-169">इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-169">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="02f43-170">कर के बाद कोट की गई राशि</span><span class="sxs-lookup"><span data-stu-id="02f43-170">Quoted Amount after Tax</span></span> | <span data-ttu-id="02f43-171">कर के बाद यह फ़ील्ड कोटेशन लाइन राशि है और केवल पढ़ी जाती है.</span><span class="sxs-lookup"><span data-stu-id="02f43-171">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="02f43-172">इस फ़ील्ड में राशि की गणना *क्वोट की गई राशि + कर* के रूप में की जाती है.</span><span class="sxs-lookup"><span data-stu-id="02f43-172">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="02f43-173">इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-173">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="02f43-174">सीमा-में रखें सीमा</span><span class="sxs-lookup"><span data-stu-id="02f43-174">Not-to-exceed Limit</span></span> | <span data-ttu-id="02f43-175">यह फ़ील्ड संपादन योग्य है और केवल परियोजना-आधारित कोटेशन लाइनों पर उपलब्ध है जिसमें **समय और सामग्री** बिलिंग विधि है.</span><span class="sxs-lookup"><span data-stu-id="02f43-175">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="02f43-176">इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-176">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="02f43-177">ग्राहक बजट</span><span class="sxs-lookup"><span data-stu-id="02f43-177">Customer Budget</span></span> | <span data-ttu-id="02f43-178">यह फ़ील्ड संपादन योग्य है और यदि कोटेशन एक अवसर से बनाया गया था तो अवसर लाइन पर संबंधित फ़ील्ड से कॉपी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-178">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="02f43-179">इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-179">This value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="02f43-180">परियोजना-आधारित कोटेशन लाइनों के सामान्य टैब पर फ़ील्डों के लिए सत्यापन नियम</span><span class="sxs-lookup"><span data-stu-id="02f43-180">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="02f43-181">**नियम 1**: यदि **शामिल किए गए कार्य** फ़ील्ड खाली है, या यदि यह **सभी परियोजना कार्य** के लिए सेट है, तो कोटेशन लाइन में एक परियोजना शामिल की जाती है.</span><span class="sxs-lookup"><span data-stu-id="02f43-181">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="02f43-182">**नियम 2**: यदि **शामिल किए गए कार्य** फ़ील्ड खाली है, या यदि यह **सभी परियोजना कार्य** के लिए सेट है, तो केवल कोटेशन की परियोजना-आधारित एक कोटेशन लाइन पर एक परियोजना और एक निश्चित लेनदेन वर्ग को शामिल किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-182">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="02f43-183">**नियम 3**: यदि **शामिल किए गए कार्य** फ़ील्ड को **केवल चयनित परियोजना कार्य** के लिए सेट किया गया है, तो एक परियोजना और एक निश्चित लेनदेन वर्ग को कोटेशन की परियोजना-आधारित कई कोटेशन लाइनों पर शामिल किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-183">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="02f43-184">**नियम 4**: यदि किसी अवसर में कई कोटेशन हैं, तो विभिन्न कोटेशनों से कोटेशन लाइनें हो सकती हैं जो सभी एक ही परियोजना का संदर्भ देती हैं और एक ही लेनदेन वर्ग को शामिल करती हैं.</span><span class="sxs-lookup"><span data-stu-id="02f43-184">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="02f43-185">**नियम 5**: यदि कोटेशन उसी समान अवसर से संबंधित नहीं हैं, तो वे समान परियोजना और लेनदेन वर्ग को शामिल नहीं कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="02f43-185">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p><span data-ttu-id="02f43-186">
                    <strong>अवसर</strong>
                </span><span class="sxs-lookup"><span data-stu-id="02f43-186">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="39" valign="top">
                <p><span data-ttu-id="02f43-187">
                    <strong>कोट</strong>
                </span><span class="sxs-lookup"><span data-stu-id="02f43-187">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="40" valign="top">
                <p><span data-ttu-id="02f43-188">
                    <strong>कोट पंक्ति</strong>
                </span><span class="sxs-lookup"><span data-stu-id="02f43-188">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="02f43-189">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="02f43-189">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="77" valign="top">
                <p><span data-ttu-id="02f43-190">
                    <strong>शामिल कार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="02f43-190">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="45" valign="top">
                <p><span data-ttu-id="02f43-191">
                    <strong>समय शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="02f43-191">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="46" valign="top">
                <p><span data-ttu-id="02f43-192">
                    <strong>व्यय शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="02f43-192">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="43" valign="top">
                <p><span data-ttu-id="02f43-193">
                    <strong>सामग्री शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="02f43-193">
                    <strong>Include Material</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="02f43-194">
                    <strong>शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="02f43-194">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="02f43-195">
                    <strong>शुल्क</strong>
                </span><span class="sxs-lookup"><span data-stu-id="02f43-195">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="49" valign="top">
                <p><span data-ttu-id="02f43-196">
                    <strong>मान्य/ मान्य नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="02f43-196">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="200" valign="top">
                <p><span data-ttu-id="02f43-197">
                    <strong>कारण</strong>
                </span><span class="sxs-lookup"><span data-stu-id="02f43-197">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="02f43-198">O1</span><span class="sxs-lookup"><span data-stu-id="02f43-198">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="02f43-199">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="02f43-199">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="02f43-200">QL1</span><span class="sxs-lookup"><span data-stu-id="02f43-200">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-201">P1</span><span class="sxs-lookup"><span data-stu-id="02f43-201">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="02f43-202">रिक्त</span><span class="sxs-lookup"><span data-stu-id="02f43-202">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="02f43-203">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-203">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="02f43-204">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-204">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="02f43-205">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-205">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-206">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-206">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="02f43-207">मान्य नहीं है</span><span class="sxs-lookup"><span data-stu-id="02f43-207">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="02f43-208">नियम #2 का उल्लंघन.</span><span class="sxs-lookup"><span data-stu-id="02f43-208">Violation of Rule #2.</span></span> <span data-ttu-id="02f43-209">P1 परियोजना पर समय, ख़र्च और शुल्क कोटेशन लाइनों QL1 और QL2 पर शामिल हैं</span><span class="sxs-lookup"><span data-stu-id="02f43-209">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="02f43-210">O1</span><span class="sxs-lookup"><span data-stu-id="02f43-210">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="02f43-211">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="02f43-211">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="02f43-212">QL2</span><span class="sxs-lookup"><span data-stu-id="02f43-212">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-213">P1</span><span class="sxs-lookup"><span data-stu-id="02f43-213">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="02f43-214">रिक्त</span><span class="sxs-lookup"><span data-stu-id="02f43-214">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="02f43-215">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-215">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="02f43-216">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-216">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="02f43-217">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-217">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-218">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-218">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="02f43-219">O1</span><span class="sxs-lookup"><span data-stu-id="02f43-219">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="02f43-220">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="02f43-220">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="02f43-221">QL1</span><span class="sxs-lookup"><span data-stu-id="02f43-221">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-222">P1</span><span class="sxs-lookup"><span data-stu-id="02f43-222">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="02f43-223">रिक्त</span><span class="sxs-lookup"><span data-stu-id="02f43-223">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="02f43-224">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-224">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="02f43-225">No</span><span class="sxs-lookup"><span data-stu-id="02f43-225">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="02f43-226">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-226">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-227">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-227">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="02f43-228">मान्य नहीं है</span><span class="sxs-lookup"><span data-stu-id="02f43-228">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="02f43-229">नियम #2 का उल्लंघन.</span><span class="sxs-lookup"><span data-stu-id="02f43-229">Violation of Rule #2.</span></span> <span data-ttu-id="02f43-230">P1 परियोजना पर समय, सामग्री और शुल्क कोटेशन लाइनों QL1 और QL2 पर शामिल हैं</span><span class="sxs-lookup"><span data-stu-id="02f43-230">Time, Material, and Fees on P1 project are included on quote lines QL1 and QL2</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="02f43-231">O1</span><span class="sxs-lookup"><span data-stu-id="02f43-231">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="02f43-232">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="02f43-232">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="02f43-233">QL2</span><span class="sxs-lookup"><span data-stu-id="02f43-233">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-234">P1</span><span class="sxs-lookup"><span data-stu-id="02f43-234">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="02f43-235">रिक्त</span><span class="sxs-lookup"><span data-stu-id="02f43-235">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="02f43-236">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-236">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="02f43-237">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-237">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="02f43-238">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-238">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-239">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-239">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="02f43-240">O1</span><span class="sxs-lookup"><span data-stu-id="02f43-240">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="02f43-241">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="02f43-241">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="02f43-242">QL1</span><span class="sxs-lookup"><span data-stu-id="02f43-242">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-243">P1</span><span class="sxs-lookup"><span data-stu-id="02f43-243">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="02f43-244">रिक्त</span><span class="sxs-lookup"><span data-stu-id="02f43-244">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="02f43-245">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-245">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="02f43-246">No</span><span class="sxs-lookup"><span data-stu-id="02f43-246">No</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="02f43-247">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-247">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-248">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-248">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="02f43-249">मान्य</span><span class="sxs-lookup"><span data-stu-id="02f43-249">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="02f43-250">P1 परियोजना पर समय, सामग्री और शुल्क QL1 पर शामिल हैं</span><span class="sxs-lookup"><span data-stu-id="02f43-250">Time, Material, and Fees on P1 project are included on QL1</span></span> <br>
<span data-ttu-id="02f43-251">P1 परियोजना पर ख़र्च QL2 पर शामिल है</span><span class="sxs-lookup"><span data-stu-id="02f43-251">Expense on P1 project is included on QL2</span></span> <br>
<span data-ttu-id="02f43-252">प्रत्येक कोट लाइन पर जो कुछ भी शामिल किया जा रहा है उनमें ओवरलैप नहीं है और इसलिए मान्य है.</span><span class="sxs-lookup"><span data-stu-id="02f43-252">No overlap in what is being included on each quote line and therefore valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="02f43-253">O1</span><span class="sxs-lookup"><span data-stu-id="02f43-253">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="02f43-254">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="02f43-254">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="02f43-255">QL2</span><span class="sxs-lookup"><span data-stu-id="02f43-255">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-256">P1</span><span class="sxs-lookup"><span data-stu-id="02f43-256">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="02f43-257">रिक्त</span><span class="sxs-lookup"><span data-stu-id="02f43-257">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="02f43-258">No</span><span class="sxs-lookup"><span data-stu-id="02f43-258">No</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="02f43-259">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-259">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="02f43-260">No</span><span class="sxs-lookup"><span data-stu-id="02f43-260">No</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-261">No</span><span class="sxs-lookup"><span data-stu-id="02f43-261">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="02f43-262">O1</span><span class="sxs-lookup"><span data-stu-id="02f43-262">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="02f43-263">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="02f43-263">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="02f43-264">QL1</span><span class="sxs-lookup"><span data-stu-id="02f43-264">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-265">P1</span><span class="sxs-lookup"><span data-stu-id="02f43-265">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="02f43-266">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="02f43-266">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="02f43-267">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-267">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="02f43-268">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-268">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="02f43-269">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-269">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-270">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-270">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="02f43-271">मान्य नहीं है</span><span class="sxs-lookup"><span data-stu-id="02f43-271">Not valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="02f43-272">नियम #2 का उल्लंघन</span><span class="sxs-lookup"><span data-stu-id="02f43-272">Violation of Rule #2</span></span> </p>
                <p>
<span data-ttu-id="02f43-273">Q1 परियोजना P1 पर कार्यों के सबसेट पर समय, सामग्री, व्यय और शुल्क को शामिल करता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-273">Q1 includes Time, Material, Expenses and Fees on a subset of tasks on project P1</span></span> </p>
                <p>
<span data-ttu-id="02f43-274">QL2 में पूरे परियोजना P1 के लिए समय, व्यय और शुल्क शामिल है और इसलिए Q1 में जो भी शामिल है, उसके साथ ओवरलैप होता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-274">QL2 includes Time, Expenses, and Fees for the whole project P1 and therefore overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="02f43-275">O1</span><span class="sxs-lookup"><span data-stu-id="02f43-275">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="02f43-276">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="02f43-276">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="02f43-277">QL2</span><span class="sxs-lookup"><span data-stu-id="02f43-277">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-278">P1</span><span class="sxs-lookup"><span data-stu-id="02f43-278">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="02f43-279">रिक्त</span><span class="sxs-lookup"><span data-stu-id="02f43-279">Blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="02f43-280">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-280">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="02f43-281">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-281">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="02f43-282">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-282">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-283">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-283">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="02f43-284">O1</span><span class="sxs-lookup"><span data-stu-id="02f43-284">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="02f43-285">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="02f43-285">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="02f43-286">QL1</span><span class="sxs-lookup"><span data-stu-id="02f43-286">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-287">P1</span><span class="sxs-lookup"><span data-stu-id="02f43-287">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="02f43-288">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="02f43-288">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="02f43-289">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-289">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="02f43-290">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-290">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="02f43-291">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-291">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-292">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-292">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="02f43-293">मान्य</span><span class="sxs-lookup"><span data-stu-id="02f43-293">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="02f43-294">प्रति नियम #3,</span><span class="sxs-lookup"><span data-stu-id="02f43-294">Per Rule #3,</span></span> </p>
                <p>
<span data-ttu-id="02f43-295">Q1 परियोजना P1 पर कार्यों के सबसेट पर समय, सामग्री, व्यय और शुल्क को शामिल करता है.</span><span class="sxs-lookup"><span data-stu-id="02f43-295">Q1 includes Time, Material, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="02f43-296">QL2 में परियोजना P1 पर कार्यों के सबसेट के लिए समय, सामग्री, व्यय और शुल्क शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="02f43-296">QL2 includes Time, Material, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="02f43-297">एकमात्र अतिरिक्त सत्यापन QL1 पर कार्यों के सबसेट के आसपास है जो QL2 पर कार्यों के सबसेट से अलग है ताकि यह सुनिश्चित किया जा सके कि कोई ओवरलैप नहीं है.</span><span class="sxs-lookup"><span data-stu-id="02f43-297">The only additional validation is around the subset of tasks on QL1 which is different from the subset of tasks on QL2 to ensure that there is no overlap.</span></span> <span data-ttu-id="02f43-298">यह सिस्टम द्वारा किया जाता है जब कार्य संबध्द होते हैं.</span><span class="sxs-lookup"><span data-stu-id="02f43-298">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="02f43-299">O1</span><span class="sxs-lookup"><span data-stu-id="02f43-299">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="02f43-300">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="02f43-300">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="02f43-301">QL2</span><span class="sxs-lookup"><span data-stu-id="02f43-301">QL2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-302">P1</span><span class="sxs-lookup"><span data-stu-id="02f43-302">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="02f43-303">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="02f43-303">Selected tasks only</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="02f43-304">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-304">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="02f43-305">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-305">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="02f43-306">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-306">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-307">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-307">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="02f43-308">O1</span><span class="sxs-lookup"><span data-stu-id="02f43-308">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="02f43-309">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="02f43-309">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="02f43-310">QL1</span><span class="sxs-lookup"><span data-stu-id="02f43-310">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-311">P1</span><span class="sxs-lookup"><span data-stu-id="02f43-311">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="02f43-312">सभी परियोजना कार्य या रिक्त</span><span class="sxs-lookup"><span data-stu-id="02f43-312">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="02f43-313">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-313">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="02f43-314">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-314">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="02f43-315">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-315">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-316">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-316">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="02f43-317">मान्य</span><span class="sxs-lookup"><span data-stu-id="02f43-317">Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="02f43-318">नियम #5 के अनुसार, Q1 और Q2 एक ही अवसर पर दो कोट हैं, इसलिए वे दोनों एक परियोजना के एक जैसे घटकों के लिए अनुमान लगा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="02f43-318">Per Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="02f43-319">O1</span><span class="sxs-lookup"><span data-stu-id="02f43-319">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="02f43-320">तिमाही 2</span><span class="sxs-lookup"><span data-stu-id="02f43-320">Q2</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="02f43-321">QL1</span><span class="sxs-lookup"><span data-stu-id="02f43-321">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-322">P1</span><span class="sxs-lookup"><span data-stu-id="02f43-322">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="02f43-323">सभी परियोजना कार्य या रिक्त</span><span class="sxs-lookup"><span data-stu-id="02f43-323">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="02f43-324">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-324">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="02f43-325">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-325">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="02f43-326">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-326">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-327">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-327">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="02f43-328">O1</span><span class="sxs-lookup"><span data-stu-id="02f43-328">O1</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="02f43-329">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="02f43-329">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="02f43-330">QL1</span><span class="sxs-lookup"><span data-stu-id="02f43-330">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-331">P1</span><span class="sxs-lookup"><span data-stu-id="02f43-331">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="02f43-332">सभी परियोजना कार्य या रिक्त</span><span class="sxs-lookup"><span data-stu-id="02f43-332">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="02f43-333">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-333">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="02f43-334">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-334">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="02f43-335">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-335">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-336">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-336">Yes</span></span> </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
<span data-ttu-id="02f43-337">मान्य नहीं है</span><span class="sxs-lookup"><span data-stu-id="02f43-337">Not Valid</span></span> </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
<span data-ttu-id="02f43-338">नियम #4 के अनुसार, Q1 और Q2 विभिन्न अवसरों पर दो कोटेशन हैं, इसलिए वे एक ही परियोजना के एक जैसे घटकों के लिए अनुमान नहीं लगा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="02f43-338">Per Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
<span data-ttu-id="02f43-339">O2</span><span class="sxs-lookup"><span data-stu-id="02f43-339">O2</span></span> </p>
            </td>
            <td width="39" valign="top">
                <p>
<span data-ttu-id="02f43-340">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="02f43-340">Q1</span></span> </p>
            </td>
            <td width="40" valign="top">
                <p>
<span data-ttu-id="02f43-341">QL1</span><span class="sxs-lookup"><span data-stu-id="02f43-341">QL1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-342">P1</span><span class="sxs-lookup"><span data-stu-id="02f43-342">P1</span></span> </p>
            </td>
            <td width="77" valign="top">
                <p>
<span data-ttu-id="02f43-343">सभी परियोजना कार्य या रिक्त</span><span class="sxs-lookup"><span data-stu-id="02f43-343">All project tasks or blank</span></span> </p>
            </td>
            <td width="45" valign="top">
                <p>
<span data-ttu-id="02f43-344">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-344">Yes</span></span> </p>
            </td>
            <td width="46" valign="top">
                <p>
<span data-ttu-id="02f43-345">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-345">Yes</span></span> </p>
            </td>
            <td width="43" valign="top">
                <p>
<span data-ttu-id="02f43-346">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-346">Yes</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="02f43-347">हाँ</span><span class="sxs-lookup"><span data-stu-id="02f43-347">Yes</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
