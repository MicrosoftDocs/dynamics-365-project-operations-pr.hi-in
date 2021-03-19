---
title: परियोजना अवस्थाएँ
description: यह विषय Microsoft Dynamics Project Operations में उपलब्ध परियोजना चरणों के बारे में जानकारी देता है.
author: ruhercul
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: a5c695e0cd39f8a222e719cc6c9ffe984fe80b07
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286790"
---
# <a name="project-stages"></a><span data-ttu-id="68496-103">परियोजना अवस्थाएँ</span><span class="sxs-lookup"><span data-stu-id="68496-103">Project stages</span></span>

<span data-ttu-id="68496-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="68496-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="68496-105">परियोजना अवस्थाओं को किसी परियोजना की स्थिति और उसकी प्रगति दर्शाने के लिए अद्यतन किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="68496-105">Project stages are designed to reflect the state of the project as it progresses.</span></span> <span data-ttu-id="68496-106">व्यवसाय प्रोसेस फ़्लो, Power Automate या प्लग-इन एक्सटेंशन के साथ अवस्थाओं का स्वचालित रूप से अद्यतन करने के लिए अनुकूलनों का उपयोग किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="68496-106">Customizations can be used to automatically update the stages with business process flows, Power Automate, or plug-in extensions.</span></span>

<span data-ttu-id="68496-107">डिफाल्ड व्यवसाय प्रक्रिया फ़्लो में निम्नलिखित अवस्थाएँ परिभाषित हैं:</span><span class="sxs-lookup"><span data-stu-id="68496-107">The following stages are defined in the default business process flow:</span></span>

- <span data-ttu-id="68496-108">नया</span><span class="sxs-lookup"><span data-stu-id="68496-108">New</span></span>
- <span data-ttu-id="68496-109">भाव प्रस्ताव</span><span class="sxs-lookup"><span data-stu-id="68496-109">Quote</span></span>
- <span data-ttu-id="68496-110">योजना</span><span class="sxs-lookup"><span data-stu-id="68496-110">Plan</span></span>
- <span data-ttu-id="68496-111">डिलीवर करें</span><span class="sxs-lookup"><span data-stu-id="68496-111">Deliver</span></span>
- <span data-ttu-id="68496-112">पूर्ण करें</span><span class="sxs-lookup"><span data-stu-id="68496-112">Complete</span></span>
- <span data-ttu-id="68496-113">बंद करें</span><span class="sxs-lookup"><span data-stu-id="68496-113">Close</span></span> 

## <a name="new"></a><span data-ttu-id="68496-114">नया</span><span class="sxs-lookup"><span data-stu-id="68496-114">New</span></span>

<span data-ttu-id="68496-115">जब आप एक प्रोजेक्ट बनाते हैं, तो प्रोजेक्ट के चरण को **नया** सेट किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="68496-115">When you create a project, the project stage is set to **New**.</span></span> <span data-ttu-id="68496-116">यदि प्रोजेक्ट को टैम्पलेट द्वारा बनाया गया है तो इसमें शेड्यूल, प्राक्कलन और टीम का डेटा होगा।</span><span class="sxs-lookup"><span data-stu-id="68496-116">If the project was created from a template, it might have schedule, estimate, and team data.</span></span> <span data-ttu-id="68496-117">अन्यथा, यह प्रोजेक्ट का केवल आउटलाइन होगा और शेष घटकों को दर्ज करना होगा.</span><span class="sxs-lookup"><span data-stu-id="68496-117">Otherwise, it's an outline of the project, and the remaining components must be entered.</span></span>

## <a name="quote"></a><span data-ttu-id="68496-118">कोट</span><span class="sxs-lookup"><span data-stu-id="68496-118">Quote</span></span>

<span data-ttu-id="68496-119">जब आप एक प्रोजेक्ट को एक कोट से जोड़ते हैं या जब आप कोट से प्रोजेक्ट बनाते हैं तो प्रोजेक्ट की अवस्था **कोट** में सेट की जाती है और आकलन प्रारंभ व अंतिम तिथियाँ अपडेट की जाती हैं।</span><span class="sxs-lookup"><span data-stu-id="68496-119">When you associate a project with a quote, or when you create a project from a quote, the project stage is set to **Quote**, and the estimated start and end dates are updated.</span></span> <span data-ttu-id="68496-120">जब प्रोजेक्ट **कोट** चरण में होता है तो **प्रोजेक्ट एंटिटी** पेज पर **विक्रय** टैब कोट के विवरण दिखाता है।</span><span class="sxs-lookup"><span data-stu-id="68496-120">While the project is in the **Quote** stage, the **Sales** tab on the **Project Entity** page shows details of the quote.</span></span>

## <a name="plan"></a><span data-ttu-id="68496-121">योजना</span><span class="sxs-lookup"><span data-stu-id="68496-121">Plan</span></span>

<span data-ttu-id="68496-122">जब आपका कोट स्वीकृत होता है जो किसी प्रोजेक्ट से संबद्ध होता है और प्रोजेक्ट को **अनुबंध** अवस्था में भेजा जाता है, तो प्रोजेक्ट की अवस्था को **योजना** में अपडेट किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="68496-122">When you win a quote that is associated with a project, and the project is moved to the **Contract** phase, the project stage is updated to **Plan**.</span></span> <span data-ttu-id="68496-123">जब प्रोजेक्ट **योजना** अवस्था में होता है तो **प्रोजेक्ट एंटिटी** पेज अनुबंध के विवरण दिखाता है।</span><span class="sxs-lookup"><span data-stu-id="68496-123">While the project is in the **Plan** stage, the **Project Entity** page shows details of the contract.</span></span>

## <a name="deliver"></a><span data-ttu-id="68496-124">डिलीवर करें</span><span class="sxs-lookup"><span data-stu-id="68496-124">Deliver</span></span>

<span data-ttu-id="68496-125">जब प्रोजेक्ट की योजना पूरी हो जाती है और प्रोजेक्ट को शुरु करने के लिए तैयार होते हैं तो प्रोजेक्ट मैनेजर को प्रोजेक्ट की अवस्था को **डिलीवर** में अपडेट करनी चाहिए ताकि यह दिखाया जा सके कि प्रोजेक्ट शुरु हो गया है।</span><span class="sxs-lookup"><span data-stu-id="68496-125">When the project plan is completed, and you're ready to start the project, the project manager should update the project stage to **Deliver** to show that the project has started.</span></span>

## <a name="complete"></a><span data-ttu-id="68496-126">पूर्ण</span><span class="sxs-lookup"><span data-stu-id="68496-126">Complete</span></span> 

<span data-ttu-id="68496-127">जब प्रोजेक्ट का काम पूरी हो जाता है तो प्रोजेक्ट मैनेजर इस अवस्था को **पूर्ण** में अपडेट कर सकता है।</span><span class="sxs-lookup"><span data-stu-id="68496-127">When the work for the project is completed, the project manager can update the stage to **Complete**.</span></span> <span data-ttu-id="68496-128">प्रोजेक्ट अवस्था को **पूर्ण** में अपडेट करते हुए, प्रोजेक्ट मैनेजर यह दर्शाते हैं कि काम 100 प्रतिशत पूरी हो गया है लेकिन प्रोजेक्ट को खुला रखा गया है ताकि किसी लंबित समय या खर्च की प्रविष्टियाँ की जा सकें।</span><span class="sxs-lookup"><span data-stu-id="68496-128">By updating the project stage to **Complete**, the project manager indicates that the work is 100-percent completed, but that the project is being kept open so that any pending time or expense entries can be recorded.</span></span>

## <a name="close"></a><span data-ttu-id="68496-129">बंद करें</span><span class="sxs-lookup"><span data-stu-id="68496-129">Close</span></span>

<span data-ttu-id="68496-130">जब किसी प्रोजेक्ट के सभी लेनदेन दर्ज कर लिए जाते हैं तो प्रोजेक्ट मैनेजर इस अवस्था को **बंद करें** में अपडेट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="68496-130">When all transactions are recorded for the project, the project manager can update the stage to **Close**.</span></span> <span data-ttu-id="68496-131">इस समय, कोई लेनदेन दर्ज नहीं किए जा सकते और प्रोजेक्ट केवल पाठीय में सेट हो जाता है।</span><span class="sxs-lookup"><span data-stu-id="68496-131">At that point, no transactions can be recorded, and the project is set to read-only.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]