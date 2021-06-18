---
title: कार्य घंटों का एक टेम्पलेट बनाएँ
description: यह विषय बताता है कि Project Service में कार्य के घंटों का टेम्प्लेट कैसे बनाया जाए.
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: 105e3cb2ef7b904e96dc21013906e0b7444e3b88
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997198"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="ae07d-103">कार्य घंटों का टेम्पलेट बनाना (Project Service)</span><span class="sxs-lookup"><span data-stu-id="ae07d-103">Create a work hours template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="ae07d-104">परियोजना बनाने और प्रबंधित करने के लिए, आपको परियोजना के लिए कैलेंडर टेम्प्लेट लागू करना होगा.</span><span class="sxs-lookup"><span data-stu-id="ae07d-104">To create and manage a project, you must apply a calendar template to the project.</span></span> <span data-ttu-id="ae07d-105">कैलेंडर टेम्पलेट निम्नलिखित परियोजना विशेषताओं को परिभाषित करता है:</span><span class="sxs-lookup"><span data-stu-id="ae07d-105">The calendar template defines the following project attributes:</span></span>

- <span data-ttu-id="ae07d-106">काम के घंटे, शुरूआत और समाप्ति समय सहित</span><span class="sxs-lookup"><span data-stu-id="ae07d-106">Working hours, including start and end time</span></span>
- <span data-ttu-id="ae07d-107">काम के दिन</span><span class="sxs-lookup"><span data-stu-id="ae07d-107">Working days</span></span>
- <span data-ttu-id="ae07d-108">कैलेंडर अपवाद जैसे कि गैर-कार्य दिवस</span><span class="sxs-lookup"><span data-stu-id="ae07d-108">Calendar exceptions such as non-working days</span></span>

<span data-ttu-id="ae07d-109">कैलेंडर टेम्पलेट जो किसी परियोजना पर लागू होता है, आपके संगठन की सेटिंग में परिभाषित कैलेंडर टेम्पलेट की एक प्रति है.</span><span class="sxs-lookup"><span data-stu-id="ae07d-109">The calendar template that's applied to a project is a copy of the calendar template defined in your organization’s settings.</span></span>

> [!NOTE]
> <span data-ttu-id="ae07d-110">यदि आप कैलेंडर टेम्प्लेट बदलते हैं, तो वे परिवर्तन परियोजना के काम के घंटों के लिए प्रचारित नहीं होते हैं.</span><span class="sxs-lookup"><span data-stu-id="ae07d-110">If you change the calendar template, those changes don't propagate to the working hours of the project.</span></span> <span data-ttu-id="ae07d-111">परियोजना के काम के घंटे बदलने के लिए, एक नया टेम्पलेट लागू किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="ae07d-111">To change the working hours of the project, a new template must be applied.</span></span>

<span data-ttu-id="ae07d-112">अपने संगठन के लिए एक कैलेंडर टेम्प्लेट बनाने के लिए, दो मुख्य आवश्यकताएं हैं:</span><span class="sxs-lookup"><span data-stu-id="ae07d-112">To create a calendar template for your organization, there are two key requirements:</span></span>

- <span data-ttu-id="ae07d-113">एक नए या मौजूदा बुक करने योग्य संसाधन का उपयोग करके टेम्पलेट के वांछित कार्य घंटों को परिभाषित करें.</span><span class="sxs-lookup"><span data-stu-id="ae07d-113">Define the desired working hours of the template using a new or existing bookable resource.</span></span>
- <span data-ttu-id="ae07d-114">एक नया कैलेंडर टेम्प्लेट बनाएं और टेम्पलेट को बुक करने योग्य संसाधन के साथ जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="ae07d-114">Create a new calendar template and associate the template with the bookable resource.</span></span>

<span data-ttu-id="ae07d-115">**टेम्पलेट के काम के घंटे निर्धारित करें**</span><span class="sxs-lookup"><span data-stu-id="ae07d-115">**Define the working hours of the template**</span></span>

1. <span data-ttu-id="ae07d-116">**संसाधन** \> **संसाधन** पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="ae07d-116">Go to **Resources** \> **Resources**.</span></span>
2. <span data-ttu-id="ae07d-117">कैलेंडर टेम्पलेट में संदर्भ के लिए एक नया संसाधन बनाएं, या किसी मौजूदा संसाधन का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="ae07d-117">Create a new resource to reference in the calendar template, or select an existing resource.</span></span>
3. <span data-ttu-id="ae07d-118">संसाधन के **कार्य के घंटे** टैब का चयन करें और कैलेंडर नियमों को कॉन्फ़िगर करने के लिए [संसाधन के लिए काम के घंटे निर्धारित करें](/dynamics365/field-service/set-work-hours-resource.md) में दिए गए निर्देशों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="ae07d-118">Select the **Work Hours** tab of the resource and complete the instructions in [Set work hours for a resource](/dynamics365/field-service/set-work-hours-resource.md) to configure the calendar rules.</span></span>

<span data-ttu-id="ae07d-119">**नया कैलेंडर टेम्पलेट बनाये**</span><span class="sxs-lookup"><span data-stu-id="ae07d-119">**Create a new calendar template**</span></span>

1. <span data-ttu-id="ae07d-120">**सेटिंग्स** \> **कैलेंडर टेम्पलेट** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="ae07d-120">Go to **Settings** \> **Calendar Template**.</span></span>
2. <span data-ttu-id="ae07d-121">**नया** चुनें, और एक नाम, विवरण और टेम्पलेट संसाधन दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="ae07d-121">Select **New**, and enter a name, description, and template resource.</span></span>


> [!NOTE]
> <span data-ttu-id="ae07d-122">जब किसी संसाधन को कैलेंडर टेम्पलेट में संदर्भित किया जाता है, तो संसाधन के कैलेंडर की एक कॉपी कैलेंडर टेम्पलेट से संबद्ध हो जाती है.</span><span class="sxs-lookup"><span data-stu-id="ae07d-122">When a resource is referenced in a calendar template, a copy of the resource’s calendar is associated with the calendar template.</span></span> <span data-ttu-id="ae07d-123">यदि कॉपी किए गए टेम्प्लेट के काम के घंटे बदल जाते हैं, तो वे परिवर्तन कैलेंडर टेम्प्लेट में प्रचारित नहीं होंगे.</span><span class="sxs-lookup"><span data-stu-id="ae07d-123">If the working hours of the copied template change, those changes will not propagate to the calendar template.</span></span>


### <a name="see-also"></a><span data-ttu-id="ae07d-124">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="ae07d-124">See Also</span></span>  
 [<span data-ttu-id="ae07d-125">संसाधन सेट अप करें</span><span class="sxs-lookup"><span data-stu-id="ae07d-125">Set up resources</span></span>](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
