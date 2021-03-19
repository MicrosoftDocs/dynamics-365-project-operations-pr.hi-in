---
title: परियोजना-आधारित कोट पंक्तियाँ ओवरव्यू
description: यह विषय परियोजना कार्य के लिए परियोजना-आधारित कोटेशन लाइनों का उपयोग करने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: e61a9fbf357123884397b930662d11f22bfdeaa0
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5277790"
---
# <a name="project-based-quote-lines-overview"></a><span data-ttu-id="d0e69-103">परियोजना-आधारित कोट पंक्तियाँ ओवरव्यू</span><span class="sxs-lookup"><span data-stu-id="d0e69-103">Project-based quote lines overview</span></span>

<span data-ttu-id="d0e69-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="d0e69-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="d0e69-105">परियोजना-आधारित कोटेशन लाइनों को एक सगाई पर परियोजना के काम का अनुमान लगाने में मदद करने के लिए डिज़ाइन कर रहे हैं.</span><span class="sxs-lookup"><span data-stu-id="d0e69-105">Project-based quote lines are designed to help estimate the project work on an engagement.</span></span> <span data-ttu-id="d0e69-106">परियोजना-आधारित कोटेशन लाइन की संरचना को निम्नलिखित अवधारणाओं के साथ परियोजना अनुमानों के लिए बढ़ाया गया है:</span><span class="sxs-lookup"><span data-stu-id="d0e69-106">The structure of a project-based quote line is extended for project estimates with the following concepts:</span></span>

- <span data-ttu-id="d0e69-107">बिलिंग विधि</span><span class="sxs-lookup"><span data-stu-id="d0e69-107">Billing Method</span></span>
- <span data-ttu-id="d0e69-108">प्रोजेक्ट मैपिंग</span><span class="sxs-lookup"><span data-stu-id="d0e69-108">Project Mapping</span></span>
- <span data-ttu-id="d0e69-109">शामिल लेनदेन कक्षाएं</span><span class="sxs-lookup"><span data-stu-id="d0e69-109">Included Transaction classes</span></span>
- <span data-ttu-id="d0e69-110">सीमा-में रखें सीमा</span><span class="sxs-lookup"><span data-stu-id="d0e69-110">Not-to-Exceed Limit</span></span>
- <span data-ttu-id="d0e69-111">प्रभार्यता सेटअप</span><span class="sxs-lookup"><span data-stu-id="d0e69-111">Chargeability setup</span></span>
- <span data-ttu-id="d0e69-112">कोटेशन लाइन विवरणों का उपयोग करके अनुमान लगाना</span><span class="sxs-lookup"><span data-stu-id="d0e69-112">Estimation using Quote Line Details</span></span>
- <span data-ttu-id="d0e69-113">कोट पंक्ति ग्राहक</span><span class="sxs-lookup"><span data-stu-id="d0e69-113">Quote line Customers</span></span>

<span data-ttu-id="d0e69-114">निम्नलिखित तालिका परियोजना-आधारित कोटेशन लाइन के **सामान्य** टैब पर फ़ील्ड के बारे में जानकारी प्रदान करती है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-114">The following table provides information about the fields on the **General** tab of project-based quote line.</span></span> <span data-ttu-id="d0e69-115">ये फ़ील्ड परियोजना कार्य के लिए विस्तृत, बुनियादी अनुमान के आधार सेट करने में मदद करते हैं.</span><span class="sxs-lookup"><span data-stu-id="d0e69-115">These fields help set up the basis for a detailed, ground-up estimation for project work.</span></span>

| <span data-ttu-id="d0e69-116">**फ़ील्ड**</span><span class="sxs-lookup"><span data-stu-id="d0e69-116">**Field**</span></span> | <span data-ttu-id="d0e69-117">**वर्णन**</span><span class="sxs-lookup"><span data-stu-id="d0e69-117">**Description**</span></span> | <span data-ttu-id="d0e69-118">**डाउनस्ट्रीम प्रभाव**</span><span class="sxs-lookup"><span data-stu-id="d0e69-118">**Downstream impact**</span></span> |
| --- | --- | --- |
| <span data-ttu-id="d0e69-119">नाम</span><span class="sxs-lookup"><span data-stu-id="d0e69-119">Name</span></span> | <span data-ttu-id="d0e69-120">कोटेशन लाइन का नाम जिससे आपको अनुमानित किए जा रहे कोटेशन के अलग घटक की पहचान करने में मदद मिलनी चाहिए.</span><span class="sxs-lookup"><span data-stu-id="d0e69-120">The name of quote line which should help you identify the discrete component of the quote that is being estimated.</span></span> | <span data-ttu-id="d0e69-121">कोटेशन जीतने के बाद इस कोटेशन लाइन से बनाए गए परियोजना अनुबंध लाइन में कॉपी किया गया.</span><span class="sxs-lookup"><span data-stu-id="d0e69-121">Copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d0e69-122">बिलिंग विधि</span><span class="sxs-lookup"><span data-stu-id="d0e69-122">Billing Method</span></span> | <span data-ttu-id="d0e69-123">एक अवसर से बनाई गई कोटेशन पर, इस मूल्य को अवसर लाइन पर संबंधित फ़ील्ड से कॉपी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-123">On a quote created from an opportunity, this value is copied from the corresponding field on the opportunity line.</span></span> <span data-ttu-id="d0e69-124">इस फ़ील्ड में Dynamics 365 Project Operations समर्थित दो मुख्य अनुबंध मॉडल शामिल हैं:</span><span class="sxs-lookup"><span data-stu-id="d0e69-124">This field includes the two main contracting models supported by Dynamics 365 Project Operations:</span></span></br><span data-ttu-id="d0e69-125">- निश्चित मूल्य</span><span class="sxs-lookup"><span data-stu-id="d0e69-125">- Fixed price</span></span></br><span data-ttu-id="d0e69-126">- समय और सामग्री.</span><span class="sxs-lookup"><span data-stu-id="d0e69-126">- Time and material.</span></span>| <span data-ttu-id="d0e69-127">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-127">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d0e69-128">Project</span><span class="sxs-lookup"><span data-stu-id="d0e69-128">Project</span></span> | <span data-ttu-id="d0e69-129">इस वैकल्पिक फ़ील्ड का उपयोग परियोजना की पहचान करने में करें जिसका उपयोग इस अनुबंध पर कार्य निष्पादन के लिए किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="d0e69-129">Use this optional field to identify the project that will be used to deliver the work on this engagement.</span></span> <span data-ttu-id="d0e69-130">जब किसी परियोजना का कोटेशन लाइन में मानचित्रण किया जाता है, तो यह देय योग्य कार्यों को सेट करने और कोटेशन लाइन विवरणों के रूप में कोटेशन लाइन पर परियोजना-आधारित अनुमान को उत्पन्न करने में भी मदद करता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-130">When a project is mapped to a quote line, it helps with setting up chargeable tasks and also with bringing in a project-based estimate to the quote line as quote line details.</span></span> <span data-ttu-id="d0e69-131">जब किसी परियोजना का परियोजना-आधारित कोटेशन लाइन पर मानचित्रण नहीं किया जाता है, तो प्रत्येक कोटेशन लाइन विवरण बनाकर मैन्युअल रूप से अनुमान बनाया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="d0e69-131">When a project is not mapped to a project-based quote line, the estimate should be created manually by creating each quote line detail.</span></span> | <span data-ttu-id="d0e69-132">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-132">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d0e69-133">समय शामिल करें</span><span class="sxs-lookup"><span data-stu-id="d0e69-133">Include Time</span></span> | <span data-ttu-id="d0e69-134">एक **हाँ**/**नहीं** निशान इंगित करता है कि क्या चयनित परियोजना पर समय की लेनदेन या श्रम लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="d0e69-134">A **Yes**/**No** flag indicates if time transactions or labor costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="d0e69-135">एक **नहीं** मान इंगित करता है कि समय की लेनदेन या श्रम लागत इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="d0e69-135">A **No** value indicates that the time transactions or labor cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="d0e69-136">एक **हाँ** मान इंगित करता है कि समय की लेनदेन या श्रम लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="d0e69-136">A **Yes** value indicates that the time transactions or labor cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="d0e69-137">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-137">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d0e69-138">व्यय शामिल करें</span><span class="sxs-lookup"><span data-stu-id="d0e69-138">Include Expense</span></span> | <span data-ttu-id="d0e69-139">एक **हाँ**/**नहीं** निशान इंगित करता है कि क्या चयनित परियोजना पर ख़र्च लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="d0e69-139">A **Yes**/**No** flag indicates if expense costs on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="d0e69-140">एक **नहीं** मान इंगित करता है कि ख़र्च लागत इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="d0e69-140">A **No** value indicates that the expense cost will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="d0e69-141">एक **हाँ** मान इंगित करता है कि ख़र्च लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="d0e69-141">A **Yes** value indicates that the expense cost will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="d0e69-142">इस फ़ील्ड मान को परियोजना अनुबंध लाइन पर कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-142">This field value is copied over to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d0e69-143">शुल्क शामिल करें</span><span class="sxs-lookup"><span data-stu-id="d0e69-143">Include Fee</span></span> | <span data-ttu-id="d0e69-144">एक **हाँ**/**नहीं** निशान इंगित करता है कि क्या चयनित परियोजना पर शुल्क इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="d0e69-144">A **Yes**/**No** flag indicates if fees on the selected project will be included in the estimate on this quote line.</span></span> <span data-ttu-id="d0e69-145">एक **नहीं** मान इंगित करता है कि शुल्क को इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="d0e69-145">A **No** value indicates that the Fees will not be included in the estimate on this quote line.</span></span> <span data-ttu-id="d0e69-146">एक **हाँ** मान इंगित करता है कि शुल्क को इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="d0e69-146">A **Yes** value indicates that the Fees will be included in the estimate on this quote line.</span></span> | <span data-ttu-id="d0e69-147">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-147">This field value is copied to the Project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d0e69-148">कोट की गई राशि</span><span class="sxs-lookup"><span data-stu-id="d0e69-148">Quoted Amount</span></span> | <span data-ttu-id="d0e69-149">यह वह राशि है जिसे इस परियोजना-आधारित कोटेशन लाइन पर पूर्वानुमानित सभी कार्यों के लिए ग्राहक को प्रस्तुत किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="d0e69-149">This is amount that will be quoted to the customer for all the work forecasted on this project-based quote line.</span></span> <span data-ttu-id="d0e69-150">एक अवसर से बनाई गई कोटेशन पर, इस मान को अवसर लाइन पर **ग्राहक बजट** फ़ील्ड से कॉपी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-150">On a quote created from an opportunity, this value is copied from the **Customer Budget** field on the opportunity line.</span></span> <span data-ttu-id="d0e69-151">जब परियोजना-आधारित कोटेशन लाइन में लाइन विवरण होते हैं, तो इस फ़ील्ड को संपादन के लिए लॉक कर दिया जाता है और कोटेशन लाइन विवरणों पर दर्ज राशि से संक्षेपित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-151">When the project-based quote line has line details, this field is locked for editing and is summarized from the amount on the quote line details.</span></span> | <span data-ttu-id="d0e69-152">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-152">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d0e69-153">अनुमानित कर</span><span class="sxs-lookup"><span data-stu-id="d0e69-153">Estimated Tax</span></span> | <span data-ttu-id="d0e69-154">यह उपयोगकर्ता के लिए कोटेशन लाइन पर अनुमानित कर राशि जोड़ने के लिए एक संपादन योग्य फ़ील्ड है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-154">This is an editable field for the user to add the estimated tax amount on the quote line.</span></span> <span data-ttu-id="d0e69-155">जब किसी परियोजना-आधारित कोटेशन लाइन में लाइन विवरण होते हैं, तो इस फ़ील्ड को संपादन के लिए लॉक कर दिया जाता है और कोटेशन लाइन विवरणों पर दर्ज कर राशि से संक्षेपित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-155">When a project-based quote line has line details, this field is locked for editing and is summarized from the tax amount on the quote line details.</span></span> | <span data-ttu-id="d0e69-156">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-156">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d0e69-157">कर के बाद कोट की गई राशि</span><span class="sxs-lookup"><span data-stu-id="d0e69-157">Quoted Amount after Tax</span></span> | <span data-ttu-id="d0e69-158">कर के बाद यह फ़ील्ड कोटेशन लाइन राशि है और केवल पढ़ी जाती है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-158">This field is the quote line amount after tax and is read-only.</span></span> <span data-ttu-id="d0e69-159">इस फ़ील्ड में राशि की गणना *क्वोट की गई राशि + कर* के रूप में की जाती है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-159">The amount in this field is calculated as *Quoted Amount + Tax*.</span></span> | <span data-ttu-id="d0e69-160">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-160">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d0e69-161">सीमा-में रखें सीमा</span><span class="sxs-lookup"><span data-stu-id="d0e69-161">Not-to-exceed Limit</span></span> | <span data-ttu-id="d0e69-162">यह फ़ील्ड संपादन योग्य है और केवल परियोजना-आधारित कोटेशन लाइनों पर उपलब्ध है जिसमें **समय और सामग्री** बिलिंग विधि है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-162">This field is editable and is only available on project-based quote lines that have a **Time and Material** billing method.</span></span> | <span data-ttu-id="d0e69-163">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-163">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |
| <span data-ttu-id="d0e69-164">ग्राहक बजट</span><span class="sxs-lookup"><span data-stu-id="d0e69-164">Customer Budget</span></span> | <span data-ttu-id="d0e69-165">यह फ़ील्ड संपादन योग्य है और यदि कोटेशन एक अवसर से बनाया गया था तो अवसर लाइन पर संबंधित फ़ील्ड से कॉपी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-165">This field is editable and is copied from the corresponding field on the opportunity line if the quote was created from an opportunity.</span></span> | <span data-ttu-id="d0e69-166">इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-166">This field value is copied to the project contract line that is created from this quote line when the quote is won.</span></span> |

## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a><span data-ttu-id="d0e69-167">परियोजना-आधारित कोटेशन लाइनों के सामान्य टैब पर फ़ील्डों के लिए सत्यापन नियम</span><span class="sxs-lookup"><span data-stu-id="d0e69-167">Validation rules for fields on the General tab of project-based quote lines</span></span>

<span data-ttu-id="d0e69-168">**नियम 1**: चयनित परियोजना पर एक निश्चित लेनदेन वर्ग को केवल कोटेशन की परियोजना-आधारित एक कोटेशन लाइन पर शामिल किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-168">**Rule 1**: A certain transaction class on the selected project can only be included on one project-based quote line of a quote.</span></span>

<span data-ttu-id="d0e69-169">**नियम 2**: यदि किसी अवसर में कई कोटेशन हैं, तो विभिन्न कोटेशनों से कोटेशन लाइनें हो सकती हैं जो सभी एक ही परियोजना का संदर्भ देती हैं और एक ही लेनदेन वर्ग को शामिल करती हैं.</span><span class="sxs-lookup"><span data-stu-id="d0e69-169">**Rule 2**: If an opportunity has multiple quotes, there can be quote lines from different quotes that all reference the same project and include the same transaction class.</span></span>

<span data-ttu-id="d0e69-170">**नियम 3**: यदि कोटेशन उसी समान अवसर से संबंधित नहीं हैं, तो वे समान परियोजना और लेनदेन वर्ग को शामिल नहीं कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="d0e69-170">**Rule 3**: If the quotes do not belong to the same opportunity, they can't include the same project and transaction class.</span></span>

<table border="1" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p><span data-ttu-id="d0e69-171">
                    <strong>अवसर</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d0e69-171">
                    <strong>Opportunity</strong>
                </span></span></p>
            </td>
            <td width="41" valign="top">
                <p><span data-ttu-id="d0e69-172">
                    <strong>कोट</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d0e69-172">
                    <strong>Quote</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="d0e69-173">
                    <strong>कोट पंक्ति</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d0e69-173">
                    <strong>Quote line</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="d0e69-174">
                    <strong>Project</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d0e69-174">
                    <strong>Project</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="d0e69-175">
                    <strong>समय शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d0e69-175">
                    <strong>Include time</strong>
                </span></span></p>
            </td>
            <td width="48" valign="top">
                <p><span data-ttu-id="d0e69-176">
                    <strong>व्यय शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d0e69-176">
                    <strong>Include expense</strong>
                </span></span></p>
            </td>
            <td width="42" valign="top">
                <p><span data-ttu-id="d0e69-177">
                    <strong>शामिल करें</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d0e69-177">
                    <strong>Include</strong>
                </span></span></p>
                <p><span data-ttu-id="d0e69-178">
                    <strong>शुल्क</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d0e69-178">
                    <strong>fee</strong>
                </span></span></p>
            </td>
            <td width="54" valign="top">
                <p><span data-ttu-id="d0e69-179">
                    <strong>मान्य/ मान्य नहीं</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d0e69-179">
                    <strong>Valid/ Not valid</strong>
                </span></span></p>
            </td>
            <td width="308" valign="top">
                <p><span data-ttu-id="d0e69-180">
                    <strong>कारण</strong>
                </span><span class="sxs-lookup"><span data-stu-id="d0e69-180">
                    <strong>Reason</strong>
                </span></span></p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d0e69-181">O1</span><span class="sxs-lookup"><span data-stu-id="d0e69-181">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d0e69-182">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="d0e69-182">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-183">QL1</span><span class="sxs-lookup"><span data-stu-id="d0e69-183">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-184">P1</span><span class="sxs-lookup"><span data-stu-id="d0e69-184">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-185">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-185">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-186">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-186">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-187">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-187">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d0e69-188">मान्य नहीं है</span><span class="sxs-lookup"><span data-stu-id="d0e69-188">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d0e69-189">नियम #1 का उल्लंघन.</span><span class="sxs-lookup"><span data-stu-id="d0e69-189">Violation of Rule #1.</span></span> <span data-ttu-id="d0e69-190">P1 परियोजना पर समय, ख़र्च और शुल्क दोनों कोटेशन लाइनों, QL1 और QL2 पर शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="d0e69-190">Time, Expense, and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d0e69-191">O1</span><span class="sxs-lookup"><span data-stu-id="d0e69-191">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d0e69-192">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="d0e69-192">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-193">QL2</span><span class="sxs-lookup"><span data-stu-id="d0e69-193">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-194">P1</span><span class="sxs-lookup"><span data-stu-id="d0e69-194">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-195">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-195">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-196">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-196">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-197">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-197">Yes</span></span> </p>
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
<span data-ttu-id="d0e69-198">O1</span><span class="sxs-lookup"><span data-stu-id="d0e69-198">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d0e69-199">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="d0e69-199">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-200">QL1</span><span class="sxs-lookup"><span data-stu-id="d0e69-200">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-201">P1</span><span class="sxs-lookup"><span data-stu-id="d0e69-201">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-202">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-202">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-203">No</span><span class="sxs-lookup"><span data-stu-id="d0e69-203">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-204">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-204">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d0e69-205">मान्य नहीं है</span><span class="sxs-lookup"><span data-stu-id="d0e69-205">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d0e69-206">नियम #1 का उल्लंघन.</span><span class="sxs-lookup"><span data-stu-id="d0e69-206">Violation of Rule #1.</span></span> <span data-ttu-id="d0e69-207">P1 परियोजना पर समय और शुल्क दोनों कोटेशन लाइनों, QL1 और QL2 पर शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="d0e69-207">Time and Fees on P1 project are included on both quote lines, QL1 and QL2.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d0e69-208">O1</span><span class="sxs-lookup"><span data-stu-id="d0e69-208">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d0e69-209">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="d0e69-209">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-210">QL2</span><span class="sxs-lookup"><span data-stu-id="d0e69-210">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-211">P1</span><span class="sxs-lookup"><span data-stu-id="d0e69-211">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-212">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-212">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-213">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-213">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-214">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-214">Yes</span></span> </p>
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
<span data-ttu-id="d0e69-215">O1</span><span class="sxs-lookup"><span data-stu-id="d0e69-215">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d0e69-216">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="d0e69-216">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-217">QL1</span><span class="sxs-lookup"><span data-stu-id="d0e69-217">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-218">P1</span><span class="sxs-lookup"><span data-stu-id="d0e69-218">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-219">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-219">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-220">No</span><span class="sxs-lookup"><span data-stu-id="d0e69-220">No</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-221">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-221">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d0e69-222">मान्य</span><span class="sxs-lookup"><span data-stu-id="d0e69-222">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                 <p>
<span data-ttu-id="d0e69-223">P1 परियोजना पर समय और शुल्क QL1 पर शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="d0e69-223">Time and fees on P1 project are included on QL1.</span></span>
<span data-ttu-id="d0e69-224">P1 परियोजना पर ख़र्च QL2 पर शामिल है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-224">Expense on P1 project is included on QL2.</span></span>
<span data-ttu-id="d0e69-225">प्रत्येक कोटेशन लाइन पर जो भी शामिल किया जा रहा है उनमें ओवरलैप नहीं है इसलिए यह मान्य है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-225">There is no overlap in what is being included on each quote line so it is valid.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d0e69-226">O1</span><span class="sxs-lookup"><span data-stu-id="d0e69-226">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d0e69-227">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="d0e69-227">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-228">QL2</span><span class="sxs-lookup"><span data-stu-id="d0e69-228">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-229">P1</span><span class="sxs-lookup"><span data-stu-id="d0e69-229">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-230">No</span><span class="sxs-lookup"><span data-stu-id="d0e69-230">No</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-231">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-231">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-232">No</span><span class="sxs-lookup"><span data-stu-id="d0e69-232">No</span></span> </p>
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
<span data-ttu-id="d0e69-233">O1</span><span class="sxs-lookup"><span data-stu-id="d0e69-233">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d0e69-234">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="d0e69-234">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-235">QL1</span><span class="sxs-lookup"><span data-stu-id="d0e69-235">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-236">P1</span><span class="sxs-lookup"><span data-stu-id="d0e69-236">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-237">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-237">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-238">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-238">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-239">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-239">Yes</span></span> </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d0e69-240">मान्य नहीं है</span><span class="sxs-lookup"><span data-stu-id="d0e69-240">Not valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d0e69-241">नियम #1 का उल्लंघन</span><span class="sxs-lookup"><span data-stu-id="d0e69-241">Violation of Rule #1 above</span></span> </p>
                <p>
<span data-ttu-id="d0e69-242">Q1 में संपूर्ण परियोजना P1 के लिए समय, ख़र्च और शुल्क शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="d0e69-242">Q1 includes Time, Expenses, and Fees for the whole project P1.</span></span>
                </p>
                <p>
<span data-ttu-id="d0e69-243">QL2 में संपूर्ण परियोजना P1 के लिए समय, ख़र्च और शुल्क शामिल हैं और Q1 पर जो भी शामिल है उसके साथ ओवरलैप करती है.</span><span class="sxs-lookup"><span data-stu-id="d0e69-243">QL2 includes Time, Expenses, and Fees for the whole project P1 and overlaps with what is included on Q1.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d0e69-244">O1</span><span class="sxs-lookup"><span data-stu-id="d0e69-244">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d0e69-245">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="d0e69-245">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-246">QL2</span><span class="sxs-lookup"><span data-stu-id="d0e69-246">QL2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-247">P1</span><span class="sxs-lookup"><span data-stu-id="d0e69-247">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-248">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-248">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-249">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-249">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-250">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-250">Yes</span></span> </p>
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
<span data-ttu-id="d0e69-251">O1</span><span class="sxs-lookup"><span data-stu-id="d0e69-251">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d0e69-252">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="d0e69-252">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-253">QL1</span><span class="sxs-lookup"><span data-stu-id="d0e69-253">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-254">P1</span><span class="sxs-lookup"><span data-stu-id="d0e69-254">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-255">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-255">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-256">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-256">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-257">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-257">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="d0e69-258">मान्य</span><span class="sxs-lookup"><span data-stu-id="d0e69-258">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d0e69-259">नियम #2 के आधार पर, Q1 और Q2 एक ही अवसर पर दो उद्धरण हैं, इसलिए वे दोनों एक परियोजना के समान घटकों के लिए अनुमान लगा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="d0e69-259">Based on Rule #2, Q1 and Q2 are two quotes on the same opportunity, so they can both estimate for the same components of a project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d0e69-260">O1</span><span class="sxs-lookup"><span data-stu-id="d0e69-260">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d0e69-261">तिमाही 2</span><span class="sxs-lookup"><span data-stu-id="d0e69-261">Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-262">Q2 पर QL1</span><span class="sxs-lookup"><span data-stu-id="d0e69-262">QL1 on Q2</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-263">P1</span><span class="sxs-lookup"><span data-stu-id="d0e69-263">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-264">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-264">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-265">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-265">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-266">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-266">Yes</span></span> </p>
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
<span data-ttu-id="d0e69-267">O1</span><span class="sxs-lookup"><span data-stu-id="d0e69-267">O1</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d0e69-268">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="d0e69-268">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-269">QL1</span><span class="sxs-lookup"><span data-stu-id="d0e69-269">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-270">P1</span><span class="sxs-lookup"><span data-stu-id="d0e69-270">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-271">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-271">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-272">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-272">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-273">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-273">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="d0e69-274">मान्य</span><span class="sxs-lookup"><span data-stu-id="d0e69-274">Valid</span></span> </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
<span data-ttu-id="d0e69-275">नियम #3 पर आधारित, Q1 और Q2 विभिन्न अवसरों पर दो कोटेशन हैं, इसलिए वे एक ही परियोजना के समान घटकों के लिए अनुमान नहीं लगा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="d0e69-275">Based on Rule #3, Q1 and Q2 are two quotes on different opportunities, so they can't estimate for the same components of the same project.</span></span>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
<span data-ttu-id="d0e69-276">O2</span><span class="sxs-lookup"><span data-stu-id="d0e69-276">O2</span></span> </p>
            </td>
            <td width="41" valign="top">
                <p>
<span data-ttu-id="d0e69-277">तिमाही 1</span><span class="sxs-lookup"><span data-stu-id="d0e69-277">Q1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-278">QL1</span><span class="sxs-lookup"><span data-stu-id="d0e69-278">QL1</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-279">P1</span><span class="sxs-lookup"><span data-stu-id="d0e69-279">P1</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-280">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-280">Yes</span></span> </p>
            </td>
            <td width="48" valign="top">
                <p>
<span data-ttu-id="d0e69-281">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-281">Yes</span></span> </p>
            </td>
            <td width="42" valign="top">
                <p>
<span data-ttu-id="d0e69-282">हाँ</span><span class="sxs-lookup"><span data-stu-id="d0e69-282">Yes</span></span> </p>
            </td>
            <td width="54" valign="top">
                <p>
<span data-ttu-id="d0e69-283">मान्य नहीं है</span><span class="sxs-lookup"><span data-stu-id="d0e69-283">Not Valid</span></span> </p>
            </td>
        </tr>
    </tbody>
</table>



[!INCLUDE[footer-include](../includes/footer-banner.md)]