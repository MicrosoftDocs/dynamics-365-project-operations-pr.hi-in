---
title: Project Operations ड्यूल-राइट एकीकरण
description: Project Operations ड्यूल-राइट एकीकरण अवलोकन.
author: sigitac
ms.date: 04/28/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d9d6a7c367872219b4aca32aecb15d6837ebe296
ms.sourcegitcommit: 02f00960198cc78a5e96955a9e4390c2c6393bbf
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/28/2021
ms.locfileid: "5955660"
---
# <a name="project-operations-dual-write-integration-overview"></a><span data-ttu-id="8fb1a-103">Project Operations ड्यूल-राइट एकीकरण अवलोकन</span><span class="sxs-lookup"><span data-stu-id="8fb1a-103">Project Operations dual-write integration overview</span></span>

<span data-ttu-id="8fb1a-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations_</span><span class="sxs-lookup"><span data-stu-id="8fb1a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="8fb1a-105">Project Operations Microsoft Dataverse और Dynamics 365 Finance में डेटा को सिंक्रनाइज़ करने के लिए [दोहरा-लेखन क्षमता](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="8fb1a-105">Project Operations uses [dual-write capabilities](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) to synchronize data across Microsoft Dataverse and Dynamics 365 Finance.</span></span>

<span data-ttu-id="8fb1a-106">निम्नलिखित चित्रण बताता है कि डेटा को Dataverse और फाइनेंस के बीच इस एकीकरण के हिस्से के रूप में कैसे सिंक्रनाइज़ किया गया है.</span><span class="sxs-lookup"><span data-stu-id="8fb1a-106">The following illustration shows how data is synchronized as part of this integration between Dataverse and Finance.</span></span>

![Project Operations डेटा प्रवाह अवलोकन](./media/ProjectOperationsFlows.jpg)

<span data-ttu-id="8fb1a-108">Dataverse पर Project Operations Power Platform क्षमताओं का उपयोग करके एक आधुनिक उपयोगकर्ता इंटरफ़ेस (UI) और आसान नो-कोड/कम-कोड विस्तारणीयता प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="8fb1a-108">Project Operations on Dataverse provides a modern user interface (UI) and easy no-code/low-code extensibility using Power Platform capabilities.</span></span> <span data-ttu-id="8fb1a-109">प्रोजेक्ट मैनेजर, रिसोर्स मैनेजर, प्रोजेक्ट टीम के सदस्य और अन्य फ्रंट-ऑफिस व्यक्ति, Dataverse पर Project Operations में अपनी गतिविधियां प्रदर्शित करते हैं.</span><span class="sxs-lookup"><span data-stu-id="8fb1a-109">Project managers, Resource managers, Project team members, and other front-office personas, perform their activities in Project Operations on Dataverse.</span></span>

<span data-ttu-id="8fb1a-110">फाइनैंस में Project Operations प्रोजेक्ट लेखांकन और राजस्व मान्यता सहायता प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="8fb1a-110">Project Operations in Finance provides project accounting and revenue recognition support.</span></span> <span data-ttu-id="8fb1a-111">Project Operations बिक्री कर गणना, मुद्रा विनिमय दरों, वित्तीय आयाम रिपोर्टिंग इत्यादि के लिए फाइनेंस में फाइनेंशियल फ्रेमवर्क के लिए प्लग करता है.</span><span class="sxs-lookup"><span data-stu-id="8fb1a-111">Project Operations plugs in to the financial framework in Finance for sales tax calculation, currency exchange rates, financial dimension reporting, and more.</span></span> <span data-ttu-id="8fb1a-112">प्रोजेक्ट अकाउंटेंट के अनुभव ज्यादातर फाइऩेंस आधारित होते हैं.</span><span class="sxs-lookup"><span data-stu-id="8fb1a-112">The Project accountant experiences are mostly based in Finance.</span></span>

<span data-ttu-id="8fb1a-113">Project Operations एकीकरण में निम्नलिखित घटक एकीकरण शामिल हैं:</span><span class="sxs-lookup"><span data-stu-id="8fb1a-113">Project Operations integration consists of the following component integration:</span></span>


- [<span data-ttu-id="8fb1a-114">Project Operations सेटअप और कॉन्फ़िगरेशन डेटा एकीकरण</span><span class="sxs-lookup"><span data-stu-id="8fb1a-114">Project Operations setup and configuration data integration</span></span>](resource-dual-write-setup-integration.md) 
- [<span data-ttu-id="8fb1a-115">परियोजना अनुमान और वास्तविक आकड़ें</span><span class="sxs-lookup"><span data-stu-id="8fb1a-115">Project estimates and actuals</span></span>](resource-dual-write-estimates-actuals.md)
- [<span data-ttu-id="8fb1a-116">परियोजना इनवॉइस</span><span class="sxs-lookup"><span data-stu-id="8fb1a-116">Project invoices</span></span>](resource-dual-write-project-invoice.md)
- [<span data-ttu-id="8fb1a-117">व्यय प्रबंधन</span><span class="sxs-lookup"><span data-stu-id="8fb1a-117">Expense management</span></span>](resource-dual-write-expense.md)
- [<span data-ttu-id="8fb1a-118">विक्रेता इनवॉइस</span><span class="sxs-lookup"><span data-stu-id="8fb1a-118">Vendor invoice</span></span>](resource-dual-write-vendor-invoice.md)
