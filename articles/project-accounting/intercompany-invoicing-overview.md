---
title: अंतरकंपनी इनवॉइसिंग ओवरव्यू
description: यह विषय परियोजनाओं के लिए अंतरकंपनी इनवॉइस के बारे में जानकारी और उदाहरण प्रदान करता है.
author: sigitac
manager: tfehr
ms.date: 11/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 670b5d15ecf1ef7dcc034064e625814cbe6d54b0
ms.sourcegitcommit: addbe0647619413e85e7cde80f6a21db95ab623e
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/20/2020
ms.locfileid: "4595483"
---
# <a name="intercompany-invoicing-overview"></a><span data-ttu-id="9e7aa-103">अंतरकंपनी इनवॉइसिंग ओवरव्यू</span><span class="sxs-lookup"><span data-stu-id="9e7aa-103">Intercompany invoicing overview</span></span>

<span data-ttu-id="9e7aa-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="9e7aa-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="9e7aa-105">आपके संगठन में कई विभाग, सहायक और अन्य कानूनी संस्थाएं हो सकती हैं जो उत्पादों और सेवाओं को परियोजनाओं के लिए एक दूसरे को हस्तांतरित करती हैं.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-105">Your organization might have multiple divisions, subsidiaries, and other legal entities that transfer products and services to each other for projects.</span></span> <span data-ttu-id="9e7aa-106">सेवा या उत्पाद प्रदान करने वाले कानूनी निकाय को *लेंडिंग कानूनी निकाय* कहा जाता है.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-106">The legal entity that provides the service or product is called the *lending legal entity*.</span></span> <span data-ttu-id="9e7aa-107">सेवा या उत्पाद प्राप्त करने वाले कानूनी निकाय को *बॉरोइंग कानूनी निकाय* कहा जाता है.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-107">The legal entity that receives the service or product is called the *borrowing legal entity*.</span></span>

<span data-ttu-id="9e7aa-108">निम्नलिखित चित्रण एक विशिष्ट परिदृश्य को दर्शाता है, जहां दो कानूनी निकाय, Contoso Robotics USA (बॉरोइंग कानूनी निकाय) और Contoso Robotics UK (लेंडिंग कानूनी निकाय) ग्राहक, एडवेंचर वर्क्स के लिए एक परियोजना देने के लिए संसाधनों को साझा करते हैं.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-108">The following illustration shows a typical scenario where two legal entities, Contoso Robotics USA (the borrowing legal entity) and Contoso Robotics UK (the lending legal entity) share resources to deliver a project for the customer, Adventure works.</span></span> <span data-ttu-id="9e7aa-109">इस परिदृश्य के लिए, Contoso Robotics USA को एडवेंचर वर्क्स को कार्य वितरित करने के लिए अनुबंधित किया गया है.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-109">For this scenario, Contoso Robotics USA is contracted to deliver the work to Adventure Works.</span></span>

![इंटरकंपनी इनवॉइसिंग](./media/IntercompanyScenario.png) 

<span data-ttu-id="9e7aa-111">Dynamics 365 Project Operations अंतरकंपनी लेनदेन को संसाधित करने के लिए निम्न प्रवाह का उपयोग करता है:</span><span class="sxs-lookup"><span data-stu-id="9e7aa-111">Dynamics 365 Project Operations uses the following flow to process intercompany transactions:</span></span>

1. <span data-ttu-id="9e7aa-112">लेंडिंग कानूनी निकाय के संसाधन, बॉरोइंग कानूनी निकाय में परियोजनाओं के विरुद्ध समय और व्यय को बुक करके अंतरकंपनी समय या व्यय लेनदेन रिकॉर्ड करते हैं.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-112">Resources from the lending legal entity record intercompany time or expense transactions by booking time and expense against projects in the borrowing legal entity.</span></span>
2. <span data-ttu-id="9e7aa-113">लेंडिंग कंपनी में समय और व्यय लागतों को बॉरोइंग कंपनी की इकाई लागत मूल्य सूची का उपयोग करके रिकॉर्ड किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-113">Time and expense costs are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
3. <span data-ttu-id="9e7aa-114">लेंडिंग कंपनी में अंतरकंपनी बिल न किए गए विक्रय लेनदेनों को बॉरोइंग कंपनी की इकाई लागत मूल्य सूची का उपयोग करके रिकॉर्ड किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-114">Intercompany unbilled sale transactions are recorded in the lending company by using the borrowing company's unit cost price list.</span></span>
4. <span data-ttu-id="9e7aa-115">परियोजना अनुबंध विक्रय मूल्य सूची का उपयोग करके बॉरोइंग कंपनी में बिल न की गई आय को रिकॉर्ड किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-115">Unbilled revenue is recorded in the borrowing company using the project contract sales price list.</span></span> <span data-ttu-id="9e7aa-116">बिल न की गई आय को रिकॉर्ड किए जाने पर ग्राहक को बिल किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-116">The customer can be billed when unbilled revenue is recorded.</span></span> <span data-ttu-id="9e7aa-117">अंतरकंपनी इनवॉइस प्रक्रिया के पूरा होने तक ग्राहक को प्रतीक्षा नहीं करनी होती है.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-117">The customer doesn't have to wait until intercompany invoice processing is complete.</span></span>
5. <span data-ttu-id="9e7aa-118">लेंडिंग कंपनी में अंतरकंपनी ग्राहक इनवॉइस आवधिक आधार पर बनाए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-118">Intercompany customer invoices are created on a periodic basis in the lending company.</span></span> <span data-ttu-id="9e7aa-119">इनवॉइस मैन्युअल रूप से या आवधिक स्वचालित प्रक्रिया का उपयोग करके बनाए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-119">The invoices are created manually or by using a periodic automated process.</span></span> <span data-ttu-id="9e7aa-120">प्रत्येक बॉरोइंग कानूनी निकाय के लिए एक एकल इनवॉइस बनाया जा सकता है या परियोजना द्वारा अलग-अलग इनवॉइस बनाए जा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-120">A single invoice can be created for each borrowing legal entity or separate invoices can be created by project.</span></span>
6. <span data-ttu-id="9e7aa-121">लेंडिंग कानूनी निकाय में अंतरकंपनी ग्राहक इनवॉइस के पोस्ट किए जाने पर, बॉरोइंग कानूनी निकाय में संबंधित लंबित विक्रेता इनवॉइस बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-121">When the intercompany customer invoice is posted in the lending legal entity, the corresponding pending vendor invoice is created in the borrowing legal entity.</span></span> <span data-ttu-id="9e7aa-122">इनवॉइस के पोस्ट किए जाने पर, लंबित विक्रेता इनवॉइस की लागत को परियोजना सबलेज़र में रिकॉर्ड किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-122">The costs in the pending vendor invoice will be recorded to the project subledger when the invoice is posted.</span></span>

<span data-ttu-id="9e7aa-123">निम्न आरेख अंतरकंपनी इनवॉइस को दिखाता है, क्योंकि यह लेखांकन इवेंट और सामान्य लेज़र के लिए अपेक्षित पोस्टिंग से संबंधित है.</span><span class="sxs-lookup"><span data-stu-id="9e7aa-123">The following diagram illustrates intercompany invoicing as it relates to accounting events and expected postings to the general ledger.</span></span>

![अंतरकंपनी प्रवाह](./media/IntercompanyFlow.png)

## <a name="additional-resources"></a><span data-ttu-id="9e7aa-125">अतिरिक्त संसाधन</span><span class="sxs-lookup"><span data-stu-id="9e7aa-125">Additional resources</span></span>

- [<span data-ttu-id="9e7aa-126">अंतरकंपनी इनवॉइस को कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="9e7aa-126">Configure intercompany invoicing</span></span>](configure-intercompany-invoicing.md)
- [<span data-ttu-id="9e7aa-127">अंतरकंपनी लेनदेन रिकॉर्ड करें</span><span class="sxs-lookup"><span data-stu-id="9e7aa-127">Record intercompany transactions</span></span>](create-intercompany-transactions.md)
- [<span data-ttu-id="9e7aa-128">अंतरकंपनी ग्राहक और विक्रेता इनवॉइस बनाएँ</span><span class="sxs-lookup"><span data-stu-id="9e7aa-128">Create intercompany customer and vendor invoices</span></span>](create-intercompany-customer-vendor-invoices.md)
