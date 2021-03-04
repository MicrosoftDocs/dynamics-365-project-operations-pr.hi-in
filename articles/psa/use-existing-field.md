---
title: मूल्य निर्धारण आयाम के रूप में Project Service में एक मौजूदा फ़ील्ड का उपयोग करें
description: यह विषय मूल्य निर्धारण आयामों के रूप में मौजूदा Project Service क्षेत्रों के उपयोग के बारे में जानकारी प्रदान करता है।
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 11/19/2018
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 8bc3a1df7669dac43b45d781448ed5c795a65be4
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144161"
---
# <a name="use-an-existing-field-in-project-service-as-a-pricing-dimension"></a><span data-ttu-id="71289-103">मूल्य निर्धारण आयाम के रूप में Project Service में एक मौजूदा फ़ील्ड का उपयोग करें</span><span class="sxs-lookup"><span data-stu-id="71289-103">Use an existing field in Project Service as a pricing dimension</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="71289-104">Project Service Automation (PSA) में **वास्तविक** इकाई में कई क्षेत्र हैं जिनका उपयोग परियोजना संस्थानों में संसाधन-आधारित मूल्य निर्धारण के लिए मूल्य निर्धारण आयामों के रूप में किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="71289-104">Project Service Automation (PSA) has many fields on the **Actuals** entity that can be used as pricing dimensions for resource-based pricing in project organizations.</span></span> <span data-ttu-id="71289-105">उदाहरण के लिए, एक सामान्य क्षेत्र **बुक करने योग्य संसाधन** है।</span><span class="sxs-lookup"><span data-stu-id="71289-105">For example, one common field is **Bookable Resource**.</span></span> <span data-ttu-id="71289-106">छोटी कंपनियां जिनके पास 20-30 से कम बिल योग्य संसाधन हैं, उनके लिए प्रत्येक संसाधन के लिए विशिष्ट बिल और लागत दरें होना, एक सरल तरीका है।</span><span class="sxs-lookup"><span data-stu-id="71289-106">Smaller companies that have fewer than 20-30 billable resources may find that having bill and cost rates specific to each resource is a simpler approach.</span></span> <span data-ttu-id="71289-107">हालांकि, जैसा कि बिल योग्य कार्यबल बढ़ता है, इसे बनाए रखने के लिए विशिष्ट दरें अवास्तविक हो सकती है, क्योंकि जैसे-जैसे संसाधनों को बढ़ावा मिलता है, अधिक अनुभव प्राप्त होता है या एक अलग स्किल सेट अर्जित होता है, तो संसाधन की लागत और बिल दरों में भिन्नता आने लगती है.</span><span class="sxs-lookup"><span data-stu-id="71289-107">However, as the billable workforce grows, specific rates could become unrealistic to maintain as resource cost and bill rates begin to vary as resources get promoted, gain more experience, or acquire a different skill set.</span></span> <span data-ttu-id="71289-108">क्योंकि यह तरीका अभी भी एक निश्चित आकार की कंपनियों के लिए काम करता है, यह समझने के लिए कि मौजूदा Project Service फ़ील्ड को मूल्य निर्धारण आयाम के रूप में कैसे उपयोग किया जा सकता है, [मूल्य निर्धारण आयाम के रूप में एक बुक करने योग्य संसाधन का उपयोग करें](bookable-resource-pricing-dimension.md) देखें.</span><span class="sxs-lookup"><span data-stu-id="71289-108">Because this approach still works for companies of a certain size, see [Use a bookable resource as a pricing dimension](bookable-resource-pricing-dimension.md) to understand how an existing Project Service field can be used as a pricing dimension.</span></span>

<span data-ttu-id="71289-109">एक अन्य उदाहरण लेन-देन श्रेणी का है।</span><span class="sxs-lookup"><span data-stu-id="71289-109">Another example is that of transaction category.</span></span> <span data-ttu-id="71289-110">ग्राहकों और कार्यान्वयनकर्ताओं ने कार्य को वर्गीकृत करने और कार्य की श्रेणी के आधार पर मूल्य और लागत के क्षेत्र का उपयोग करने के लिए PSA में लेन-देन श्रेणी का उपयोग किया है।</span><span class="sxs-lookup"><span data-stu-id="71289-110">Customers and Implementers have used the transaction category in PSA to classify work and use the field to price and cost based on the category of work.</span></span> <span data-ttu-id="71289-111">अधिक जानकारी के लिए देखें, [मूल्य निर्धारण आयाम के रूप में लेन-देन श्रेणी का उपयोग करें](transaction-category-pricing-dimension.md).</span><span class="sxs-lookup"><span data-stu-id="71289-111">For more information, see [Use transaction category as a pricing dimension](transaction-category-pricing-dimension.md).</span></span>
