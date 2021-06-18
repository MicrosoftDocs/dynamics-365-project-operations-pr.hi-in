---
title: परियोजना कैलेंडर परिभाषित करें
description: यह विषय परियोजना शेड्यूल को ट्रैक करने के लिए किसी परियोजना के लिए कैलेंडर टेम्पलेट को कैसे लागू करें, इसके बारे में जानकारी प्रदान करता है.
author: ruhercul
ms.date: 02/05/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: ruhercul
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 0d1a2c4bd2d4022bbf79afcef79170eb482e6418
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5998998"
---
# <a name="define-project-calendars"></a><span data-ttu-id="7c19e-103">परियोजना कैलेंडर परिभाषित करें</span><span class="sxs-lookup"><span data-stu-id="7c19e-103">Define project calendars</span></span>

<span data-ttu-id="7c19e-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="7c19e-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="7c19e-105">परियोजना बनाने और प्रबंधित करने के लिए, आपको परियोजना के लिए कैलेंडर टेम्प्लेट लागू करना होगा.</span><span class="sxs-lookup"><span data-stu-id="7c19e-105">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="7c19e-106">कैलेंडर टेम्पलेट निम्नलिखित परियोजना विशेषताओं को परिभाषित करता है:</span><span class="sxs-lookup"><span data-stu-id="7c19e-106">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="7c19e-107">काम के घंटे, शुरूआत और समाप्ति समय सहित</span><span class="sxs-lookup"><span data-stu-id="7c19e-107">Working hours, including start and end time</span></span>
- <span data-ttu-id="7c19e-108">काम के दिन</span><span class="sxs-lookup"><span data-stu-id="7c19e-108">Working days</span></span>
- <span data-ttu-id="7c19e-109">कैलेंडर अपवाद जैसे कि गैर-कार्य दिवस</span><span class="sxs-lookup"><span data-stu-id="7c19e-109">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="7c19e-110">कैलेंडर टेम्पलेट जो किसी परियोजना पर लागू होता है, आपके संगठन की सेटिंग में परिभाषित कैलेंडर टेम्पलेट की एक प्रति है.</span><span class="sxs-lookup"><span data-stu-id="7c19e-110">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="7c19e-111">यदि आप कैलेंडर टेम्प्लेट बदलते हैं, तो वे परिवर्तन परियोजना के काम के घंटों के लिए प्रचारित नहीं होते हैं.</span><span class="sxs-lookup"><span data-stu-id="7c19e-111">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="7c19e-112">परियोजना के काम के घंटे बदलने के लिए, एक नया टेम्पलेट लागू किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="7c19e-112">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="7c19e-113">अपने संगठन के लिए एक कैलेंडर टेम्प्लेट बनाने के लिए, दो मुख्य आवश्यकताएं हैं:</span><span class="sxs-lookup"><span data-stu-id="7c19e-113">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="7c19e-114">एक नए या मौजूदा बुक करने योग्य संसाधन का उपयोग करके टेम्पलेट के वांछित कार्य घंटों को परिभाषित करें.</span><span class="sxs-lookup"><span data-stu-id="7c19e-114">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="7c19e-115">एक नया कैलेंडर टेम्प्लेट बनाएं और टेम्पलेट को बुक करने योग्य संसाधन के साथ जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="7c19e-115">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="7c19e-116">**टेम्पलेट के काम के घंटे निर्धारित करें**</span><span class="sxs-lookup"><span data-stu-id="7c19e-116">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="7c19e-117">**संसाधन** \> **संसाधन** पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="7c19e-117">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="7c19e-118">कैलेंडर टेम्पलेट में संदर्भ के लिए एक नया संसाधन बनाएं, या किसी मौजूदा संसाधन का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="7c19e-118">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="7c19e-119">संसाधन के **कार्य के घंटे** टैब का चयन करें और कैलेंडर नियमों को कॉन्फ़िगर करने के लिए [संसाधन के लिए काम के घंटे निर्धारित करें](/dynamics365/field-service/set-work-hours-resource.md) में दिए गए निर्देशों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="7c19e-119">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](/dynamics365/field-service/set-work-hours-resource.md) to configure the calendar rules.</span></span>

<span data-ttu-id="7c19e-120">**नया कैलेंडर टेम्पलेट बनाये**</span><span class="sxs-lookup"><span data-stu-id="7c19e-120">**Create a new calendar template**</span></span>

1. <span data-ttu-id="7c19e-121">**सेटिंग्स** \> **कैलेंडर टेम्पलेट** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="7c19e-121">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="7c19e-122">**नया** चुनें, और एक नाम, विवरण और टेम्पलेट संसाधन दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="7c19e-122">Select **New**, and enter a name, description, and template resource.</span></span>

> [!NOTE]
> <span data-ttu-id="7c19e-123">जब किसी संसाधन को कैलेंडर टेम्पलेट में संदर्भित किया जाता है, तो संसाधन के कैलेंडर की एक कॉपी कैलेंडर टेम्पलेट से संबद्ध हो जाती है.</span><span class="sxs-lookup"><span data-stu-id="7c19e-123">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="7c19e-124">यदि कॉपी किए गए टेम्प्लेट के काम के घंटे बदल जाते हैं, तो वे परिवर्तन कैलेंडर टेम्प्लेट में प्रचारित नहीं होंगे.</span><span class="sxs-lookup"><span data-stu-id="7c19e-124">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>

<span data-ttu-id="7c19e-125">अब आप वर्क टैम्पलेट को प्रोजेक्ट कैलेंडर के टैम्पलेट से जोड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="7c19e-125">You can now associate the work template with a project calendar template.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]

