---
title: परियोजना कोट प्रबंधित करें
description: यह विषय परियोजना कोट के बारे में जानकारी प्रदान करता है.
author: rumant
ms.date: 10/26/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 8e0b20d4780a14edc3c242e261e22d4905f783a4
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994813"
---
# <a name="manage-project-quotes"></a><span data-ttu-id="cf030-103">परियोजना कोट प्रबंधित करें</span><span class="sxs-lookup"><span data-stu-id="cf030-103">Manage project quotes</span></span>

<span data-ttu-id="cf030-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="cf030-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="cf030-105">Dynamics 365 Project Operations में, परियोजना कोट परियोजना कार्य के प्रस्तावों का निर्माण करने में मदद करने के लिए डिज़ाइन किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="cf030-105">In Dynamics 365 Project Operations, project quotes are designed to help build proposals for project work.</span></span> <span data-ttu-id="cf030-106">Project Operations में परियोजना कोट की संरचना निम्न घटकों के साथ परियोजना प्रस्तावों के लिए संरचित की गई है:</span><span class="sxs-lookup"><span data-stu-id="cf030-106">The structure of a project quote in Project Operations is structured for project proposals with the following components:</span></span>

  - <span data-ttu-id="cf030-107">वे कोट पंक्तियाँ, जो कार्य के उन असतत घटकों की पहचान करती हैं, जिन्हें उच्च-स्तरीय घटकों के रूप में प्रस्तुत किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="cf030-107">Quote lines that identify the discrete components of work that will be presented as high-level components.</span></span>
  - <span data-ttu-id="cf030-108">वे कोट पंक्ति विवरण, जो प्रत्येक उच्च-स्तरीय घटक या कोट पंक्ति के लिए कार्य की पहचान और अनुमान लगाते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf030-108">Quote line details that identify and estimate the work for each high-level component or quote line.</span></span> <span data-ttu-id="cf030-109">शेड्यूल या दिनांक अनुमान और कार्य के लिए वित्तीय पहलू उस कोट पंक्ति से जुड़े हैं.</span><span class="sxs-lookup"><span data-stu-id="cf030-109">Schedule or date estimates and the financial aspects for the work are tied to that quote line.</span></span>
  - <span data-ttu-id="cf030-110">प्रत्येक कोट पंक्ति के लिए अनुबंध मॉडल और प्रभार्य घटक सेट अप किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf030-110">Contracting models and chargeable components are set up for each quote line.</span></span> <span data-ttu-id="cf030-111">यह सेट अप प्रत्येक कोट पंक्ति और समग्र कोट के लिए आय, खर्च, और लाभप्रदता के प्रसार का अनुमान लगाने में मदद करता है.</span><span class="sxs-lookup"><span data-stu-id="cf030-111">This set up helps estimate the spread of revenue, spend, and profitability for each quote line and the overall quote.</span></span>

## <a name="view-all-project-based-quotes"></a><span data-ttu-id="cf030-112">सभी परियोजना-आधारित कोट देखें</span><span class="sxs-lookup"><span data-stu-id="cf030-112">View all project-based quotes</span></span>

<span data-ttu-id="cf030-113">**कोट** सूची पृष्ठ से सभी परियोजना कोट की एक सूची देखी जा सकती है.</span><span class="sxs-lookup"><span data-stu-id="cf030-113">A list of all the project quotes can be seen from the **Quotes** list page.</span></span> 

1. <span data-ttu-id="cf030-114">**विक्रय** > **कोट** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="cf030-114">Go to **Sales** > **Quotes**.</span></span> <span data-ttu-id="cf030-115">सिस्टम में आपके सभी परियोजना कोट की एक सूची दिखाई गई है.</span><span class="sxs-lookup"><span data-stu-id="cf030-115">A list of all your project quotes in the system are shown.</span></span> 
2. <span data-ttu-id="cf030-116">कोट के अन्य फ़िल्टर किए गए दृश्य चुनने के लिए **दृश्य स्विचर** का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="cf030-116">Use the **View Switcher** to select other filtered views of the quotes.</span></span> <span data-ttu-id="cf030-117">कस्टम फ़िल्टर मापदंड का उपयोग करके, आप अपने स्वयं के दृश्यों और नेविगेशन विकल्पों को कॉन्फ़िगर कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="cf030-117">Using custom filter criteria, you can configure your own views and navigation options.</span></span>

<span data-ttu-id="cf030-118">कोट को इस सूची पृष्ठ या विवरण पृष्ठों पर बनाया या हटाया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="cf030-118">Quotes can be created or deleted from this list page or detail pages.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]