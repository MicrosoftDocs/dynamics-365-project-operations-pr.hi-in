---
title: Project Service Automation से सीधे Finance and Operations में परियोजना कार्यों को सिंक्रनाइज़ करें
description: यह विषय टेम्प्लेट और अंतर्निहित कार्य का वर्णन करता है जिसका इस्तेमाल परियोजना कार्यों को सीधे Microsoft Dynamics 365 Project Service Automation से Dynamics 365 Finance में सिंक्रनाइज़ करने के लिए किया जाता है.
author: Yowelle
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 16cd38f2f190414d7be9c93e8ab90d55006f47e1
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6009978"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="39a63-103">Project Service Automation से सीधे Finance and Operations में परियोजना कार्यों को सिंक्रनाइज़ करें</span><span class="sxs-lookup"><span data-stu-id="39a63-103">Synchronize project tasks directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="39a63-104">यह विषय टेम्प्लेट और अंतर्निहित कार्य का वर्णन करता है जिसका इस्तेमाल परियोजना कार्यों को सीधे Dynamics 365 Project Service Automation से Dynamics 365 Finance में सिंक्रनाइज़ करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="39a63-104">This topic describes the template and underlying task that are used to synchronize project tasks directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="39a63-105">परियोजना कार्य एकीककरण, व्यय लेनदेन श्रेणियां, घंटा अनुमान, व्यय अनुमान, और कार्यात्मकता लॉकिंग वर्शन 8.0 में उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="39a63-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="39a63-106">अगर आप KB 4132657 और KB 4132660 इंस्टॉल करने के बाद, Enterprise Edition 7.3.0 इस्तेमाल कर रहे हैं तो आप परियोजना कार्यों, व्यय लेनदेन श्रेणियों, घंटे के अनुमानों, व्यय के अनुमानों और वास्तविक आकड़ों को एकीकृत करने के लिए टेम्पलेट्स का इस्तेमाल करने और कार्यात्मकता को कॉन्फ़िगर करने में सक्षम होंगे.</span><span class="sxs-lookup"><span data-stu-id="39a63-106">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="39a63-107">यदि आपको लेखांकन वितरणों को रीसेट करना ही है, तो हम अनुशंसित करते हैं कि आप KB 4131710 को भी इंस्टॉल करें.</span><span class="sxs-lookup"><span data-stu-id="39a63-107">If you must reset the accounting distributions, we recommended that you also install KB 4131710.</span></span>
> - <span data-ttu-id="39a63-108">वास्तविक आंकड़ों का एकीकरण वर्शन 8.0.1 और आगे के वर्शन में उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="39a63-108">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="39a63-109">Project Service Automation से Finance के लिए डेटा प्रवाह</span><span class="sxs-lookup"><span data-stu-id="39a63-109">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="39a63-110">Project Service Automation से Finance एकीकरण समाधान Project Service Automation और Finance के उदाहरणों में डेटा सिन्क्रोनाइज करने के लिए डेटा एकीकरण सुविधा का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="39a63-110">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="39a63-111">डेटा एकीकरण सुविधा के साथ उपलब्ध एकीकरण टेम्पलेट Project Service Automation से वित्त तक परियोजना कार्य के बारे में डेटा के प्रवाह को सक्षम करता है.</span><span class="sxs-lookup"><span data-stu-id="39a63-111">The integration template that is available with the Data integration feature enables the flow of data about project tasks from Project Service Automation to Finance.</span></span>

<span data-ttu-id="39a63-112">निम्नलिखित दृष्टांत दर्शाता है कि Project Service Automation और Finance के बीच डेटा को सिन्क्रोनाइज कैसे किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="39a63-112">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="39a63-113">[![वित्त के साथ Project Service Automation एकीकरण के लिए डेटा प्रवाह](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span><span class="sxs-lookup"><span data-stu-id="39a63-113">[![Data flow for Project Service Automation integration with Finance](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)</span></span>

## <a name="template-and-task"></a><span data-ttu-id="39a63-114">टेम्पलेट और कार्य</span><span class="sxs-lookup"><span data-stu-id="39a63-114">Template and task</span></span>

<span data-ttu-id="39a63-115">टेम्पलेट तक पहुंचने के लिए, Microsoft Power Apps एडमिन सेंटर में, **परियोजना** का चयन करें, और फिर, ऊपरी-दाएं कोने में, सार्वजनिक टेम्पलेट्स का चयन करने के लिए **नई परियोजना** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="39a63-115">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="39a63-116">यह विषय टेम्प्लेट और अंतर्निहित कार्य का वर्णन करता है जिसका इस्तेमाल परियोजना कार्यों को सीधे Project Service Automation से Finance में सिंक्रनाइज़ करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="39a63-116">The following template and underlying task are used to synchronize project tasks from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="39a63-117">**डेटा एकीकरण में टेम्पलेट का नाम:** परियोजना कार्य (PSA से Fin और Ops)</span><span class="sxs-lookup"><span data-stu-id="39a63-117">**Name of the template in Data integration:** Project tasks (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="39a63-118">**परियोजना में कार्य का नाम:** परियोजना के कार्य</span><span class="sxs-lookup"><span data-stu-id="39a63-118">**Name of the task in the project:** Project tasks</span></span>

<span data-ttu-id="39a63-119">परियोजना कार्यों का सिंक्रनाइज़ेशन होने से पहले, आपको परियोजना अनुबंधों और परियोजनाओं को सिंक्रनाइज़ करना होगा.</span><span class="sxs-lookup"><span data-stu-id="39a63-119">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="entity-set"></a><span data-ttu-id="39a63-120">निकाय सेट</span><span class="sxs-lookup"><span data-stu-id="39a63-120">Entity set</span></span>

| <span data-ttu-id="39a63-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="39a63-121">Project Service Automation</span></span> | <span data-ttu-id="39a63-122">वित्त</span><span class="sxs-lookup"><span data-stu-id="39a63-122">Finance</span></span>                             |
|----------------------------|-------------------------------------|
| <span data-ttu-id="39a63-123">परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="39a63-123">Project Tasks</span></span>              | <span data-ttu-id="39a63-124">परियोजना कार्य के लिए एकीकरण निकाय</span><span class="sxs-lookup"><span data-stu-id="39a63-124">Integration entity for project task</span></span> |

## <a name="entity-flow"></a><span data-ttu-id="39a63-125">निकाय प्रवाह</span><span class="sxs-lookup"><span data-stu-id="39a63-125">Entity flow</span></span>

<span data-ttu-id="39a63-126">परियोजना कार्यों को Project Service Automation में प्रबंधित किया जाता है, और उन्हें परियोजना गतिविधियों के रूप में Finance में सिंक्रनाइज़ किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="39a63-126">Project tasks are managed in Project Service Automation, and they are synchronized to Finance as project activities.</span></span>

## <a name="prerequisites-and-mapping-setup"></a><span data-ttu-id="39a63-127">आवश्यकताएँ और मानचित्रण सेटअप</span><span class="sxs-lookup"><span data-stu-id="39a63-127">Prerequisites and mapping setup</span></span>

<span data-ttu-id="39a63-128">परियोजना कार्यों का सिंक्रनाइज़ेशन होने से पहले, आपको परियोजना अनुबंधों और परियोजनाओं को सिंक्रनाइज़ करना होगा.</span><span class="sxs-lookup"><span data-stu-id="39a63-128">Before synchronization of project tasks can occur, you must synchronize project contracts and projects.</span></span>

## <a name="power-query"></a><span data-ttu-id="39a63-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="39a63-129">Power Query</span></span>

<span data-ttu-id="39a63-130">अगर यह शर्त पूरी होती है तो आपको डेटा फ़िल्टर करने के लिए Excel के लिए Microsoft Power Query का उपयोग करना चाहिए:</span><span class="sxs-lookup"><span data-stu-id="39a63-130">You must use Microsoft Power Query for Excel to filter data if this condition is met:</span></span>

- <span data-ttu-id="39a63-131">आपके पास परियोजना कार्य में संसाधन-विशिष्ट रिकॉर्ड होते हैं.</span><span class="sxs-lookup"><span data-stu-id="39a63-131">You have resource-specific records in a project task.</span></span>

<span data-ttu-id="39a63-132">यदि आपको Power Query का उपयोग करना ही है, इस दिशानिर्देश का पालन करें:</span><span class="sxs-lookup"><span data-stu-id="39a63-132">If you must use Power Query, follow this guideline:</span></span>

- <span data-ttu-id="39a63-133">परियोजना कार्यों (PSA से Fin and Ops में) टेम्पलेट में डिफ़ॉल्ट फ़िल्टर होता है, जो **IsLineTask** से **गलत** पर फ़िल्टर सेट करके किसी परियोजना कार्य से संसाधन-विशिष्ट रिकॉर्ड को अलग करता है.</span><span class="sxs-lookup"><span data-stu-id="39a63-133">The Project tasks (PSA to Fin and Ops) template has a default filter that excludes resource-specific records from a project task by setting the filter on **IsLineTask** to **False**.</span></span> <span data-ttu-id="39a63-134">यदि आप अपना टेम्पलेट बनाते हैं, तो आपको यह फिल्टर जोड़ना होगा.</span><span class="sxs-lookup"><span data-stu-id="39a63-134">If you create your own template, you must add this filter.</span></span>

## <a name="template-mapping-in-data-integration"></a><span data-ttu-id="39a63-135">डेटा इंटीग्रेशन में टेम्पलेट मैपिंग</span><span class="sxs-lookup"><span data-stu-id="39a63-135">Template mapping in Data integration</span></span>

<span data-ttu-id="39a63-136">निम्नलिखित चित्रण डेटा इंटीग्रेशन में टेम्पलेट टास्क मैपिंग का उदाहरण दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="39a63-136">The following illustration shows an example of the template task mappings in Data integration.</span></span> <span data-ttu-id="39a63-137">मानचित्रण फील्ड की जानकारी को प्रदर्शित करता है जिसे Project Service Automation से Finance तक सिन्क्रोनाइज्ड किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="39a63-137">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="39a63-138">-[![टेम्पलेट मैपिंग](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span><span class="sxs-lookup"><span data-stu-id="39a63-138">[![Template mapping](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]