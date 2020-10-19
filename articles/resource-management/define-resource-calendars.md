---
title: संसाधन कैलेंडरों को परिभाषित करें
description: यह विषय Project Operations में साधनों के लिए काम के घंटे को स्पष्ट करने के तरीके के बारे में जानकारी देता है.
author: ruhercul
manager: Annbe
ms.date: 10/05/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: ab39d7e5dc2d8c01ed49ca0f1a4d1691aaf15637
ms.sourcegitcommit: 396e0fea2f1598a5313cb0128eca4fe0bb5aade9
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961876"
---
# <a name="define-resource-calendars"></a><span data-ttu-id="40c30-103">संसाधन कैलेंडरों को परिभाषित करें</span><span class="sxs-lookup"><span data-stu-id="40c30-103">Define resource calendars</span></span>

<span data-ttu-id="40c30-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="40c30-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="40c30-105">परियोजना पर काम करने वाले प्रत्येक बुक करने योग्य संसाधन में उनकी उपलब्धता को स्पष्ट करने के लिए काम के घंटे का कैलेंडर होना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="40c30-105">Each bookable resource working on a project must have a calendar of working hours to define their availability.</span></span> <span data-ttu-id="40c30-106">किसी संसाधन के लिए कार्य के घंटे को दो तरीकों से परिभाषित किया जा सकता है:</span><span class="sxs-lookup"><span data-stu-id="40c30-106">Workings hours for a resource can be defined in two ways:</span></span> 

   - <span data-ttu-id="40c30-107">संसाधन के लिए व्यक्तिगत कैलेंडर नियमों को स्पष्ट करें</span><span class="sxs-lookup"><span data-stu-id="40c30-107">Define individual calendar rules for a resource</span></span>
   - <span data-ttu-id="40c30-108">संसाधन के लिए मौजूदा कैलेंडर टेम्पलेट लागू करें</span><span class="sxs-lookup"><span data-stu-id="40c30-108">Apply an existing calendar template for the resource</span></span>

## <a name="define-a-resources-working-hours"></a><span data-ttu-id="40c30-109">संसाधन के काम के घंटे स्पष्ट करें</span><span class="sxs-lookup"><span data-stu-id="40c30-109">Define a resource's working hours</span></span>

1. <span data-ttu-id="40c30-110">**संसाधन** मेनू पर, **साधन** चुनें.</span><span class="sxs-lookup"><span data-stu-id="40c30-110">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="40c30-111">ग्रिड दृश्य से, लागू **बुक करने योग्य संसाधन** चुनें.</span><span class="sxs-lookup"><span data-stu-id="40c30-111">From the grid view, select the applicable **Bookable Resource**.</span></span>
3. <span data-ttu-id="40c30-112">**संसाधन विवरण** पृष्ठ पर, **कार्य के घंटे** टैब चुनें. डिफ़ॉल्ट रूप से, बुक करने योग्य संसाधन कैलेंडर संगठन के लिए निर्धारित डिफ़ॉल्ट कार्य घंटे टेम्पलेट के कार्य घंटों के लिए डिफ़ॉल्ट होता है.</span><span class="sxs-lookup"><span data-stu-id="40c30-112">On the **Resource Details** page, select the **Working Hours** tab. By default, the bookable resources calendar defaults to the working hours of the default work hour template that is defined for the organization.</span></span>
4. <span data-ttu-id="40c30-113">काम के घंटों को अद्यतन करने के लिए, परिभाषित किए जाने वाले प्रस्तावित कैलेंडर नियम की प्रारंभ तिथि पर राइट-क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="40c30-113">To update the working hours, right-click on the start date of the proposed calendar rule to be defined.</span></span> <span data-ttu-id="40c30-114">विशेष दिन के लिए श्रृंखला के शेष या पूरे कैलेंडर के लिए कैलेंडर नियम को स्पष्ट करने के लिए कैलेंडर नियम मेनू को इस्तेमाल करें.</span><span class="sxs-lookup"><span data-stu-id="40c30-114">Use the calendar rule menu to define a calendar rule for a specific day, the remainder of the series, or the entire calendar.</span></span>
5. <span data-ttu-id="40c30-115">विकल्प चुने जाने के बाद आप परिभाषित कर सकते/सकती हैं:</span><span class="sxs-lookup"><span data-stu-id="40c30-115">After the option is selected, you can then define:</span></span>

    - <span data-ttu-id="40c30-116">ह्फ़्ते का वह दिन जब काम के घंटे लागू होंगे.</span><span class="sxs-lookup"><span data-stu-id="40c30-116">The day of the week where the working hours will apply.</span></span>
    - <span data-ttu-id="40c30-117">प्रत्येक दिन के भीतर काम करने का समय.</span><span class="sxs-lookup"><span data-stu-id="40c30-117">The working times within each day.</span></span>
    - <span data-ttu-id="40c30-118">कैलेंडर नियम के लिए समय क्षेत्र.</span><span class="sxs-lookup"><span data-stu-id="40c30-118">The time zone for the calendar rule.</span></span>
    - <span data-ttu-id="40c30-119">यदि लागू हो, तो नियम के लिए काम न करने का समय भी निर्दिष्ट किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="40c30-119">If applicable, non-working time can also be specified for the rule.</span></span>

## <a name="applying-a-calendar-template-to-a-resource"></a><span data-ttu-id="40c30-120">किसी संसाधन पर कैलेंडर टेम्पलेट लागू करना</span><span class="sxs-lookup"><span data-stu-id="40c30-120">Applying a calendar template to a resource</span></span>

1. <span data-ttu-id="40c30-121">**संसाधन** मेनू पर, **साधन** चुनें.</span><span class="sxs-lookup"><span data-stu-id="40c30-121">On the **Resources** menu, select **Resources**.</span></span>
2. <span data-ttu-id="40c30-122">ग्रिड दृश्य से, अपडेट करने के लिए 25 **बुक करने योग्य संसाधन** तक का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="40c30-122">From the grid view, select up to 25 **Bookable Resources** to update.</span></span>
3. <span data-ttu-id="40c30-123">**कैलेंडर सेट करें** चुनें और एक संवाद आपको उपलब्ध काम के घंटे के टेम्पलेट्स की सूची के साथ संकेत देगा.</span><span class="sxs-lookup"><span data-stu-id="40c30-123">Select **Set Calendar** and a dialog will prompt you with a list of available work hour templates.</span></span>
4. <span data-ttu-id="40c30-124">आप जिस टेम्पलेट का उपयोग करना चाहते/चाहती हैं, उसे चुनें, और फिर **लागू करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="40c30-124">Select the template you want to use, and then select **Apply**.</span></span>
