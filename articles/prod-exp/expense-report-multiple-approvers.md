---
title: एक ख़र्च रिपोर्ट पर कई अनुमोदक
description: यह विषय उन ख़र्च रिपोर्ट के बारे में जानकारी देता है जिन्हें एक से अधिक लोगों की स्वीकृति की ज़रूरत होती है.
author: saraschi2
manager: AnnBe
ms.date: 02/23/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvExpensesReportList
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 9b6d07f00fd6c1ba2d860787665d95f95f7b1a89
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960609"
---
# <a name="multiple-approvers-on-an-expense-report"></a><span data-ttu-id="69a2b-103">एक ख़र्च रिपोर्ट पर कई अनुमोदक</span><span class="sxs-lookup"><span data-stu-id="69a2b-103">Multiple approvers on an expense report</span></span>

<span data-ttu-id="69a2b-104">आपके संगठन की ख़र्च अनुमोदन नीतियों के आधार पर, एक से अधिक व्यक्ति को एक कर्मचारी द्वारा प्रस्तुत ख़र्च रिपोर्ट को मंजूरी देनी पड़ सकती है.</span><span class="sxs-lookup"><span data-stu-id="69a2b-104">Depending on your organization's expense approval policies, more than one person might have to approve an expense report that is submitted by an employee.</span></span> <span data-ttu-id="69a2b-105">जब आप व्यय रिपोर्ट अनुमोदन के लिए कार्यप्रवाह प्रक्रिया सेट करते हैं तो आप कार्यप्रवाह के अवयव जोड़ सकते हैं, जिसमें एक या कई व्यय रिपोर्ट अनुमोदकों के लिए कार्य या चरण शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="69a2b-105">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="69a2b-106">उदाहरण के लिए, आपको यह आवश्यक हो सकता है कि सभी ख़र्च रिपोर्टों को पहले उस कर्मचारी के प्रबंधक द्वारा अनुमोदित किया जाए जिसने रिपोर्ट प्रस्तुत की है और फिर लेखा देय समन्वयक द्वारा.</span><span class="sxs-lookup"><span data-stu-id="69a2b-106">For example, you might require that all expense reports be approved first by the manager of the employee who submitted the report and then by the Accounts payable coordinator.</span></span>

<span data-ttu-id="69a2b-107">यदि आपको कई व्यय रिपोर्ट अनुमोदकों की ज़रूरत होती है, तो आप निम्नलिखित में से किसी भी तरीके से कार्यप्रवाह अवयवों को जोड़ सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="69a2b-107">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="69a2b-108">एक स्वीकृति अवयव जोड़ें जिसमें एक चरण हो.</span><span class="sxs-lookup"><span data-stu-id="69a2b-108">Add one approval element that has one step.</span></span> <span data-ttu-id="69a2b-109">उदाहरण के लिए, चरण के लिए यह ज़रूरी हो सकता है कि व्यय रिपोर्ट उपयोगकर्ता समूह को सौंपी जाए और उपयोगकर्ता समूह के 50 प्रतिशत सदस्य इसे स्वीकृत करें.</span><span class="sxs-lookup"><span data-stu-id="69a2b-109">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="69a2b-110">एक स्वीकृति अवयव जोड़ें, जिसमें कई चरण हों.</span><span class="sxs-lookup"><span data-stu-id="69a2b-110">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="69a2b-111">उदाहरण के लिए, स्वीकृति अवयव में निम्नांकित चरण हो सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="69a2b-111">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="69a2b-112">व्यय रिपोर्ट सबमिट करने वाला कर्मचारी प्रबंधक इसे अनुमोदित करता है.</span><span class="sxs-lookup"><span data-stu-id="69a2b-112">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="69a2b-113">लेखा देय लिपिक प्राप्तियों और व्यय रिपोर्ट मदों की पुष्टि करता है.</span><span class="sxs-lookup"><span data-stu-id="69a2b-113">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="69a2b-114">बजट मालिक व्यय रिपोर्ट को स्वीकृत करता है.</span><span class="sxs-lookup"><span data-stu-id="69a2b-114">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="69a2b-115">कई स्वीकृत अवयव जोड़ें, जिनमें से प्रत्येक में एक चरण है.</span><span class="sxs-lookup"><span data-stu-id="69a2b-115">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="69a2b-116">उदाहरण के लिए, आप निम्नांकित चरणों में से प्रत्येक के लिए अलग स्वीकृति अवयव जोड़ सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="69a2b-116">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="69a2b-117">कर्मचारी का प्रबंधक व्यय रिपोर्ट को स्वीकृत करता है.</span><span class="sxs-lookup"><span data-stu-id="69a2b-117">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="69a2b-118">बजट मालिक व्यय रिपोर्ट को स्वीकृत करता है.</span><span class="sxs-lookup"><span data-stu-id="69a2b-118">The budget owner approves the expense report.</span></span>
