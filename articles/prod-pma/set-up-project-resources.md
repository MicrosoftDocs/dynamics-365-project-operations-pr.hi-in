---
title: प्रोजेक्ट संसाधन सेट अप करना
description: यह विषय परियोजना संसाधनों को सेट करने या अनुरोध के बारे में जानकारी प्रदान करता है.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
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
ms.openlocfilehash: 0bf146c3bfb2fd558c471d8a9e980834cb1b87df
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5288741"
---
# <a name="set-up-project-resources"></a><span data-ttu-id="74790-103">प्रोजेक्ट संसाधन सेट अप करना</span><span class="sxs-lookup"><span data-stu-id="74790-103">Set up project resources</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="74790-104">आपको एक कैलेंडर व्यवस्थित करना होगा और इसे किसी कर्मचारी या कामगार के साथ जोड़ना होगा.</span><span class="sxs-lookup"><span data-stu-id="74790-104">You must set up a calendar and associate it with an employee or a worker.</span></span> <span data-ttu-id="74790-105">कैलेंडर का उपयोग परियोजना को शेड्यूल करने तथा उन संसाधनों के कार्य समय के लिए किया जाता है जो परियोजना के लिए आरक्षित होते हैं.</span><span class="sxs-lookup"><span data-stu-id="74790-105">The calendar is used to schedule the project and the working time of the resources that are reserved for the project.</span></span> <span data-ttu-id="74790-106">कैलेंडर व्यवस्थापन के दौरान परियोजना प्रबंधक के द्वारा संसाधन अनुकूलन के भाग के रूप में संसाधन समतलन किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="74790-106">During calendar setup, project managers can do resource leveling as part of resource optimization.</span></span> <span data-ttu-id="74790-107">कैलेंडर शेड्यूल के आधार पर, संसाधनों पर प्रतिबंध लगाया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="74790-107">Based on the calendar schedule, restrictions can be put on resources.</span></span> <span data-ttu-id="74790-108">आप **कैलेंडर** पृष्ठ पर एक कैलेंडर सेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="74790-108">You can set up a calendar on the **Calendars** page.</span></span>

<span data-ttu-id="74790-109">जब आप एक श्रमिक को एक परियोजना संसाधन के रूप में सेट करते हैं, तो आप उन श्रमिकों में से जो कंपनी में काम करते हैं जिनके लिए आप संसाधन सेट कर रहे हैं उन्हें चुन सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="74790-109">When you set up a worker as a project resource, you can select from workers who work in the company that you're setting up resources for.</span></span> <span data-ttu-id="74790-110">वैकल्पिक रूप से, आप अपने संगठन में अन्य कंपनियों से श्रमिकों का चयन कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="74790-110">Alternatively, you can select workers from other companies in your organization.</span></span> <span data-ttu-id="74790-111">इन श्रमिकों को कंपनियों के बीच के संसाधन के रूप में जाना जाता है.</span><span class="sxs-lookup"><span data-stu-id="74790-111">These workers are known as intercompany resources.</span></span>

<span data-ttu-id="74790-112">निम्नलिखित प्रक्रियाएं समझाती हैं कि आपकी कंपनी में एक परियोजना संसाधन के रूप में एक श्रमिक को कैसे सेट किया जाए और कंपनियों के बीच के एक परियोजना संसाधन को कैसे सेट किया जाए.</span><span class="sxs-lookup"><span data-stu-id="74790-112">The following procedures explain how to set up a worker as a project resource in your company and how to set up an intercompany project resource.</span></span>

## <a name="set-up-a-worker-as-a-project-resource"></a><span data-ttu-id="74790-113">एक परियोजना संसाधन के रूप में एक श्रमिक को सेट करें</span><span class="sxs-lookup"><span data-stu-id="74790-113">Set up a worker as a project resource</span></span>

1. <span data-ttu-id="74790-114">**श्रमिक** पृष्ठ पर, **श्रमिक** सूची में, उस श्रमिक का चयन करें जिसे आप एक परियोजना संसाधन के रूप में जोड़ रहे हैं, और श्रमिक रिकॉर्ड खोलें.</span><span class="sxs-lookup"><span data-stu-id="74790-114">On the **Workers** page, in the **Workers** list, select the worker that you're adding as a project resource, and open the worker record.</span></span>
2. <span data-ttu-id="74790-115">क्रिया-कलाप फलक पर, **परियोजना** &gt; **सेटअप** &gt; **परियोजना सेटअप** चुनें .</span><span class="sxs-lookup"><span data-stu-id="74790-115">On the Action Pane, select **Project** &gt; **Setup** &gt; **Project setup**.</span></span>
3. <span data-ttu-id="74790-116">कैलेंडर का चयन करें, और उसके बाद पृष्ठ बंद करें.</span><span class="sxs-lookup"><span data-stu-id="74790-116">Select a calendar, and then close the page.</span></span>

<span data-ttu-id="74790-117">आप पूर्व-कार्यभार के एक प्रकार के रूप में संसाधन के लिए डिफ़ॉल्ट परियोजनाओं को भी निर्दिष्ट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="74790-117">You can also specify default projects for a resource as a type of pre-assignment.</span></span> <span data-ttu-id="74790-118">जब संसाधन प्रबंधक या परियोजना प्रबंधक जानता है कि संसाधन पहले से किन परियोजनाओं पर काम कर रहा होगा, तो पूर्व-कार्यभार का उपयोग किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="74790-118">Pre-assignments can be used when the resource manager or project manager knows which projects the resource will be working on in advance.</span></span> <span data-ttu-id="74790-119">पूर्व-कार्यभार किसी परियोजना प्रायोजक या ग्राहक के अनुरोध पर भी आधारित हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="74790-119">Pre-assignments can also be based on the request of a project sponsor or customer.</span></span> <span data-ttu-id="74790-120">एक परियोजना को पहले से नियत करने के लिए, **परियोजनाओं को नियत करें** पृष्ठ पर, **परियोजनाएं** टैब पर, **शेष परियोजनाएं** सूची में, उपयुक्त परियोजना का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="74790-120">To pre-assign a project, on the **Assign projects** page, on the **Projects** tab, in the **Remaining projects** list, select the appropriate project.</span></span>

## <a name="set-up-an-intercompany-resource"></a><span data-ttu-id="74790-121">एक इंटरकंपनी संसाधन सेट करें</span><span class="sxs-lookup"><span data-stu-id="74790-121">Set up an intercompany resource</span></span>

<span data-ttu-id="74790-122">जब आप कंपनियों के बीच के एक संसाधन के रूप में एक श्रमिक को सेट करते हैं, तो आपको ऋण देने वाली कंपनी और लेने वाली कंपनी दोनों में सेटअप पूरा करना होगा.</span><span class="sxs-lookup"><span data-stu-id="74790-122">When you set up a worker as an intercompany resource, you must complete the setup in both the lending company and the borrowing company.</span></span>

### <a name="in-the-lending-company"></a><span data-ttu-id="74790-123">ऋण देने वाली कंपनी में</span><span class="sxs-lookup"><span data-stu-id="74790-123">In the lending company</span></span>

1. <span data-ttu-id="74790-124">फाइनैन्स में, सत्यापित करें कि ऋण देने वाली कंपनी का चयन किया जाता है, और फिर पिछले अनुभाग में प्रक्रिया पूरी करें, "एक परियोजना संसाधन के रूप में एक श्रमिक को सेट करें."</span><span class="sxs-lookup"><span data-stu-id="74790-124">In Finance, verify that the lending company is selected, and then complete the procedure in the previous section, "Set up a worker as a project resource."</span></span>
2. <span data-ttu-id="74790-125">**कंपनियों के बीच लेखांकन** पृष्ठ पर, **नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="74790-125">On the **Intercompany accounting** page, select **New**.</span></span>
3. <span data-ttu-id="74790-126">**कानूनी निकाय ID** फ़ील्ड में, ऋण देने वाली कंपनी का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="74790-126">In the **Legal entity ID** field, select the lending company.</span></span> <span data-ttu-id="74790-127">उपयुक्त के रूप में शेष फ़ील्ड में भरें, और फिर **सहेजें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="74790-127">Fill in the remaining fields as appropriate, and then select **Save**.</span></span>
4. <span data-ttu-id="74790-128">**स्थानांतरण मूल्य** पृष्ठ पर **नया** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="74790-128">On the **Transfer price** page, select **New**.</span></span>
5. <span data-ttu-id="74790-129">**ऋण लेने वाली कानूनी निकाय** फ़ील्ड में, उपयुक्त कंपनी का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="74790-129">In the **Borrowing legal entity** field, select the appropriate company.</span></span>
6. <span data-ttu-id="74790-130">ऋण लेने वाली कंपनी को केवल उस संसाधन को ऋण देने के लिए जो आपने इस अनुभाग की शुरुआत में बनाया, **संसाधन** फ़ील्ड में, आपके द्वारा बनाए गए संसाधन का नाम चुनें.</span><span class="sxs-lookup"><span data-stu-id="74790-130">To lend the borrowing company only the resource that you created at the beginning of this section, in the **Resource** field, select the name of the resource that you created.</span></span> <span data-ttu-id="74790-131">ऋण देने वाली कंपनी में सभी संसाधनों को ऋण लेने वाली कंपनी को उपलब्ध कराने के लिए, **संसाधन** फील्ड खाली छोड़ दें.</span><span class="sxs-lookup"><span data-stu-id="74790-131">To make all resources in the lending company available to the borrowing company, leave the **Resource** field blank.</span></span>
7. <span data-ttu-id="74790-132">**परियोजना प्रबंधन और लेखांकन मापदंड** पृष्ठ पर **इंटरकंपनी** टैब पर, **कंपनियों के बीच संसाधन शेड्यूलिंग और टाइमशीट सक्षम करें** विकल्प को **हां** पर सेट करें.</span><span class="sxs-lookup"><span data-stu-id="74790-132">On the **Project management and accounting parameters** page, on the **Intercompany** tab, set the **Enable intercompany resource scheduling and timesheets** option to **Yes**.</span></span>

### <a name="in-the-borrowing-company"></a><span data-ttu-id="74790-133">ऋण लेने वाली कंपनी में</span><span class="sxs-lookup"><span data-stu-id="74790-133">In the borrowing company</span></span>

- <span data-ttu-id="74790-134">**संसाधन सूची** पृष्ठ पर, खोज फ़िल्टर में, आपके द्वारा ऋण देने वाली कंपनी के लिए बनाए गए संसाधन का नाम दर्ज करें, यह सत्यापित करने के लिए कि नाम ऋण लेने वाली कंपनी के लिए संसाधन सूची में शामिल है.</span><span class="sxs-lookup"><span data-stu-id="74790-134">On the **Resources list** page, in the search filter, enter the name of the resource that you created for the lending company, to verify that the name is included in the resource list for the borrowing company.</span></span>

## <a name="request-project-resources"></a><span data-ttu-id="74790-135">प्रोजेक्ट संसाधनों अनुरोध</span><span class="sxs-lookup"><span data-stu-id="74790-135">Request project resources</span></span>
<span data-ttu-id="74790-136">परियोजना संसाधन शेड्यूलिंग के लिए कार्यक्षमता केवल संसाधन प्रबंधकों को काम या परियोजना में कर्मचारी संसाधनों को वितरित करने देती है.</span><span class="sxs-lookup"><span data-stu-id="74790-136">The functionality for project resource scheduling only lets resource managers distribute staffed resources on engagements or projects.</span></span> <span data-ttu-id="74790-137">इस कार्यक्षमता को सक्षम करने के लिए निम्नलिखित कार्य पूरा करें या सत्यापित करें कि वो पूरे हो गए हैं:</span><span class="sxs-lookup"><span data-stu-id="74790-137">To enable this functionality, complete the following tasks, or verify that they have been completed:</span></span>

- <span data-ttu-id="74790-138">संख्या क्रम सेट करें.</span><span class="sxs-lookup"><span data-stu-id="74790-138">Set up number sequences.</span></span>
- <span data-ttu-id="74790-139">परियोजना प्रबंधन और लेखांकन कार्यप्रवाह सेट करें.</span><span class="sxs-lookup"><span data-stu-id="74790-139">Set up project management and accounting workflows.</span></span>
- <span data-ttu-id="74790-140">संसाधन अनुरोध वर्कफ़्लोज़ सक्षम करें.</span><span class="sxs-lookup"><span data-stu-id="74790-140">Enable resource request workflows.</span></span>

<span data-ttu-id="74790-141">पूर्ववर्ती कार्य पूरे होने के बाद, आप अपनी ज़रूरत के अनुसार निम्नांकित कार्यों को पूरा कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="74790-141">After the preceding tasks have been completed, you can complete the following tasks as you require:</span></span>

- <span data-ttu-id="74790-142">सॉफ्ट-बुक किए गए कर्मचारी संसाधन से संसाधन अनुरोध बनाएं.</span><span class="sxs-lookup"><span data-stu-id="74790-142">Create a resource request from a soft-booked staffed resource.</span></span>
- <span data-ttu-id="74790-143">संसाधन अनुरोधों की निगरानी करें.</span><span class="sxs-lookup"><span data-stu-id="74790-143">Monitor resource requests.</span></span>
- <span data-ttu-id="74790-144">पूर्णता संसाधन अनुरोध.</span><span class="sxs-lookup"><span data-stu-id="74790-144">Fulfill resource requests.</span></span>
- <span data-ttu-id="74790-145">WBS से कर्मचारी संसाधन का अनुरोध करें.</span><span class="sxs-lookup"><span data-stu-id="74790-145">Request a staffed resource from a WBS.</span></span>
- <span data-ttu-id="74790-146">कर्मचारी संसाधन के लिए अनुरोध के बिना परियोजना के लिए संसाधन बुक करें.</span><span class="sxs-lookup"><span data-stu-id="74790-146">Book resources to a project without having a request for a staffed resource.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]