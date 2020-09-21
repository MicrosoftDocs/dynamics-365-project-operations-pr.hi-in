---
title: प्रोजेक्ट अवस्थाएँ
description: इस विषय में प्रोजेक्ट के चरणों की जानकारी दी गई है।
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 983c25a0-ed21-4151-a109-b385a88285fa
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 70aa057e127df7ba925e84f5d056a06a4cc8833e
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3751990"
---
# <a name="project-stages"></a><span data-ttu-id="a3223-103">प्रोजेक्ट अवस्थाएँ</span><span class="sxs-lookup"><span data-stu-id="a3223-103">Project stages</span></span> 

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a3223-104">परियोजना के चरणों को किसी परियोजना की स्थिति और उसकी प्रगति दर्शाने के लिए अपडेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="a3223-104">Project stages are updated to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="a3223-105">डिफाल्ट व्यवसाय प्रोसेस फ़्लो स्वचालित रूप से परियोजना के कुछ चरणों को अपडेट कर देता है, जबकि अन्य को परियोजना प्रबंधक मैनुअल रूप से अपडेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="a3223-105">The default business process flow automatically updates some stages of the project while others are manually updated by the project manager.</span></span> 

<span data-ttu-id="a3223-106">डिफाल्ड BPF में निम्नलिखित अवस्थाएँ परिभाषित हैं:</span><span class="sxs-lookup"><span data-stu-id="a3223-106">The following stages are defined in the default BPF:</span></span>

- <span data-ttu-id="a3223-107">नया</span><span class="sxs-lookup"><span data-stu-id="a3223-107">New</span></span>
- <span data-ttu-id="a3223-108">कोट</span><span class="sxs-lookup"><span data-stu-id="a3223-108">Quote</span></span>
- <span data-ttu-id="a3223-109">योजना</span><span class="sxs-lookup"><span data-stu-id="a3223-109">Plan</span></span>
- <span data-ttu-id="a3223-110">डिलीवर करें</span><span class="sxs-lookup"><span data-stu-id="a3223-110">Deliver</span></span>
- <span data-ttu-id="a3223-111">पूर्ण</span><span class="sxs-lookup"><span data-stu-id="a3223-111">Complete</span></span>
- <span data-ttu-id="a3223-112">बंद करें</span><span class="sxs-lookup"><span data-stu-id="a3223-112">Close</span></span> 

## <a name="new"></a><span data-ttu-id="a3223-113">नया</span><span class="sxs-lookup"><span data-stu-id="a3223-113">New</span></span>

<span data-ttu-id="a3223-114">जब आप एक प्रोजेक्ट बनाते हैं, तो प्रोजेक्ट के चरण को **नया** सेट किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="a3223-114">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="a3223-115">यदि प्रोजेक्ट को टैम्पलेट द्वारा बनाया गया है तो इसमें शेड्यूल, प्राक्कलन और टीम का डेटा होगा।</span><span class="sxs-lookup"><span data-stu-id="a3223-115">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="a3223-116">अन्यथा, यह प्रोजेक्ट का केवल आउटलाइन होगा और शेष घटकों को दर्ज करना होगा।</span><span class="sxs-lookup"><span data-stu-id="a3223-116">Otherwise, it's just an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="a3223-117">कोट</span><span class="sxs-lookup"><span data-stu-id="a3223-117">Quote</span></span>

<span data-ttu-id="a3223-118">जब आप एक प्रोजेक्ट को एक कोट से जोड़ते हैं या जब आप कोट से प्रोजेक्ट बनाते हैं तो प्रोजेक्ट की अवस्था **कोट** में सेट की जाती है और आकलन प्रारंभ व अंतिम तिथियाँ अपडेट की जाती हैं।</span><span class="sxs-lookup"><span data-stu-id="a3223-118">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="a3223-119">जब प्रोजेक्ट **कोट** चरण में होता है तो **प्रोजेक्ट एंटिटी** पेज पर **विक्रय** टैब कोट के विवरण दिखाता है।</span><span class="sxs-lookup"><span data-stu-id="a3223-119">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="a3223-120">योजना</span><span class="sxs-lookup"><span data-stu-id="a3223-120">Plan</span></span>

<span data-ttu-id="a3223-121">जब आपका कोट स्वीकृत होता है जो किसी प्रोजेक्ट से संबद्ध होता है और प्रोजेक्ट को **अनुबंध** अवस्था में भेजा जाता है, तो प्रोजेक्ट की अवस्था को **योजना** में अपडेट किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="a3223-121">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="a3223-122">जब प्रोजेक्ट **योजना** अवस्था में होता है तो **प्रोजेक्ट एंटिटी** पेज अनुबंध के विवरण दिखाता है।</span><span class="sxs-lookup"><span data-stu-id="a3223-122">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="a3223-123">डिलीवर करें</span><span class="sxs-lookup"><span data-stu-id="a3223-123">Deliver</span></span>

<span data-ttu-id="a3223-124">जब प्रोजेक्ट की योजना पूरी हो जाती है और प्रोजेक्ट को शुरु करने के लिए तैयार होते हैं तो प्रोजेक्ट मैनेजर को प्रोजेक्ट की अवस्था को **डिलीवर** में अपडेट करनी चाहिए ताकि यह दिखाया जा सके कि प्रोजेक्ट शुरु हो गया है।</span><span class="sxs-lookup"><span data-stu-id="a3223-124">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="a3223-125">पूर्ण</span><span class="sxs-lookup"><span data-stu-id="a3223-125">Complete</span></span> 

<span data-ttu-id="a3223-126">जब प्रोजेक्ट का काम पूरी हो जाता है तो प्रोजेक्ट मैनेजर इस अवस्था को **पूर्ण** में अपडेट कर सकता है।</span><span class="sxs-lookup"><span data-stu-id="a3223-126">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="a3223-127">प्रोजेक्ट अवस्था को **पूर्ण** में अपडेट करते हुए, प्रोजेक्ट मैनेजर यह दर्शाते हैं कि काम 100 प्रतिशत पूरी हो गया है लेकिन प्रोजेक्ट को खुला रखा गया है ताकि किसी लंबित समय या खर्च की प्रविष्टियाँ की जा सकें।</span><span class="sxs-lookup"><span data-stu-id="a3223-127">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="a3223-128">बंद करें</span><span class="sxs-lookup"><span data-stu-id="a3223-128">Close</span></span>

<span data-ttu-id="a3223-129">जब किसी प्रोजेक्ट के सभी लेनदेन दर्ज कर लिए जाते हैं तो प्रोजेक्ट मैनेजर इस अवस्था को **बंद करें** में अपडेट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="a3223-129">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="a3223-130">इस समय, कोई लेनदेन दर्ज नहीं किए जा सकते और प्रोजेक्ट केवल पाठीय में सेट हो जाता है।</span><span class="sxs-lookup"><span data-stu-id="a3223-130">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>
