---
title: व्यय प्रबंधन के लिए कार्यप्रवाह सेट करना
description: आप कार्यप्रवाह प्रक्रिया सेट कर सकते हैं जिसका इस्तेमाल यात्रा और व्यय दस्तावेजों की समीक्षा और स्वीकृत करने के लिए किया जाता है.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: af6463b07e282ae1ff6aa7dc1a540ff7c8cc318a
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127700"
---
# <a name="set-up-workflows-for-expense-management"></a><span data-ttu-id="34ed7-103">व्यय प्रबंधन के लिए कार्यप्रवाह सेट करना</span><span class="sxs-lookup"><span data-stu-id="34ed7-103">Set up workflows for Expense management</span></span>

<span data-ttu-id="34ed7-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="34ed7-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="34ed7-105">आप यात्रा और व्यय दस्तावेजों की समीक्षा और स्वीकृति के लिए कार्यप्रवाह प्रक्रिया सेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="34ed7-105">You can set up a workflow process to review and approve travel and expense documents.</span></span> <span data-ttu-id="34ed7-106">आप व्यय रिपोर्ट, यात्रा मांग-पत्र और नकद अग्रिम अनुरोधों के लिए कार्यप्रवाह निर्धारित कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="34ed7-106">You can define workflows for expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="34ed7-107">कार्यप्रवाह व्यावसायिक प्रक्रिया का प्रतिनिधित्व करता है और परिभाषित करता है कि सिस्टम के माध्यम से दस्तावेज़ कैसे प्रवाहित होता है.</span><span class="sxs-lookup"><span data-stu-id="34ed7-107">A workflow represents a business process and defines how a document flows through the system.</span></span> <span data-ttu-id="34ed7-108">कार्यप्रवाह यह भी दिखाता है कि किसे कार्य पूरा या दस्तावेज़ को स्वीकृत करना है.</span><span class="sxs-lookup"><span data-stu-id="34ed7-108">The workflow also indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="34ed7-109">आपके संगठन में कार्यप्रवाह सिस्टम इस्तेमाल करने के कई फ़ायदे हैं:</span><span class="sxs-lookup"><span data-stu-id="34ed7-109">There are several benefits of using the workflow system in your organization:</span></span>

- <span data-ttu-id="34ed7-110">**सुसंगत प्रक्रियाएं**: आप विशिष्ट दस्तावेजों के लिए स्वीकृति प्रक्रिया को निर्धारित कर सकते हैं, जैसे कि खरीद मांग-पत्र और व्यय रिपोर्ट.</span><span class="sxs-lookup"><span data-stu-id="34ed7-110">**Consistent processes**: You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="34ed7-111">कार्यप्रवाह सिस्टम का इस्तेमाल यह सुनिश्चित करने में सहायता करता है कि दस्तावेजों को सुसंगत और कुशल तरीके से संसाधित और स्वीकृत किया जाए.</span><span class="sxs-lookup"><span data-stu-id="34ed7-111">Using the workflow system helps ensure that documents are processed and approved in a consistent and efficient manner.</span></span>
- <span data-ttu-id="34ed7-112">**प्रक्रिया दृश्यता**: आप किसी विशिष्ट कार्यप्रवाह उदाहरण की स्थिति, इतिहास और प्रदर्शन मेट्रिक्स पर नज़र रख सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="34ed7-112">**Process visibility**: You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="34ed7-113">यह आपको यह निर्धारित करने में मदद करता है कि दक्षता में सुधार के लिए कार्यप्रवाह में परिवर्तन किए जाने चाहिए या नहीं.</span><span class="sxs-lookup"><span data-stu-id="34ed7-113">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>
- <span data-ttu-id="34ed7-114">**केंद्रीकृत कार्य सूची**:उपयोगकर्ता कार्यप्रवाह टास्कों और उन्हें सौंपे गए स्वीकृतियों को देखने के लिए केंद्रीकृत कार्य सूची देख सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="34ed7-114">**Centralized work list**: Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

## <a name="workflow-types"></a><span data-ttu-id="34ed7-115">कार्यप्रवाह प्रकार</span><span class="sxs-lookup"><span data-stu-id="34ed7-115">Workflow types</span></span>

<span data-ttu-id="34ed7-116">निम्न तालिका उन कार्यप्रवाहों के प्रकारों को सूचीबद्ध करती है जिन्हें आप **व्यय प्रबंधन** में बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="34ed7-116">The following table lists the types of workflows that you can create in **Expense Management**.</span></span>


|              <span data-ttu-id="34ed7-117"><strong>प्रकार</strong></span><span class="sxs-lookup"><span data-stu-id="34ed7-117"><strong>Type</strong></span></span>              |                   <span data-ttu-id="34ed7-118"><strong>इस प्रकार का उपयोग करें</strong></span><span class="sxs-lookup"><span data-stu-id="34ed7-118"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|   <span data-ttu-id="34ed7-119"><strong>व्यय रिपोर्ट स्वत: स्वीकृति</strong></span><span class="sxs-lookup"><span data-stu-id="34ed7-119"><strong>Expense report auto approval</strong></span></span> |            <span data-ttu-id="34ed7-120">व्यय रिपोर्ट के लिए स्वीकृति कार्यप्रवाह बनाएं.</span><span class="sxs-lookup"><span data-stu-id="34ed7-120">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="34ed7-121"><strong>व्यय रिपोर्ट स्वत: पोस्टिंग</strong></span><span class="sxs-lookup"><span data-stu-id="34ed7-121"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="34ed7-122">व्यय रिपोर्ट के लिए स्वचालित पोस्टिंग कार्यप्रवाह बनाएं.</span><span class="sxs-lookup"><span data-stu-id="34ed7-122">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="34ed7-123"><strong>व्यय लाइन आइटम</strong></span><span class="sxs-lookup"><span data-stu-id="34ed7-123"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="34ed7-124">व्यय रिपोर्ट पर लाइन आइटम के लिए स्वीकृति कार्यप्रवाह बनाएं.</span><span class="sxs-lookup"><span data-stu-id="34ed7-124">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="34ed7-125"><strong>व्यय लाइन आइटम स्वत: पोस्टिंग</strong></span><span class="sxs-lookup"><span data-stu-id="34ed7-125"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="34ed7-126">व्यय रिपोर्ट पर लाइन आइटम के लिए स्वचालित पोस्टिंग कार्यप्रवाह बनाएं.</span><span class="sxs-lookup"><span data-stu-id="34ed7-126">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="34ed7-127"><strong>यात्रा की आवश्यकता</strong></span><span class="sxs-lookup"><span data-stu-id="34ed7-127"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="34ed7-128">यात्रा मांग-पत्रों के लिए स्वीकृति कार्यप्रवाह बनाएं.</span><span class="sxs-lookup"><span data-stu-id="34ed7-128">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="34ed7-129"><strong>नकद अग्रिम अनुरोध</strong></span><span class="sxs-lookup"><span data-stu-id="34ed7-129"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="34ed7-130">नकद अग्रिम अनुरोधों के लिए स्वीकृति कार्यप्रवाह बनाएं.</span><span class="sxs-lookup"><span data-stu-id="34ed7-130">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="34ed7-131"><strong>VAT कर रिकवरी</strong></span><span class="sxs-lookup"><span data-stu-id="34ed7-131"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="34ed7-132">मूल्य वर्धित कर (VAT) की वसूली के लिए स्वीकृति कार्यप्रवाह बनाएं.</span><span class="sxs-lookup"><span data-stu-id="34ed7-132">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |
