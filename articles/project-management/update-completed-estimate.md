---
title: पूर्णता पर अनुमानित लागत अद्यतित करें
description: यह विषय परियोजना पर प्रयास के अनुमान को अद्यतन करने के बारे में जानकारी देता है.
author: ruhercul
manager: AnnBe
ms.date: 09/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 16393133a5de17308caceb069d7bca670caa04c8
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077883"
---
# <a name="update-estimate-at-completion"></a><span data-ttu-id="e5178-103">पूर्णता पर अनुमानित लागत अद्यतित करें</span><span class="sxs-lookup"><span data-stu-id="e5178-103">Update estimate at completion</span></span>

<span data-ttu-id="e5178-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="e5178-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e5178-105">टास्क के मूल अनुमानों को संशोधित करना प्रोजेक्ट मैनेजर के लिए आम बात है।</span><span class="sxs-lookup"><span data-stu-id="e5178-105">It's common for a project manager to revise the original estimates on a task.</span></span> <span data-ttu-id="e5178-106">परियोजना की चालू अवस्था के बारे में, परियोजना का दोबारा अनुमान लगाना, दृष्टिकोण को लेकर परियोजना प्रबंधक के विचार होते हैं.</span><span class="sxs-lookup"><span data-stu-id="e5178-106">Project reprojections are a project manager's perception of estimates, given the current state of a project.</span></span> <span data-ttu-id="e5178-107">बहरहाल, हम इस बात की सिफारिश नहीं करते कि प्रोजेक्ट मैनेजर बेसलाइन अंकों को बदलें क्योंकि प्रोजेक्ट की बेसलाइन प्रोजेक्ट के शेड्यूल और लागत के प्राक्कलनों की सच्चाई के स्थापित स्रोत होती है और लागत अनुमान और प्रोजेक्ट के सभी भागीदार उस पर सहमत होते हैं।</span><span class="sxs-lookup"><span data-stu-id="e5178-107">However, we don't recommend that project managers change the baseline numbers, because the project baseline represents the established source of truth for the project's schedule and cost estimate, and all project stakeholders have agreed to it.</span></span>

<span data-ttu-id="e5178-108">ऐसे दो तरीके हैं जिससे परियोजना प्रबंधक कार्यों के प्रयासों का दोबारा अनुमान लगा सकता है:</span><span class="sxs-lookup"><span data-stu-id="e5178-108">There are two ways that a project manager can reproject effort on tasks:</span></span>

- <span data-ttu-id="e5178-109">कार्य में वास्तविक बाकी प्रयास के नए अनुमान के साथ (ETC) को पूरा करने के लिए डिफ़ॉल्ट अनुमान को ओवरराइड करें.</span><span class="sxs-lookup"><span data-stu-id="e5178-109">Override the default estimate to complete (ETC) with a new estimate of the actual remaining effort on the task.</span></span> 
- <span data-ttu-id="e5178-110">टास्क पर सही प्रगति के एक नए अनुमान के साथ डिफ़ॉल्ट प्रगति प्रतिशत को ओवरराइड करें।</span><span class="sxs-lookup"><span data-stu-id="e5178-110">Override the default progress percentage with a new estimate of the true progress on the task.</span></span>

<span data-ttu-id="e5178-111">इनमें से प्रत्येक दृष्टिकोण कार्य के ETC,पूर्ण होने पर अनुमान (EAC) और प्रगति प्रतिशत और कार्य के लिए अनुमानित प्रयास भिन्नता की पुनर्गणना का कारण बनता है.</span><span class="sxs-lookup"><span data-stu-id="e5178-111">Each of these approaches cause a recalculation of the task's ETC, estimate at complete (EAC), and progress percentage, and the projected effort variance on a task.</span></span> <span data-ttu-id="e5178-112">समरी टास्क पर EAC, ETC और प्रगति के प्रतिशत का दोबारा परिकलन किया जाता है और प्रयास की भिन्नता का नया अनुमान किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="e5178-112">The EAC, ETC, and progress percentage on the summary tasks are recalculated, and produce a new projection of effort variance.</span></span>
