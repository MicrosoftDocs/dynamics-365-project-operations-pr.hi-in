---
title: अनुमोदन के लिए डेवलपर नोट्स
description: यह विषय अनुमोदनों के साथ कार्य करने के बारे में अतिरिक्त डेवलपर जानकारी प्रदान करता है.
author: stsporen
ms.date: 11/09/2020
ms.topic: article
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: a89ea669a262c145b9f391fddc19e79a425fabb5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5996793"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="84f8e-103">अनुमोदन के लिए डेवलपर नोट्स</span><span class="sxs-lookup"><span data-stu-id="84f8e-103">Developer notes for Approvals</span></span>

<span data-ttu-id="84f8e-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="84f8e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="84f8e-105">Dynamics 365 Project Operations में सत्यापन तर्क शामिल है, जो अनुमोदन चरणों के दौरान सही रिकॉर्ड संक्रमण को सुनिश्चित करता है.</span><span class="sxs-lookup"><span data-stu-id="84f8e-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="84f8e-106">सही रिकॉर्ड संक्रमण निम्न सुनिश्चित करते हैं:</span><span class="sxs-lookup"><span data-stu-id="84f8e-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="84f8e-107">सभी सहायक पंक्तियाँ संबंधित तालिकाओं में बनाई गई हैं, जैसे जर्नल और वास्तविक.</span><span class="sxs-lookup"><span data-stu-id="84f8e-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="84f8e-108">आगे बढ़ने से पहले परियोजना में अनुमोदनकर्ता को एक **परियोजना अनुमोदनकर्ता** के रूप में चिह्नित किया गया है.</span><span class="sxs-lookup"><span data-stu-id="84f8e-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]