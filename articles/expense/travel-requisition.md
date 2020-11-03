---
title: यात्रा की आवश्यकता
description: यह विषय यात्रा मांग-पत्र के बारे में जानकारी प्रदान करता है.
author: suvaidya
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 0261405abb9305d7f6abcde9cb90d9b184868580
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077569"
---
# <a name="travel-requisitions"></a><span data-ttu-id="12cc8-103">यात्रा की आवश्यकता</span><span class="sxs-lookup"><span data-stu-id="12cc8-103">Travel requisitions</span></span>

<span data-ttu-id="12cc8-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="12cc8-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="12cc8-105">यात्रा की आवश्यकता उन खर्चों को सूचीबद्ध करती है जो यात्रा के उद्देश्य से किए जाएंगे।</span><span class="sxs-lookup"><span data-stu-id="12cc8-105">A travel requisition lists the expenses that will be incurred for the purpose of travel.</span></span> <span data-ttu-id="12cc8-106">यात्रा आवश्यकता समीक्षा के लिए सबमिट की जाती है और इसे खर्चों को अधिकृत करने के लिए उपयोग किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="12cc8-106">A travel requisition is submitted for review and can be used to authorize expenses.</span></span>

<span data-ttu-id="12cc8-107">इससे पहले कि आप ऐसा कोई खर्च करें जिसे संगठन से वसूला जाना है आपको यात्रा आवश्यकता सबमिट करनी होगी।</span><span class="sxs-lookup"><span data-stu-id="12cc8-107">You may be required to submit a travel requisition before you incur any expense that is charged to the organization.</span></span> <span data-ttu-id="12cc8-108">यह आवश्यकता लागू होती है, इस बात पर ध्यान दिए बिना कि आप किसी कॉर्पोरेट क्रेडिट कार्ड से खर्च करते हैं, नकद अग्रिम से प्राप्त नकद खर्च करते हैं, या जेब से खर्च उठाते हैं जिसकी संगठन द्वारा प्रतिपूर्ति की जाएगी।</span><span class="sxs-lookup"><span data-stu-id="12cc8-108">This requirement applies, regardless of whether you charge expenses to a corporate credit card, spend cash that you received from a cash advance, or incur out-of-pocket expenses that will be reimbursed by the organization.</span></span>

<span data-ttu-id="12cc8-109">यात्रा व्यय और नीतियों का उपयोग संगठन व्यय को प्रबंधित करने में मदद के लिए किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="12cc8-109">Travel requisitions and policies can be used to help manage organization expenditures.</span></span> <span data-ttu-id="12cc8-110">उदाहरण के लिए, यदि आपका संगठन एक निश्चित मूल्य की परियोजना पर काम कर रहा है जिसमें यात्रा की आवश्यकता है, तो परियोजना टीम के सदस्यों का यात्रा व्यय परियोजना बजट के भीतर होना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="12cc8-110">For example, if your organization is working on a fixed-price project that requires travel, the travel expenses of the project's team members must fit within the project budget.</span></span> <span data-ttu-id="12cc8-111">यह मांग करके कि यात्रा के खर्चों को करने से पहले मंजूरी दे दी जाए, संगठन यह सुनिश्चित करने में मदद कर सकता है कि परियोजना बजट के भीतर बनी हुई है।</span><span class="sxs-lookup"><span data-stu-id="12cc8-111">By requiring that travel expenses be approved before they are incurred, the organization can help make sure that the project remains within budget.</span></span>

## <a name="configuration"></a><span data-ttu-id="12cc8-112">कॉन्फ़िगरेशन</span><span class="sxs-lookup"><span data-stu-id="12cc8-112">Configuration</span></span> 

<span data-ttu-id="12cc8-113">व्यय प्रबंधन मापदंड में "यात्रा का पूर्व-प्राधिकरण अनिवार्य है" मापदंड को सक्षम करके यात्रा आवश्यकताओं को "अनिवार्य" के रूप में कॉन्फ़िगर किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="12cc8-113">Travel Requisitions can be configured as "mandatory" by enabling the "Pre-authorization of travel is mandatory" parameter in Expense Management Parameters.</span></span> 

## <a name="create-and-submit-a-travel-requisition"></a><span data-ttu-id="12cc8-114">एक यात्रा आवश्यकता बनाएं और सबमिट करें</span><span class="sxs-lookup"><span data-stu-id="12cc8-114">Create and submit a travel requisition</span></span>

1. <span data-ttu-id="12cc8-115">**मेरे खर्च: यात्रा आवश्यकता** , पर जाएं, और **नई यात्रा आवश्यकता** चुनें।</span><span class="sxs-lookup"><span data-stu-id="12cc8-115">Go to **My expenses: Travel Requisition** , and select **New travel Requisition**.</span></span>
2. <span data-ttu-id="12cc8-116">आवश्यकता के लिए उद्देश्य और मंजिल दर्ज करें।</span><span class="sxs-lookup"><span data-stu-id="12cc8-116">Enter a purpose and destination for the requisition.</span></span>
3. <span data-ttu-id="12cc8-117">**यात्रा विवरण** फ़ील्ड में, कोई भी अतिरिक्त जानकारी दर्ज करें।</span><span class="sxs-lookup"><span data-stu-id="12cc8-117">In the  **Travel description** field, enter any additional information.</span></span> 
4. <span data-ttu-id="12cc8-118">प्रत्येक अपेक्षित खर्चों के लिए, जैसे उड़ान, भोजन, या कार किराए पर लेना, एक खर्च लाइन आइटम बनाएं।</span><span class="sxs-lookup"><span data-stu-id="12cc8-118">For each of the expected expenses, such as Flight, meals, or car rental, create an expense line item.</span></span> <span data-ttu-id="12cc8-119">प्रत्येक खर्च के लिए अनुमानित तिथि, अनुमानित राशि और मुद्रा शामिल करें।</span><span class="sxs-lookup"><span data-stu-id="12cc8-119">Include the estimated date, estimated amount, and the currency for each expense.</span></span> 
5. <span data-ttu-id="12cc8-120">जब आप अपेक्षित खर्चों को जोड़ना समाप्त कर लें, तो **सहेजें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="12cc8-120">When you have finished adding the expected expenses, select **Save**.</span></span>
6. <span data-ttu-id="12cc8-121">जब आप यात्रा की आवश्यकता को सबमिट करने के लिए तैयार हों, तो **वर्कफ़्लो** > **सबमिट** चुनें।</span><span class="sxs-lookup"><span data-stu-id="12cc8-121">When you are ready to submit the travel requisition, select **Workflow** > **Submit**.</span></span>

<span data-ttu-id="12cc8-122">आप **मेरे व्यय: यात्रा आवश्यकता** के तहत अपनी स्वीकृत यात्रा आवश्यकताओं को देख सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="12cc8-122">You can view your approved travel requisitions under **My Expenses: Travel Requisition**.</span></span> 

## <a name="view-available-travel-requisitions"></a><span data-ttu-id="12cc8-123">उपलब्ध यात्रा आवश्यकताएं देखें</span><span class="sxs-lookup"><span data-stu-id="12cc8-123">View available travel requisitions</span></span>

<span data-ttu-id="12cc8-124">आप अपनी यात्रा की सभी आवश्यकताएं **मेरे व्यय: यात्रा आवश्यकताएं** के तहत देख सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="12cc8-124">You can view all of your travel requisitions under **My Expenses: Travel Requisitions**.</span></span>

## <a name="approve-travel-requisitions"></a><span data-ttu-id="12cc8-125">मंजूरी यात्रा की आवश्यकता</span><span class="sxs-lookup"><span data-stu-id="12cc8-125">Approve travel requisitions</span></span>

<span data-ttu-id="12cc8-126">उस यात्रा आवश्यकता का चयन करें जिसे आप स्वीकृत करना चाहते हैं, और फिर **वर्कफ़्लो** > **स्वीकृत करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="12cc8-126">Select the travel requisition that you want to approve, and then select **Workflow** > **Approve**.</span></span>  

## <a name="submit-an-expense-report-using-your-approved-travel-requisition"></a><span data-ttu-id="12cc8-127">अपनी स्वीकृत यात्रा आवश्यकता का उपयोग करके व्यय रिपोर्ट सबमिट करें</span><span class="sxs-lookup"><span data-stu-id="12cc8-127">Submit an expense report using your approved travel requisition</span></span>

1. <span data-ttu-id="12cc8-128">नई व्यय रिपोर्ट बनाएं और व्यय रिपोर्ट हेडर में, और स्वीकृत यात्रा आवश्यकताओं की सूची से, **यात्रा आवश्यकता के लिए मानचित्र** चुनें।</span><span class="sxs-lookup"><span data-stu-id="12cc8-128">Create a new expense report and in the expense report header, and from the list of approved travel requisitions, select **Map to Travel requisition**.</span></span>
2. <span data-ttu-id="12cc8-129">व्यय रिपोर्ट हेडर में **यात्रा आवश्यकता राशि** फ़ील्ड अपने आप अपडेट हो जाती है।</span><span class="sxs-lookup"><span data-stu-id="12cc8-129">The **Travel requisition amount** field is automatically updated in the expense report header.</span></span>
3. <span data-ttu-id="12cc8-130">यात्रा के लिए किए गए प्रत्येक व्यय को जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="12cc8-130">Add each expense incurred for the trip.</span></span> <span data-ttu-id="12cc8-131">यदि **पूर्व-अधिकृत** फ़ील्ड सक्षम है, तो विशिष्ट व्यय श्रेणी के लिए मिलान राशि और अधिकृत राशि अपडेट की जाएगी।</span><span class="sxs-lookup"><span data-stu-id="12cc8-131">If the **Pre-authorized** field is enabled, the reconciled amount and authorized amount for the specific expense category will be updated.</span></span>

> [!NOTE]
> <span data-ttu-id="12cc8-132">जब आप किसी स्वीकृत यात्रा आवश्यकता के लिए व्यय रिपोर्ट मैप करते हैं, तो लेनदेन राशि अधिकृत राशि से अधिक नहीं हो सकती है।</span><span class="sxs-lookup"><span data-stu-id="12cc8-132">When you map an expense report to an approved travel requisition, the transaction amount can't be greater than the authorized amount.</span></span> 
