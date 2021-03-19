---
title: व्यय अनुमान
description: यह विषय परियोजना-आधारित व्यय को स्पष्ट करने या उनका आकलन करने के बारे में जानकारी देता है.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 3f0429366c69346113003355679c055cd2c74ca3
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5287060"
---
# <a name="expense-estimates"></a><span data-ttu-id="e8d6e-103">व्यय अनुमान</span><span class="sxs-lookup"><span data-stu-id="e8d6e-103">Expense estimates</span></span>
<span data-ttu-id="e8d6e-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="e8d6e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e8d6e-105">संसाधन-आधारित अनुमानों को परिभाषित करने के साथ-साथ, Dynamics 365 Project Operations की मदद से परियोजना प्रबंधक प्रत्येक परियोजना के लिए परियोजना-आधारित खर्चों को परिभाषित कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="e8d6e-105">Along with defining resource-based estimates, Dynamics 365 Project Operations allows Project managers to define project-based expenses for each project.</span></span> <span data-ttu-id="e8d6e-106">प्रत्येक व्यय वस्तु विशिष्ट परियोजना कार्य या व्यय श्रेणी से जुड़ी हो सकती है.</span><span class="sxs-lookup"><span data-stu-id="e8d6e-106">Each expense item can be associated with a specific project task or expense category.</span></span> <span data-ttu-id="e8d6e-107">व्यय श्रेणियों को आमतौर पर संगठनात्मक स्तर पर स्पष्ट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="e8d6e-107">Expense categories are typically defined at the organizational level.</span></span> <span data-ttu-id="e8d6e-108">प्रत्येक व्यय श्रेणी के लिए मूल्य निर्धारण आमतौर पर निम्नंकित पदानुक्रम में स्पष्ट किया गया है:</span><span class="sxs-lookup"><span data-stu-id="e8d6e-108">Pricing for each expense category is typically defined in the following hierarchy:</span></span>

- <span data-ttu-id="e8d6e-109">संगठन</span><span class="sxs-lookup"><span data-stu-id="e8d6e-109">Organization</span></span>
- <span data-ttu-id="e8d6e-110">ग्राहक</span><span class="sxs-lookup"><span data-stu-id="e8d6e-110">Customer</span></span>
- <span data-ttu-id="e8d6e-111">कोट/अनुबंध</span><span class="sxs-lookup"><span data-stu-id="e8d6e-111">Quote/contract</span></span>

<span data-ttu-id="e8d6e-112">परियोजना व्यय देखने, जोड़ने या हटाने के लिए निम्नांकित चरण पूरे करें.</span><span class="sxs-lookup"><span data-stu-id="e8d6e-112">Complete the following steps to view, add, or delete a project expense.</span></span>

1. <span data-ttu-id="e8d6e-113">**परियोजना** पर जाएं, और वह परियोजना चुनें जिस पर आप काम करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="e8d6e-113">Go to **Projects**, and select the project you want to work on.</span></span>
2. <span data-ttu-id="e8d6e-114">**परियोजना अनुमान** टैब चुनें और परियोजना व्यय की सूची देखें.</span><span class="sxs-lookup"><span data-stu-id="e8d6e-114">Select the **Project Estimates** tab and view the list of project expenses.</span></span>
3. <span data-ttu-id="e8d6e-115">व्यय जोड़ने के लिए **नया व्यय** चुनें.</span><span class="sxs-lookup"><span data-stu-id="e8d6e-115">Select **New Expense** to add an expense.</span></span> <span data-ttu-id="e8d6e-116">या हटाने के लिए व्यय चुनें और फिर **व्यय हटाएं** चुनें.</span><span class="sxs-lookup"><span data-stu-id="e8d6e-116">Or, select an expense to delete, and then select **Delete Expense**.</span></span>

<span data-ttu-id="e8d6e-117">निम्नांकित एट्रिब्यूट्स प्रत्येक व्यय पंक्ति वस्तु के लिए स्पष्ट किए गए हैं:</span><span class="sxs-lookup"><span data-stu-id="e8d6e-117">The following attributes are defined for each expense line item:</span></span>

- <span data-ttu-id="e8d6e-118">**श्रेणी**: आम समूहकरण परियोजना पर किए गए सभी व्यय का वर्णन करने में इस्तेमाल किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="e8d6e-118">**Category**: The common groupings used to describe all expenses incurred on a project.</span></span>
- <span data-ttu-id="e8d6e-119">**प्रारंभ तिथि**: वह तिथि जब व्यय का अनुमान लगाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="e8d6e-119">**Start Date**: The date when the expense is forecasted to be incurred.</span></span>
- <span data-ttu-id="e8d6e-120">**मात्रा**: किसी विशेष श्रेणी के लिए व्यय वस्तुओं की अनुमानित संख्या.</span><span class="sxs-lookup"><span data-stu-id="e8d6e-120">**Quantity**: The estimated number of expense items for a specific category.</span></span>
- <span data-ttu-id="e8d6e-121">**इकाई लागत मूल्य**: व्यय की लागत की गणना करने के लिए इस्तेमाल किया जाने वाला इकाई मूल्य.</span><span class="sxs-lookup"><span data-stu-id="e8d6e-121">**Unit Cost Price**: The unit price used to calculate to cost of the expense.</span></span>
- <span data-ttu-id="e8d6e-122">**इकाई बिक्री मूल्य**: व्यय की बिक्री कीमतों की गणना करने के लिए इस्तेमाल किया जाने वाला इकाई मूल्य.</span><span class="sxs-lookup"><span data-stu-id="e8d6e-122">**Unit Sales Price**: The unit price used to calculate the sale prices of the expense.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]