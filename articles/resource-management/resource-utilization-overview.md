---
title: संसाधन उपयोग अवलोकन
description: इस विषय में Project Operations में संसाधन उपयोग के बारे में जानकारी दी गई है.
author: ruhercul
manager: Annbe
ms.date: 11/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 8b85464dbb68523b122116225a604f67e7236f3e
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401378"
---
# <a name="resource-utilization-overview"></a><span data-ttu-id="8750c-103">संसाधन उपयोग अवलोकन</span><span class="sxs-lookup"><span data-stu-id="8750c-103">Resource utilization overview</span></span>

<span data-ttu-id="8750c-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="8750c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8750c-105">संसाधनों का लक्षित बिलेबल उपयोग हो सकता है।</span><span class="sxs-lookup"><span data-stu-id="8750c-105">Resources can have a target billable utilization.</span></span> <span data-ttu-id="8750c-106">इस लक्षित उपयोग को संसाधन की डिफ़ॉल्ट भूमिका में विशेषता के रूप में परिभाषित किया जाता है या व्यक्तिगत बुक करने योग्य संसाधन के रिकॉर्ड पर सेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8750c-106">This target utilization is defined as an attribute on a resource's default role or set on the record of the individual bookable resource.</span></span> <span data-ttu-id="8750c-107">उपयोगिता की गणनाएं संसाधनों द्वारा की गई अनुमोदित समय संबंधी प्रविष्टियों का उपयोग कर रिपोर्ट की जाती हैं।</span><span class="sxs-lookup"><span data-stu-id="8750c-107">Utilization calculations are based on the actual hours that resources have reported by using approved time entries.</span></span>

<span data-ttu-id="8750c-108">उपयोगिता की गणना के लिए निम्न सूत्र उपयोग किये जाते हैं:</span><span class="sxs-lookup"><span data-stu-id="8750c-108">The following formulas are used to calculate utilization:</span></span>

  - <span data-ttu-id="8750c-109">बिलेबल उपयोगिता = वास्तविक चार्जेबल घंटे ÷ संसाधन की क्षमता</span><span class="sxs-lookup"><span data-stu-id="8750c-109">Billable utilization = Chargeable actual hours ÷ Resource capacity</span></span>
  - <span data-ttu-id="8750c-110">गैर-बिलेबल उपयोगिता = बिलिंग टाइप आईडी सहित वास्तविक समय = गैर-बिलेबल, पूरक, या उपलब्ध नहीं ÷ संसाधन की क्षमता</span><span class="sxs-lookup"><span data-stu-id="8750c-110">Non-billable utilization = Actual time with billing type ID = Non-chargeable, Complementary, or Not available ÷ Resource capacity</span></span>
  - <span data-ttu-id="8750c-111">आंतरिक = बिना बिक्री अनुबंध के लगाया गया वास्तविक समय ÷ संसाधन की क्षमता</span><span class="sxs-lookup"><span data-stu-id="8750c-111">Internal = Actual time with no sales contract ÷ Resource capacity</span></span>
  - <span data-ttu-id="8750c-112">संसाधन की क्षमता = संसाधन का कार्य समय - कार्यालय से बाहर समय - गैर-कार्य दिवस</span><span class="sxs-lookup"><span data-stu-id="8750c-112">Resource capacity = Resource work hours – Out-of-office – Non-working days</span></span>

<span data-ttu-id="8750c-113">आप **संसाधन उपयोगिता** **Resources** पेन में देख सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="8750c-113">You can find the **Resource Utilization** view in the **Resources** pane.</span></span>

<span data-ttu-id="8750c-114">ग्रिड में प्रत्येक सेल किसी प्रदत्त अवधि जैसे कि एक दिन, सप्ताह या महीने में संसाधन की बिलेबल उपयोगिता प्रतिशत का सूचक है।</span><span class="sxs-lookup"><span data-stu-id="8750c-114">Each cell in the grid represents the billable utilization percentage of the resource in a period, such as a day, week, or month.</span></span> <span data-ttu-id="8750c-115">सेलों को रंगने के लिए निम्न सूत्र उपयोग किए जाते हैं:</span><span class="sxs-lookup"><span data-stu-id="8750c-115">The following formulas are used to color the cells:</span></span>

  - <span data-ttu-id="8750c-116">**हरा**: बिल करने योग्य उपयोग >= संसाधन लक्षित उपयोग</span><span class="sxs-lookup"><span data-stu-id="8750c-116">**Green**: Billable utilization >= Resource target utilization</span></span>
  - <span data-ttu-id="8750c-117">**पीला**: लक्षित उपयोग – 20 <= बिल करने योग्य उपयोग < लक्षित उपयोग</span><span class="sxs-lookup"><span data-stu-id="8750c-117">**Yellow**: Target utilization – 20 <= Billable utilization < Target utilization</span></span>
  - <span data-ttu-id="8750c-118">**लाल**: बिल करने योग्य उपयोग < लक्षित उपयोग – 20</span><span class="sxs-lookup"><span data-stu-id="8750c-118">**Red**: Billable utilization < Target utilization – 20</span></span>

<span data-ttu-id="8750c-119">चूंकि **संसाधन की उपयोगिता** दृश्य शेड्यूल बोर्ड पर आधारित है, आप अपने परिणामों को फ़िल्टर करने के लिए शेड्यूल बोर्ड की फ़िल्टरिंग क्षमताओं का उपयोग कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="8750c-119">Because the **Resource Utilization** view is based on the Schedule Board, you can use the filtering capabilities of the Schedule Board to filter your results.</span></span>

<span data-ttu-id="8750c-120">ग्रिड के लिए वांछित है कि आप रोल या व्यक्तिगत संसाधन पर आधारित लक्षित उपयोगिता सेट करें।</span><span class="sxs-lookup"><span data-stu-id="8750c-120">The grid requires that you set a target utilization on either the role or the individual resource.</span></span> <span data-ttu-id="8750c-121">यह सेटअप करने के लिए, **संसाधन** > **संसाधन भूमिकाएं** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="8750c-121">To do this setup, go to **Resources** > **Resource roles**.</span></span>

<span data-ttu-id="8750c-122">इसके अतिरिक्त प्रत्येक बुक करने योग्य संसाधन के लिए कोई डिफ़ॉल्ट रोल एसाइन किया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="8750c-122">Additionally, a default role must be assigned to each bookable resource.</span></span> <span data-ttu-id="8750c-123">**संसाधन** > **संसाधन** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="8750c-123">Go to **Resources** > **Resources**.</span></span> <span data-ttu-id="8750c-124">**Project Service** टैब पर सत्यापित करें कि संसाधन का रोल परिभाषित किया गया है और यह कि **डिफ़ॉल्ट है** फ़ील्ड को **हां** पर सेट किया गया है.</span><span class="sxs-lookup"><span data-stu-id="8750c-124">On the **Project Service** tab, verify that a resource role is defined, and that the **Is Default** field is set to **Yes**.</span></span> <span data-ttu-id="8750c-125">जहां **डिफ़ॉल्ट है** = **नहीं** है, आप अतिरिक्त भूमिकाएं जोड़ सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="8750c-125">You can add additional roles where **Is Default** = **No**.</span></span> <span data-ttu-id="8750c-126">जिस भूमिका में, जहाँ **डिफ़ॉल्ट है** = **हाँ** है, उसका उपयोग उस भूमिका के लक्ष्य के एवज़ में संसाधन के उपयोग का मूल्यांकन करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8750c-126">The role where the **Is Default** = **Yes** is used to evaluate the resource's utilization against the target for that role.</span></span>

<span data-ttu-id="8750c-127">**Project Service** टैब पर आप जाकर किसी संसाधन के लिए व्यक्तिगत लक्षित उपयोगिता भी सेट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="8750c-127">On the **Project Service** tab, you can also set an individual target utilization for the resource.</span></span> <span data-ttu-id="8750c-128">उस मामले में उपयोगिता की गणना संसाधन के डिफ़ॉल्ट रोल के लक्ष्य के बजाय संसाधन की लक्षित उपयोगिता के आधार पर की जाती है।</span><span class="sxs-lookup"><span data-stu-id="8750c-128">The utilization calculation then uses that target utilization to evaluate the resource's target instead of the target of the resource's default role.</span></span>

<span data-ttu-id="8750c-129">किसी संसाधन के लिए उपयोग तभी दिखाया जाता है, जब ग्रिड में दिखाई गई अवधि के दौरान उस संसाधन ने प्रभार्य समय को स्वीकृति दी हो.</span><span class="sxs-lookup"><span data-stu-id="8750c-129">Utilization is only shown for a resource if that resource has approved, chargeable time during the period shown in the grid.</span></span>
