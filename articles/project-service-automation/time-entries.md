---
title: समय प्रविष्टि बनाएँ
description: इस टॉपिक में टाइम एंट्री बनाने के बारे में जानकारी प्रदान की गई है।
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 05/20/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: 90f6450b-e0c4-4d86-b8f5-ffb1a2b1e38a
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: ae3af7d62d93884c7fa9881394b7129daeb8bf7e
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3752058"
---
# <a name="create-time-entries"></a><span data-ttu-id="83dbc-103">समय प्रविष्टि बनाएँ</span><span class="sxs-lookup"><span data-stu-id="83dbc-103">Create time entries</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="83dbc-104">Dynamics 365 Project Service Automation के पिछले संस्करणों में टाइम एंट्री साप्ताहिक आधार पर दर्ज की जाती थीं।</span><span class="sxs-lookup"><span data-stu-id="83dbc-104">In previous versions of Dynamics 365 Project Service Automation, time entries were entered on a weekly basis.</span></span> <span data-ttu-id="83dbc-105">Project Service Automation के संस्करण 3 में टाइम एंट्री दैनिक आधार पर दर्ज की जाती हैं।</span><span class="sxs-lookup"><span data-stu-id="83dbc-105">In version 3 of Project Service Automation, time entries are entered on a daily basis.</span></span> <span data-ttu-id="83dbc-106">हालाँकि कुछ बार टाइम एंट्री करने के बाद आप उन्हें बल्क में बना सकते हैं या फिर कॉपी कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="83dbc-106">However, after a few time entries have been created, you can bulk create or copy them.</span></span>

## <a name="create-a-time-entry"></a><span data-ttu-id="83dbc-107">टाइम एंट्री बनाएँ</span><span class="sxs-lookup"><span data-stu-id="83dbc-107">Create a time entry</span></span>

<span data-ttu-id="83dbc-108">टाइम एंट्री बनाने के लिए इन चरणों का पालन करें।</span><span class="sxs-lookup"><span data-stu-id="83dbc-108">Follow these steps to create a time entry.</span></span>

1. <span data-ttu-id="83dbc-109">**टाइम एंट्री** पृष्ठ पर **नया** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="83dbc-109">On the **Time Entries** page, select **New**.</span></span>
2. <span data-ttu-id="83dbc-110">**तुरंत बनाएं: टाइम एंट्री** डायलॉग बॉक्स में टाइम एंट्री को मिनट, घंटे या दिनों के हिसाब से दर्ज करें।</span><span class="sxs-lookup"><span data-stu-id="83dbc-110">In the **Quick Create: Time Entry** dialog box, enter the duration of the time entry in minutes, hours, or days.</span></span> <span data-ttu-id="83dbc-111">अवधि को इस फॉर्मेट में दर्ज किया जाना चाहिए: *x* मिनट, *x* घंटे, या *x* दिन।</span><span class="sxs-lookup"><span data-stu-id="83dbc-111">The duration must be entered in the following format: *x* minutes, *x* hours, or *x* days.</span></span> <span data-ttu-id="83dbc-112">घंटों और दिनों को डेसिमल मानों के रूप में भी दर्ज किया जा सकता है जैसे *x।x* घंटे या *x।x* दिन।</span><span class="sxs-lookup"><span data-stu-id="83dbc-112">Hours and days can also be entered as decimal values, such as *x.x* hours or *x.x* days.</span></span>
3. <span data-ttu-id="83dbc-113">टाइम एंट्री और उस परियोजना, जिसके लिए और टाइम एंट्री कर रहे हैं, का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="83dbc-113">Select the type of time entry and the project that you're entering the time entry for.</span></span>
4. <span data-ttu-id="83dbc-114">**परियोजना कार्य** फ़ील्ड में इस टाइम एंट्री के लिए कार्य खोजें।</span><span class="sxs-lookup"><span data-stu-id="83dbc-114">In the **Project Task** field, find the task for this time entry.</span></span>

    > [!NOTE]
    > <span data-ttu-id="83dbc-115">यदि आप किसी ऐसे कार्य के लिए टाइम एंट्री बना रहे हैं जो किसी यूज़र को एसाइन नहीं किया गया है तो **परियोजना कार्य** फ़ील्ड में **खोजें** बटन का चयन करें, **दृश्य बदलें** चुनें और फिर सभी कार्यों की सूची बनाने के लिए **सभी सक्रिय परियोजना कार्य** चुनें।</span><span class="sxs-lookup"><span data-stu-id="83dbc-115">If you're creating a time entry for a task that isn't assigned to a user, in the **Project Task** field, select the **Search** button, select **Change View**, and then select **All Active Project Tasks** to list all tasks.</span></span>

5. <span data-ttu-id="83dbc-116">यदि कोई विवरण आवश्यक है तो इसे दर्ज करें और फिर **सेव करें और बंद करें** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="83dbc-116">Enter a description, if a description is required, and then select **Save and Close**.</span></span>

<span data-ttu-id="83dbc-117">टाइम एंट्री के बनने और सेव होने के बाद आप इसे टाइम एंट्री ग्रिड में एडिट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="83dbc-117">After the time entry is created and saved, you can edit it in the time entry grid.</span></span> <span data-ttu-id="83dbc-118">टाइम एंट्री ग्रिड दो फॉर्मेट का समर्थन करती है:</span><span class="sxs-lookup"><span data-stu-id="83dbc-118">The time entry grid supports two formats:</span></span>

- <span data-ttu-id="83dbc-119">आप **hh:mm** फॉर्मेट में टाइम एंट्री दर्ज कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="83dbc-119">You can enter time entries in **hh:mm** format.</span></span> <span data-ttu-id="83dbc-120">फिर इस फॉर्मेट को फिर घंटों और फ्रैक्शन में परिवर्तित किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="83dbc-120">This format is then converted to hours and fractions.</span></span>
- <span data-ttu-id="83dbc-121">आप सीधे ही घंटे और फ्रैक्शन दर्ज कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="83dbc-121">You can enter hours and fractions directly.</span></span>

<span data-ttu-id="83dbc-122">ध्यान दें कि घंटे की फ्रैक्शन का अर्थ मिनट नहीं है।</span><span class="sxs-lookup"><span data-stu-id="83dbc-122">Note that the fractions of an hour aren't minutes.</span></span> <span data-ttu-id="83dbc-123">इसलिए 1.5 घंटे का अर्थ है 1 घंटा और 30 मिनट।</span><span class="sxs-lookup"><span data-stu-id="83dbc-123">Therefore, 1.5 hours represents 1 hour and 30 minutes.</span></span> <span data-ttu-id="83dbc-124">यही नियम किसी दिन की फ्रैक्शन पर लागू होता है।</span><span class="sxs-lookup"><span data-stu-id="83dbc-124">The same rule applies to fractions of a day.</span></span> <span data-ttu-id="83dbc-125">एक दिन का अर्थ है 24 घंटे, और 0.5 दिन का अर्थ है 12 घंटे।</span><span class="sxs-lookup"><span data-stu-id="83dbc-125">One day is 24 hours, and 0.5 days represents 12 hours.</span></span>

## <a name="bulk-create-time-entries"></a><span data-ttu-id="83dbc-126">बल्क में टाइम एंट्री बनाएँ</span><span class="sxs-lookup"><span data-stu-id="83dbc-126">Bulk create time entries</span></span>

<span data-ttu-id="83dbc-127">कुछेक बार टाइम एंट्री करने के बाद आप उन्हें बल्क में बनाने के लिए उन्हें कॉपी कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="83dbc-127">After a few time entries have been created, you can copy them to create additional time entries in bulk.</span></span>

1. <span data-ttu-id="83dbc-128">**टाइम एंट्री** पृष्ठ पर **सप्ताह को कॉपी करें** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="83dbc-128">On the **Time Entries** page, select **Copy Week**.</span></span>
2. <span data-ttu-id="83dbc-129">**अवधि से** फ़ील्ड समूह में **प्रारंभ दिनांक** और **समाप्ति दिनांक** फ़ील्ड में वे तिथियां स्पेसिफाई करें, जिनके लिए टाइम एंट्री कॉपी करना चाहहते हैं।</span><span class="sxs-lookup"><span data-stu-id="83dbc-129">In the **From Period** field group, in the **Start Date** and **End Date** fields, define the date range to copy time entries from.</span></span>
3. <span data-ttu-id="83dbc-130">**अवधि से** फ़ील्ड समूह में **प्रारंभ दिनांक** फ़ील्ड में वे तिथि स्पेसिफाई करें जिसके लिए एंट्री कॉपी करना चाहते हैं।</span><span class="sxs-lookup"><span data-stu-id="83dbc-130">In the **To Period** field group, in the **Start Date** field, specify the date to create time entries for.</span></span>
4. <span data-ttu-id="83dbc-131">**कॉपी** का चयन कर उन टाइम एंट्री की कॉपी करें जो **अवधि तक** फ़ील्ड समूह में सप्ताह के स्पेसिफाई किये गए दिन के अनुरूप है।</span><span class="sxs-lookup"><span data-stu-id="83dbc-131">Select **Copy** to create a copy of the time entries that correspond to the day of the week that is specified in the **To Period** field group.</span></span> <span data-ttu-id="83dbc-132">उदाहरण के लिए पिछले सप्ताह के सोमवार की टाइम एंट्री को उस सप्ताह के सोमवार में कॉपी किया जाता है जिसे **अवधि तक** फ़ील्ड समूह में स्पेसिफाई किया गया है।</span><span class="sxs-lookup"><span data-stu-id="83dbc-132">For example, the time entry for Monday of last week is copied to Monday of the week that is specified in the **To Period** field group.</span></span>

## <a name="import-data-for-time-entries"></a><span data-ttu-id="83dbc-133">टाइम एंट्री के लिए डेटा इम्पोर्ट करें</span><span class="sxs-lookup"><span data-stu-id="83dbc-133">Import data for time entries</span></span>

<span data-ttu-id="83dbc-134">आप परियोजना बुकिंग और एसाइनमेंट से डेटा इम्पोर्ट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="83dbc-134">You can import data from project bookings and assignments.</span></span> <span data-ttu-id="83dbc-135">डेटा इम्पोर्ट करते समय आप इम्पोर्ट करने के लिए बुकिंग की तिथि का रेंज स्पेसिफाई कर उन बुकिंग को स्पष्ट रूप से चुन सकते हैं, जिन्हें **ड्राफ्ट** टाइम एंट्री के तौर पर बनाया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="83dbc-135">When you import data, you can specify the date range of the bookings to import and then explicitly select the bookings that should be created as **Draft** time entries.</span></span>

## <a name="group-by-sort-search-and-filter-capabilities"></a><span data-ttu-id="83dbc-136">के लिहाज़ से समूह बनाएं, सॉर्ट करें, खोज और फ़िल्टरिंग की क्षमताएं</span><span class="sxs-lookup"><span data-stu-id="83dbc-136">Group by, sort, search, and filter capabilities</span></span>

<span data-ttu-id="83dbc-137">आप कॉलम में स्पेसिफाई किये गए आयामों के लिहाज़ से टाइम एंट्री का समूह बना सकते हैं और उन्हें फ़िल्टर कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="83dbc-137">You can group and filter time entries by the dimensions that are specified in the columns.</span></span> <span data-ttu-id="83dbc-138">**समूहन फ़ील्ड द्वारा** में, टाइम एंट्री को फ़िल्टर करने के लिए उपयोग में लाने वाले आयाम का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="83dbc-138">In the **Group by** field, select the dimension to use to filter time entries.</span></span> <span data-ttu-id="83dbc-139">आप कॉलम हेडिंग पर सॉर्ट एरो का उपयोग कर टाइम एंट्री के रिकॉर्ड को घटते या बढ़ते क्रम में भी सॉर्ट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="83dbc-139">You can also sort the time entry records in ascending or descending order by using the sort arrow on the column headings.</span></span> <span data-ttu-id="83dbc-140">इसके अतिरिक्त आप कॉलम हेडिंग पर **फ़िल्टर** बटन का चयन कर एंट्री को दिखा या छिपा सकते हैं और फिर **खोज करें** बॉक्स में वो टेक्स्ट लिख सकते हैं, जिसे परियोजना के नाम, परियोजना कार्य, टाइम एंट्री या संसाधन के लिहाज़ से खोजने के लिए प्रयोग किया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="83dbc-140">Additionally, you can show or hide entries by selecting the **Filter** button on the column headings, and then, in the **Search** box, entering the text that should be used to search for time entries by project name, project task, time entry, or resource.</span></span>
