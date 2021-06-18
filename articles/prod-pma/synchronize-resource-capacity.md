---
title: संसाधन क्षमता सिंक्रनाइज़ करें
description: यह विषय कैलेंडर और परियोजनाओं में संसाधन की क्षमता को सिंक्रनाइज़ करने के तरीके के बारे में जानकारी देता है.
author: Yowelle
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 8bde3c434680f0651293cbce13ecdce945c3a743
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997513"
---
# <a name="synchronize-resource-capacity"></a><span data-ttu-id="5990f-103">संसाधन क्षमता सिंक्रनाइज़ करें</span><span class="sxs-lookup"><span data-stu-id="5990f-103">Synchronize resource capacity</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="5990f-104">संसाधन सिंक्रनाइज़ेशन की प्रक्रियाएं कैलेंडर और बेस कैलेंडर के लिए जानकारी परियोजना संसाधन शेड्यूलिंग में नीचे भेजने में मदद करने की गारंटी देती हैं.</span><span class="sxs-lookup"><span data-stu-id="5990f-104">The processes for resource synchronization help guarantee that information for the calendar and base calendar trickles down into project resource scheduling.</span></span> <span data-ttu-id="5990f-105">यदि कैलेंडर को बदला जाता है, तो प्रक्रियाएं परियोजना संसाधनों को शेड्यूल करने के लिए ज़रूरी अद्यतन करती हैं.</span><span class="sxs-lookup"><span data-stu-id="5990f-105">If the calendar is changed, the processes make the required updates to the scheduling of project resources.</span></span> <span data-ttu-id="5990f-106">प्रक्रियाएं प्रदर्शन बेहतर बनाने में भी सहायता करती हैं, क्योंकि कैलेंडर की संसाधन जानकारी पहले में सिंक्रनाइज़ की जाती है.</span><span class="sxs-lookup"><span data-stu-id="5990f-106">The processes also help improve performance, because the calendar's resource information is synchronized in advance.</span></span> <span data-ttu-id="5990f-107">इसलिए, संसाधन शेड्यूलिंग जानकारी के अद्यतन ज़्यादा तेज़ी से होते हैं.</span><span class="sxs-lookup"><span data-stu-id="5990f-107">Therefore, updates to resource scheduling information occur more quickly.</span></span> <span data-ttu-id="5990f-108">हम सुझाव देते हैं कि आप एक बार में एक की बजाय बैच के रूप में प्रक्रियाओं को शेड्यूल करें.</span><span class="sxs-lookup"><span data-stu-id="5990f-108">We recommend that you schedule the processes as a batch instead of one at a time.</span></span> <span data-ttu-id="5990f-109">अन्यथा, यहां जोखिम होता है कि कोई व्यक्ति समावेशी तिथियों को भूल जाएगा, जब जानकारी अंतिम बार सिंक्रनाइज़ की गई थी.</span><span class="sxs-lookup"><span data-stu-id="5990f-109">Otherwise, there is a risk that someone will forget the inclusive dates when the information was last synchronized.</span></span> <span data-ttu-id="5990f-110">यदि संयुक्त तिथियों का इस्तेमाल नहीं किया जाता है तो तिथि सिंक्रनाइज़ेशन के दौरान अंतराल हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="5990f-110">If inclusive dates aren't used, gaps can occur during date synchronization.</span></span>

![कैलेंडर सिंक्रनाइज़ेशन](./media/projectresourcing04-1024x471.jpg)

## <a name="synchronize-resource-capacity-roll-ups"></a><span data-ttu-id="5990f-112">एकत्र संसाधन क्षमता को सिंक्रनाइज़ करें</span><span class="sxs-lookup"><span data-stu-id="5990f-112">Synchronize resource capacity roll-ups</span></span>

<span data-ttu-id="5990f-113">सिंक्रनाइज़ेशन प्रक्रिया को सभी संसाधन कैलेंडर जानकारी सिंक्रनाइज़ करने के लिए डिज़ाइन किया गया है.</span><span class="sxs-lookup"><span data-stu-id="5990f-113">The synchronization process is designed to synchronize all resource calendar information.</span></span> <span data-ttu-id="5990f-114">इस जानकारी में परियोजना की संसाधन कैलेंडर क्षमता तालिका में किसी भी बदलाव के बारे में आधार कैलेंडर जानकारी शामिल है.</span><span class="sxs-lookup"><span data-stu-id="5990f-114">This information includes base calendar information about any changes to the project's Resource calendar capacity table.</span></span> <span data-ttu-id="5990f-115">यदि नए संसाधन परियोजना में जोड़े जाते हैं, तो सिंक्रनाइज़ेशन गारंटी देता है कि अद्यतन कैलेंडर जानकारी मौजूद है.</span><span class="sxs-lookup"><span data-stu-id="5990f-115">If new resources are added in the project, synchronization helps guarantee that the updated calendar information is available.</span></span> <span data-ttu-id="5990f-116">यह सिंक्रनाइज़ेशन किसी भी समय किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="5990f-116">This synchronization can be done at any time.</span></span>

<span data-ttu-id="5990f-117">हम सुझाव देते हैं कि आप बैच का इस्तेमाल करें.</span><span class="sxs-lookup"><span data-stu-id="5990f-117">We recommend that you use a batch.</span></span> <span data-ttu-id="5990f-118">क्षमता आरक्षण के सिंक्रनाइज़ेशन के दौरान विकल्प मौजूद हैं.</span><span class="sxs-lookup"><span data-stu-id="5990f-118">The options are available during synchronization of capacity reservations.</span></span>

1. <span data-ttu-id="5990f-119">चुनते हैं **परियोजना प्रबंधन और लेखांकन** &gt; **आवधिक** &gt; **क्षमता सिंक्रनाइज़ेशन** &gt; **एकत्र संसाधन क्षमता को सिंक्रनाइज़ करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="5990f-119">Select **Project management and accounting** &gt; **Periodic** &gt; **Capacity synchronization** &gt; **Synchronize resources capacity roll-ups**.</span></span>
2. <span data-ttu-id="5990f-120">निम्नलिखित तालिका में विकल्प निर्धारित करें.</span><span class="sxs-lookup"><span data-stu-id="5990f-120">Set the options in the following table.</span></span>

    | <span data-ttu-id="5990f-121">विकल्प</span><span class="sxs-lookup"><span data-stu-id="5990f-121">Option</span></span>      | <span data-ttu-id="5990f-122">वर्णन</span><span class="sxs-lookup"><span data-stu-id="5990f-122">Description</span></span> |
    |-------------|-------------|
    | <span data-ttu-id="5990f-123">अवधि कोड</span><span class="sxs-lookup"><span data-stu-id="5990f-123">Period code</span></span> | <span data-ttu-id="5990f-124">विकल्प रूप से संसाधन क्षमता एकत्र करने के लिए सिंक्रनाइज़ेशन प्रक्रिया की आरंभ और समाप्ति तिथि निर्धारित करने के लिए प्रधान खाता-बही तिथि अंतराल कोड चुनें.</span><span class="sxs-lookup"><span data-stu-id="5990f-124">Optionally select the General ledger date interval code to set the start and end dates for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="5990f-125">प्रारंभ तिथि</span><span class="sxs-lookup"><span data-stu-id="5990f-125">Start date</span></span>  | <span data-ttu-id="5990f-126">संसाधन क्षमता एकत्र करने के लिए सिंक्रनाइज़ेशन प्रक्रिया की आरंभ तिथि दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="5990f-126">Enter the start date for the synchronization process for resource capacity roll-ups.</span></span> |
    | <span data-ttu-id="5990f-127">समाप्ति दिनांक</span><span class="sxs-lookup"><span data-stu-id="5990f-127">End date</span></span>    | <span data-ttu-id="5990f-128">संसाधन क्षमता एकत्र करने के लिए सिंक्रनाइज़ेशन प्रक्रिया की समाप्ति तिथि दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="5990f-128">Enter the end date for the synchronization process for resource capacity roll-ups.</span></span> |

<span data-ttu-id="5990f-129">[![सिंक्रनाइज़ेशन प्रक्रिया](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span><span class="sxs-lookup"><span data-stu-id="5990f-129">[![Synchronization process](./media/projectresourcing09.jpg)](./media/projectresourcing09.jpg)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]