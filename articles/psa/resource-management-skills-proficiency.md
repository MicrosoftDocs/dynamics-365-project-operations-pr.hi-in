---
title: कौशल और दक्षता मॉडल्स
description: इस टॉपिक में कौशल और प्रवीणता मॉडल का उपयोग करने के तरीके के बारे में जानकारी प्रदान की गई है।
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/13/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 82eeab4c9682e5b777da4e66f6c4f3f1afb3c19b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5282965"
---
# <a name="skills-and-proficiency-models"></a><span data-ttu-id="f33dc-103">कौशल और दक्षता मॉडल्स</span><span class="sxs-lookup"><span data-stu-id="f33dc-103">Skills and proficiency models</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="f33dc-104">कौशल संसाधनों की वे विशेषताएँ हैं जो Dynamics 365 Project Service Automation और Dynamics 365 Field Service के बीच (यदि मौजूद हो तो) साझा की जाती हैं।</span><span class="sxs-lookup"><span data-stu-id="f33dc-104">Skills are resource characteristics that are shared between Dynamics 365 Project Service Automation and if present, Dynamics 365 Field Service.</span></span> 

<span data-ttu-id="f33dc-105">Project Service Automation में कौशलों की रिपॉज़िटरी बनाए रखने के लिए **संसाधन** \> **संसाधनों के कौशल** पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="f33dc-105">To maintain the repository of skills in Project Service Automation, go to **Resources** \> **Resource Skills**.</span></span> 

> ![संसाधन कौशल](media/Resource-Management-image84.png)

## <a name="use-proficiency-models-to-rate-resources"></a><span data-ttu-id="f33dc-107">संसाधनों को रेट करने के लिए दक्षता मॉडल का उपयोग करें</span><span class="sxs-lookup"><span data-stu-id="f33dc-107">Use proficiency models to rate resources</span></span>

<span data-ttu-id="f33dc-108">संसाधनों के कौशलों का मूल्यांकन दक्षता मॉडल से किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="f33dc-108">Skills for resources are rated by proficiency models.</span></span> <span data-ttu-id="f33dc-109">व्यक्तिगत रेटिंग एक दक्षता मॉडल में हैं.</span><span class="sxs-lookup"><span data-stu-id="f33dc-109">The individual ratings are in a proficiency model.</span></span> 

1. <span data-ttu-id="f33dc-110">प्रवीणता मॉडल बनाने के लिए **संसाधन** \> **प्रवीणता मॉडल** पर जाएं और फिर **नया** का चुनाव करें।</span><span class="sxs-lookup"><span data-stu-id="f33dc-110">To create a proficiency model, go to **Resources** \> **Proficiency Models**, and then select **New**.</span></span>
2. <span data-ttu-id="f33dc-111">नए रेटिंग मॉडल में न्यूनतम रेटिंग का मान, अधिकतम रेटिंग का मान और जिस इकाई को रेटिंग दी जा रही है, उसके बारे में जानकारी दें।</span><span class="sxs-lookup"><span data-stu-id="f33dc-111">In the new rating model, specify the minimum rating value, the maximum rating value, and the entity that is being rated.</span></span>
3. <span data-ttu-id="f33dc-112">**रेटिंग मान** सबग्रिड में आप न्यूनतम से लेकर अधिकतम तक रेटिंग के विभिन्न मान परिभाषित कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="f33dc-112">In the **Rating Values** subgrid, you can define the different rating values, from the minimum to the maximum.</span></span>

> ![न्यूनतम और अधिकतम रेटिंग्स निर्धारित](media/Resource-Management-image85.png)

<span data-ttu-id="f33dc-114">ये रेटिंग मान **संसाधनों की आवश्यकताएँ**, **शेड्यूल बोर्ड**, और **शेड्यूल असिस्टेंट** फ़िल्टर पर दर्शाये जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="f33dc-114">These rating values are shown on the **Resource Requirements**, **Schedule Board**, and **Schedule Assistant** filters.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]