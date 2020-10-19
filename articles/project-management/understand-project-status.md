---
title: परियोजना की स्थिति को समझें
description: यह विषय Dynamics 365 परियोजना संचालन में परियोजनाओं को सौंपी गई स्थिति के बारे में जानकारी प्रदान करता है।
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 336e479ad39653af14cca7930fe63e906b7de489
ms.sourcegitcommit: fd8ea1779db2bb39a428f459ae3293c4fd785572
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/06/2020
ms.locfileid: "3965678"
---
# <a name="understand-project-status"></a><span data-ttu-id="fbe3f-103">परियोजना की स्थिति को समझें</span><span class="sxs-lookup"><span data-stu-id="fbe3f-103">Understand project status</span></span>

<span data-ttu-id="fbe3f-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="fbe3f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="fbe3f-105"> **स्थिति** पृष्ठ पर **परियोजना निकाय** अनुभाग लागत और प्रयास के आधार पर परियोजना के स्वास्थ्य का सारांश प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="fbe3f-105">The **Status** section on the **Project Entity** page provides a summary of a project's health based upon cost and effort.</span></span>


## <a name="status-summary-fields"></a><span data-ttu-id="fbe3f-106">स्थिति सारांश फ़ील्ड</span><span class="sxs-lookup"><span data-stu-id="fbe3f-106">Status summary fields</span></span>

- <span data-ttu-id="fbe3f-107"> **संपूर्ण परियोजना स्थिति**  फील्ड एक एडिट करने योग्य फील्ड होता है जो प्रोजेक्ट का संपूर्ण स्टेटस दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="fbe3f-107">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="fbe3f-108">यह फ़ील्ड बढ़ते जोखिम को दर्शाने के लिए हरे, पीले और लाल जैसी रंग-कोडिंग का उपयोग करता.</span><span class="sxs-lookup"><span data-stu-id="fbe3f-108">This field uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> 
- <span data-ttu-id="fbe3f-109"> **टिप्पणियां** फ़ील्ड परियोजना प्रबंधक को स्थिति के बारे में विशिष्ट टिप्पणी दर्ज करने देता है।</span><span class="sxs-lookup"><span data-stu-id="fbe3f-109">The **Comments** field lets the project manager enter specific comments about the status.</span></span> 
- <span data-ttu-id="fbe3f-110"> **पर अपडेट की गई स्थिति** फ़ील्ड संपादन योग्य नहीं है।</span><span class="sxs-lookup"><span data-stu-id="fbe3f-110">The **Status updated on** field isn't editable.</span></span> <span data-ttu-id="fbe3f-111">इस क्षेत्र में मान एक टाइमस्टैम्प है, जो दर्शाता है कि स्थिति को अंतिम बार कब अपडेट किया गया था.</span><span class="sxs-lookup"><span data-stu-id="fbe3f-111">The value in this field is a timestamp that indicates when the status was last updated.</span></span>
- <span data-ttu-id="fbe3f-112"> **शेड्यूल प्रदर्शन** और **लागत प्रदर्शन** फ़ील्ड ट्रैकिंग ग्रिड से सेट किए गए हैं।</span><span class="sxs-lookup"><span data-stu-id="fbe3f-112">The **Schedule performance** and **Cost performance** fields are set from the tracking grid.</span></span> <span data-ttu-id="fbe3f-113">जब **प्रयास ट्रैकिंग** दृश्य में रूट नोड के लिए शेड्यूल और लागत विचलन सकारात्मक हैं, तो इन फ़ील्ड को  **Ahead**पर अपडेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="fbe3f-113">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, these fields are updated to **Ahead**.</span></span> <span data-ttu-id="fbe3f-114">जब रूट नोड के लिए शेड्यूल और लागत विचलन नकारात्मक होते हैं, तो इन फ़ील्ड को **पीछे** पर सेट किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="fbe3f-114">When the schedule and cost variance for the root node are negative, these fields are set to **Behind**.</span></span>
