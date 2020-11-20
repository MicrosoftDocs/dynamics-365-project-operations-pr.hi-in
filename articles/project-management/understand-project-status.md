---
title: परियोजना की स्थिति को समझें
description: यह विषय Dynamics 365 परियोजना संचालन में परियोजनाओं को सौंपी गई स्थिति के बारे में जानकारी प्रदान करता है।
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: bc5bc174518e46b32cf88ea7231bb2df10fde292
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127295"
---
# <a name="understand-project-status"></a><span data-ttu-id="b07bc-103">परियोजना की स्थिति को समझें</span><span class="sxs-lookup"><span data-stu-id="b07bc-103">Understand project status</span></span>

<span data-ttu-id="b07bc-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="b07bc-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>


<span data-ttu-id="b07bc-105">**परियोजना निकाय** पृष्ठ पर **स्थिति** अनुभाग, लागत और प्रयास के आधार पर परियोजना के स्वास्थ्य का सारांश प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="b07bc-105">The **Status** section on the **Project Entity** page provides a summary of a project's health based upon cost and effort.</span></span>


## <a name="status-summary-fields"></a><span data-ttu-id="b07bc-106">स्थिति सारांश फ़ील्ड</span><span class="sxs-lookup"><span data-stu-id="b07bc-106">Status summary fields</span></span>

- <span data-ttu-id="b07bc-107">**संपूर्ण परियोजना स्थिति** फील्ड एक एडिट करने योग्य फील्ड होता है जो प्रोजेक्ट का संपूर्ण स्टेटस दिखाता है।</span><span class="sxs-lookup"><span data-stu-id="b07bc-107">The **Overall project status** field is an editable field that shows the overall status of the project.</span></span> <span data-ttu-id="b07bc-108">यह फ़ील्ड बढ़ते जोखिम को दर्शाने के लिए हरे, पीले और लाल जैसी रंग-कोडिंग का उपयोग करता.</span><span class="sxs-lookup"><span data-stu-id="b07bc-108">This field uses color-coding, such as green, yellow, and red, to indicate increasing risk.</span></span> 
- <span data-ttu-id="b07bc-109">**टिप्पणियां** फ़ील्ड परियोजना प्रबंधक को स्थिति के बारे में विशिष्ट टिप्पणी दर्ज करने देता है.</span><span class="sxs-lookup"><span data-stu-id="b07bc-109">The **Comments** field lets the project manager enter specific comments about the status.</span></span> 
- <span data-ttu-id="b07bc-110">**स्थिति इस समय अपडोट की गई** फ़ील्ड संपादन योग्य नहीं है.</span><span class="sxs-lookup"><span data-stu-id="b07bc-110">The **Status updated on** field isn't editable.</span></span> <span data-ttu-id="b07bc-111">इस क्षेत्र में मान एक टाइमस्टैम्प है, जो दर्शाता है कि स्थिति को अंतिम बार कब अपडेट किया गया था.</span><span class="sxs-lookup"><span data-stu-id="b07bc-111">The value in this field is a timestamp that indicates when the status was last updated.</span></span>
- <span data-ttu-id="b07bc-112">**शेड्यूल प्रदर्शन** और **लागत प्रदर्शन** फ़ील्ड ट्रैकिंग ग्रिड से सेट किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="b07bc-112">The **Schedule performance** and **Cost performance** fields are set from the tracking grid.</span></span> <span data-ttu-id="b07bc-113">जब **प्रयास ट्रैकिंग** दृश्य में रूट नोड के लिए शेड्यूल और लागत भिन्नता सकारात्मक होते हैं, तो इन फ़ील्ड को **आगे** पर अपडेट कर दिया जाता है.</span><span class="sxs-lookup"><span data-stu-id="b07bc-113">When the schedule and cost variance for the root node in the **Effort tracking** view are positive, these fields are updated to **Ahead**.</span></span> <span data-ttu-id="b07bc-114">जब रूट नोड के लिए शेड्यूल और लागत भिन्नता नकारात्मक होते हैं, तो इन फ़ील्ड को **पीछे** पर सेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="b07bc-114">When the schedule and cost variance for the root node are negative, these fields are set to **Behind**.</span></span>
