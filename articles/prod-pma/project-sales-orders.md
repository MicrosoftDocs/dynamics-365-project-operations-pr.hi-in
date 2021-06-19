---
title: समय और सामग्री परियोजनाओं के लिए सेल्स ऑर्डर का अनुमान लगाएं
description: यह विषय बताता है कि समय और सामग्री परियोजनाओं के लिए परियोजना-आधारित सेल्स ऑर्डर कैसे बनाएं.
author: Yowelle
ms.date: 04/05/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2019-04-05
ms.dyn365.ops.version: AX 10.0.2
ms.openlocfilehash: dec9bc700d18f71ec7c9e976b38cb8cbb41f21b5
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6009663"
---
# <a name="project-sales-orders-for-time-and-material-projects"></a><span data-ttu-id="92cb6-103">समय और सामग्री परियोजनाओं के लिए सेल्स ऑर्डर का अनुमान लगाएं</span><span class="sxs-lookup"><span data-stu-id="92cb6-103">Project sales orders for time and material projects</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="92cb6-104">यह विषय बताता है कि किसी परियोजना के लिए सेल्स ऑर्डर कैसे बनाया जाए.</span><span class="sxs-lookup"><span data-stu-id="92cb6-104">This topic describes how to create a sales order for a project.</span></span> <span data-ttu-id="92cb6-105">सेल्स ऑर्डर केवल **समय और सामग्री** प्रकार की परियोजनाओं के लिए बनाए जा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="92cb6-105">Sales orders can only be created for projects of type **time and material**.</span></span>

<span data-ttu-id="92cb6-106">यदि समय और सामग्री परियोजना में परियोजना अनुबंध पर कई निधीयन स्रोत हैं तो आपको **परियोजना प्रबंधन और लेखांकन मापदंड** पेज पर **कई निधीयन स्त्रोत वाली परियोजनाओं के लिए सेल्स ऑर्डर देने की अनुमति दें** मापदंड सक्षम करना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="92cb6-106">If a time and material project has multiple funding sources on the project contract, you must enable the **Allow sales orders for projects with multiple funding sources** parameter on the **Project management and accounting parameters** page.</span></span> 

> [!NOTE]
> - <span data-ttu-id="92cb6-107">कई निधीयन स्रोतों से परियोजना के सेल्स ऑर्डर का समर्थन अनुप्रयोग रिलीज़ 10.0.2 और उच्चतर के साथ शुरू होता है.</span><span class="sxs-lookup"><span data-stu-id="92cb6-107">Support for project sales orders with multiple funding sources is available starting with application release 10.0.2 and higher.</span></span>
> - <span data-ttu-id="92cb6-108">कई निधीयन स्रोतों के साथ परियोजना के सेल्स ऑर्डर के लिए समर्थन को सक्षम करने के लिए मापदंड को अप्रैल 2020 के रिलीज वेव में हटा दिया जाएगा, जिसके बाद कार्यक्षमता हमेशा सक्षम होगी.</span><span class="sxs-lookup"><span data-stu-id="92cb6-108">The parameter to enable the support for project sales orders with multiple funding sources will be removed in the April 2020 release wave, after which the functionality will always be enabled.</span></span>

<span data-ttu-id="92cb6-109">आप दो तरीकों से परियोजना-आधारित सेल्स ऑर्डर बना सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="92cb6-109">You can create project-based sales orders in two ways:</span></span>

- <span data-ttu-id="92cb6-110">प्रोजेक्ट पर ही जाएं.</span><span class="sxs-lookup"><span data-stu-id="92cb6-110">Go to the project itself.</span></span> <span data-ttu-id="92cb6-111">कार्रवाई फलक पर, **प्रबंधित करें > आइटम कार्य > सेल्स ऑर्डर** चुनें.</span><span class="sxs-lookup"><span data-stu-id="92cb6-111">On the Action Pane, select **Manage > Item tasks > Sales order**.</span></span> <span data-ttu-id="92cb6-112">परियोजना की जानकारी परियोजना से सेल्स ऑर्डर के लिए डिफ़ॉल्ट होगी.</span><span class="sxs-lookup"><span data-stu-id="92cb6-112">The project information will default to the sales order from the project.</span></span> <span data-ttu-id="92cb6-113">यदि परियोजना अनुबंध में एक से अधिक निधीयन स्रोत हैं, तो आपको सेल्स ऑर्डर के लिए ग्राहक को निर्धारित करने के लिए निधीयन स्रोत को चुनना होगा.</span><span class="sxs-lookup"><span data-stu-id="92cb6-113">If the project contract has more than one funding source, you will need to select the funding source to set the customer for the sales order.</span></span> <span data-ttu-id="92cb6-114">यदि परियोजना के लिए केवल एक निधीयन स्रोत है, तो ग्राहक अपने आप निर्धारत हो जाएगा.</span><span class="sxs-lookup"><span data-stu-id="92cb6-114">If there is only one funding source for the project, the customer will be automatically set.</span></span>
- <span data-ttu-id="92cb6-115">**सभी सेल्स ऑर्डर** सूची पृष्ठ पर जाएं और नया सेल्स ऑर्डर बनाएं.</span><span class="sxs-lookup"><span data-stu-id="92cb6-115">Go to the **All sales order** list page and create a new sales order.</span></span> <span data-ttu-id="92cb6-116">आपको सेल्स ऑर्डर के लिए परियोजना चुननी होगी.</span><span class="sxs-lookup"><span data-stu-id="92cb6-116">You will need to select the project for the sales order.</span></span> <span data-ttu-id="92cb6-117">परियोजना चुनने के बाद, ग्राहक को निधीयन स्त्रोत से निर्धारित किया जाएगा या आपको निधीयन स्त्रोत चुनने की ज़रूरत होगी, अगर परियोजना अनुबंध में कई निधीयन स्त्रोत हैं.</span><span class="sxs-lookup"><span data-stu-id="92cb6-117">After the project is selected, the customer will be set from the funding source or you will need to select the funding source if the project contract has multiple funding sources.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]