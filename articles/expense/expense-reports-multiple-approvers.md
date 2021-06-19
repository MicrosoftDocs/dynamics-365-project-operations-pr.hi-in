---
title: व्यय रिपोर्ट और कई अनुमोदनकर्ता
description: यह विषय उन व्यय रिपोर्ट के बारे में जानकारी देता है जिन्हें एक से अधिक लोगों की स्वीकृति की ज़रूरत होती है.
author: suvaidya
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 2502b2975ad3aebad720970e693ea68eac0a302c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6002058"
---
# <a name="expense-reports-and-multiple-approvers"></a><span data-ttu-id="a8b63-103">व्यय रिपोर्ट और कई अनुमोदनकर्ता</span><span class="sxs-lookup"><span data-stu-id="a8b63-103">Expense reports and multiple approvers</span></span>

<span data-ttu-id="a8b63-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="a8b63-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="a8b63-105">आपके संगठन की व्यय अनुमोदन नीतियों के आधार पर, एक से अधिक लोगों को सबमिट की गई व्यय रिपोर्ट को अनुमोदित करना पड़ सकता है.</span><span class="sxs-lookup"><span data-stu-id="a8b63-105">Depending on your organization's expense approval policies, more than one person might have to approve a submitted expense report.</span></span> <span data-ttu-id="a8b63-106">जब आप व्यय रिपोर्ट अनुमोदन के लिए कार्यप्रवाह प्रक्रिया सेट करते हैं तो आप कार्यप्रवाह के अवयव जोड़ सकते हैं, जिसमें एक या कई व्यय रिपोर्ट अनुमोदकों के लिए कार्य या चरण शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="a8b63-106">When you set up the workflow process for expense report approval, you can add workflow elements that include tasks or steps for one or more expense report approvers.</span></span> <span data-ttu-id="a8b63-107">उदाहरण के लिए, आपको ज़रूरत हो सकती है कि सभी व्यय रिपोर्ट को दो अलग-अलग लोग अनुमोदित करें, जैसे कि कर्मचारी प्रबंधक, जिसने रिपोर्ट सबमिट की है और लेखा देय समन्वयक.</span><span class="sxs-lookup"><span data-stu-id="a8b63-107">For example, you might require that all expense reports be approved by two separate people, the manager of the employee who submitted the report and the Accounts payable coordinator.</span></span>

<span data-ttu-id="a8b63-108">यदि आपको कई व्यय रिपोर्ट अनुमोदकों की ज़रूरत होती है, तो आप निम्नलिखित में से किसी भी तरीके से कार्यप्रवाह अवयवों को जोड़ सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="a8b63-108">If you decide to require multiple expense report approvers, you can add the workflow elements in any of the following ways:</span></span>

- <span data-ttu-id="a8b63-109">एक स्वीकृति अवयव जोड़ें जिसमें एक चरण हो.</span><span class="sxs-lookup"><span data-stu-id="a8b63-109">Add one approval element that has one step.</span></span> <span data-ttu-id="a8b63-110">उदाहरण के लिए, चरण के लिए यह ज़रूरी हो सकता है कि व्यय रिपोर्ट उपयोगकर्ता समूह को सौंपी जाए और उपयोगकर्ता समूह के 50 प्रतिशत सदस्य इसे स्वीकृत करें.</span><span class="sxs-lookup"><span data-stu-id="a8b63-110">For example, the step might require that an expense report be assigned to a user group, and that it be approved by 50 percent of the user group's members.</span></span>
- <span data-ttu-id="a8b63-111">एक स्वीकृति अवयव जोड़ें, जिसमें कई चरण हों.</span><span class="sxs-lookup"><span data-stu-id="a8b63-111">Add one approval element that has multiple steps.</span></span> <span data-ttu-id="a8b63-112">उदाहरण के लिए, स्वीकृति अवयव में निम्नांकित चरण हो सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="a8b63-112">For example, the approval element might have the following steps:</span></span>

    1. <span data-ttu-id="a8b63-113">व्यय रिपोर्ट सबमिट करने वाला कर्मचारी प्रबंधक इसे अनुमोदित करता है.</span><span class="sxs-lookup"><span data-stu-id="a8b63-113">The manager of the employee who submitted the expense report approves it.</span></span>
    2. <span data-ttu-id="a8b63-114">लेखा देय लिपिक प्राप्तियों और व्यय रिपोर्ट मदों की पुष्टि करता है.</span><span class="sxs-lookup"><span data-stu-id="a8b63-114">The Accounts payable clerk verifies the receipts and the expense report items.</span></span>
    3. <span data-ttu-id="a8b63-115">बजट मालिक व्यय रिपोर्ट को स्वीकृत करता है.</span><span class="sxs-lookup"><span data-stu-id="a8b63-115">The budget owner approves the expense report.</span></span>

- <span data-ttu-id="a8b63-116">कई स्वीकृत अवयव जोड़ें, जिनमें से प्रत्येक में एक चरण है.</span><span class="sxs-lookup"><span data-stu-id="a8b63-116">Add multiple approval elements, each of which has one step.</span></span> <span data-ttu-id="a8b63-117">उदाहरण के लिए, आप निम्नांकित चरणों में से प्रत्येक के लिए अलग स्वीकृति अवयव जोड़ सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="a8b63-117">For example, you might add a separate approval element for each of the following steps:</span></span>

    1. <span data-ttu-id="a8b63-118">कर्मचारी का प्रबंधक व्यय रिपोर्ट को स्वीकृत करता है.</span><span class="sxs-lookup"><span data-stu-id="a8b63-118">The employee's manager approves the expense report.</span></span>
    2. <span data-ttu-id="a8b63-119">बजट मालिक व्यय रिपोर्ट को स्वीकृत करता है.</span><span class="sxs-lookup"><span data-stu-id="a8b63-119">The budget owner approves the expense report.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]