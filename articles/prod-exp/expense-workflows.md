---
title: ख़र्च प्रबंधन कार्यप्रवाह सेट करें
description: आप यात्रा और व्यय दस्तावेजों की समीक्षा और स्वीकृति के लिए कार्यप्रवाह प्रक्रिया सेट कर सकते हैं.
author: ShylaThompson
manager: AnnBe
ms.date: 09/13/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WorkflowtableListPageRnr
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0af23ed2cf172e4c90de72f5db389c349303c039
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077854"
---
# <a name="set-up-expense-management-workflows"></a><span data-ttu-id="69105-103">ख़र्च प्रबंधन कार्यप्रवाह सेट करें</span><span class="sxs-lookup"><span data-stu-id="69105-103">Set up Expense management workflows</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="69105-104">आप कार्यप्रवाह प्रक्रिया सेट कर सकते हैं जिसका इस्तेमाल यात्रा और व्यय दस्तावेजों की समीक्षा और स्वीकृत करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="69105-104">You can set up a workflow process that is used to review and approve travel and expense documents.</span></span> <span data-ttu-id="69105-105">जिन दस्तावेजों के लिए कार्यप्रवाहों को परिभाषित किया जा सकता है उनमें ख़र्च रिपोर्ट, यात्रा मांग और नकद अग्रिम अनुरोध शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="69105-105">The documents for which workflows can be defined include expense reports, travel requisitions, and cash advance requests.</span></span>

<span data-ttu-id="69105-106">एक कार्यप्रवाह एक व्यावसायिक प्रक्रिया का प्रतिनिधित्व करता है.</span><span class="sxs-lookup"><span data-stu-id="69105-106">A workflow represents a business process.</span></span> <span data-ttu-id="69105-107">यह परिभाषित करता है कि कोई दस्तावेज़ सिस्टम के माध्यम से कैसे आगे बढ़ता है और इंगित करता है कि किसी कार्य को किसे पूरा करना चाहिए या दस्तावेज़ को अनुमोदित करना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="69105-107">It defines how a document flows through the system and indicates who must complete a task or approve a document.</span></span> <span data-ttu-id="69105-108">आपके संगठन में कार्यप्रवाह सिस्टम इस्तेमाल करने के कई फ़ायदे हैं:</span><span class="sxs-lookup"><span data-stu-id="69105-108">There are several benefits of using the workflow system in your organization:</span></span>

-   <span data-ttu-id="69105-109">**सुसंगत प्रक्रियाएं** — आप विशिष्ट दस्तावेजों के लिए स्वीकृति प्रक्रिया को निर्धारित कर सकते हैं, जैसे कि खरीद मांग-पत्र और व्यय रिपोर्ट.</span><span class="sxs-lookup"><span data-stu-id="69105-109">**Consistent processes** — You can define the approval process for specific documents, such as purchase requisitions and expense reports.</span></span> <span data-ttu-id="69105-110">कार्यप्रवाह सिस्टम का इस्तेमाल यह सुनिश्चित करने में सहायता करता है कि दस्तावेजों को सुसंगत और कुशल तरीके से संसाधित और स्वीकृत किया गया है.</span><span class="sxs-lookup"><span data-stu-id="69105-110">Using the workflow system helps to ensure that documents are processed and approved in a consistent and efficient manner.</span></span>

-   <span data-ttu-id="69105-111">प्रक्रिया दृश्यता — आप किसी विशिष्ट कार्यप्रवाह उदाहरण की स्थिति, इतिहास और प्रदर्शन मेट्रिक्स पर नज़र रख सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="69105-111">Process visibility — You can track the status, history, and performance metrics of a specific workflow instance.</span></span> <span data-ttu-id="69105-112">यह आपको यह निर्धारित करने में मदद करता है कि दक्षता में सुधार के लिए कार्यप्रवाह में परिवर्तन किए जाने चाहिए या नहीं.</span><span class="sxs-lookup"><span data-stu-id="69105-112">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>

-   <span data-ttu-id="69105-113">केंद्रीकृत कार्य सूची — उपयोगकर्ता कार्यप्रवाह टास्कों और उन्हें सौंपे गए स्वीकृतियों को देखने के लिए केंद्रीकृत कार्य सूची देख सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="69105-113">Centralized work list — Users can view a centralized work list to view the workflow tasks and approvals assigned to them.</span></span> 

<span data-ttu-id="69105-114">**कार्यप्रवाह के प्रकार जिसे आप बना सकते हैं**</span><span class="sxs-lookup"><span data-stu-id="69105-114">**The types of workflows you can create**</span></span>

<span data-ttu-id="69105-115">निम्न तालिका उन कार्यप्रवाहों के प्रकारों को सूचीबद्ध करती है जिन्हें आप **ख़र्च** में बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="69105-115">The following table lists the types of workflows that you can create in **Expense**.</span></span>


|              <span data-ttu-id="69105-116"><strong>प्रकार</strong></span><span class="sxs-lookup"><span data-stu-id="69105-116"><strong>Type</strong></span></span>              |                   <span data-ttu-id="69105-117"><strong>इस प्रकार का उपयोग करें</strong></span><span class="sxs-lookup"><span data-stu-id="69105-117"><strong>Use this type to</strong></span></span>                   |
|-------------------------------------------------|-----------------------------------------------------------------------|
|         <span data-ttu-id="69105-118"><strong>व्यय की रिपोर्ट</strong></span><span class="sxs-lookup"><span data-stu-id="69105-118"><strong>Expense report</strong></span></span>         |            <span data-ttu-id="69105-119">व्यय रिपोर्ट के लिए स्वीकृति कार्यप्रवाह बनाएं.</span><span class="sxs-lookup"><span data-stu-id="69105-119">Create approval workflows for expense reports.</span></span>             |
|  <span data-ttu-id="69105-120"><strong>व्यय रिपोर्ट स्वत: पोस्टिंग</strong></span><span class="sxs-lookup"><span data-stu-id="69105-120"><strong>Expense report auto posting</strong></span></span>   |        <span data-ttu-id="69105-121">व्यय रिपोर्ट के लिए स्वचालित पोस्टिंग कार्यप्रवाह बनाएं.</span><span class="sxs-lookup"><span data-stu-id="69105-121">Create automatic posting workflows for expense reports.</span></span>        |
|       <span data-ttu-id="69105-122"><strong>व्यय लाइन आइटम</strong></span><span class="sxs-lookup"><span data-stu-id="69105-122"><strong>Expense line item</strong></span></span>        |     <span data-ttu-id="69105-123">व्यय रिपोर्ट पर लाइन आइटम के लिए स्वीकृति कार्यप्रवाह बनाएं.</span><span class="sxs-lookup"><span data-stu-id="69105-123">Create approval workflows for line items on expense reports.</span></span>      |
| <span data-ttu-id="69105-124"><strong>व्यय लाइन आइटम स्वत: पोस्टिंग</strong></span><span class="sxs-lookup"><span data-stu-id="69105-124"><strong>Expense line item auto posting</strong></span></span> | <span data-ttu-id="69105-125">व्यय रिपोर्ट पर लाइन आइटम के लिए स्वचालित पोस्टिंग कार्यप्रवाह बनाएं.</span><span class="sxs-lookup"><span data-stu-id="69105-125">Create automatic posting workflows for line items on expense reports.</span></span> |
|       <span data-ttu-id="69105-126"><strong>यात्रा की आवश्यकता</strong></span><span class="sxs-lookup"><span data-stu-id="69105-126"><strong>Travel requisition</strong></span></span>       |          <span data-ttu-id="69105-127">यात्रा मांग-पत्रों के लिए स्वीकृति कार्यप्रवाह बनाएं.</span><span class="sxs-lookup"><span data-stu-id="69105-127">Create approval workflows for travel requisitions.</span></span>           |
|      <span data-ttu-id="69105-128"><strong>नकद अग्रिम अनुरोध</strong></span><span class="sxs-lookup"><span data-stu-id="69105-128"><strong>Cash advance request</strong></span></span>      |         <span data-ttu-id="69105-129">नकद अग्रिम अनुरोधों के लिए स्वीकृति कार्यप्रवाह बनाएं.</span><span class="sxs-lookup"><span data-stu-id="69105-129">Create approval workflows for cash advance requests.</span></span>          |
|        <span data-ttu-id="69105-130"><strong>VAT कर रिकवरी</strong></span><span class="sxs-lookup"><span data-stu-id="69105-130"><strong>VAT tax recovery</strong></span></span>        | <span data-ttu-id="69105-131">मूल्य वर्धित कर (VAT) की वसूली के लिए स्वीकृति कार्यप्रवाह बनाएं.</span><span class="sxs-lookup"><span data-stu-id="69105-131">Create approval workflows for the recovery of value-added tax (VAT).</span></span>  |

