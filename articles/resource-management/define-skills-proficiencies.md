---
title: कौशल और दक्षता को परिभाषित करें
description: यह विषय संसाधनों के मूल्यांकन के लिए दक्षता मॉडल सेट करने के तरीके के बारे में जानकारी देता है.
author: ruhercul
manager: AnnBe
ms.date: 09/23/2020
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
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 24538ed1d610a0cae4c2badc0fd33c2f738a8338
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077644"
---
# <a name="define-skills-and-proficiencies"></a><span data-ttu-id="99968-103">कौशल और दक्षता को परिभाषित करें</span><span class="sxs-lookup"><span data-stu-id="99968-103">Define skills and proficiencies</span></span>

<span data-ttu-id="99968-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="99968-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="99968-105">कौशल संसाधनों की वे विशेषताएँ हैं जो Dynamics 365 Project Operations और Dynamics 365 Field Service के बीच (यदि मौजूद हो तो) साझा की जाती हैं.</span><span class="sxs-lookup"><span data-stu-id="99968-105">Skills are resource characteristics that are shared between Dynamics 365 Project Operations and if present, Dynamics 365 Field Service.</span></span> 

- <span data-ttu-id="99968-106">परियोजना संचालन में कौशलों की रिपॉज़िटरी बनाए रखने के लिए **संसाधन** \> **संसाधनों के कौशल** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="99968-106">To maintain the repository of skills in Project Operations, go to **Resources** \> **Resource Skills**.</span></span> 

## <a name="use-proficiency-models-to-rate-resources"></a><span data-ttu-id="99968-107">संसाधनों को रेट करने के लिए दक्षता मॉडल का उपयोग करें</span><span class="sxs-lookup"><span data-stu-id="99968-107">Use proficiency models to rate resources</span></span>

<span data-ttu-id="99968-108">संसाधनों के कौशलों का मूल्यांकन दक्षता मॉडल से किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="99968-108">Skills for resources are rated by proficiency models.</span></span> <span data-ttu-id="99968-109">व्यक्तिगत रेटिंग एक दक्षता मॉडल में हैं.</span><span class="sxs-lookup"><span data-stu-id="99968-109">The individual ratings are in a proficiency model.</span></span> 

1. <span data-ttu-id="99968-110">प्रवीणता मॉडल बनाने के लिए **संसाधन** \> **प्रवीणता मॉडल** पर जाएं और फिर **नया** का चुनाव करें।</span><span class="sxs-lookup"><span data-stu-id="99968-110">To create a proficiency model, go to **Resources** \> **Proficiency Models** , and then select **New**.</span></span>
2. <span data-ttu-id="99968-111">नए रेटिंग मॉडल में न्यूनतम रेटिंग का मान, अधिकतम रेटिंग का मान और जिस इकाई को रेटिंग दी जा रही है, उसके बारे में जानकारी दें।</span><span class="sxs-lookup"><span data-stu-id="99968-111">In the new rating model, specify the minimum rating value, the maximum rating value, and the entity that is being rated.</span></span>
3. <span data-ttu-id="99968-112">**रेटिंग मान** सब-ग्रिड में आप न्यूनतम से लेकर अधिकतम तक रेटिंग के विभिन्न मान परिभाषित कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="99968-112">In the **Rating Values** sub-grid, you can define the different rating values, from the minimum to the maximum.</span></span>


<span data-ttu-id="99968-113">ये रेटिंग मान **संसाधनों की आवश्यकताएँ** , **शेड्यूल बोर्ड** , और **शेड्यूल असिस्टेंट** फ़िल्टर पर दर्शाये जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="99968-113">These rating values are shown on the **Resource Requirements** , **Schedule Board** , and **Schedule Assistant** filters.</span></span>
