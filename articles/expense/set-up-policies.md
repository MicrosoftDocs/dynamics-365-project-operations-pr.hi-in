---
title: व्यय नीतियों को परिभाषित करें
description: आप व्यय नीतियां निर्धारित कर सकते हैं जिनका आपके कर्मचारियों को व्यय रिपोर्ट दर्ज करने और यात्रा मांग-पत्र दर्ज करने और सबमिट करने के दौरान पालन करना चाहिए.
author: suvaidya
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: fa108db9aa0d2a22c35d2d046917ddae1f3842c1
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001878"
---
# <a name="define-expense-policies"></a><span data-ttu-id="179b4-103">व्यय नीतियों को परिभाषित करें</span><span class="sxs-lookup"><span data-stu-id="179b4-103">Define expense policies</span></span>

<span data-ttu-id="179b4-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="179b4-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="179b4-105">आप उन नीतियों को निर्धारित कर सकते हैं जिनका आपके कर्मचारियों को व्यय रिपोर्ट दर्ज करने और यात्रा मांग-पत्र को दर्ज करने और सबमिट करने के दौरान पालन करना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="179b4-105">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="179b4-106">व्यय नीतियों को लागू करके आप व्यय को प्रभावपूर्ण तरीके से प्रबंधित कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="179b4-106">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="179b4-107">उदाहरण के लिए, आप न्यूयॉर्क शहर में होटल के व्यय के लिए नीति निर्धारित कर सकते हैं, जिसमें बताया गया है कि प्रति रात का खर्च USD 250 से अधिक नहीं हो सकता है.</span><span class="sxs-lookup"><span data-stu-id="179b4-107">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="179b4-108">यदि कोई कर्मचारी व्यय रिपोर्ट या यात्रा ज़रूरत सबमिट करता है, जहां कमरे की दर इस राशि से अधिक है,</span><span class="sxs-lookup"><span data-stu-id="179b4-108">If a worker submits an expense report or travel requisition where the room rate exceeds this amount, the system will notify the</span></span>         
<span data-ttu-id="179b4-109">तो सिस्टम इसकी सूचना देगा कि कर्मचारी व्यय पॉलिसी द्वारा निर्धारित राशि से अधिक है.</span><span class="sxs-lookup"><span data-stu-id="179b4-109">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="179b4-110">आप उस संदेश को कॉन्फ़िगर कर सकते हैं जो कर्मचारी को तब प्राप्त होगा</span><span class="sxs-lookup"><span data-stu-id="179b4-110">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="179b4-111">जब आप नीति निर्धारित करते है.</span><span class="sxs-lookup"><span data-stu-id="179b4-111">define the policy.</span></span>      
        
<span data-ttu-id="179b4-112">आप तीन प्रकार की नीतियों को निर्धारित कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="179b4-112">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="179b4-113">**चेतावनी** कार्यकर्ता को व्यय रिपोर्ट या यात्रा अनुरोध प्रस्तुत करने की अनुमति देता है, लेकिन व्यय को सभी अनुमोदनकर्ताओं के लिए चिह्नित किया जाएगा और</span><span class="sxs-lookup"><span data-stu-id="179b4-113">**Warning**: Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>         
  <span data-ttu-id="179b4-114">लेकिन व्यय को सभी अनुमोदकों और बाद में रिपोर्टिंग के लिए.</span><span class="sxs-lookup"><span data-stu-id="179b4-114">for later reporting.</span></span>        

- <span data-ttu-id="179b4-115">**त्रुटि**: व्यय रिपोर्ट या यात्रा मांग-पत्र सबमिट करने से पहले कर्मचारी को नीति के अनुपालन के लिए व्यय को संशोधित करने की ज़रूरती होती है.</span><span class="sxs-lookup"><span data-stu-id="179b4-115">**Error**: Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>        
 
 - <span data-ttu-id="179b4-116">**तर्गसंगतता**: व्यय रिपोर्ट या यात्रा मांग-पत्र सबमिट करने से पहले कर्मचारी या प्रबंधक को पॉलिसी राशि से अधिक होने की तर्गसंगतता दर्ज करने की ज़रूरत होती है.</span><span class="sxs-lookup"><span data-stu-id="179b4-116">**Justification**: Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="179b4-117">नीति युक्तियाँ</span><span class="sxs-lookup"><span data-stu-id="179b4-117">Policy tips</span></span>
<span data-ttu-id="179b4-118">यहां कुछ सुझाव दिए गए हैं जो व्यय प्रबंधन के लिए नई नीतियां बनाते समय आपकी मदद कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="179b4-118">Here are a few suggestions that can assist you when creating new policies for expense management:</span></span> 

- <span data-ttu-id="179b4-119">नीतियां प्रभावी होती हैं, जिसका मतलब है कि पॉलिसी तब प्रभावी नहीं होगी जब यह उस तिथि के बाद बनाई गई हो, जब व्यय हुआ था.</span><span class="sxs-lookup"><span data-stu-id="179b4-119">Policies are date effective which means a policy won't take effect if it's created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="179b4-120">उदाहरण के लिए, आप $50 के अधिकतम भोजन व्यय को लागू करने के लिए आज नई नीति बनाते हैं.</span><span class="sxs-lookup"><span data-stu-id="179b4-120">For example, you create a new policy today to enforce a maximum meal expense of $50.</span></span> <span data-ttu-id="179b4-121">कल के रूप में दर्ज किए गए किसी भी मौजूदा व्यय की इस नीति के सापेक्ष जाँच नहीं की जाएगी.</span><span class="sxs-lookup"><span data-stu-id="179b4-121">Any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
- <span data-ttu-id="179b4-122">व्यय श्रेणी के लिए नीति बनाते समय जिसे मदवार किया जा सकता है, व्यय लाइन प्रकार के लिए शर्त जोड़ने पर विचार करें.</span><span class="sxs-lookup"><span data-stu-id="179b4-122">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="179b4-123">कुछ नीतियां, जैसे कि रसीद की आवश्यकता, मदवार पंक्तियों के लिए मायने नहीं रखती है.</span><span class="sxs-lookup"><span data-stu-id="179b4-123">Some policies, such as requiring a receipt, may not make sense for itemized lines.</span></span> <span data-ttu-id="179b4-124">इस स्थिति में, नीति केवल हेडर लाइन या गैर-मदवार लाइन पर लागू होती है.</span><span class="sxs-lookup"><span data-stu-id="179b4-124">In this situation, the policy only is applied to the header line or a non-itemized line.</span></span> 
- <span data-ttu-id="179b4-125">डिफ़ॉल्ट रूप से स्रोत निकाय के सापेक्ष व्यय प्रबंधन नीतियों का मूल्यांकन किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="179b4-125">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="179b4-126">इंटरकंपनी परिदृश्यों के लिए, आप इसके बजाय गंतव्य निकाय (उधार निकाय) के सापेक्ष मूल्यांकन की जाने वाली नीति निर्धारित कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="179b4-126">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="179b4-127">गंतव्य निकाय के विरूध्द नीतियों को चलाने के लिए, **फीचर प्रबंधन** कार्यक्षेत्र में **कानूनी निकाय सुविधा उधार लेने की तुलना में खर्च नीति का मूल्यांकन करें** फ़ीचर को चालू करें.</span><span class="sxs-lookup"><span data-stu-id="179b4-127">To run the policies against the destination entity, turn on the **Evaluate Expense policy against borrowing legal entity** feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="179b4-128">नीतियों का मूल्यांकन कब करें</span><span class="sxs-lookup"><span data-stu-id="179b4-128">When to evaluate policies</span></span>

<span data-ttu-id="179b4-129">व्यय प्रबंधन मापदंडों में जब कोई लाइन सहेजी जाती है या व्यय रिपोर्ट सबमिट की जाती है, तो आप व्यय प्रबंधन नीतियों का मूल्यांकन कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="179b4-129">In expense management parameters, you can select to evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="179b4-130">यदि आप किसी पंक्ति को सहेजने पर मूल्यांकन करना चुनते हैं तो उपयोगकर्ताओं को पहले दृश्यता होगी कि उन्हें उनकी व्यय रिपोर्ट को एक बार में पूरा करने के लिए क्या करना होगा.</span><span class="sxs-lookup"><span data-stu-id="179b4-130">If you choose to evaluate when a line is saved, users will have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="179b4-131">नहीं तो, आप कार्यप्रवाह को सबमिट करने के दौरान नीति मूल्यांकन में देरी कर सकते हैं और अंत में सत्यापन करके समय बचा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="179b4-131">Otherwise, you can delay policy evaluation and save time by validating at the end, during the submission to workflow.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]