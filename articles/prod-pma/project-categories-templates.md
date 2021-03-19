---
title: Finance and Operations और Project Service Automation के बीच परियोजना व्यय श्रेणियों को सिन्क्रोनाइज करें
description: यह विषय टेम्पलेट्स और अंतर्निहित कार्यों का वर्णन करता है जिनका उपयोग Microsoft Dynamics 365 Finance और Dynamics 365 Project Service Automation के बीच परियोजना व्यय श्रेणियों को सिन्क्रोनाइज करने के लिए किया जाता है.
author: Yowelle
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: 4abb7fe6554825b97df4cc04ee1b02d731cb4af9
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289641"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a><span data-ttu-id="36a17-103">Finance and Operations और Project Service Automation के बीच परियोजना व्यय श्रेणियों को सिन्क्रोनाइज करें</span><span class="sxs-lookup"><span data-stu-id="36a17-103">Synchronize project expense categories between Finance and Operations and Project Service Automation</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="36a17-104">यह विषय टेम्पलेट्स और अंतर्निहित कार्यों का वर्णन करता है जिनका उपयोग Dynamics 365 Finance और Dynamics 365 Project Service Automation के बीच परियोजना व्यय श्रेणियों को सिन्क्रोनाइज करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="36a17-104">This topic describes the templates and underlying tasks that are used to synchronize project expense categories between Dynamics 365 Finance and Dynamics 365 Project Service Automation.</span></span>

> [!NOTE]
> - <span data-ttu-id="36a17-105">परियोजना कार्य एकीककरण, व्यय लेनदेन श्रेणियां, घंटा अनुमान, व्यय अनुमान, और कार्यात्मकता लॉकिंग वर्शन 8.0 में उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="36a17-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking are available in version 8.0.</span></span>
> - <span data-ttu-id="36a17-106">वास्तविक आंकड़ों का एकीकरण वर्शन 8.0.1 और आगे के वर्शन में उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="36a17-106">Actuals integration is available in version 8.0.1 or later.</span></span>
> - <span data-ttu-id="36a17-107">अगर आप KB 4132657 और KB 4132660 इंस्टॉल करने के बाद, Enterprise Edition 7.3.0 इस्तेमाल कर रहे हैं तो आप परियोजना कार्यों, व्यय लेनदेन श्रेणियों, घंटे के अनुमानों, व्यय के अनुमानों और वास्तविक आकड़ों को एकीकृत करने के लिए टेम्पलेट्स का इस्तेमाल करने और कार्यात्मकता को कॉन्फ़िगर करने में सक्षम होंगे.</span><span class="sxs-lookup"><span data-stu-id="36a17-107">If you're using Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="36a17-108">यदि आपको लेखांकन वितरणों को रीसेट करना ही है, तो हम अनुशंसित करते हैं कि आप KB 4131710 को भी इंस्टॉल करें.</span><span class="sxs-lookup"><span data-stu-id="36a17-108">If you must reset the accounting distributions, we recommend that you also install KB 4131710.</span></span>

## <a name="data-flow-for-project-service-automation-and-finance"></a><span data-ttu-id="36a17-109">Project Service Automation और Finance के लिए डेटा प्रवाह</span><span class="sxs-lookup"><span data-stu-id="36a17-109">Data flow for Project Service Automation and Finance</span></span>

<span data-ttu-id="36a17-110">Project Service Automation और Finance एकीकरण समाधान Project Service Automation और Finance के उदाहरणों में डेटा सिन्क्रोनाइज करने के लिए डेटा एकीकरण सुविधा का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="36a17-110">The Project Service Automation and Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="36a17-111">एकीकरण टेम्पलेट्स जो डेटा एकीकरण सुविधा के साथ उपलब्ध हैं Finance और Project Service Automation के बीच परियोजना व्यय लेनदेन की श्रेणियों के बारे में डेटा के प्रवाह को सक्षम करते हैं.</span><span class="sxs-lookup"><span data-stu-id="36a17-111">The integration templates that are available with the Data integration feature enable the flow of data about project expense transaction categories between Finance and Project Service Automation.</span></span>

<span data-ttu-id="36a17-112">यदि परियोजना व्यय श्रेणियों को Finance में महारत हासिल है, तो एकीकरण प्रवाह Finance से Project Service Automation तक प्रथम है.</span><span class="sxs-lookup"><span data-stu-id="36a17-112">If the project expense categories are mastered in Finance, the integration flow is first from Finance to Project Service Automation.</span></span> <span data-ttu-id="36a17-113">परियोजना व्यय श्रेणियों की एकीकरण IDs, Project Service Automation से Finance तक सिन्क्रोनाइजेशन के माध्यम से अपडेट होती हैं.</span><span class="sxs-lookup"><span data-stu-id="36a17-113">The integration IDs of the project expense categories are then updated through synchronization from Project Service Automation to Finance.</span></span>

<span data-ttu-id="36a17-114">यदि परियोजना व्यय श्रेणियों को Project Service Automation में महारत हासिल है, तो एकीकरण प्रवाह Project Service Automation से Finance तक प्रथम है.</span><span class="sxs-lookup"><span data-stu-id="36a17-114">If the project expense categories are mastered in Project Service Automation, the integration flow is first from Project Service Automation to Finance.</span></span> <span data-ttu-id="36a17-115">Project Service Automation से सिन्क्रोनाइजेशन से पहले परियोजना श्रेणियों को पहले से ही Finance में कॉन्फ़िगर किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="36a17-115">The project categories must already be configured in Finance before the synchronization from Project Service Automation.</span></span> <span data-ttu-id="36a17-116">फिर Finance से Project Service Automation के लिए वापस सिन्क्रोनाइज करें, और फिर Project Service Automation से Finance के लिए फिर से करें.</span><span class="sxs-lookup"><span data-stu-id="36a17-116">Then synchronize from Finance back to Project Service Automation, and then from Project Service Automation to Finance again.</span></span> <span data-ttu-id="36a17-117">इस तरह से, आप यह गारंटी देने में मदद करते हैं कि श्रेणियां जुड़ी हुई हैं, और कोई डुप्लिकेट नहीं बनाई जाती हैं.</span><span class="sxs-lookup"><span data-stu-id="36a17-117">In this way, you help guarantee that the categories are linked, and that no duplicates are created.</span></span>

> [!NOTE]
> <span data-ttu-id="36a17-118">आमतौर पर, परियोजना व्यय श्रेणियों को Finance में महारत हासिल है.</span><span class="sxs-lookup"><span data-stu-id="36a17-118">Typically, the project expense categories are mastered in Finance.</span></span> <span data-ttu-id="36a17-119">हालांकि, यदि वे नहीं हैं, या यदि Project Service Automation में व्यय श्रेणियां पहले ही बनाई जा चुकी हैं, तो आपको पहले परियोजना व्यय लेनदेन की श्रेणियों (PSA से Fin और Ops) की टेम्पलेट का उपयोग करके सिन्क्रोनाइज करना होगा.</span><span class="sxs-lookup"><span data-stu-id="36a17-119">However, if they aren't, or if expense categories have already been created in Project Service Automation, you must first synchronize by using the Project expense transaction categories (PSA to Fin and Ops) template.</span></span> <span data-ttu-id="36a17-120">फिर परियोजना व्यय लेनदेन की श्रेणियों (Fin और Ops से PSA) की टेम्पलेट का उपयोग करके सिन्क्रोनाइज करें.</span><span class="sxs-lookup"><span data-stu-id="36a17-120">Then synchronize by using the Project expense transaction categories (Fin and Ops to PSA) template.</span></span> <span data-ttu-id="36a17-121">इसके बाद आपको Project Service Automation से Finance तक एक और बार सिन्क्रोनाइजेशन को चलाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="36a17-121">You should then run the synchronization from Project Service Automation to Finance one more time.</span></span>
>
> <span data-ttu-id="36a17-122">यदि आप Project Service Automation से सिन्क्रोनाइज पहले करते हैं, तो सिन्क्रोनाइजेशन चलाने से पहले Finance में निम्नलिखित आवश्यकताओं को पूरा किया जाना चाहिए:</span><span class="sxs-lookup"><span data-stu-id="36a17-122">If you synchronize first from Project Service Automation, the following requirements must be met in Finance before the synchronization is run:</span></span>
>
> - <span data-ttu-id="36a17-123">Project Service Automation में स्थापित परियोजना श्रेणी से मेल खाती साझा श्रेणी जरूर मौजूद होनी चाहिए, और इसे **परियोजना** और **व्यय** दोनों के लिए सक्षम होना जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="36a17-123">The shared category that matches the project category that is set up in Project Service Automation must exist, and it must be enabled for both **Project** and **Expense**.</span></span>
> - <span data-ttu-id="36a17-124">प्रत्येक Finance legal निकाय के लिए जिसे एकीकृत किया जाना चाहिए, निम्नलिखित परियोजना श्रेणियां जरूर मौजूद होनी चाहिए:</span><span class="sxs-lookup"><span data-stu-id="36a17-124">For each Finance legal entity that must be integrated with, the following project categories must exist:</span></span>
>
>     - <span data-ttu-id="36a17-125">**प्रोजेक्ट श्रेणी** मौजूद है.</span><span class="sxs-lookup"><span data-stu-id="36a17-125">**Project category** exists.</span></span> 
>     - <span data-ttu-id="36a17-126">**व्यय में उपयोग** सक्षम है.</span><span class="sxs-lookup"><span data-stu-id="36a17-126">**Use in Expense** is enabled.</span></span>
>     - <span data-ttu-id="36a17-127">**जर्नल में सक्रिय** सक्षम है.</span><span class="sxs-lookup"><span data-stu-id="36a17-127">**Active in journal** is enabled.</span></span>
>     - <span data-ttu-id="36a17-128">**लेनदेन के प्रकार** **खर्च** के लिए सेट है.</span><span class="sxs-lookup"><span data-stu-id="36a17-128">**Transaction type** is set to **Expense**.</span></span>

<span data-ttu-id="36a17-129">निम्नलिखित दृष्टांत दर्शाता है कि Project Service Automation और Finance के बीच डेटा को सिन्क्रोनाइज कैसे किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="36a17-129">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="36a17-130">[![वित्त के साथ Project Service Automation एकीकरण के लिए डेटा प्रवाह](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="36a17-130">[![Data flow for Project Service Automation integration with Finance](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)</span></span>

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a><span data-ttu-id="36a17-131">Finance से Project Service Automation के लिए परियोजना व्यय श्रेणी सिन्क्रोनाइजेशन</span><span class="sxs-lookup"><span data-stu-id="36a17-131">Project expense category synchronization from Finance to Project Service Automation</span></span>

### <a name="template-and-task"></a><span data-ttu-id="36a17-132">टेम्पलेट और कार्य</span><span class="sxs-lookup"><span data-stu-id="36a17-132">Template and task</span></span>

<span data-ttu-id="36a17-133">टेम्पलेट तक पहुंचने के लिए, Microsoft Power Apps एडमिन सेंटर में, **परियोजना** का चयन करें, और फिर, ऊपरी-दाएं कोने में, सार्वजनिक टेम्पलेट्स का चयन करने के लिए **नई परियोजना** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="36a17-133">To access the template, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="36a17-134">निम्नलिखित टेम्पलेट और अंतर्निहित कार्य का उपयोग Finance से Project Service Automation तक परियोजना व्यय श्रेणियों को सिन्क्रोनाइज करने के लिए किया जाता है:</span><span class="sxs-lookup"><span data-stu-id="36a17-134">The following template and underlying task are used to synchronize project expense categories from Finance to Project Service Automation:</span></span>

- <span data-ttu-id="36a17-135">**डेटा एकीकरण में टेम्पलेट का नाम:** परियोजना व्यय लेनदेन की श्रेणियां (Fin और Ops से PSA)</span><span class="sxs-lookup"><span data-stu-id="36a17-135">**Name of the template in Data integration:** Project expense transaction categories (Fin and Ops to PSA)</span></span>
- <span data-ttu-id="36a17-136">**परियोजना में कार्य का नाम:** PSA से श्रेणियों को सिंक करें</span><span class="sxs-lookup"><span data-stu-id="36a17-136">**Name of the task in the project:** Sync categories to PSA</span></span>

### <a name="entity-set"></a><span data-ttu-id="36a17-137">निकाय सेट</span><span class="sxs-lookup"><span data-stu-id="36a17-137">Entity set</span></span>

| <span data-ttu-id="36a17-138">वित्त</span><span class="sxs-lookup"><span data-stu-id="36a17-138">Finance</span></span>                           | <span data-ttu-id="36a17-139">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="36a17-139">Project Service Automation</span></span> |
|-----------------------------------|----------------------------|
| <span data-ttu-id="36a17-140">श्रेणियों के लिए एकीकरण निकाय</span><span class="sxs-lookup"><span data-stu-id="36a17-140">Integration entity for categories</span></span> | <span data-ttu-id="36a17-141">लेन-देन श्रेणियाँ</span><span class="sxs-lookup"><span data-stu-id="36a17-141">Transaction categories</span></span>     |

### <a name="entity-flow"></a><span data-ttu-id="36a17-142">निकाय प्रवाह</span><span class="sxs-lookup"><span data-stu-id="36a17-142">Entity flow</span></span>

<span data-ttu-id="36a17-143">परियोजना व्यय श्रेणियों को Finance में प्रबंधित किया जाता है, और उन्हें लेनदेन श्रेणियों के रूप में Project Service Automation के लिए सिन्क्रोनाइज किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="36a17-143">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="36a17-144">Power Query</span><span class="sxs-lookup"><span data-stu-id="36a17-144">Power Query</span></span>

<span data-ttu-id="36a17-145">जब आप Project Service Automation से सिन्क्रोनाइज कर रहे हैं, तो आपको लेनदेन श्रेणी पर बिलिंग प्रकार सेट करने के लिए Excel के लिए Microsoft Power Query का उपयोग करना होगा.</span><span class="sxs-lookup"><span data-stu-id="36a17-145">When you're synchronizing to Project Service Automation, you must use Microsoft Power Query for Excel to set the billing type on the transaction category.</span></span> <span data-ttu-id="36a17-146">परियोजना व्यय लेनदेन की श्रेणियों (Fin और Ops से PSA) का टेम्पलेट एक डिफ़ॉल्ट कॉलम और मानचित्रण प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="36a17-146">The Project expense transaction categories (Fin and Ops to PSA) template provides a default column and mapping.</span></span> <span data-ttu-id="36a17-147">यदि आप अपना खुद का टेम्पलेट बनाते हैं, तो आपको Power Query में एक सशर्त कॉलम जोड़ना होगा.</span><span class="sxs-lookup"><span data-stu-id="36a17-147">If you create your own template, you must add a conditional column in Power Query.</span></span> <span data-ttu-id="36a17-148">इन चरणों का अनुसरण करें.</span><span class="sxs-lookup"><span data-stu-id="36a17-148">Follow these steps.</span></span>

1. <span data-ttu-id="36a17-149">परियोजना व्यय लेनदेन की श्रेणियों (Fin और Ops से PSA) के टेम्पलेट में परियोजना व्यय श्रेणियों के कार्य का मानचित्रण खोलने के लिए तीर पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="36a17-149">Click the arrow to open the mapping of the project expense categories task in the Project expense transaction categories (Fin and Ops to PSA) template.</span></span>
2. <span data-ttu-id="36a17-150">Power Query खोलने के लिए **उन्नत क्वेरी और फ़िल्टरिंग** लिंक पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="36a17-150">Click the **Advance Query and Filtering** link to open Power Query.</span></span>
2. <span data-ttu-id="36a17-151">**सशर्त कॉलम जोड़ें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="36a17-151">Select **Add Conditional Column**.</span></span>
3. <span data-ttu-id="36a17-152">नए स्तंभ के लिए एक नाम दर्ज करें, जैसे **बिलिंग प्रकार**.</span><span class="sxs-lookup"><span data-stu-id="36a17-152">Enter a name for the new column, such as **BillingType**.</span></span>
4. <span data-ttu-id="36a17-153">निम्नलिखित शर्त दर्ज करें: **यदि CATEGORYID शून्य के बराबर नहीं है तो 19235001, अन्यथा शून्य**.</span><span class="sxs-lookup"><span data-stu-id="36a17-153">Enter the following condition: **if CATEGORYID not equal to null then 19235001, Otherwise null**.</span></span>
5. <span data-ttu-id="36a17-154">कॉलम पर **ठीक है** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="36a17-154">Click **OK** on the column.</span></span>
6. <span data-ttu-id="36a17-155">मानचित्रण पृष्ठ पर इस नए कॉलम का मानचित्र बनाना सुनिश्चित करें.</span><span class="sxs-lookup"><span data-stu-id="36a17-155">Be sure to map this new column on the mapping page.</span></span>

<span data-ttu-id="36a17-156">निम्नलिखित चित्रण डेटा इंटीग्रेशन में टेम्पलेट टास्क मैपिंग का उदाहरण दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="36a17-156">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="36a17-157">मानचित्रण फील्ड की जानकारी को प्रदर्शित करता है जिसे Finance से Project Service Automation तक सिन्क्रोनाइज्ड किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="36a17-157">The mapping shows the field information that will be synchronized from Finance to Project Service Automation.</span></span>

<span data-ttu-id="36a17-158">[![परियोजना व्यय श्रेणी से Project Service Automation टेम्पलेट मैपिंग](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="36a17-158">[![Project expense category to Project Service Automation template mapping](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)</span></span>

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a><span data-ttu-id="36a17-159">Project Service Automation to Finance के लिए परियोजना व्यय श्रेणी सिन्क्रोनाइजेशन</span><span class="sxs-lookup"><span data-stu-id="36a17-159">Project expense category synchronization from Project Service Automation to Finance</span></span>

### <a name="template-and-task"></a><span data-ttu-id="36a17-160">टेम्पलेट और कार्य</span><span class="sxs-lookup"><span data-stu-id="36a17-160">Template and task</span></span>

<span data-ttu-id="36a17-161">निम्नलिखित टेम्पलेट और अंतर्निहित कार्य का उपयोग Project Service Automation to Finance तक परियोजना व्यय श्रेणियों को सिन्क्रोनाइज करने के लिए किया जाता है:</span><span class="sxs-lookup"><span data-stu-id="36a17-161">The following template and underlying task are used to synchronize project expense categories from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="36a17-162">**डेटा एकीकरण में टेम्पलेट का नाम:** परियोजना व्यय लेनदेन की श्रेणियां (PSA से Fin और Ops)</span><span class="sxs-lookup"><span data-stu-id="36a17-162">**Name of the template in Data integration:** Project expense transaction categories (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="36a17-163">**परियोजना में कार्य का नाम:** Fin Ops से श्रेणियों को सिंक करें</span><span class="sxs-lookup"><span data-stu-id="36a17-163">**Name of the task in the project:** Sync categories to Fin Ops</span></span>

### <a name="entity-set"></a><span data-ttu-id="36a17-164">निकाय सेट</span><span class="sxs-lookup"><span data-stu-id="36a17-164">Entity set</span></span>

| <span data-ttu-id="36a17-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="36a17-165">Project Service Automation</span></span> | <span data-ttu-id="36a17-166">वित्त</span><span class="sxs-lookup"><span data-stu-id="36a17-166">Finance</span></span>                           |
|----------------------------|-----------------------------------|
| <span data-ttu-id="36a17-167">लेन-देन श्रेणियाँ</span><span class="sxs-lookup"><span data-stu-id="36a17-167">Transaction categories</span></span>     | <span data-ttu-id="36a17-168">श्रेणियों के लिए एकीकरण निकाय</span><span class="sxs-lookup"><span data-stu-id="36a17-168">Integration entity for categories</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="36a17-169">निकाय प्रवाह</span><span class="sxs-lookup"><span data-stu-id="36a17-169">Entity flow</span></span>

<span data-ttu-id="36a17-170">परियोजना व्यय श्रेणियों को Finance में प्रबंधित किया जाता है, और उन्हें लेनदेन श्रेणियों के रूप में Project Service Automation के लिए सिन्क्रोनाइज किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="36a17-170">Project expense categories are managed in Finance, and they are synchronized to Project Service Automation as transaction categories.</span></span> <span data-ttu-id="36a17-171">Finance के लिए वापस सिन्क्रोनाइजेशन Project Service Automation से एकीकरण ID के साथ Finance में परियोजना श्रेणी को अपडेट करता है.</span><span class="sxs-lookup"><span data-stu-id="36a17-171">The synchronization back to Finance updates the project category in Finance with the integration ID from Project Service Automation.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="36a17-172">डेटा इंटीग्रेशन में टेम्पलेट मैपिंग</span><span class="sxs-lookup"><span data-stu-id="36a17-172">Template mapping in Data integration</span></span>

<span data-ttu-id="36a17-173">निम्नलिखित चित्रण डेटा इंटीग्रेशन में टेम्पलेट टास्क मैपिंग का उदाहरण दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="36a17-173">The following illustration shows an example of the template task mapping in Data integration.</span></span>

> [!NOTE]
> <span data-ttu-id="36a17-174">मानचित्रण फील्ड की जानकारी को प्रदर्शित करता है जिसे Project Service Automation से Finance तक सिन्क्रोनाइज्ड किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="36a17-174">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="36a17-175">[![Project Service Automation से Finance टेम्पलेट मैपिंग](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="36a17-175">[![Project Service Automation to Finance template mapping](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]