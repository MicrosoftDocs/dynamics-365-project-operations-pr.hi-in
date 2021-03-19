---
title: बुकिंग बनाम असाइनमेंट
description: यह विषय संसाधन बुकिंग और संसाधन असाइनमेंट के बीच अंतर की जानकारी देता है.
author: ruhercul
manager: Annbe
ms.date: 01/08/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 3aaf8dcbae0a5762879c2b1223eba3bdc33af1a7
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5279905"
---
# <a name="bookings-vs-assignments"></a><span data-ttu-id="9c3ec-103">बुकिंग बनाम असाइनमेंट</span><span class="sxs-lookup"><span data-stu-id="9c3ec-103">Bookings vs assignments</span></span>

<span data-ttu-id="9c3ec-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="9c3ec-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="9c3ec-105">बुकिंग किसी परियोजना के लिए संसाधनों का कठिन या आसान आवंटन है।</span><span class="sxs-lookup"><span data-stu-id="9c3ec-105">Bookings are the hard or soft allocation of resources to a project.</span></span> <span data-ttu-id="9c3ec-106">हार्ड बुकिंग किसी संसाधन की क्षमता का उपभोग करते हैं।</span><span class="sxs-lookup"><span data-stu-id="9c3ec-106">Hard bookings consume a resource's capacity.</span></span> <span data-ttu-id="9c3ec-107">बुकिंग टीमों के लिए संगठनात्मक अवधारणाओं का प्रतिनिधित्व करती हैं ताकि वे समझ सकें कि विभिन्न परियोजनाओं में संसाधन कैसे लगेंगे.</span><span class="sxs-lookup"><span data-stu-id="9c3ec-107">Bookings represent organizational concepts for teams so that they can understand how resources will be engaged across various projects.</span></span> <span data-ttu-id="9c3ec-108">Dynamics 365 Project Operations परियोजना-स्तरीय अवधारणा को बुक करने पर विचार करता है.</span><span class="sxs-lookup"><span data-stu-id="9c3ec-108">Dynamics 365 Project Operations considers bookings a project-level concept.</span></span> 

<span data-ttu-id="9c3ec-109">बुकिंग के विपरीत, असाइनमेंट्स, परियोजना शेड्यूल में परियोजना कार्यों के लिए संसाधनों की प्रतिबद्धता हैं.</span><span class="sxs-lookup"><span data-stu-id="9c3ec-109">Unlike bookings, assignments are the commitment of resources to project tasks in the project schedule.</span></span> <span data-ttu-id="9c3ec-110">संसाधनों को नाम दिया जा सकता है या वे जेनेरिक हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="9c3ec-110">The resources can be named or generic.</span></span>  <span data-ttu-id="9c3ec-111">जब संसाधन आवश्यकता परियोजना कार्य असाइनमेंट्स से उत्पन्न होती है, तो Project Operations संसाधन आवश्यकता विवरण की आकृति बनाने के लिए संसाधन असाइनमेंट की प्रयास आकृति का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="9c3ec-111">When a resource requirement is derived from the project task assignments, Project Operations uses the effort contours of the resources assignment to build the contours of the resource requirement details.</span></span> <span data-ttu-id="9c3ec-112">हालाँकि, संसाधन असाइनमेंट के संदर्भ को कायम नहीं रखा गया है.</span><span class="sxs-lookup"><span data-stu-id="9c3ec-112">However, a refence to the resource assignments isn't maintained.</span></span> <span data-ttu-id="9c3ec-113">संसाधन आवश्यकता से प्राप्त बुकिंग के अद्यतन किसी भी संसाधन असाइनमेंट को अद्यतन नहीं करते हैं.</span><span class="sxs-lookup"><span data-stu-id="9c3ec-113">Updates to the bookings derived from the resource requirement don't update any resource assignments.</span></span>

<span data-ttu-id="9c3ec-114">आमतौर पर, संसाधन के लिए बुकिंग का योग एक या कई कार्यों में संसाधन के असाइनमेंट के योग को बराबर होगा.</span><span class="sxs-lookup"><span data-stu-id="9c3ec-114">Typically, the sum of the bookings for a resource will equal the sum of the resource's assignments across one or many tasks.</span></span> <span data-ttu-id="9c3ec-115">हालाँकि, Project Operations इस समझौते को लागू नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="9c3ec-115">However, Project Operations doesn't enforce this agreement.</span></span> <span data-ttu-id="9c3ec-116">**समायोजन** दृश्य परियोजना प्रबंधक को वे स्थान दिखाता है, जहां संसाधन की बुकिंग और असाइनमेंट सहमत नहीं होते हैं.</span><span class="sxs-lookup"><span data-stu-id="9c3ec-116">The **Reconciliation** view shows the Project manager places where a resource's bookings and assignments don't agree.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]