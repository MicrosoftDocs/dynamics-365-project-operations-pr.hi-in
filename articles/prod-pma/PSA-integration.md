---
title: Project Service Automation अवलोकन
description: यह विषय Dynamics 365 Project Service Automation के Dynamics 365 Finance में एकीकरण समाधान के बारे में जानकारी प्रदान करता है.
author: ruhercul
manager: AnnBe
ms.date: 07/25/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: ruhercul
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: ruhercul
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: d9ccbb29d5035ea061d232011af87cef2c81e76c
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/25/2020
ms.locfileid: "4642455"
---
# <a name="project-service-automation-overview"></a><span data-ttu-id="0be6a-103">Project Service Automation अवलोकन</span><span class="sxs-lookup"><span data-stu-id="0be6a-103">Project Service Automation overview</span></span>

[!include[banner](../includes/banner.md)]
[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="0be6a-104">यह विषय Dynamics 365 Project Service Automation के Dynamics 365 Finance में एकीकरण समाधान डेटा एकीकरण सुविधा का उपयोग Common Data Service के माध्यम से Dynamics 365 Finance और Dynamics 365 Project Service Automation के इंस्टेंस में डेटा को सिंक्रनाइज़ करने के लिए करता है.</span><span class="sxs-lookup"><span data-stu-id="0be6a-104">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Dynamics 365 Finance and Dynamics 365 Project Service Automation via Common Data Service.</span></span> <span data-ttu-id="0be6a-105">डेटा एकीकरण फ़ीचर के साथ उपलब्ध एकीकरण टेम्पलेट Project Service Automation से Finance में परियोजनाओं, परियोजना अनुबंधों, परियोजना अनुबंध लाइनों, परियोजना अनुबंध लाइन उपलब्धि, परियोजना कार्य, व्यय लेनदेन श्रेणियों और व्यय अनुमान के प्रवाह को सक्षम करते हैं.</span><span class="sxs-lookup"><span data-stu-id="0be6a-105">The integration templates that are available with the Data integration feature enable the flow of projects, project contracts, project contract lines, project contract line milestones, project tasks, expense transaction categories, hour estimates, and expense estimates from Project Service Automation to Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="0be6a-106">यदि आप वर्जन 7.3.0 का इस्तेमाल कर रहे हैं तो आपको KB 4074835 इंस्टॉल करना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="0be6a-106">If you're using version 7.3.0, you must install KB 4074835.</span></span> <span data-ttu-id="0be6a-107">इसके बाद आप निर्धारित मूल्य परियोजनाओं को एकीकृत कर पाएंगे.</span><span class="sxs-lookup"><span data-stu-id="0be6a-107">You will then be able to integrate fixed price projects.</span></span>
> - <span data-ttu-id="0be6a-108">अगर आप 7.3.0 वर्शन का उपयोग कर रहे हैं, और आप Project Service Automation से शुल्क लेनदेन ला रहे हैं, तो आपको परियोजना इनवॉइस में उन शुक्लों को शामिल करने के लिए KB 4345320 इंस्टॉल करना होगा.</span><span class="sxs-lookup"><span data-stu-id="0be6a-108">If you're using version 7.3.0, and you are bringing fee transactions over from Project Service Automation, you must install KB 4345320 in order to include those fees in the project invoice.</span></span>
> - <span data-ttu-id="0be6a-109">अगर आप वर्शन 8.0 का उपयोग कर रहे हैं, तो आप परियोजना कार्य एकीकरण, व्यय लेनदेन श्रणियों, घंटा अनुमानों, व्यय अनुमानों, तथा कार्यात्मकता लॉकिंग का उपयोग कर पाएंगे.</span><span class="sxs-lookup"><span data-stu-id="0be6a-109">If you're using version 8.0, you will be able to use project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking.</span></span>
> - <span data-ttu-id="0be6a-110">अगर आप वर्शन 8.0.1 का उपयोग कर रहे हैं, तो आप वास्तविक आंकड़ों को संकालित कर पाएंगे.</span><span class="sxs-lookup"><span data-stu-id="0be6a-110">If you're using version 8.0.1 or later, you will be able to synchronize actuals.</span></span>

<span data-ttu-id="0be6a-111">इससे पहले कि आप Project Service Automation फाइनेंस को एकीकृत करें, आपको Project Service Automation एकीकरण मानक को कन्फीगर करना होगा.</span><span class="sxs-lookup"><span data-stu-id="0be6a-111">Before you can integrate Project Service Automation Finance, you must configure the Project Service Automation integration parameters.</span></span> <span data-ttu-id="0be6a-112">और जानकारी: [Project Service Automation एकीकरण मानक](PSA-parameters.md) देखें.</span><span class="sxs-lookup"><span data-stu-id="0be6a-112">For more information, see [Project Service Automation integration parameters](PSA-parameters.md).</span></span>

<span data-ttu-id="0be6a-113">एकीकरण का यह समाधान निम्न परिदृश्यों में सीधे संकालन को सक्रिय करता है:</span><span class="sxs-lookup"><span data-stu-id="0be6a-113">This integration solution enables direct synchronization in the following scenarios:</span></span>

- <span data-ttu-id="0be6a-114">Project Service Automation में परियोजना अनुबंध को बरकरार रखता है, और उन्हें Project Service Automation से फाइनेंस में सीधे संकालित करता है.</span><span class="sxs-lookup"><span data-stu-id="0be6a-114">Maintain project contracts in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="0be6a-115">Project Service Automation में परियोजना तैयार करता है, तथा उन्हें Project Service Automation से फाइनेंस में सीधे संकालित करता है.</span><span class="sxs-lookup"><span data-stu-id="0be6a-115">Create projects in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="0be6a-116">Project Service Automation में परियोजना अनुबंध पंक्ति को बरकरार रखता है, और उन्हें Project Service Automation से फाइनेंस में सीधे संकालित करता है.</span><span class="sxs-lookup"><span data-stu-id="0be6a-116">Maintain project contract lines in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="0be6a-117">Project Service Automation में परियोजना अनुबंध पंक्ति माइलस्टोन को बरकरार रखता है, और उन्हें Project Service Automation से फाइनेंस में सीधे संकालित करता है.</span><span class="sxs-lookup"><span data-stu-id="0be6a-117">Maintain project contract line milestones in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="0be6a-118">Project Service Automation में परियोजना कार्यों को बरकरार रखता है, और उन्हें Project Service Automation से फाइनेंस में सीधे संकालित करता है.</span><span class="sxs-lookup"><span data-stu-id="0be6a-118">Maintain project tasks in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="0be6a-119">फाइनेंस में व्यय लेनदेन श्रेणियों को बरकरार रखता है और उन्हें फाइनेंस से सीधे Project Service Automation में संकालित करता है.</span><span class="sxs-lookup"><span data-stu-id="0be6a-119">Maintain expense transaction categories in Finance, and synchronize them directly from Finance to Project Service Automation.</span></span>
- <span data-ttu-id="0be6a-120">Project Service Automation में परियोजना घंटा अनुमान को तैयार करता है, और उन्हें Project Service Automation से फाइनेंस में सीधे संकालित करता है.</span><span class="sxs-lookup"><span data-stu-id="0be6a-120">Create project hour estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="0be6a-121">Project Service Automation में परियोजना व्यय अनुमान को तैयार करता है, और उन्हें Project Service Automation से फाइनेंस में सीधे संकालित करता है.</span><span class="sxs-lookup"><span data-stu-id="0be6a-121">Create project expense estimates in Project Service Automation, and synchronize them directly from Project Service Automation to Finance.</span></span>
- <span data-ttu-id="0be6a-122">Project Service Automation में परियोजना समय, व्यय और शुल्क के वास्तविक आंकड़े को तैयार करता है, और Project Service Automation एकीकरण जर्नल में परियोजना लेनदेन तैयार करता है ताकि उन्हें फाइनेंस में पोस्ट किया जा सके.</span><span class="sxs-lookup"><span data-stu-id="0be6a-122">Create project time, expense, and fee actuals in Project Service Automation, and create project transactions in the Project Service Automation integration journal so that they can be posted in Finance.</span></span>

## <a name="data-synchronization"></a><span data-ttu-id="0be6a-123">डेटा सिंक्रोनाइज़ेशन</span><span class="sxs-lookup"><span data-stu-id="0be6a-123">Data synchronization</span></span>

<span data-ttu-id="0be6a-124">निम्न चित्रण दिखाता है कि आंकड़े Project Service Automation और फाइनेंस के बीच एकीकरण के रूप में किस तरह से संकालित होते हैं.</span><span class="sxs-lookup"><span data-stu-id="0be6a-124">The following illustration shows how data is synchronized as part of the integration between Project Service Automation and Finance.</span></span>

> [!NOTE]
> <span data-ttu-id="0be6a-125">सभी टेम्प्लेट अभी उपलब्ध नहीं हैं.</span><span class="sxs-lookup"><span data-stu-id="0be6a-125">Not all templates are currently available.</span></span> <span data-ttu-id="0be6a-126">पूरा होते हैं टेम्प्लेट जारी किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="0be6a-126">Templates will be released as they are completed.</span></span>

<span data-ttu-id="0be6a-127">[![फाइनेंस के साथ Project Service Automation का एकीकरण](./media/PSA-integration.png)](./media/PSA-integration.png)</span><span class="sxs-lookup"><span data-stu-id="0be6a-127">[![Project Service Automation integration with Finance](./media/PSA-integration.png)](./media/PSA-integration.png)</span></span>

## <a name="system-requirements-for-finance"></a><span data-ttu-id="0be6a-128">वित्त के लिए सिस्टम आवश्यकताएँ</span><span class="sxs-lookup"><span data-stu-id="0be6a-128">System requirements for Finance</span></span>

<span data-ttu-id="0be6a-129">फाइनेंस एकीकरण समाधान में Project Service Automation के उपयोग के लिए, आपको प्लेटफॉर्म अपडेट 12 या बाद वाले अपडेट के साथ Enterprise Edition 7.3 इंस्टॉल करना होगा.</span><span class="sxs-lookup"><span data-stu-id="0be6a-129">To use the Project Service Automation to Finance integration solution, you must install Enterprise edition 7.3 with Platform update 12 or later.</span></span>

## <a name="system-requirements-for-project-service-automation"></a><span data-ttu-id="0be6a-130">सिस्टम को Project Service Automation की जरूरत है</span><span class="sxs-lookup"><span data-stu-id="0be6a-130">System requirements for Project Service Automation</span></span>

<span data-ttu-id="0be6a-131">फाइनेंस एकीकरण समाधान में Project Service Automation के उपयोग के लिए, आपको निम्नलिखित घटक इंस्टॉल करने होंगे.</span><span class="sxs-lookup"><span data-stu-id="0be6a-131">To use the Project Service Automation to Finance integration solution, you must install the following components:</span></span>

- <span data-ttu-id="0be6a-132">Dynamics 365 Project Service Automation संस्करण 9.0.0.0 या बाद का संस्करण</span><span class="sxs-lookup"><span data-stu-id="0be6a-132">Dynamics 365 Project Service Automation version 9.0.0.0 or later</span></span>
- <span data-ttu-id="0be6a-133">Dynamics 365 Sales, वर्शन 1.14.0.0 (v14) या आगे के वर्शन के लिए नकदी समाधान की संभावना</span><span class="sxs-lookup"><span data-stu-id="0be6a-133">Prospect to cash solution for Dynamics 365 Sales, version 1.14.0.0 (v14) or later</span></span>
- <span data-ttu-id="0be6a-134">Dynamics 365 Project Service Automation वर्शन1.0.0.0 या आगे के वर्शन के लिए Project Service Automation टू फाइनेंस समाधान</span><span class="sxs-lookup"><span data-stu-id="0be6a-134">Project Service Automation to Finance solution for Dynamics 365 Project Service Automation version 1.0.0.0 or later</span></span>

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a><span data-ttu-id="0be6a-135">Project Service Automation टू फाइनेंस एकीकरण समाधान को अपने Project Service Automation आवृत्ति में इंस्टॉल करें</span><span class="sxs-lookup"><span data-stu-id="0be6a-135">Install the Project Service Automation to Finance integration solution in your Project Service Automation instance</span></span>

<span data-ttu-id="0be6a-136">Project Service Automation टू फाइनेंस एकीकरण समाधान को [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=57016) से डाउनलोड करें, और समाधान के साथ शामिल निर्देशों का पालन करें.</span><span class="sxs-lookup"><span data-stu-id="0be6a-136">Download the Project Service Automation to Finance integration solution from [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=57016), and follow the instructions that are included with the solution.</span></span>
