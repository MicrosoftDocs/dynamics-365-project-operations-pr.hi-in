---
title: व्यय नीतियों सेट अप करें
description: आप व्यय नीतियां निर्धारित कर सकते हैं जिनका आपके कर्मचारियों को व्यय रिपोर्ट दर्ज करने और Microsoft Dynamics 365 Finance में यात्रा आवश्यकताएं दर्ज करने और सबमिट करने के दौरान पालन करना चाहिए.
author: suvaidya
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysPolicyListPage, TrvPolicyRule
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: suvaidya
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: ab99c0ec769eb2e0914fc7d993f83d20e2c327f6
ms.sourcegitcommit: 9f31b33ed6e7f1b49200a407913201a1337f3401
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 01/14/2021
ms.locfileid: "4960699"
---
# <a name="set-up-expense-policies"></a><span data-ttu-id="39ac5-103">व्यय नीतियों सेट अप करें</span><span class="sxs-lookup"><span data-stu-id="39ac5-103">Set up expense policies</span></span>

<span data-ttu-id="39ac5-104">आप उन नीतियों को निर्धारित कर सकते हैं जिनका आपके कर्मचारियों को व्यय रिपोर्ट दर्ज करने और यात्रा मांग-पत्र को दर्ज करने और सबमिट करने के दौरान पालन करना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="39ac5-104">You can define policies that your workers must follow when entering and submitting expense reports and travel requisitions.</span></span>         
<span data-ttu-id="39ac5-105">व्यय नीतियों को लागू करके आप व्यय को प्रभावपूर्ण तरीके से प्रबंधित कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="39ac5-105">Implementing expense policies can help you manage expenses effectively.</span></span>         

<span data-ttu-id="39ac5-106">उदाहरण के लिए, आप न्यूयॉर्क शहर में होटल के व्यय के लिए नीति निर्धारित कर सकते हैं, जिसमें बताया गया है कि प्रति रात का खर्च USD 250 से अधिक नहीं हो सकता है.</span><span class="sxs-lookup"><span data-stu-id="39ac5-106">For example, you can set a policy for hotel expenses in New York City, which states that the per night expense cannot exceed USD 250.</span></span>       
<span data-ttu-id="39ac5-107">यदि कोई कार्यकर्ता व्यय रिपोर्ट या यात्रा मांग प्रस्तुत करता है, जिसमें कमरे की दर इस राशि से अधिक हो, तो सिस्टम निम्न जानकारी से सूचित करेगा</span><span class="sxs-lookup"><span data-stu-id="39ac5-107">If a worker submits an expense report or a travel requisition in which the room rate exceeds this amount, the system will notify the</span></span>        
<span data-ttu-id="39ac5-108">तो सिस्टम इसकी सूचना देगा कि कर्मचारी व्यय पॉलिसी द्वारा निर्धारित राशि से अधिक है.</span><span class="sxs-lookup"><span data-stu-id="39ac5-108">worker that the policy amount for the expense has been exceeded.</span></span> <span data-ttu-id="39ac5-109">आप उस संदेश को कॉन्फ़िगर कर सकते हैं जो कर्मचारी को तब प्राप्त होगा</span><span class="sxs-lookup"><span data-stu-id="39ac5-109">You can configure the message that the worker will receive when you</span></span>        
<span data-ttu-id="39ac5-110">जब आप नीति निर्धारित करते है.</span><span class="sxs-lookup"><span data-stu-id="39ac5-110">define the policy.</span></span>      
        
<span data-ttu-id="39ac5-111">आप तीन प्रकार की नीतियों को निर्धारित कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="39ac5-111">You can define three types of policies:</span></span>         
        
- <span data-ttu-id="39ac5-112">चेतावनी - कार्यकर्ता को व्यय रिपोर्ट या यात्रा अनुरोध प्रस्तुत करने की अनुमति देता है, लेकिन व्यय को सभी अनुमोदनकर्ताओं के लिए चिह्नित किया जाएगा और</span><span class="sxs-lookup"><span data-stu-id="39ac5-112">Warning – Allows the worker to submit an expense report or travel requisition but the expense will be marked for all approvers and</span></span>        
  <span data-ttu-id="39ac5-113">लेकिन व्यय को सभी अनुमोदकों और बाद में रिपोर्टिंग के लिए.</span><span class="sxs-lookup"><span data-stu-id="39ac5-113">for later reporting.</span></span>        

- <span data-ttu-id="39ac5-114">त्रुटि – व्यय रिपोर्ट या यात्रा मांग-पत्र सबमिट करने से पहले कर्मचारी को नीति के अनुपालन के लिए व्यय को संशोधित करने की ज़रूरती होती है.</span><span class="sxs-lookup"><span data-stu-id="39ac5-114">Error – Requires the worker to revise the expense to comply with the policy before submitting the expense report or travel requisition.</span></span>       
 
 - <span data-ttu-id="39ac5-115">तर्गसंगतता – व्यय रिपोर्ट या यात्रा मांग-पत्र सबमिट करने से पहले कर्मचारी या प्रबंधक को पॉलिसी राशि से अधिक होने की तर्गसंगतता दर्ज करने की ज़रूरत होती है.</span><span class="sxs-lookup"><span data-stu-id="39ac5-115">Justification – Requires the worker or a manager to enter a justification for exceeding the policy amount before submitting the expense report or travel requisition.</span></span>        

## <a name="policy-tips"></a><span data-ttu-id="39ac5-116">नीति युक्तियाँ</span><span class="sxs-lookup"><span data-stu-id="39ac5-116">Policy tips</span></span>
<span data-ttu-id="39ac5-117">यहां कुछ सुझाव दिए गए हैं जो व्यय प्रबंधन के लिए नई नीतियां बनाते समय आपकी मदद कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="39ac5-117">Here are a few suggestions that can assist you when creating new policies for expense management.</span></span> 
* <span data-ttu-id="39ac5-118">नीतियां तिथि प्रभावी हैं और यह तब प्रभावी नहीं होगा जब पॉलिसी व्यय होने की तिथि के बाद बनाई गई हो.</span><span class="sxs-lookup"><span data-stu-id="39ac5-118">Policies are date effective and won't take effect if the policy is created with a date after the date that the expense occurred.</span></span> <span data-ttu-id="39ac5-119">उदाहरण के लिए, यदि आप भोजन मद के अधिकतम व्यय $50 लागू करने के लिए आज एक नई नीति बना रहे हैं, तो बीते हुए कल की तारीख को दर्ज किया गया कोई मौजूदा खर्च की जांच इस नीति के बरक्स नहीं होगी.</span><span class="sxs-lookup"><span data-stu-id="39ac5-119">For example, if you are creating a new policy today to enforce a maximum meal expense of $50, then any existing expenses entered as of yesterday won't be checked against this policy.</span></span>
* <span data-ttu-id="39ac5-120">व्यय श्रेणी के लिए नीति बनाते समय जिसे मदवार किया जा सकता है, व्यय लाइन प्रकार के लिए शर्त जोड़ने पर विचार करें.</span><span class="sxs-lookup"><span data-stu-id="39ac5-120">When creating a policy for an expense category that can be itemized, consider adding a condition for expense line type.</span></span> <span data-ttu-id="39ac5-121">कुछ नीतियों में रसीद आदि की आवश्यकता होती है ऐसी नीति मदवार लाइन के लिए कोई अर्थ नहीं बनाती है और इसे केवल हेडर लाइन अथवा गैर-मदवार लाइन के लिए लागू किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="39ac5-121">Some policies such as requiring a receipt may not make sense for itemized lines and should only be applied to the header line or a non-itemized line.</span></span> 
* <span data-ttu-id="39ac5-122">डिफ़ॉल्ट रूप से स्रोत निकाय के सापेक्ष व्यय प्रबंधन नीतियों का मूल्यांकन किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="39ac5-122">Expense management policies are evaluated against the source entity by default.</span></span> <span data-ttu-id="39ac5-123">इंटरकंपनी परिदृश्यों के लिए, आप इसके बजाय गंतव्य निकाय (उधार निकाय) के सापेक्ष मूल्यांकन की जाने वाली नीति निर्धारित कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="39ac5-123">For intercompany scenarios, you can set the policy to be evaluated against the destination entity (borrowing entity) instead.</span></span> <span data-ttu-id="39ac5-124">गंतव्य निकाय के विरूध्द नीतियों को चलाने के लिए, **फीचर प्रबंधन** कार्यक्षेत्र में "कानूनी निकाय सुविधा उधार लेने की तुलना में खर्च नीति का मूल्यांकन करें" फ़ीचर को चालू करें.</span><span class="sxs-lookup"><span data-stu-id="39ac5-124">To run the policies against the destination entity, turn on the "Evaluate Expense policy against borrowing legal entity" feature in the **Feature Management** workspace.</span></span>

## <a name="when-to-evaluate-policies"></a><span data-ttu-id="39ac5-125">नीतियों का मूल्यांकन कब करें</span><span class="sxs-lookup"><span data-stu-id="39ac5-125">When to evaluate policies</span></span>

<span data-ttu-id="39ac5-126">व्यय प्रबंधन मापदंडों में, व्यय प्रबंधन नीतियों का मूल्यांकन करने का एक विकल्प होता है जो किसी लाइन के सेव होने पर या किसी व्यय रिपोर्ट के जमा होने पर व्यय प्रबंधन का मूल्यांकन करता है.</span><span class="sxs-lookup"><span data-stu-id="39ac5-126">In expense management parameters, there is an option to either evaluate expense management policies when a line is saved or when an expense report is submitted.</span></span> <span data-ttu-id="39ac5-127">यदि आप किसी लाइन के सेव रहने पर मूल्यांकन किए जाने की प्रक्रिया का चयन करते/करती हैं तो यह सुनिश्चित करता है कि उपयोकर्ता को इस बात की पहले से जानकारी है कि उन्हें अपनी व्यय रिपोर्ट एक ही बार में पूरा करने के लिए क्या करने की आवश्यकता है.</span><span class="sxs-lookup"><span data-stu-id="39ac5-127">If you choose to evaluate when a line is saved this ensures that users have earlier visibility into what they need to do to complete their expense report all at once.</span></span> <span data-ttu-id="39ac5-128">अन्यथा, आप नीति मूल्यांकन में देरी कर सकते/सकती हैं और समय बचा सकते/सकती हैं यदि आपके पास वर्कफ़्लो प्रस्तुत करने के दौरान, अंत में सत्यापन का कार्य करने का विकल्प है.</span><span class="sxs-lookup"><span data-stu-id="39ac5-128">Otherwise, you can delay policy evaluation and save time if you have validation occur at the end, during submission to workflow.</span></span>
