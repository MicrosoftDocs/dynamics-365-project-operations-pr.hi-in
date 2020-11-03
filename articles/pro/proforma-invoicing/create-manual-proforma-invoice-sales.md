---
title: एक मैनुअल प्रोफ़ॉर्मा इनवॉइस बनाना
description: यह विषय Project Operations में एक मैनुअल प्रोफ़ॉर्मा इनवॉइस बनाने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d5e93206737507bf6698a9746815c790d3dfc904
ms.sourcegitcommit: 3a0c18823a7ad23df5aa3de272779313abe56c82
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/20/2020
ms.locfileid: "4077929"
---
# <a name="creating-a-manual-proforma-invoice"></a><span data-ttu-id="78795-103">एक मैनुअल प्रोफ़ॉर्मा इनवॉइस बनाना</span><span class="sxs-lookup"><span data-stu-id="78795-103">Creating a manual proforma invoice</span></span>

<span data-ttu-id="78795-104">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="78795-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="78795-105">Dynamics 365 Project Operations में, प्रोफ़ॉर्मा इनवॉइस को आवश्यकतानुसार मैन्युअल रूप से बनाया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="78795-105">In Dynamics 365 Project Operations, proforma invoices can be created manually as needed.</span></span> <span data-ttu-id="78795-106">आप मैन्युअल रूप से **प्रोजेक्ट अनुबंध** सूची पृष्ठ से या **प्रोजेक्ट अनुबंध** विवरण पृष्ठ से एक प्रोफ़ॉर्मा इनवॉइस बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="78795-106">You can manually create a proforma invoice from the **Project Contracts** list page or from the **Project Contract** details page.</span></span>

##  <a name="project-contracts-list-page"></a><span data-ttu-id="78795-107">प्रोजेक्ट अनुबंध सूची पृष्ठ</span><span class="sxs-lookup"><span data-stu-id="78795-107">Project Contracts list page</span></span>

<span data-ttu-id="78795-108">**प्रोजेक्ट अनुबंध** सूची पृष्ठ से, एक या एक से अधिक प्रोजेक्ट अनुबंधों का चयन करें, और सभी चयनित रिकॉर्ड के लिए इनवॉइस बनाएं.</span><span class="sxs-lookup"><span data-stu-id="78795-108">From **Project Contracts** list page, select one or more project contracts, and create invoices for all of the selected records.</span></span>

<span data-ttu-id="78795-109">सिस्टम यह देखने के लिए जांच करता है कि चयनित प्रोजेक्ट अनुबंधों में से कौन सा पुराना **इनवॉइस के लिए तैयार** बैकलॉग आज की तिथि से पहले है.</span><span class="sxs-lookup"><span data-stu-id="78795-109">The system checks to see which of the selected project contracts has a **Ready to Invoice** backlog  dated before today's date.</span></span> <span data-ttu-id="78795-110">उन अनुबंधों से, सिस्टम ड्राफ्ट प्रोफ़ॉर्मा इनवॉइस बनाता है.</span><span class="sxs-lookup"><span data-stu-id="78795-110">From those contracts, the system creates draft proforma invoices.</span></span> <span data-ttu-id="78795-111">यदि किसी प्रोजेक्ट अनुबंध में कई ग्राहक हैं, तो प्रति ग्राहक एक इनवॉइस बनाया जा सकता है, और प्रति प्रोजेक्ट अनुबंध कई इनवॉइस हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="78795-111">If a project contract has multiple customers, there may be one invoice created per customer, and multiple invoices per project contract.</span></span>

<span data-ttu-id="78795-112">बनाए गए सभी प्रोजेक्ट इनवॉइस **सेल्स** क्षेत्र के **बिलिंग** अनुभाग में **इनवॉइस** पृष्ठ पर उपलब्ध हैं.</span><span class="sxs-lookup"><span data-stu-id="78795-112">All of the created project invoices are available on the **Invoice** page in the **Billing** section of the **Sales** area.</span></span>

## <a name="project-contract-details-page"></a><span data-ttu-id="78795-113">प्रोजेक्ट अनुबंध विवरण पृष्ठ</span><span class="sxs-lookup"><span data-stu-id="78795-113">Project Contract details page</span></span>

<span data-ttu-id="78795-114">**प्रोजेक्ट अनुबंध** विवरण पृष्ठ से एक प्रोफ़ॉर्मा इनवॉइस भी बनाया जा सकता है, जो उस विशिष्ट प्रोजेक्ट अनुबंध के लिए इनवॉइस बनाता है.</span><span class="sxs-lookup"><span data-stu-id="78795-114">A proforma invoice can also be created from the **Project Contract** details page, which creates the invoice for that specific project contract.</span></span> <span data-ttu-id="78795-115">सिस्टम सत्यापित करता है कि प्रोजेक्ट अनुबंध में **इनवॉइस के लिए तैयार** बैकलॉग है जो आज की तिथि से पहले का है.</span><span class="sxs-lookup"><span data-stu-id="78795-115">The system verifies that the project contract has a **Ready to Invoice** backlog that is dated before today's date.</span></span> <span data-ttu-id="78795-116">इन अनुबंधों से, सिस्टम प्रत्येक अनुबंध लाइन पर ग्राहकों की संख्या के आधार पर ड्राफ्ट प्रोफ़ॉर्मा इनवॉइस बनाता है.</span><span class="sxs-lookup"><span data-stu-id="78795-116">From these contracts, the system creates draft proforma invoices based on the number of customers on each contract line.</span></span>

<span data-ttu-id="78795-117">जब एक भी प्रोफ़ॉर्मा इनवॉइस बनाया जाता है, तो **इनवॉइस** पृष्ठ खुलता है.</span><span class="sxs-lookup"><span data-stu-id="78795-117">When there's a single proforma invoice created, the **Invoice** page opens.</span></span> <span data-ttu-id="78795-118">अगर उस प्रोजेक्ट अनुबंध के लिए कई इनवॉइस बनाए गए हैं, तो सभी बनाए गए इनवॉइस दिखाने के लिए **इनवॉइस** सूची पृष्ठ खुलता है.</span><span class="sxs-lookup"><span data-stu-id="78795-118">If there are multiple invoices created for that project contract, then the **Invoices** list page opens to show all of the created invoices.</span></span>
