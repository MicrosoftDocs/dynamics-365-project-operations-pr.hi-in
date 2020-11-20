---
title: परियोजना-आधारित कोट पंक्तियाँ ओवरव्यू - लाइट
description: यह विषय परियोजना कार्य के लिए परियोजना-आधारित कोटेशन लाइनों का उपयोग करने के बारे में जानकारी प्रदान करता है. (प्रो)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: be1663c0d226fa19fe4b9df566e16d215f1fc08e
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181094"
---
# <a name="project-based-quote-lines-overview---lite"></a><span data-ttu-id="dd115-104">परियोजना-आधारित कोट पंक्तियाँ ओवरव्यू - लाइट</span><span class="sxs-lookup"><span data-stu-id="dd115-104">Project-based quote lines overview - lite</span></span>

<span data-ttu-id="dd115-105">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="dd115-105">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="dd115-106">परियोजना-आधारित कोटेशन लाइनों को एक सगाई पर परियोजना के काम का अनुमान लगाने में मदद करने के लिए डिज़ाइन कर रहे हैं.</span><span class="sxs-lookup"><span data-stu-id="dd115-106">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="dd115-107">परियोजना-आधारित कोटेशन लाइन की संरचना को निम्नलिखित अवधारणाओं के साथ परियोजना अनुमानों के लिए बढ़ाया गया है:</span><span class="sxs-lookup"><span data-stu-id="dd115-107">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="dd115-108">बिलिंग विधि</span><span class="sxs-lookup"><span data-stu-id="dd115-108">Billing Method</span></span>
- <span data-ttu-id="dd115-109">प्रोजेक्ट और टास्क मैपिंग</span><span class="sxs-lookup"><span data-stu-id="dd115-109">Project and Task Mapping</span></span>
- <span data-ttu-id="dd115-110">शामिल लेनदेन कक्षाएं</span><span class="sxs-lookup"><span data-stu-id="dd115-110">Included Transaction classes</span></span>
- <span data-ttu-id="dd115-111">सीमा-में रखें सीमा</span><span class="sxs-lookup"><span data-stu-id="dd115-111">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="dd115-112">प्रभार्यता सेटअप</span><span class="sxs-lookup"><span data-stu-id="dd115-112">Chargeability setup</span></span>
- <span data-ttu-id="dd115-113">कोटेशन लाइन विवरणों का उपयोग करके अनुमान लगाना</span><span class="sxs-lookup"><span data-stu-id="dd115-113">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="dd115-114">कोट पंक्ति ग्राहक</span><span class="sxs-lookup"><span data-stu-id="dd115-114">Quote line Customers</span></span>

<span data-ttu-id="dd115-115">निम्नलिखित तालिका परियोजना-आधारित कोटेशन लाइन के **सामान्य** टैब पर फ़ील्ड के बारे में जानकारी प्रदान करती है.</span><span class="sxs-lookup"><span data-stu-id="dd115-115">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="dd115-116">ये फ़ील्ड परियोजना कार्य के लिए विस्तृत, बुनियादी अनुमान के आधार सेट करने में मदद करते हैं.</span><span class="sxs-lookup"><span data-stu-id="dd115-116">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="dd115-117">**फ़ील्ड**</span><span class="sxs-lookup"><span data-stu-id="dd115-117">**Field**</span></span> | <span data-ttu-id="dd115-118">**वर्णन**</span><span class="sxs-lookup"><span data-stu-id="dd115-118">**Description**</span></span> | <span data-ttu-id="dd115-119">**डाउनस्ट्रीम प्रभाव**</span><span class="sxs-lookup"><span data-stu-id="dd115-119">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="dd115-120">नाम</span><span class="sxs-lookup"><span data-stu-id="dd115-120">Name</span></span> | <span data-ttu-id="dd115-121">कोटेशन लाइन का नाम जिससे आपको अनुमानित किए जा रहे कोटेशन के अलग घटक की पहचान करने में मदद मिलनी चाहिए.</span><span class="sxs-lookup"><span data-stu-id="dd115-121">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="dd115-122">कोटेशन जीतने के बाद इस कोटेशन लाइन से बनाए गए परियोजना अनुबंध लाइन में कॉपी किया गया.</span><span class="sxs-lookup"><span data-stu-id="dd115-122">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dd115-123">बिलिंग विधि</span><span class="sxs-lookup"><span data-stu-id="dd115-123">Billing Method</span></span> | <span data-ttu-id="dd115-124">एक अवसर से बनाई गई कोटेशन पर, इस मूल्य को अवसर लाइन पर संबंधित फ़ील्ड से कॉपी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-124">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="dd115-125">इस फ़ील्ड में Dynamics 365 Project Operations द्वारा समर्थित दो मुख्य अनुबंध मॉडल शामिल हैं:</span><span class="sxs-lookup"><span data-stu-id="dd115-125">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="dd115-126">- निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="dd115-126">- Fixed price</span></span></br><span data-ttu-id="dd115-127">- समय और सामग्री.</span><span class="sxs-lookup"><span data-stu-id="dd115-127">- Time and material.</span></span>| <span data-ttu-id="dd115-128">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-128">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dd115-129">Project</span><span class="sxs-lookup"><span data-stu-id="dd115-129">Project</span></span> | <span data-ttu-id="dd115-130">इस वैकल्पिक फ़ील्ड का उपयोग परियोजना की पहचान करने में करें जिसका उपयोग इस अनुबंध पर कार्य निष्पादन के लिए किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="dd115-130">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="dd115-131">जब किसी परियोजना का कोटेशन लाइन में मानचित्रण किया जाता है, तो यह देय योग्य कार्यों को सेट करने और कोटेशन लाइन विवरणों के रूप में कोटेशन लाइन पर परियोजना-आधारित अनुमान को उत्पन्न करने में भी मदद करता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-131">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="dd115-132">जब किसी परियोजना का परियोजना-आधारित कोटेशन लाइन पर मानचित्रण नहीं किया जाता है, तो प्रत्येक कोटेशन लाइन विवरण बनाकर मैन्युअल रूप से अनुमान बनाया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="dd115-132">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="dd115-133">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-133">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span>|
| <span data-ttu-id="dd115-134">शामिल कार्य</span><span class="sxs-lookup"><span data-stu-id="dd115-134">Included Tasks</span></span> | <span data-ttu-id="dd115-135">इंगित करता है कि क्या इस कोटेशन लाइन का उपयोग चयनित परियोजना के लिए सभी या कुछ परियोजना कार्यों के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-135">Indicates if this quote line is used for all or some of the project tasks for the selected project.</span></span> <span data-ttu-id="dd115-136">इस फ़ील्ड में निम्नलिखित संभावित मान हैं:</span><span class="sxs-lookup"><span data-stu-id="dd115-136">This field has the following possible values:</span></span></br><span data-ttu-id="dd115-137">- सभी परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="dd115-137">- All project tasks</span></span></br><span data-ttu-id="dd115-138">- केवल चयनित परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="dd115-138">- Selected project tasks only</span></span></br><span data-ttu-id="dd115-139">इस फ़ील्ड में एक खाली मान **सभी परियोजना कार्य** विकल्प के समान है.</span><span class="sxs-lookup"><span data-stu-id="dd115-139">A blank value in this field is equivalent to the **All project tasks** option.</span></span> | <span data-ttu-id="dd115-140">जब **केवल चयनित परियोजना कार्य** को चुना जाता है तो परियोजना पृष्ठ पर, **कार्य बिलिंग सेटअप** टैब आपको इस कोटेशन लाइन से संबद्ध करने के लिए विशिष्ट कार्यों का चयन करने की अनुमति देता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-140">When **Selected project tasks only** is selected then on the project page, the **Task billing setup** tab allows you to select specific tasks to associate them to this quote line.</span></span> <span data-ttu-id="dd115-141">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-141">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dd115-142">समय शामिल करें</span><span class="sxs-lookup"><span data-stu-id="dd115-142">Include Time</span></span> | <span data-ttu-id="dd115-143">एक **हाँ**/**नहीं** निशान इंगित करता है कि क्या चयनित परियोजना पर समय की लेनदेन या श्रम लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="dd115-143">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="dd115-144">एक **नहीं** मान इंगित करता है कि समय की लेनदेन या श्रम लागत इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="dd115-144">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="dd115-145">एक **हाँ** मान इंगित करता है कि समय की लेनदेन या श्रम लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="dd115-145">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="dd115-146">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-146">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dd115-147">व्यय शामिल करें</span><span class="sxs-lookup"><span data-stu-id="dd115-147">Include Expense</span></span> | <span data-ttu-id="dd115-148">एक **हाँ**/**नहीं** निशान इंगित करता है कि क्या चयनित परियोजना पर ख़र्च लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="dd115-148">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="dd115-149">एक **नहीं** मान इंगित करता है कि ख़र्च लागत इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="dd115-149">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="dd115-150">एक **हाँ** मान इंगित करता है कि ख़र्च लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="dd115-150">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="dd115-151">इस फ़ील्ड मान को परियोजना अनुबंध लाइन पर कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-151">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dd115-152">शुल्क शामिल करें</span><span class="sxs-lookup"><span data-stu-id="dd115-152">Include Fee</span></span> | <span data-ttu-id="dd115-153">एक **हाँ**/**नहीं** निशान इंगित करता है कि क्या चयनित परियोजना पर शुल्क इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="dd115-153">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="dd115-154">एक **नहीं** मान इंगित करता है कि शुल्क को इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="dd115-154">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="dd115-155">एक **हाँ** मान इंगित करता है कि शुल्क को इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="dd115-155">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="dd115-156">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-156">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dd115-157">कोट की गई राशि</span><span class="sxs-lookup"><span data-stu-id="dd115-157">Quoted Amount</span></span> | <span data-ttu-id="dd115-158">यह वह राशि है जिसे इस परियोजना-आधारित कोटेशन लाइन पर पूर्वानुमानित सभी कार्यों के लिए ग्राहक को प्रस्तुत किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="dd115-158">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="dd115-159">एक अवसर से बनाई गई कोटेशन पर, इस मान को अवसर लाइन पर **ग्राहक बजट** फ़ील्ड से कॉपी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-159">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="dd115-160">जब परियोजना-आधारित कोटेशन लाइन में लाइन विवरण होते हैं, तो इस फ़ील्ड को संपादन के लिए लॉक कर दिया जाता है और कोटेशन लाइन विवरणों पर दर्ज राशि से संक्षेपित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-160">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="dd115-161">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-161">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dd115-162">अनुमानित कर</span><span class="sxs-lookup"><span data-stu-id="dd115-162">Estimated Tax</span></span> | <span data-ttu-id="dd115-163">यह उपयोगकर्ता के लिए कोटेशन लाइन पर अनुमानित कर राशि जोड़ने के लिए एक संपादन योग्य फ़ील्ड है.</span><span class="sxs-lookup"><span data-stu-id="dd115-163">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="dd115-164">जब किसी परियोजना-आधारित कोटेशन लाइन में लाइन विवरण होते हैं, तो इस फ़ील्ड को संपादन के लिए लॉक कर दिया जाता है और कोटेशन लाइन विवरणों पर दर्ज कर राशि से संक्षेपित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-164">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="dd115-165">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-165">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dd115-166">कर के बाद कोट की गई राशि</span><span class="sxs-lookup"><span data-stu-id="dd115-166">Quoted Amount after Tax</span></span> | <span data-ttu-id="dd115-167">कर के बाद यह फ़ील्ड कोटेशन लाइन राशि है और केवल पढ़ी जाती है.</span><span class="sxs-lookup"><span data-stu-id="dd115-167">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="dd115-168">इस फ़ील्ड में राशि की गणना *क्वोट की गई राशि + कर* के रूप में की जाती है.</span><span class="sxs-lookup"><span data-stu-id="dd115-168">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="dd115-169">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-169">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dd115-170">सीमा-में रखें सीमा</span><span class="sxs-lookup"><span data-stu-id="dd115-170">Not-to-exceed Limit</span></span> | <span data-ttu-id="dd115-171">यह फ़ील्ड संपादन योग्य है और केवल परियोजना-आधारित कोटेशन लाइनों पर उपलब्ध है जिसमें **समय और सामग्री** बिलिंग विधि है.</span><span class="sxs-lookup"><span data-stu-id="dd115-171">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="dd115-172">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-172">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="dd115-173">ग्राहक बजट</span><span class="sxs-lookup"><span data-stu-id="dd115-173">Customer Budget</span></span> | <span data-ttu-id="dd115-174">यह फ़ील्ड संपादन योग्य है और यदि कोटेशन एक अवसर से बनाया गया था तो अवसर लाइन पर संबंधित फ़ील्ड से कॉपी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-174">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="dd115-175">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-175">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="dd115-176">परियोजना-आधारित कोटेशन लाइनों के सामान्य टैब पर फ़ील्डों के लिए सत्यापन नियम</span><span class="sxs-lookup"><span data-stu-id="dd115-176">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="dd115-177">**नियम 1**: यदि **शामिल किए गए कार्य** फ़ील्ड खाली है, या यदि यह **सभी परियोजना कार्य** के लिए सेट है, तो कोटेशन लाइन में एक परियोजना शामिल की जाती है.</span><span class="sxs-lookup"><span data-stu-id="dd115-177">**Rule 1**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project is included in the quote line.</span></span>

<span data-ttu-id="dd115-178">**नियम 2**: यदि **शामिल किए गए कार्य** फ़ील्ड खाली है, या यदि यह **सभी परियोजना कार्य** के लिए सेट है, तो केवल कोटेशन की परियोजना-आधारित एक कोटेशन लाइन पर एक परियोजना और एक निश्चित लेनदेन वर्ग को शामिल किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-178">**Rule 2**: If the **Included Tasks** field is blank, or if it is set to **All project tasks**, a project and a certain transaction class can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="dd115-179">**नियम 3**: यदि **शामिल किए गए कार्य** फ़ील्ड को **केवल चयनित परियोजना कार्य** के लिए सेट किया गया है, तो एक परियोजना और एक निश्चित लेनदेन वर्ग को कोटेशन की परियोजना-आधारित कई कोटेशन लाइनों पर शामिल किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="dd115-179">**Rule 3**: If the **Included Tasks** field is set to **Selected project tasks only**, a project and a certain transaction class can be included on multiple project-based quote lines of a quote.</span></span>

<span data-ttu-id="dd115-180">**नियम 4**: यदि किसी अवसर में कई कोटेशन हैं, तो विभिन्न कोटेशनों से कोटेशन लाइनें हो सकती हैं जो सभी एक ही परियोजना का संदर्भ देती हैं और एक ही लेनदेन वर्ग को शामिल करती हैं.</span><span class="sxs-lookup"><span data-stu-id="dd115-180">**Rule 4**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="dd115-181">**नियम 5**: यदि कोटेशन उसी समान अवसर से संबंधित नहीं हैं, तो वे समान परियोजना और लेनदेन वर्ग को शामिल नहीं कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="dd115-181">**Rule 5**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="dd115-182">
                    <strong>अवसर</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dd115-182">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="dd115-183">
                    <strong>कोट</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dd115-183">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="dd115-184">
                    <strong>कोट पंक्ति</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dd115-184">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="dd115-185">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dd115-185">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="90" valign="top">
                <p><span data-ttu-id="dd115-186">
                    <strong>शामिल कार्य</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dd115-186">
                    <strong>Included tasks</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="dd115-187">
                    <strong>समय शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dd115-187">
                    <strong>Include Time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="dd115-188">
                    <strong>व्यय शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dd115-188">
                    <strong>Include Expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="dd115-189">
                    <strong>शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dd115-189">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="dd115-190">
                    <strong>शुल्क</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dd115-190">
                    <strong>Fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="dd115-191">
                    <strong>मान्य/ मान्य नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dd115-191">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="dd115-192">
                    <strong>कारण</strong>
                </span><span class="sxs-lookup"><span data-stu-id="dd115-192">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="dd115-193">O1</span><span class="sxs-lookup"><span data-stu-id="dd115-193">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dd115-194">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="dd115-194">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-195">QL1</span><span class="sxs-lookup"><span data-stu-id="dd115-195">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-196">P1</span><span class="sxs-lookup"><span data-stu-id="dd115-196">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="dd115-197">रिक्त</span><span class="sxs-lookup"><span data-stu-id="dd115-197">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-198">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-198">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-199">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-199">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-200">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-200">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd115-201">मान्य नहीं है</span><span class="sxs-lookup"><span data-stu-id="dd115-201">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd115-202">नियम #2 का उल्लंघन.</span><span class="sxs-lookup"><span data-stu-id="dd115-202">Violation of Rule #2.</span></span> <span data-ttu-id="dd115-203">P1 परियोजना पर समय, ख़र्च और शुल्क कोटेशन लाइनों QL1 और QL2 पर शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="dd115-203">Time, Expense, and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="dd115-204">O1</span><span class="sxs-lookup"><span data-stu-id="dd115-204">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dd115-205">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="dd115-205">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-206">QL2</span><span class="sxs-lookup"><span data-stu-id="dd115-206">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-207">P1</span><span class="sxs-lookup"><span data-stu-id="dd115-207">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="dd115-208">रिक्त</span><span class="sxs-lookup"><span data-stu-id="dd115-208">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-209">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-209">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-210">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-210">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-211">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-211">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="dd115-212">O1</span><span class="sxs-lookup"><span data-stu-id="dd115-212">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dd115-213">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="dd115-213">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-214">QL1</span><span class="sxs-lookup"><span data-stu-id="dd115-214">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-215">P1</span><span class="sxs-lookup"><span data-stu-id="dd115-215">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="dd115-216">रिक्त</span><span class="sxs-lookup"><span data-stu-id="dd115-216">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-217">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-217">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-218">No</span><span class="sxs-lookup"><span data-stu-id="dd115-218">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-219">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-219">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd115-220">मान्य नहीं है</span><span class="sxs-lookup"><span data-stu-id="dd115-220">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd115-221">नियम #2 का उल्लंघन.</span><span class="sxs-lookup"><span data-stu-id="dd115-221">Violation of Rule #2.</span></span> <span data-ttu-id="dd115-222">P1 प्रोजेक्ट पर समय और शुल्क उद्धरण लाइनों QL1 और QL2 पर शामिल हैं।</span><span class="sxs-lookup"><span data-stu-id="dd115-222">Time and Fees on P1 project are included on quote lines QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="dd115-223">O1</span><span class="sxs-lookup"><span data-stu-id="dd115-223">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dd115-224">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="dd115-224">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-225">QL2</span><span class="sxs-lookup"><span data-stu-id="dd115-225">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-226">P1</span><span class="sxs-lookup"><span data-stu-id="dd115-226">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="dd115-227">रिक्त</span><span class="sxs-lookup"><span data-stu-id="dd115-227">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-228">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-228">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-229">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-229">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-230">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-230">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="dd115-231">O1</span><span class="sxs-lookup"><span data-stu-id="dd115-231">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dd115-232">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="dd115-232">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-233">QL1</span><span class="sxs-lookup"><span data-stu-id="dd115-233">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-234">P1</span><span class="sxs-lookup"><span data-stu-id="dd115-234">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="dd115-235">रिक्त</span><span class="sxs-lookup"><span data-stu-id="dd115-235">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-236">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-236">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-237">No</span><span class="sxs-lookup"><span data-stu-id="dd115-237">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-238">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-238">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd115-239">मान्य</span><span class="sxs-lookup"><span data-stu-id="dd115-239">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
<span data-ttu-id="dd115-240">P1 परियोजना पर समय और शुल्क QL1 पर शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="dd115-240">Time and Fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="dd115-241">P1 परियोजना पर ख़र्च QL2 पर शामिल है.</span><span class="sxs-lookup"><span data-stu-id="dd115-241">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="dd115-242">प्रत्येक कोटेशन लाइन पर जो भी शामिल किया जा रहा है उनमें ओवरलैप नहीं है और मान्य है.</span><span class="sxs-lookup"><span data-stu-id="dd115-242">There is no overlap in what is being included on each quote line and is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="dd115-243">O1</span><span class="sxs-lookup"><span data-stu-id="dd115-243">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dd115-244">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="dd115-244">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-245">QL2</span><span class="sxs-lookup"><span data-stu-id="dd115-245">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-246">P1</span><span class="sxs-lookup"><span data-stu-id="dd115-246">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="dd115-247">रिक्त</span><span class="sxs-lookup"><span data-stu-id="dd115-247">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-248">No</span><span class="sxs-lookup"><span data-stu-id="dd115-248">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-249">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-250">No</span><span class="sxs-lookup"><span data-stu-id="dd115-250">No</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="dd115-251">O1</span><span class="sxs-lookup"><span data-stu-id="dd115-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dd115-252">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="dd115-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-253">QL1</span><span class="sxs-lookup"><span data-stu-id="dd115-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-254">P1</span><span class="sxs-lookup"><span data-stu-id="dd115-254">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="dd115-255">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="dd115-255">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-256">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-256">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-257">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-257">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-258">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-258">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd115-259">मान्य नहीं है</span><span class="sxs-lookup"><span data-stu-id="dd115-259">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd115-260">नियम #2 ऊपर का उल्लंघन</span><span class="sxs-lookup"><span data-stu-id="dd115-260">Violation of Rule #2 above</span></span> </p>
                <p>
<span data-ttu-id="dd115-261">Q1 में परियोजना P1 पर कार्यों के सबसेट पर समय, ख़र्च और शुल्क शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="dd115-261">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="dd115-262">QL2 में संपूर्ण परियोजना P1 के लिए समय, ख़र्च और शुल्क शामिल हैं और Q1 पर जो भी शामिल है उसके साथ ओवरलैप करती है.</span><span class="sxs-lookup"><span data-stu-id="dd115-262">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="dd115-263">O1</span><span class="sxs-lookup"><span data-stu-id="dd115-263">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dd115-264">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="dd115-264">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-265">QL2</span><span class="sxs-lookup"><span data-stu-id="dd115-265">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-266">P1</span><span class="sxs-lookup"><span data-stu-id="dd115-266">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="dd115-267">रिक्त</span><span class="sxs-lookup"><span data-stu-id="dd115-267">Blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-268">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-268">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-269">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-269">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-270">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-270">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="dd115-271">O1</span><span class="sxs-lookup"><span data-stu-id="dd115-271">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dd115-272">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="dd115-272">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-273">QL1</span><span class="sxs-lookup"><span data-stu-id="dd115-273">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-274">P1</span><span class="sxs-lookup"><span data-stu-id="dd115-274">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="dd115-275">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="dd115-275">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-276">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-276">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-277">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-277">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-278">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-278">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd115-279">मान्य</span><span class="sxs-lookup"><span data-stu-id="dd115-279">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd115-280">ऊपर कहे गए नियम #3 के अनुकूल,</span><span class="sxs-lookup"><span data-stu-id="dd115-280">Per Rule #3 above,</span></span> </p>
                <p>
<span data-ttu-id="dd115-281">Q1 में परियोजना P1 पर कार्यों के सबसेट पर समय, ख़र्च और शुल्क शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="dd115-281">Q1 includes Time, Expenses, and Fees on a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="dd115-282">QL2 में परियोजना P1 पर कार्यों के सबसेट के लिए समय, ख़र्च और शुल्क शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="dd115-282">QL2 includes Time, Expenses, and Fees for a subset of tasks on project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="dd115-283">एकमात्र अतिरिक्त सत्यापन QL1 पर कार्यों के सबसेट के आसपास है जो QL2 पर कार्यों के सबसेट से अलग है.</span><span class="sxs-lookup"><span data-stu-id="dd115-283">The only additional validation is around the subset of tasks on QL1 which are different from the subset of tasks on QL2.</span></span> <span data-ttu-id="dd115-284">यह सुनिश्चित करता है कि कोई ओवरलैप नहीं हैं.</span><span class="sxs-lookup"><span data-stu-id="dd115-284">This ensures that there are no overlaps.</span></span> <span data-ttu-id="dd115-285">यह सिस्टम द्वारा किया जाता है जब कार्य संबध्द होते हैं.</span><span class="sxs-lookup"><span data-stu-id="dd115-285">This is done by the system when tasks are associated.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="dd115-286">O1</span><span class="sxs-lookup"><span data-stu-id="dd115-286">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dd115-287">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="dd115-287">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-288">QL2</span><span class="sxs-lookup"><span data-stu-id="dd115-288">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-289">P1</span><span class="sxs-lookup"><span data-stu-id="dd115-289">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="dd115-290">केवल चयनित कार्य</span><span class="sxs-lookup"><span data-stu-id="dd115-290">Selected tasks only</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-291">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-291">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-292">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-292">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-293">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-293">Yes</span></span> </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="dd115-294">O1</span><span class="sxs-lookup"><span data-stu-id="dd115-294">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dd115-295">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="dd115-295">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-296">QL1</span><span class="sxs-lookup"><span data-stu-id="dd115-296">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-297">P1</span><span class="sxs-lookup"><span data-stu-id="dd115-297">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="dd115-298">सभी परियोजना कार्य या रिक्त</span><span class="sxs-lookup"><span data-stu-id="dd115-298">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-299">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-299">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-300">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-300">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-301">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-301">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="dd115-302">मान्य</span><span class="sxs-lookup"><span data-stu-id="dd115-302">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd115-303">नियम #5 के आधार पर, Q1 और Q2 एक ही अवसर पर दो उद्धरण हैं, इसलिए वे दोनों एक परियोजना के समान घटकों के लिए अनुमान लगा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="dd115-303">Based on Rule #5, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="dd115-304">O1</span><span class="sxs-lookup"><span data-stu-id="dd115-304">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dd115-305">तिमाही 2</span><span class="sxs-lookup"><span data-stu-id="dd115-305">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-306">QL1</span><span class="sxs-lookup"><span data-stu-id="dd115-306">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-307">P1</span><span class="sxs-lookup"><span data-stu-id="dd115-307">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="dd115-308">सभी परियोजना कार्य या रिक्त</span><span class="sxs-lookup"><span data-stu-id="dd115-308">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-309">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-309">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-310">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-310">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-311">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-311">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="dd115-312">O1</span><span class="sxs-lookup"><span data-stu-id="dd115-312">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dd115-313">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="dd115-313">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-314">QL1</span><span class="sxs-lookup"><span data-stu-id="dd115-314">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-315">P1</span><span class="sxs-lookup"><span data-stu-id="dd115-315">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="dd115-316">सभी परियोजना कार्य या रिक्त</span><span class="sxs-lookup"><span data-stu-id="dd115-316">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-317">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-317">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-318">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-318">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-319">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-319">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="dd115-320">मान्य</span><span class="sxs-lookup"><span data-stu-id="dd115-320">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="dd115-321">नियम #4 पर आधारित, Q1 और Q2 विभिन्न अवसरों पर दो कोटेशन हैं, इसलिए वे एक ही परियोजना के समान घटकों के लिए अनुमान नहीं लगा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="dd115-321">Based on Rule #4, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="dd115-322">O2</span><span class="sxs-lookup"><span data-stu-id="dd115-322">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="dd115-323">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="dd115-323">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-324">QL1</span><span class="sxs-lookup"><span data-stu-id="dd115-324">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-325">P1</span><span class="sxs-lookup"><span data-stu-id="dd115-325">P1</span></span> </p>
            </td>
            <td width="90" valign="top">
                <p>
<span data-ttu-id="dd115-326">सभी परियोजना कार्य या रिक्त</span><span class="sxs-lookup"><span data-stu-id="dd115-326">All project tasks or blank</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-327">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-327">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="dd115-328">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-328">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="dd115-329">हाँ</span><span class="sxs-lookup"><span data-stu-id="dd115-329">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="dd115-330">मान्य नहीं है</span><span class="sxs-lookup"><span data-stu-id="dd115-330">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>

