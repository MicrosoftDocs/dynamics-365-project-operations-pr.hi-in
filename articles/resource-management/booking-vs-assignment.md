---
title: बुकिंग बनाम असाइनमेंट
description: यह विषय संसाधन बुकिंग और संसाधन असाइनमेंट के बीच अंतर की जानकारी देता है.
author: ruhercul
manager: Annbe
ms.date: 10/26/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 8fe6937dfdfe137f28917c16da1d7dc6155284ae
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130220"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="f4796-103">बुकिंग बनाम असाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="f4796-103">Bookings vs assignments</span></span>

<span data-ttu-id="f4796-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="f4796-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="f4796-105">बुकिंग किसी परियोजना के लिए संसाधनों का कठिन या आसान आवंटन है।</span><span class="sxs-lookup"><span data-stu-id="f4796-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="f4796-106">हार्ड बुकिंग किसी संसाधन की क्षमता का उपभोग करते हैं।</span><span class="sxs-lookup"><span data-stu-id="f4796-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="f4796-107">बुकिंग टीमों के लिए संगठनात्मक अवधारणाओं का प्रतिनिधित्व करती हैं ताकि वे समझ सकें कि विभिन्न परियोजनाओं में संसाधन कैसे लगेंगे.</span><span class="sxs-lookup"><span data-stu-id="f4796-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="f4796-108">Dynamics 365 Project Operations बुकिंग को परियोजना-स्तरीय अवधारणा मानता है.</span><span class="sxs-lookup"><span data-stu-id="f4796-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="f4796-109">बुकिंग के विपरीत, असाइनमेंट्स, परियोजना शेड्यूल में परियोजना कार्यों के लिए संसाधनों की प्रतिबद्धता हैं.</span><span class="sxs-lookup"><span data-stu-id="f4796-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="f4796-110">संसाधनों को नाम दिया जा सकता है या वे जेनेरिक हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="f4796-110">The resources can be named or generic.</span></span> 

<span data-ttu-id="f4796-111">आमतौर पर, संसाधन के लिए बुकिंग का योग एक या कई कार्यों में संसाधन के असाइनमेंट के योग को बराबर होगा.</span><span class="sxs-lookup"><span data-stu-id="f4796-111">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="f4796-112">हालाँकि, Project Operations इस समझौते को लागू नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="f4796-112">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="f4796-113">**समायोजन** दृश्य परियोजना प्रबंधक को वे स्थान दिखाता है, जहां संसाधन की बुकिंग और असाइनमेंट सहमत नहीं होते हैं.</span><span class="sxs-lookup"><span data-stu-id="f4796-113">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>
