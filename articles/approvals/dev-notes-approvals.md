---
title: अनुमोदन के लिए डेवलपर नोट्स
description: यह विषय अनुमोदनों के साथ कार्य करने के बारे में अतिरिक्त डेवलपर जानकारी प्रदान करता है.
author: stsporen
manager: Annbe
ms.date: 11/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 9e4e910d0ff0a5f2603148fcc5daa0d423a4d174
ms.sourcegitcommit: a9dbcd3aff4c6ae495412e4980e105ae160fd1ec
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/10/2020
ms.locfileid: "4483950"
---
# <a name="developer-notes-for-approvals"></a><span data-ttu-id="a5ec4-103">अनुमोदन के लिए डेवलपर नोट्स</span><span class="sxs-lookup"><span data-stu-id="a5ec4-103">Developer notes for Approvals</span></span>

<span data-ttu-id="a5ec4-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="a5ec4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a5ec4-105">Dynamics 365 Project Operations में सत्यापन तर्क शामिल है, जो अनुमोदन चरणों के दौरान सही रिकॉर्ड संक्रमण को सुनिश्चित करता है.</span><span class="sxs-lookup"><span data-stu-id="a5ec4-105">Dynamics 365 Project Operations includes validation logic that ensures correct record transition through the approval stages.</span></span> <span data-ttu-id="a5ec4-106">सही रिकॉर्ड संक्रमण निम्न सुनिश्चित करते हैं:</span><span class="sxs-lookup"><span data-stu-id="a5ec4-106">Correct record transitions ensure:</span></span> 

  - <span data-ttu-id="a5ec4-107">सभी सहायक पंक्तियाँ संबंधित तालिकाओं में बनाई गई हैं, जैसे जर्नल और वास्तविक.</span><span class="sxs-lookup"><span data-stu-id="a5ec4-107">All supporting rows are created in related tables, such as journals and actuals.</span></span>
  - <span data-ttu-id="a5ec4-108">आगे बढ़ने से पहले परियोजना में अनुमोदनकर्ता को एक **परियोजना अनुमोदनकर्ता** के रूप में चिह्नित किया गया है.</span><span class="sxs-lookup"><span data-stu-id="a5ec4-108">The approver is marked as a **Project Approver** in the project before proceeding.</span></span>
