---
title: परियोजना अनुबंध प्रबंधित करें
description: यह विषय परियोजना-आधारित अनुबंध देखने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5a4357d5cf184a3c6ada3ae33631694c31bb5b00
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5273201"
---
# <a name="manage-project-contracts"></a><span data-ttu-id="fb326-103">परियोजना अनुबंध प्रबंधित करें</span><span class="sxs-lookup"><span data-stu-id="fb326-103">Manage project contracts</span></span>

<span data-ttu-id="fb326-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="fb326-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="fb326-105">Dynamics 365 Project Operations में परियोजना अनुबंध, परियोजना की अनुबंधित सहमति वाली प्रतिबद्धताओं और बिलिंग विवरणों को कैप्चर और प्रबंधित करता है.</span><span class="sxs-lookup"><span data-stu-id="fb326-105">Project contracts in Dynamics 365 Project Operations capture and manage the contractually agreed on commitments and billing details of a project.</span></span> <span data-ttu-id="fb326-106">Project Operations में परियोजना अनुबंध की संरचना निम्न घटकों के साथ परियोजना-आधारित कार्य के अनुरूप है:</span><span class="sxs-lookup"><span data-stu-id="fb326-106">The structure of a project contract in Project Operations is tailored to project-based work with the following components:</span></span>

- <span data-ttu-id="fb326-107">वे अनुबंध पंक्तियाँ, जो कार्य के उन असतत घटकों की पहचान करती हैं, जिन्हें परियोजना इनवॉइस पर उच्च-स्तरीय घटकों के रूप में प्रस्तुत किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="fb326-107">Contract lines that identify the discrete components of work that will be presented as high-level components on a project invoice.</span></span>
- <span data-ttu-id="fb326-108">वे अनुबंध पंक्ति विवरण, जो प्रत्येक उच्च-स्तरीय घटक या अनुबंध पंक्ति के लिए कार्य की पहचान और अनुमान लगाते हैं.</span><span class="sxs-lookup"><span data-stu-id="fb326-108">Contract line details that identify and estimate the work for each high-level component or contract line.</span></span> <span data-ttu-id="fb326-109">अनुमान में अनुबंध पंक्ति से जुड़े कार्य के लिए शेड्यूल और वित्तीय पहलू शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="fb326-109">The estimate includes the schedule and the financial aspects for the work tied to the contract line.</span></span>
- <span data-ttu-id="fb326-110">प्रत्येक अनुबंध पंक्ति के लिए अनुबंध मॉडल और प्रभार्य घटक सेट अप किए जाते हैं, जो प्रत्येक अनुबंध पंक्ति और समग्र अनुबंध के लिए बिलिंग व्यवस्था कायम रखते हैं.</span><span class="sxs-lookup"><span data-stu-id="fb326-110">Contracting models and chargeable components are set up for each contract line that holds the billing arrangement for each contract line and the overall contract.</span></span>

## <a name="view-all-project-based-contracts"></a><span data-ttu-id="fb326-111">सभी परियोजना-आधारित अनुबंधों को देखें</span><span class="sxs-lookup"><span data-stu-id="fb326-111">View all project-based contracts</span></span>

<span data-ttu-id="fb326-112">**अनुबंध** सूची पृष्ठ पर सभी परियोजना अनुबंधों की एक सूची देखी जा सकती है.</span><span class="sxs-lookup"><span data-stu-id="fb326-112">A list of all project contracts can be seen on the **Contracts** list page.</span></span> 

1. <span data-ttu-id="fb326-113">**विक्रय** > **अनुबंध** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="fb326-113">Go to **Sales** > **Contracts**.</span></span> <span data-ttu-id="fb326-114">सिस्टम में आपके सभी परियोजना अनुबंधों की एक सूची दिखाई गई है.</span><span class="sxs-lookup"><span data-stu-id="fb326-114">A list of all your project Contracts in the system are shown.</span></span> 
2. <span data-ttu-id="fb326-115">फ़िल्टर किए गए दृश्य चुनने के लिए, **दृश्य स्विचर** (दृश्य के नाम के आगे ड्रॉप-डाउन तीर) चुनें.</span><span class="sxs-lookup"><span data-stu-id="fb326-115">Select the **View switcher** (the drop-down arrow next to the name of the view) to select other filtered views.</span></span> <span data-ttu-id="fb326-116">आप कस्टम फ़िल्टर मापदंड के साथ अपने दृश्य बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="fb326-116">You can create your own views with custom filter criteria.</span></span>

<span data-ttu-id="fb326-117">अनुबंधों को इस सूची पृष्ठ या विवरण पृष्ठों पर बनाया या हटाया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="fb326-117">Contracts can be created or deleted from this list page or detail pages.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]