---
title: सॉफ़्ट बुक की आवश्यकताएँ
description: इस टॉपिक में सॉफ्ट-बुकिंग की आवश्यकताओं के बारे में जानकारी प्रदान की गई है।
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: bc58c805bfe1a3087600b8d4a6be2d1bcdd18188
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997918"
---
# <a name="soft-book-requirements"></a><span data-ttu-id="b7909-103">सॉफ़्ट बुक की आवश्यकताएँ</span><span class="sxs-lookup"><span data-stu-id="b7909-103">Soft-book requirements</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="b7909-104">किसी संसाधन की आवश्यकता की हार्ड-बुकिंग की जा सकती है।</span><span class="sxs-lookup"><span data-stu-id="b7909-104">A resource requirement can be hard-booked.</span></span> <span data-ttu-id="b7909-105">हार्ड-बुकिंग से किसी संसाधन की क्षमता के उपभोग का प्रस्ताव निर्मित होता है।</span><span class="sxs-lookup"><span data-stu-id="b7909-105">A hard booking creates a proposal that consumes a resource's capacity.</span></span> <span data-ttu-id="b7909-106">इसके बाद प्रस्ताव को अनुमोदन के लिए अनुरोधकर्ता के पास वापस भेजा जाता है।</span><span class="sxs-lookup"><span data-stu-id="b7909-106">The proposal is then sent back to the requester for approval.</span></span> <span data-ttu-id="b7909-107">सॉफ्ट-बुकिंग के मामले में किसी संसाधन को परियोजना टीम में शामिल किया जाता है और शेड्यूल बोर्ड पर एक अलग स्थिति नज़र आती है, लेकिन इससे संसाधन की क्षमता का उपभोग नहीं होता है।</span><span class="sxs-lookup"><span data-stu-id="b7909-107">A soft booking tentatively adds a resource to a project team and has a different status on the Schedule Board, but it doesn't consume the resource's capacity.</span></span> <span data-ttu-id="b7909-108">शेड्यूल बोर्ड से संसाधन की सॉफ्ट-बुकिंग करने के लिए **बुकिंग की स्थिति** फ़ील्ड को **सॉफ्ट** पर सेट करें।</span><span class="sxs-lookup"><span data-stu-id="b7909-108">To soft-book a resource from the Schedule Board, set the **Booking Status** field to **Soft**.</span></span>

![बुकिंग की स्थिति को सॉफ्ट पर सेट किया गया](media/Resource-Management-image77.png)

<span data-ttu-id="b7909-110">जब **टीम** टैब पर **टीम के नामांकित सदस्य** का दृश्य होता है तो संसाधन वहां दिखाई देता है।</span><span class="sxs-lookup"><span data-stu-id="b7909-110">When the **Team** tab is in the **Named Team Members** view, the resource appears there.</span></span> <span data-ttu-id="b7909-111">सॉफ्ट-बुकिंग किये गए घंटे **सॉफ्ट बुकिंग के घंटे** कॉलम में रिपोर्ट किये जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="b7909-111">The soft-booked hours are reported in the **Soft Booked Hours** column.</span></span>

![टीम के नामांकित सदस्य वाले दृश्य में सॉफ्ट-बुकिंग वाले घंटे](media/Resource-Management-image78.png)

<span data-ttu-id="b7909-113">सॉफ्ट- बुकिंग किये गए टीम सदस्यों को कार्य एसाइन किये जा सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="b7909-113">Soft-booked team members can be assigned to tasks.</span></span>

![सॉफ्ट- बुकिंग किये गए टीम सदस्य को कार्य एसाइन किया गया।](media/Resource-Management-image79.png)

<span data-ttu-id="b7909-115">**समाधान** टैब पर सॉफ्ट-बुकिंग वाले संसाधन की कोई बुकिंग नहीं दिखाई जाती है क्योंकि **समाधान** टैब केवल हार्ड-बुकिंग के लिए है।</span><span class="sxs-lookup"><span data-stu-id="b7909-115">On the **Reconciliation** tab, no bookings are shown for a soft-book resource, because the **Reconciliation** tab considers only hard-bookings.</span></span>

![समाधान टैब पर बुकिंग किये बिना सॉफ्ट-बुक हुए संसाधन](media/Resource-Management-image80.png)

> [!NOTE]
> <span data-ttu-id="b7909-117">आप किसी जेनरिक टीम के सदस्य से प्राप्त आवश्यकता से किसी संसाधन की सॉफ्ट-बुकिंग नहीं कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="b7909-117">You can't soft-book a resource from a requirement that was generated from a generic team member.</span></span>

<span data-ttu-id="b7909-118">शेड्यूल बोर्ड पर किसे संसाधन की सॉफ्ट बुकिंग के लिए अलग अलग रंगों का उपयोग किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="b7909-118">On the Schedule Board, a different coloring is used for soft bookings for a resource.</span></span>

![शेड्यूल बोर्ड पर सॉफ्ट बुकिंग](media/Resource-Management-image81.png)

<span data-ttu-id="b7909-120">किसी सॉफ्ट बुकिंग को हार्ड बुकिंग में परिवर्तित करने के लिए शेड्यूल बोर्ड पर मौजूद सॉफ्ट बुकिंग पर राइट-क्लिक करें और उसके बाद **स्थिति बदलें** \> **हार्ड बुकिंग** \> **हार्ड** का चुनाव करें।</span><span class="sxs-lookup"><span data-stu-id="b7909-120">To convert a soft booking to a hard booking, on the Schedule Board, right-click the soft booking, and then select **Change Status** \> **Hard Book** \> **Hard**.</span></span>

![बुकिंग की स्थिति को परिवर्तित कर हार्ड करना](media/Resource-Management-image82.png)

<span data-ttu-id="b7909-122">बुकिंग परिवर्तित हो जाती है और शेड्यूल बोर्ड पर स्थिति में बदलाव आ जाता है।</span><span class="sxs-lookup"><span data-stu-id="b7909-122">The booking is changed, and the status is changed on the Schedule Board.</span></span> <span data-ttu-id="b7909-123">क्योंकि बुकिंग की स्थिति अब **हार्ड** हो चुकी है, संसाधन को बुक हुआ दिखाया जाता है और उसकी क्षमता और उपलब्धता को एडजस्ट किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="b7909-123">Because the booking status is now **Hard**, the resource is shown as booked, and its capacity and availability are adjusted.</span></span>

<span data-ttu-id="b7909-124">आप शेड्यूल बोर्ड से किसी हार्ड बुकिंग या सॉफ्ट बुकिंग को रद्द करने के लिए इसी विधि का उपयोग कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="b7909-124">You can use the same method to cancel a hard booking or a soft booking from the Schedule Board.</span></span>

<span data-ttu-id="b7909-125">परियोजना के **टीम** टैब पर सॉफ्ट-बुकिंग हुए संसाधन को हार्ड- बुकिंग वाला बनाने के लिए संसाधन का चुनाव कर **पुष्टि करें** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="b7909-125">To convert a resource that is soft-booked to hard-booked on the project's **Team** tab, select the resource, and then select **Confirm**.</span></span>

![कमांड की पुष्टि करें](media/Resource-Management-image83.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]