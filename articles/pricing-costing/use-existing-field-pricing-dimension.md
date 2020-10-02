---
title: मूल्य निर्धारण पैमानों के रूप में Project Operations फ़ील्ड
description: यह विषय Dynamics 365 Project Operations में मूल्य निर्धारण पैमानों के रूप में फ़ील्ड इस्तेमाल करके जानकारी देता है.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
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
ms.openlocfilehash: 3ddf3098e45fdc9b99067b64df05e2adc0b6ad05
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896418"
---
# <a name="project-operations-fields-as-pricing-dimensions"></a><span data-ttu-id="4c53c-103">मूल्य निर्धारण पैमानों के रूप में Project Operations फ़ील्ड</span><span class="sxs-lookup"><span data-stu-id="4c53c-103">Project Operations fields as pricing dimensions</span></span>

<span data-ttu-id="4c53c-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="4c53c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="4c53c-105">**वास्तविक आंकड़े** निकाय में कई फ़ील्ड हैं जिनका उपयोग साधन-आधारित मूल्य-निर्धारण के लिए मूल्य निर्धारण पैमाने के रूप में किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="4c53c-105">The **Actuals** entity has many fields that can be used as pricing dimensions for resource-based pricing.</span></span> <span data-ttu-id="4c53c-106">उदाहरण के लिए, एक सामान्य क्षेत्र **बुक करने योग्य संसाधन** है।</span><span class="sxs-lookup"><span data-stu-id="4c53c-106">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="4c53c-107">छोटी कंपनियां जिनके पास 20-30 से कम बिल योग्य संसाधन हैं, उनके लिए प्रत्येक संसाधन के लिए विशिष्ट बिल और लागत दरें होना, एक सरल तरीका है।</span><span class="sxs-lookup"><span data-stu-id="4c53c-107">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="4c53c-108">यद्यपि, जैसा कि बिल योग्य कार्यबल बढ़ता है, साधन-विशिष्ट दरें बनाए रखने के लिए अवास्तविक बन सकती हैं.</span><span class="sxs-lookup"><span data-stu-id="4c53c-108">However, as the billable workforce grows, resource-secific rates could become unrealistic to maintain.</span></span> <span data-ttu-id="4c53c-109">साधन की लागत और बिल दर अलग-अलग होने लगती हैं, क्योंकि संसाधन पदोन्नत किए जाते हैं, अधिक अनुभव प्राप्त करते हैं, या कुशलता का अलग सेट प्राप्त होता है.</span><span class="sxs-lookup"><span data-stu-id="4c53c-109">Resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different set of skills.</span></span> 

<span data-ttu-id="4c53c-110">एक अन्य उदाहरण लेन-देन श्रेणी का है।</span><span class="sxs-lookup"><span data-stu-id="4c53c-110">Another example is that of transaction category.</span></span> <span data-ttu-id="4c53c-111">ग्राहकों और कार्यान्वयनकर्ताओं ने कार्य को वर्गीकृत करने और कार्य की श्रेणी के आधार पर मूल्य और लागत के क्षेत्र का उपयोग करने के लिए लेन-देन श्रेणी का उपयोग किया है.</span><span class="sxs-lookup"><span data-stu-id="4c53c-111">Customers and Implementers have used the transaction category to classify work and use the field to price and cost based on the category of work.</span></span>
