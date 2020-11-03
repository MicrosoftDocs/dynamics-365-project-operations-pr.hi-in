---
title: समय लागत वास्तविक पर मूल्य को शून्य पर डिफ़ॉल्ट क्यों बनाया जा रहा है?
description: इस समस्या का निवारण करना कि समय लागत वास्तविक पर मूल्य को 0 पर डिफ़ॉल्ट क्यों बनाया जा रहा है.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 44d4952b77ac0a541cdf8e3e55f202c9209efdf4
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077719"
---
# <a name="why-is-the-price-defaulting-to-zero-on-time-cost-actuals"></a><span data-ttu-id="07efe-103">समय लागत वास्तविक पर मूल्य को शून्य पर डिफ़ॉल्ट क्यों बनाया जा रहा है?</span><span class="sxs-lookup"><span data-stu-id="07efe-103">Why is the price defaulting to zero on time cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="07efe-104">यह सामान्य प्रश्न उस वास्तविक के लिए लागू होता है जहाँ लेनदेन श्रेणी समय पर और लेनदेन प्रकार लागत पर सेट है.</span><span class="sxs-lookup"><span data-stu-id="07efe-104">This FAQ applies to actuals where the transaction class is set to Time and transaction type is Cost.</span></span> <span data-ttu-id="07efe-105">निम्न तीन जाँचें इस समस्या का निवारण करने में आपकी मदद करेंगी कि समय लागत वास्तविक पर मूल्य को 0 पर डिफ़ॉल्ट क्यों बनाया जा रहा है.</span><span class="sxs-lookup"><span data-stu-id="07efe-105">The following three checks will help you troubleshoot why the price is defaulting to 0 on time cost actuals.</span></span>
 
## <a name="check-1-identify-the-cost-price-list-for-the-project"></a><span data-ttu-id="07efe-106">जाँच 1: प्रोजेक्ट की लागत मूल्य सूची की पहचान करें</span><span class="sxs-lookup"><span data-stu-id="07efe-106">Check 1: Identify the cost price list for the project</span></span>

<span data-ttu-id="07efe-107">वास्तविक के प्रोजेक्ट फ़ील्ड से प्रोजेक्ट ढूँढें और फिर प्रोजेक्ट पृष्ठ पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="07efe-107">Find the project from the project field of the actual and then go to the project page.</span></span> <span data-ttu-id="07efe-108">फ़ील्ड में अनुबंध इकाई लिंक पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="07efe-108">Click on the contracting unit link in the field.</span></span> <span data-ttu-id="07efe-109">अनुबंध इकाई पृष्ठ पर, यह जाँचें कि लागत मूल्य सूचियाँ ग्रिड में अनुबंध इकाई में एक मूल्य सूची है या नहीं.</span><span class="sxs-lookup"><span data-stu-id="07efe-109">On the Contracting Unit page, check if the contracting unit has a price list in the Cost Price Lists grid.</span></span>

<span data-ttu-id="07efe-110">यदि एक से अधिक मूल्य सूचियाँ हैं, तो आपने समस्या को अलग कर दिया है.</span><span class="sxs-lookup"><span data-stu-id="07efe-110">If there is more than one price list, you have isolated the problem.</span></span> <span data-ttu-id="07efe-111">Project Service केवल एक मूल्य सूची प्रति संगठनात्मक इकाई का समर्थन करती है.</span><span class="sxs-lookup"><span data-stu-id="07efe-111">Project Service only supports one price list per organizational unit.</span></span> <span data-ttu-id="07efe-112">इस निकाय से तब तक सभी मूल्य सूचियाँ निकालें जब तक संगठनात्मक इकाई की लागत मूल्य सूचियाँ ग्रिड में केवल एक मूल्य सूची संलग्न न रह जाए.</span><span class="sxs-lookup"><span data-stu-id="07efe-112">Remove all prices lists from this entity until there is only one price list attached in the Cost Price Lists grid of the Organizational Unit.</span></span>

<span data-ttu-id="07efe-113">यदि संगठनात्मक इकाई से कोई मूल्य सूची संलग्न नहीं है, तो संगठनात्मक इकाई की मुद्रा नोट करें.</span><span class="sxs-lookup"><span data-stu-id="07efe-113">If there are no price lists attached to the Organizational Unit, make a note of the currency of the Organizational unit.</span></span> <span data-ttu-id="07efe-114">Project Service पर जाएँ और मूल्य सूचियाँ टैब खोलें. यह जाँचें कि क्या ऐसी कोई मूल्य सूची है जिसके संदर्भ को लागत और ऐसी मुद्रा पर सेट किया गया है जो संगठनात्मक इकाई की मुद्रा से मेल खाती है.</span><span class="sxs-lookup"><span data-stu-id="07efe-114">Go to the Project Service and then Parameters and open the Price Lists tab. Check if there are any price lists with context set to Cost and currency that matches the currency of the Organizational Unit.</span></span>
 
<span data-ttu-id="07efe-115">यदि ऐसी कोई मूल्य सूची नहीं है जो आपके मापदंड से मेल खाती है, तो आपने समस्या को अलग कर दिया है.</span><span class="sxs-lookup"><span data-stu-id="07efe-115">If there are no price lists that match that criteria, you have isolated the problem.</span></span> <span data-ttu-id="07efe-116">यह सुनिश्चित करें कि आपके पास कम से कम ऐसी एक मूल्य सूची है जिसके संदर्भ को लागत पर सेट किया गया है और जिसकी मुद्रा संगठनात्मक इकाई की मुद्रा से मेल खाती है.</span><span class="sxs-lookup"><span data-stu-id="07efe-116">Make sure to have at least one price list whose context is set to Cost and whose currency matches the currency of the Organizational Unit.</span></span>

<span data-ttu-id="07efe-117">यदि एक से अधिक मूल्य सूची है जो उस मापदंड से मेल खाती है, तो अधिक जाँच करने के लिए इस दस्तावेज़ को पढ़ना जारी रखें.</span><span class="sxs-lookup"><span data-stu-id="07efe-117">If there is more than one price list that match that criteria, continue reading this document to make more checks.</span></span>

## <a name="check-2-are-any-of-the-price-lists-identified-above-valid-for-the-specific-date-of-the-time-cost-actual"></a><span data-ttu-id="07efe-118">जाँच 2: क्या ऊपर पहचानी गई कोई भी मूल्य सूची समय लागत वास्तविक के विशिष्ट दिनांक के लिए मान्य है?</span><span class="sxs-lookup"><span data-stu-id="07efe-118">Check 2: Are any of the price lists identified above valid for the specific date of the time cost actual?</span></span>

<span data-ttu-id="07efe-119">मूल्य को डिफ़ॉल्ट बनाने हेतु Project Service द्वारा किसी मूल्य सूची पर विचार करने के लिए, वह मूल्य सूची समय लागत वास्तविक पर दिनांक के लिए लागू होनी चाहिए.</span><span class="sxs-lookup"><span data-stu-id="07efe-119">For Project Service to consider a price list for defaulting price, that price list should be applicable for the date on the time cost actual.</span></span> <span data-ttu-id="07efe-120">यह देखने के लिए निम्न की जाँच करें कि ऊपर पहचानी गई सूची(सूचियाँ) लागू होती हैं या नहीं.</span><span class="sxs-lookup"><span data-stu-id="07efe-120">Check the following to see if the price list(s) identified above are applicable:</span></span>

- <span data-ttu-id="07efe-121">यह जाँचें कि संलग्न मूल्य सूचियों के लिए सामान्य टैब पर प्रारंभ और समाप्ति दिनांक रिक्त नहीं हैं.</span><span class="sxs-lookup"><span data-stu-id="07efe-121">Check if the start and end dates on the general tab for the price lists attached aren’t empty.</span></span> <span data-ttu-id="07efe-122">यदि ऊपर पहचानी गए मूल्य सूचियों में प्रारंभ और समाप्ति दिनांक रिक्त हैं, तो आपने समस्या को अलग कर दिया है.</span><span class="sxs-lookup"><span data-stu-id="07efe-122">If the start and end dates on price lists identified above are empty, you have isolated the problem.</span></span> 
- <span data-ttu-id="07efe-123">अपने समय लागत वास्तविक पर प्रारंभ दिनांक फ़ील्ड नोट करें और यह जाँचें कि पहचानी गई कोई भी मूल्य सूची उस दिनांक पर लागू होती है या नहीं.</span><span class="sxs-lookup"><span data-stu-id="07efe-123">Make a note of the start date field on your time cost actual and check if any of the price lists identified is applicable for that date.</span></span> <span data-ttu-id="07efe-124">उदाहरण के लिए, समय लागत वास्तविक का दिनांक मूल्य सूची में प्रारंभ दिनांक और समाप्ति दिनांक के भीतर होना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="07efe-124">For example, the date of the time cost actual should fall within the start date and end date on the price list.</span></span> 
    - <span data-ttu-id="07efe-125">यदि ऐसी कोई मूल्य सूची नहीं है जिसमें समय लागत वास्तविक का वह दिनांक शामिल है, तो आपने समस्या को अलग कर दिया है.</span><span class="sxs-lookup"><span data-stu-id="07efe-125">If there is no price list that covers that date on the time cost actual, you have isolated the problem.</span></span> <span data-ttu-id="07efe-126">यह सुनिश्चित करने के लिए मूल्य सूची के प्रारंभ और समाप्ति दिनांक संशोधित करें कि मूल्य सूची में समय लागत वास्तविक का दिनांक शामिल है.</span><span class="sxs-lookup"><span data-stu-id="07efe-126">Modify the start and end dates of the price list to ensure that the price list covers the date of the time cost actual.</span></span> 
    - <span data-ttu-id="07efe-127">यदि एक से अधिक मूल्य सूची है जिसमें समय लागत वास्तविक का दिनांक शामिल है, तो आपने समस्या को अलग कर दिया है.</span><span class="sxs-lookup"><span data-stu-id="07efe-127">If there is more than one price list that covers the date on the time cost actual, you have isolated the problem.</span></span> <span data-ttu-id="07efe-128">आप मूल्य सूची(सूचियों) के प्रारंभ और समाप्ति दिनांक संपादित करके इसका समाधान कर सकते हैं ताकि ऐसी केवल एक मूल्य सूची हो जिसमें समय लागत वास्तविक का दिनांक शामिल हो.</span><span class="sxs-lookup"><span data-stu-id="07efe-128">You can fix this by editing the start and end dates of the price list(s) so that there is only one price list that covers the date of the time cost actual.</span></span> 
    - <span data-ttu-id="07efe-129">यदि ऐसी केवल एक मूल्य सूची है जिसमें समय लागत वास्तविक का दिनांक शामिल है, तो दस्तावेज़ में अगली जाँच पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="07efe-129">If there is only one price list that covers that date of the time cost actual, move to the next check in the document.</span></span>
<span data-ttu-id="07efe-130">आवश्यक समाधान करने के बाद, एक समय प्रविष्टि पुन: बनाएँ, उसे अनुमोदित करें और यह सत्यापित करें कि समय लागत वास्तविक एक वैध मूल्य दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="07efe-130">Once you’ve done made the required fixes, recreate a time entry, approve it, and verify that the time cost actual shows a valid price.</span></span>

## <a name="check-3-is-there-a-price-in-the-price-list-for-the-pricing-dimensions-on-the-time-cost-actual"></a><span data-ttu-id="07efe-131">जाँच 3: क्या समय लागत वास्तविक पर मूल्य निर्धारण आयामों के लिए मूल्य सूची में कोई मूल्य है?</span><span class="sxs-lookup"><span data-stu-id="07efe-131">Check 3: Is there a price in the price list for the pricing dimensions on the time cost actual?</span></span>

<span data-ttu-id="07efe-132">यदि आपने जाँच 1 और जाँच 2 को सफलतापूर्वक पूरा कर लिया है, तो अब आपके पास केवल एक मूल्य सूची होनी चाहिए जो समय लागत वास्तविक के दिनांक के लिए लागू होती है.</span><span class="sxs-lookup"><span data-stu-id="07efe-132">If you have successfully completed Check 1 and Check 2, you should now have only one price list that is applicable for the date of the time cost actual.</span></span> <span data-ttu-id="07efe-133">इस मूल्य सूची को खोलें और भूमिका मू्ल्य टैब पर जाएँ. यह सुनिश्चित करें कि समय लागत वास्तविक पर मूल्य निर्धारण आयामों के लिए ग्रिड में एक पंक्ति मौजूद है.</span><span class="sxs-lookup"><span data-stu-id="07efe-133">Open this Price List and go to the Role Prices tab. Make sure that there is a row in the grid for the pricing dimensions on the time cost actual.</span></span>

<span data-ttu-id="07efe-134">यदि समय लागत वास्तविक पर मूल्य निर्धारण आयामों के लिए भूमिका मू्ल्य ग्रिड में कोई पंक्ति मौजूद नहीं है, तो आपने समस्या को अलग कर दिया है.</span><span class="sxs-lookup"><span data-stu-id="07efe-134">If there is no row in the role price grid for the pricing dimensions on the time cost actual, then you have isolated the problem.</span></span> <span data-ttu-id="07efe-135">आपके समय लागत वास्तविक पर मूल्य निर्धारण आयामों के लिए भूमिका मू्ल्य ग्रिड में एक पंक्ति बनाएँ.</span><span class="sxs-lookup"><span data-stu-id="07efe-135">Create a row in the Role prices grid for the pricing dimensions on your time cost actual.</span></span> <span data-ttu-id="07efe-136">इसे करने के बाद, एक समय प्रविष्टि पुन: बनाएँ, उसे अनुमोदित करें और यह सत्यापित करें कि समय लागत वास्तविक एक वैध मूल्य दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="07efe-136">Once this is done, recreate time entry, approve it, and verify that the time cost actual shows a valid price.</span></span>
 
<span data-ttu-id="07efe-137">यदि उपरोक्त तीनों जाँचें करने के बाद आपको अभी भी अपने समय लागत वास्तविक पर एक वैध मूल्य दिखाई नहीं देता, तो कृपया एक समर्थन टिकट लॉग करें.</span><span class="sxs-lookup"><span data-stu-id="07efe-137">If you still don't see a valid price on your time cost actual after you’ve done the three checks above, please log a support ticket.</span></span>



