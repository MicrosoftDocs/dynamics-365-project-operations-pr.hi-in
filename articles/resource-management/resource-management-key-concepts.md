---
title: संसाधन प्रबंधन की प्रमुख अवधारणाएं
description: यह विषय Microsoft Dynamics परियोजना संचालन में संसाधन प्रबंधन क्षमताओं के बारे में जानकारी देता है।
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: bcdfc7296ec09421668673d8502e7103c887d667
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279500"
---
# <a name="resource-management-key-concepts"></a><span data-ttu-id="e476f-103">संसाधन प्रबंधन की प्रमुख अवधारणाएं</span><span class="sxs-lookup"><span data-stu-id="e476f-103">Resource management key concepts</span></span>

<span data-ttu-id="e476f-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="e476f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e476f-105">रिसोर्स सेवा आधारित संगठन की सबसे महत्वपूर्ण परिसंपत्ति होते हैं।</span><span class="sxs-lookup"><span data-stu-id="e476f-105">Resources are the most important asset of a service-based organization.</span></span> <span data-ttu-id="e476f-106">सही समय पर सही रिसोर्स का पता लगाने की योग्यता, प्रोजेक्ट में ऐसे रिसोर्स को बुक करने और उनका उपयोग करते रहने से संगठन को अपने राजस्व लक्ष्यों और ग्राहक तुष्टिकरण के लक्ष्यों को प्राप्त करने में मदद मिलती है।</span><span class="sxs-lookup"><span data-stu-id="e476f-106">The ability to find the right resources at the right time, book those resources on projects and keep them utilized, helps the organization meet revenue targets and customer satisfaction goals.</span></span> <span data-ttu-id="e476f-107">आप निम्नलिखित कार्य करने के लिए Dynamics 365 Project Operations में रिसोर्सिंग कार्यक्षमता का उपयोग कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="e476f-107">You can use the project resourcing functionality in Dynamics 365 Project Operations to do the following tasks:</span></span>

- <span data-ttu-id="e476f-108">उपलब्ध और योग्य रिसोर्स को बुक करते हुए प्रोजेक्ट टीम बनाना।</span><span class="sxs-lookup"><span data-stu-id="e476f-108">Form project teams by booking available and qualified resources.</span></span>
- <span data-ttu-id="e476f-109">सामान्य टीम सदस्य रिकार्ड बनाना और उनकी भूमिका तथा रिसोर्स ऑर्गेनाज़ेशनल यूनिट तय करना।</span><span class="sxs-lookup"><span data-stu-id="e476f-109">Create generic team member records and define their roles and resource organization unit.</span></span>
- <span data-ttu-id="e476f-110">सामान्य टीम सदस्यों के लिए उनके टास्क असाइनमेंट से रिसोर्स की आवश्यकता बनाना।</span><span class="sxs-lookup"><span data-stu-id="e476f-110">Generate resource requirements for generic team members from their task assignments.</span></span>
- <span data-ttu-id="e476f-111">उपलब्ध संसाधन कौशलों के समक्ष रिसोर्स की मांग पर निर्धारित कौशल की पहचान करते हुए कौशल का मेल करना।</span><span class="sxs-lookup"><span data-stu-id="e476f-111">Match skills by identifying the skills defined on the resource demand against available resource skills.</span></span>
- <span data-ttu-id="e476f-112">संसाधनों को प्रतिस्थापित करना।</span><span class="sxs-lookup"><span data-stu-id="e476f-112">Substitute resources.</span></span>
- <span data-ttu-id="e476f-113">प्रोजेक्ट शेड्यूल असाइनमेंट और संसाधन बुकिंग संरेखित करें.</span><span class="sxs-lookup"><span data-stu-id="e476f-113">Align project schedule assignments and resource bookings.</span></span>
- <span data-ttu-id="e476f-114">बुकिंग और कार्य में अंतर सामंजस्य.</span><span class="sxs-lookup"><span data-stu-id="e476f-114">Reconcile differences in bookings and assignments.</span></span>
- <span data-ttu-id="e476f-115">कार्यालय के बाहर की स्थिति के जवाब में संसाधन बुकिंग बदलें।</span><span class="sxs-lookup"><span data-stu-id="e476f-115">Change resource bookings in response to out-of-office status.</span></span>
- <span data-ttu-id="e476f-116">प्रोजेक्ट प्रबंधकों और संसाधन प्रबंधकों के बीच सहयोग करें.</span><span class="sxs-lookup"><span data-stu-id="e476f-116">Collaborate between project managers and resource managers.</span></span>
- <span data-ttu-id="e476f-117">किसी लक्ष्य के विरुद्ध संसाधन उपयोग का इतिहास देखें, जिसमें यह भी शामिल है कि संसाधनों के समय का उपयोग कैसे किया गया था.</span><span class="sxs-lookup"><span data-stu-id="e476f-117">View the history of resource utilization against a target, including a breakdown of how the resources' time was utilized.</span></span>
- <span data-ttu-id="e476f-118">एक कौशल और प्रवीणता भंडार बनाए रखें.</span><span class="sxs-lookup"><span data-stu-id="e476f-118">Maintain a skills and proficiency repository.</span></span>


<span data-ttu-id="e476f-119">आप परियोजना संचालन में जेनेरिक या नामित संसाधनों की टीम के साथ अपनी परियोजना संचालित कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e476f-119">You can staff your project with a team of generic or named resources in Project Operations.</span></span> <span data-ttu-id="e476f-120">आप टीम के सदस्यों को जोड़ने और असाइन करने और उनकी बुकिंग और असाइनमेंट प्रबंधित करने के लिए विभिन्न विधियों का उपयोग कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e476f-120">You can use various methods to add and assign team members and to manage their bookings and assignments.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]