---
title: Project Service Automation से Finance and Operations तक सीधे परियोजना आकलनों को सिन्क्रोनाइज करें
description: यह विषय टेम्पलेटों और अंतर्निहित कार्यों का वर्णन करता है जिनका उपयोग Microsoft Dynamics 365 Project Service Automation से Dynamics 365 Finance तक सीधे परियोजना घंटों के आकलनों और परियोजना व्यय के आकलनों को सिन्क्रोनाइज करने के लिए किया जाता है.
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
ms.openlocfilehash: a6955dcd1ebe494e0171c30ac4384089da6a8745
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999718"
---
# <a name="synchronize-project-estimates-directly-from-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="f81cc-103">Project Service Automation से Finance and Operations तक सीधे परियोजना आकलनों को सिन्क्रोनाइज करें</span><span class="sxs-lookup"><span data-stu-id="f81cc-103">Synchronize project estimates directly from Project Service Automation to Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="f81cc-104">यह विषय टेम्पलेटों और अंतर्निहित कार्यों का वर्णन करता है जिनका उपयोग Dynamics 365 Project Service Automation से Dynamics 365 Finance तक सीधे परियोजना घंटों के आकलनों और परियोजना व्यय के आकलनों को सिन्क्रोनाइज करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-104">This topic describes the templates and underlying tasks that are used to synchronize project hour estimates and project expense estimates directly from Dynamics 365 Project Service Automation to Dynamics 365 Finance.</span></span>

> [!NOTE]
> - <span data-ttu-id="f81cc-105">परियोजना कार्य एकीकरण, व्यय लेनदेन श्रणियों, घंटा अनुमानों, व्यय अनुमानों, तथा कार्यात्मकता लॉकिंग संस्करण 8.0 में उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-105">Project task integration, expense transaction categories, hour estimates, expense estimates, and functionality locking is available in version 8.0.</span></span>
> - <span data-ttu-id="f81cc-106">वास्तविक आंकड़ों का एकीकरण वर्शन 8.0.1 और आगे के वर्शन में उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-106">Actuals integration is available in version 8.0.1 or later.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance"></a><span data-ttu-id="f81cc-107">Project Service Automation से Finance के लिए डेटा प्रवाह</span><span class="sxs-lookup"><span data-stu-id="f81cc-107">Data flow for Project Service Automation to Finance</span></span>

<span data-ttu-id="f81cc-108">Project Service Automation से Finance एकीकरण समाधान Project Service Automation और Finance के उदाहरणों में डेटा सिन्क्रोनाइज करने के लिए डेटा एकीकरण सुविधा का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-108">The Project Service Automation to Finance integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance.</span></span> <span data-ttu-id="f81cc-109">एकीकरण टेम्पलेट जो डेटा एकीकरण सुविधा के साथ उपलब्ध हैं Project Service Automation से Finance तक परियोजना घंटों के आकलनों और परियोजना व्यय के आकलनों के बारे में डेटा के प्रवाह को सक्षम करते हैं.</span><span class="sxs-lookup"><span data-stu-id="f81cc-109">The integration templates that are available with the Data integration feature enable the flow of data about project hour estimates and project expense estimates from Project Service Automation to Finance.</span></span>

<span data-ttu-id="f81cc-110">निम्नलिखित दृष्टांत दर्शाता है कि Project Service Automation और Finance के बीच डेटा को सिन्क्रोनाइज कैसे किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-110">The following illustration shows how the data is synchronized between Project Service Automation and Finance.</span></span>

<span data-ttu-id="f81cc-111">[![वित्त के साथ Project Service Automation एकीकरण के लिए डेटा प्रवाह](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span><span class="sxs-lookup"><span data-stu-id="f81cc-111">[![Data flow for Project Service Automation integration with Finance](./media/ProjectEstimatesFlow.png)](./media/ProjectEstimatesFlow.png)</span></span>

## <a name="project-hour-estimates"></a><span data-ttu-id="f81cc-112">प्रोजेक्ट घंटे का अनुमान</span><span class="sxs-lookup"><span data-stu-id="f81cc-112">Project hour estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="f81cc-113">खाका और कार्य</span><span class="sxs-lookup"><span data-stu-id="f81cc-113">Template and tasks</span></span>

<span data-ttu-id="f81cc-114">उपलब्ध टेम्पलेटों तक पहुंचने के लिए, Microsoft Power Apps एडमिन सेंटर में, **परियोजनाएं** का चयन करें, और फिर, ऊपरी-दाएं कोने में, सार्वजनिक टेम्पलेटों का चयन करने के लिए **नई परियोजना** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f81cc-114">To access the available templates, in the Microsoft Power Apps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="f81cc-115">निम्नलिखित टेम्पलेट और उसके कार्य Project Service Automation से वित्त पर अनुमानित प्रोजेक्ट घंटा को सिंक्रोनाइज़ करने के लिए उपयोग होते हैं:</span><span class="sxs-lookup"><span data-stu-id="f81cc-115">The following template and underlying tasks are used to synchronize project hour estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="f81cc-116">**डेटा इंटीग्रेशन में टेम्पलेट का नाम:** प्रोजेक्ट घंटा अनुमान (Fin और Ops पर PSA)</span><span class="sxs-lookup"><span data-stu-id="f81cc-116">**Name of the template in Data integration:** Project hour estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="f81cc-117">**परियोजना में कार्य का नाम:**</span><span class="sxs-lookup"><span data-stu-id="f81cc-117">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="f81cc-118">लेन-देन संबंध</span><span class="sxs-lookup"><span data-stu-id="f81cc-118">Transaction relationships</span></span>
    - <span data-ttu-id="f81cc-119">व्यय अनुमान</span><span class="sxs-lookup"><span data-stu-id="f81cc-119">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="f81cc-120">निकाय सेट</span><span class="sxs-lookup"><span data-stu-id="f81cc-120">Entity set</span></span>

| <span data-ttu-id="f81cc-121">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f81cc-121">Project Service Automation</span></span> | <span data-ttu-id="f81cc-122">वित्त</span><span class="sxs-lookup"><span data-stu-id="f81cc-122">Finance</span></span>                                       |
|----------------------------|-----------------------------------------------|
| <span data-ttu-id="f81cc-123">परियोजना कार्य</span><span class="sxs-lookup"><span data-stu-id="f81cc-123">Project tasks</span></span>              | <span data-ttu-id="f81cc-124">प्रोजेक्ट घंटा अनुमान के लिए इंटीग्रेशन निकाय</span><span class="sxs-lookup"><span data-stu-id="f81cc-124">Integration entity for project hour estimates</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="f81cc-125">निकाय प्रवाह</span><span class="sxs-lookup"><span data-stu-id="f81cc-125">Entity flow</span></span>

<span data-ttu-id="f81cc-126">परियोजना घंटों का आकलन Project Service Automation में प्रबंधित किया जाता है, और वे परियोजना घंटे के पूर्वानुमान के रूप में Finance से सिन्क्रोनाइज होते हैं.</span><span class="sxs-lookup"><span data-stu-id="f81cc-126">Project hour estimates are managed in Project Service Automation, and they are synchronized to Finance as project hour forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="f81cc-127">पूर्वावश्यकताएँ</span><span class="sxs-lookup"><span data-stu-id="f81cc-127">Prerequisites</span></span>

<span data-ttu-id="f81cc-128">प्रोजेक्ट घंटा अनुमान का सिंक्रनाइज़ेशन होने से पहले, आपको प्रोजेक्ट, प्रोजेक्ट कार्य और प्रोजेक्ट व्यय ट्रांज़ैक्शन श्रेणियाँ सिंक्रनाइज़ करनी होंगी.</span><span class="sxs-lookup"><span data-stu-id="f81cc-128">Before synchronization of project hour estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="f81cc-129">Power Query</span><span class="sxs-lookup"><span data-stu-id="f81cc-129">Power Query</span></span>

<span data-ttu-id="f81cc-130">परियोजना घंटों का आकलन टेम्पलेट में, आपको इन कार्यों को पूरा करने के लिए Excel के लिए Microsoft Power Query का उपयोग करना होगा:</span><span class="sxs-lookup"><span data-stu-id="f81cc-130">In the project hour estimates template, you must use Microsoft Power Query for Excel to complete these tasks:</span></span>

- <span data-ttu-id="f81cc-131">डिफ़ॉल्ट पूर्वानुमान मॉडल ID सेट करें जिसका उपयोग तब किया जाएगा जब एकीकरण नए घंटे का पूर्वानुमान बनाता है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-131">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="f81cc-132">कार्य में किसी भी संसाधन-विशिष्ट रिकॉर्ड को फ़िल्टर करें जो एकीकरण को घंटे के पूर्वानुमान में विफल कर देगा.</span><span class="sxs-lookup"><span data-stu-id="f81cc-132">Filter out any resource-specific records in the task that will fail the integration into hour forecasts.</span></span>
- <span data-ttu-id="f81cc-133">किसी भी खाली लेनदेन श्रेणी की पंक्तियों को फ़िल्टर करें.</span><span class="sxs-lookup"><span data-stu-id="f81cc-133">Filter out any empty transaction category rows.</span></span> <span data-ttu-id="f81cc-134">इस कार्य को पूरा करने की विफलता गलत घंटे के पूर्वानुमान में परिणत हो सकती है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-134">Failure to complete this task might result in incorrect hour forecasts.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="f81cc-135">डिफ़ॉल्ट पूर्वानुमान मॉडल ID सेट करें</span><span class="sxs-lookup"><span data-stu-id="f81cc-135">Set the default forecast model ID</span></span>

<span data-ttu-id="f81cc-136">टेम्पलेट में डिफ़ॉल्ट पूर्वानुमान मॉडल ID को अपडेट करने के लिए, मानचित्रण खोलने के लिए **मानचित्र** तीर पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="f81cc-136">To update the default forecast model ID in the template, click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="f81cc-137">इसके बाद **उन्नत क्वेरी और फ़िल्टरिंग** लिंक का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f81cc-137">Then select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="f81cc-138">यदि आप डिफ़ॉल्ट परियोजना घंटों का आकलन (PSA से Fin और Ops) टेम्पलेट का उपयोग कर रहे हैं, तो **लागू किए गए चरण** की सूची में **डाले गए शर्त** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f81cc-138">If you're using the default Project hour estimates (PSA to Fin and Ops) template, select the **Inserted Condition** in the list of **Applied Steps**.</span></span> <span data-ttu-id="f81cc-139">**फ़ंक्शन** प्रविष्टि में, पूर्वानुमान मॉडल ID के नाम के साथ **O\_forecast** को बदलें जिसका उपयोग एकीकरण के साथ किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="f81cc-139">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="f81cc-140">डिफॉल्ट टेम्पलेट में डेमो डेटा से पूर्वानुमान मॉडल ID है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-140">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="f81cc-141">यदि आप एक नया टेम्पलेट बना रहे हैं, तो आपको यह कॉलम जोड़ना होगा.</span><span class="sxs-lookup"><span data-stu-id="f81cc-141">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="f81cc-142">Power Query में, **सशर्त कॉलम जोड़ें** का चयन करें और नए कॉलम के लिए एक नाम दर्ज करें, जैसे **ModelID**.</span><span class="sxs-lookup"><span data-stu-id="f81cc-142">In Power Query, select **Add Conditional Column**, and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="f81cc-143">स्तंभ के लिए स्थिति दर्ज करें, जहां, अगर परियोजना कार्य शून्य नहीं है, तो, \<enter the forecast model ID\>; अन्यथा अमान्य.</span><span class="sxs-lookup"><span data-stu-id="f81cc-143">Enter the condition for the column, where, if Project task is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="filter-out-resource-specific-records"></a><span data-ttu-id="f81cc-144">संसाधन-विशिष्ट रिकॉर्ड फिल्टर करें</span><span class="sxs-lookup"><span data-stu-id="f81cc-144">Filter out resource-specific records</span></span>

<span data-ttu-id="f81cc-145">परियोजना घंटे का अनुमान (PSA से Fin और Ops) टेम्पलेट में एक डिफ़ॉल्ट फ़िल्टर होता है जो किसी भी संसाधन-विशेष रिकॉर्ड को हटाता है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-145">The Project hour estimates (PSA to Fin and Ops) template has a default filter that removes any resource-specific records.</span></span> <span data-ttu-id="f81cc-146">यदि आप अपना टेम्पलेट बनाते हैं, तो आपको यह फिल्टर जोड़ना होगा.</span><span class="sxs-lookup"><span data-stu-id="f81cc-146">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="f81cc-147">**msdyn\_islinetask** कॉलम पर फिल्टर करने के लिए **उन्नत क्वेरी और फिल्टरिंग** लिंक का चयन करें ताकि केवल **गलत** रिकॉर्ड शामिल हों.</span><span class="sxs-lookup"><span data-stu-id="f81cc-147">Select the **Advanced Query and Filtering** link to filter on the **msdyn\_islinetask** column so that only **False** records are included.</span></span>

#### <a name="filter-out-empty-transaction-category-rows"></a><span data-ttu-id="f81cc-148">खाली ट्रांजैक्शन श्रेणी पंक्तियाँ फिल्टर करें</span><span class="sxs-lookup"><span data-stu-id="f81cc-148">Filter out empty transaction category rows</span></span>

<span data-ttu-id="f81cc-149">जिन पंक्तियों में खाली ट्रांजैक्शन श्रेणियाँ हैं, उन्हें हटाने के लिए आपको फिल्टर जोड़ना होगा.</span><span class="sxs-lookup"><span data-stu-id="f81cc-149">You must add a filter to remove any rows that have empty transaction categories.</span></span> <span data-ttu-id="f81cc-150">कार्य आवश्यक है, चाहे आप डिफ़ॉल्ट टेम्पलेट का उपयोग कर रहे हों या अपना टेम्पलेट बना रहे हों.</span><span class="sxs-lookup"><span data-stu-id="f81cc-150">This task is required, regardless of whether you're using the default template or creating your own template.</span></span> <span data-ttu-id="f81cc-151">यह फिल्टर Project Service Automation से पंक्तियों के सारांश को हटा देता है जिससे वित्त में घंटे का पूर्वानुमान गलत होता है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-151">This filter removes any summary rows from Project Service Automation that might cause the hour forecasts in Finance to be incorrect.</span></span> <span data-ttu-id="f81cc-152">**msdyn\_transactioncategory\_value** स्तंभ में खाली रिकॉर्ड को फिल्टर करने के लिए **उन्नत क्वेरी और फिल्टरिंग** लिंक का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f81cc-152">Select **Advanced Query and Filtering** link to filter out null records in the **msdyn\_transactioncategory\_value** column.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="f81cc-153">डेटा इंटीग्रेशन में टेम्पलेट मैपिंग</span><span class="sxs-lookup"><span data-stu-id="f81cc-153">Template mapping in Data integration</span></span>

<span data-ttu-id="f81cc-154">निम्नलिखित चित्रण डेटा इंटीग्रेशन में टेम्पलेट टास्क मैपिंग का उदाहरण दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-154">The following illustration shows an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="f81cc-155">मानचित्रण फील्ड की जानकारी को प्रदर्शित करता है जिसे Project Service Automation से Finance तक सिन्क्रोनाइज्ड किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="f81cc-155">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="f81cc-156">[![डेटा एकीकरण में टेम्पलेट मैपिंग](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="f81cc-156">[![Template task mapping in data integration](./media/ProjectHourEstimatesMapping.jpg)](./media/ProjectHourEstimatesMapping.jpg)</span></span>

## <a name="project-expense-estimates"></a><span data-ttu-id="f81cc-157">परियोजना व्यय का अनुमान</span><span class="sxs-lookup"><span data-stu-id="f81cc-157">Project expense estimates</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="f81cc-158">खाका और कार्य</span><span class="sxs-lookup"><span data-stu-id="f81cc-158">Template and tasks</span></span>

<span data-ttu-id="f81cc-159">निम्नलिखित टेम्पलेट और उसके कार्य Project Service Automation से वित्त पर अनुमानित प्रोजेक्ट खर्च को सिंक्रोनाइज़ करने के लिए उपयोग होते हैं:</span><span class="sxs-lookup"><span data-stu-id="f81cc-159">The following template and underlying tasks are used to synchronize project expense estimates from Project Service Automation to Finance:</span></span>

- <span data-ttu-id="f81cc-160">**डेटा इंटीग्रेशन में टेम्पलेट का नाम:** प्रोजेक्ट खर्च अनुमान (Fin और Ops पर PSA)</span><span class="sxs-lookup"><span data-stu-id="f81cc-160">**Name of the template in Data integration:** Project expense estimates (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="f81cc-161">**परियोजना में कार्य का नाम:**</span><span class="sxs-lookup"><span data-stu-id="f81cc-161">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="f81cc-162">लेन-देन संबंध</span><span class="sxs-lookup"><span data-stu-id="f81cc-162">Transaction relationships</span></span> 
    - <span data-ttu-id="f81cc-163">व्यय अनुमान</span><span class="sxs-lookup"><span data-stu-id="f81cc-163">Expense estimates</span></span>

### <a name="entity-set"></a><span data-ttu-id="f81cc-164">निकाय सेट</span><span class="sxs-lookup"><span data-stu-id="f81cc-164">Entity set</span></span>

| <span data-ttu-id="f81cc-165">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="f81cc-165">Project Service Automation</span></span> | <span data-ttu-id="f81cc-166">वित्त</span><span class="sxs-lookup"><span data-stu-id="f81cc-166">Finance</span></span>                                                  |
|----------------------------|----------------------------------------------------------|
| <span data-ttu-id="f81cc-167">लेनदेन कनेक्शन्स</span><span class="sxs-lookup"><span data-stu-id="f81cc-167">Transaction Connections</span></span>    | <span data-ttu-id="f81cc-168">प्रोजेक्ट ट्रांजैक्शन संबंधों के लिए इंटीग्रेशन निकाय</span><span class="sxs-lookup"><span data-stu-id="f81cc-168">Integration entity for project transaction relationships</span></span> |
| <span data-ttu-id="f81cc-169">अनुमान पंक्तियाँ</span><span class="sxs-lookup"><span data-stu-id="f81cc-169">Estimate Lines</span></span>             | <span data-ttu-id="f81cc-170">प्रोजेक्ट व्यय अनुमान के लिए इंटीग्रेशन निकाय</span><span class="sxs-lookup"><span data-stu-id="f81cc-170">Integration entity for project expense estimates</span></span>         |

### <a name="entity-flow"></a><span data-ttu-id="f81cc-171">निकाय प्रवाह</span><span class="sxs-lookup"><span data-stu-id="f81cc-171">Entity flow</span></span>

<span data-ttu-id="f81cc-172">प्रोजेक्ट व्यय अनुमान Project Service Automation में प्रबंधित होते हैं, और वे प्रोजेक्ट व्यय अनुमानों के रूप में वित्त पर सिंक्रनाइज़ होते हैं.</span><span class="sxs-lookup"><span data-stu-id="f81cc-172">Project expense estimates are managed in Project Service Automation, and they are synchronized to Finance as project expense forecasts.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="f81cc-173">पूर्वावश्यकताएँ</span><span class="sxs-lookup"><span data-stu-id="f81cc-173">Prerequisites</span></span>

<span data-ttu-id="f81cc-174">प्रोजेक्ट व्यय अनुमान का सिंक्रनाइज़ेशन होने से पहले, आपको प्रोजेक्ट, प्रोजेक्ट कार्य और प्रोजेक्ट व्यय ट्रांज़ैक्शन श्रेणियाँ सिंक्रनाइज़ करनी होंगी.</span><span class="sxs-lookup"><span data-stu-id="f81cc-174">Before synchronization of project expense estimates can occur, you must synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="f81cc-175">Power Query</span><span class="sxs-lookup"><span data-stu-id="f81cc-175">Power Query</span></span>

<span data-ttu-id="f81cc-176">प्रोजेक्ट व्यय अनुमान टेम्पलेट में, आपको निम्नलिखित कार्य पूरा करने के लिए आपको Power Query का उपयोग करना होगा:</span><span class="sxs-lookup"><span data-stu-id="f81cc-176">In the project expense estimates template, you must use Power Query to complete the following tasks:</span></span>

- <span data-ttu-id="f81cc-177">केवल व्यय अनुमान लाइन रिकॉर्ड शामिल करने के लिए फिल्टर करें.</span><span class="sxs-lookup"><span data-stu-id="f81cc-177">Filter to include only expense estimate line records.</span></span>
- <span data-ttu-id="f81cc-178">डिफ़ॉल्ट पूर्वानुमान मॉडल ID सेट करें जिसका उपयोग तब किया जाएगा जब एकीकरण नए घंटे का पूर्वानुमान बनाता है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-178">Set the default forecast model ID that will be used when the integration creates new hour forecasts.</span></span>
- <span data-ttu-id="f81cc-179">बिलिंग प्रकार बदलें.</span><span class="sxs-lookup"><span data-stu-id="f81cc-179">Transform the billing types.</span></span>
- <span data-ttu-id="f81cc-180">लेन-देन के प्रकारों को बदलना.</span><span class="sxs-lookup"><span data-stu-id="f81cc-180">Transform the transaction types.</span></span>

#### <a name="filter-to-include-only-expense-estimate-lines"></a><span data-ttu-id="f81cc-181">केवल व्यय अनुमान लाइन शामिल करने के लिए फिल्टर करें</span><span class="sxs-lookup"><span data-stu-id="f81cc-181">Filter to include only expense estimate lines</span></span>

<span data-ttu-id="f81cc-182">प्रोजेक्ट व्यय अनुमान (Fin और Ops पर PSA) टेम्पलेट में डिफ़ॉल्ट फिल्टर है जो इंटीग्रेशन में केवल व्यय लाइन शामिल करता है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-182">The Project expense estimates (PSA to Fin and Ops) template has a default filter that includes only expense lines in the integration.</span></span> <span data-ttu-id="f81cc-183">यदि आप अपना टेम्पलेट बनाते हैं, तो आपको यह फिल्टर जोड़ना होगा.</span><span class="sxs-lookup"><span data-stu-id="f81cc-183">If you create your own template, you must add this filter.</span></span> <span data-ttu-id="f81cc-184">**ट्रांज़ैक्शन संबंध** कार्य का चयन करें, और फिर मैपिंग को खोलने के लिए **मैप** तीर पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="f81cc-184">Select the **Transaction relationships** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="f81cc-185">**उन्नत क्वेरी और फिल्टरिंग** लिंक का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f81cc-185">Select the **Advanced Query and Filtering** link.</span></span> <span data-ttu-id="f81cc-186">**msdyn\_transactiontype1** स्तंभ फिल्टर करें ताकि यह केवल **msdyn\_estimateline** शामिल करे.</span><span class="sxs-lookup"><span data-stu-id="f81cc-186">Filter the **msdyn\_transactiontype1** column so that it includes only **msdyn\_estimateline**.</span></span>

#### <a name="set-the-default-forecast-model-id"></a><span data-ttu-id="f81cc-187">डिफ़ॉल्ट पूर्वानुमान मॉडल ID सेट करें</span><span class="sxs-lookup"><span data-stu-id="f81cc-187">Set the default forecast model ID</span></span>

<span data-ttu-id="f81cc-188">टेम्पलेट में डिफ़ॉल्ट पूर्वानुमान मॉडल ID उपडेट करने के लिए, **व्यय अनुमान** कार्य का चयन करें और फिर मैपिंग खोलने के लिए **मैप** तीर पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="f81cc-188">To update the default forecast model ID in the template, select the **Expense estimates** task, and then click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="f81cc-189">**उन्नत क्वेरी और फिल्टरिंग** लिंक का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f81cc-189">Select the **Advanced Query and Filtering** link.</span></span>

- <span data-ttu-id="f81cc-190">पॉवर क्वेरी में, यदि आप डिफ़ॉल्ट प्रोजेक्ट खर्च अनुमान (Fin और Ops पर PSA) टेम्पलेट का उपयोग कर रहे हैं, तो **लागू चरण** अनुभाग से पहले **प्रविष्ट अवस्था** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f81cc-190">If you're using the default Project expense estimates (PSA to Fin and Ops) template, in Power Query, select the first **Inserted Condition** from the **Applied Steps** section.</span></span> <span data-ttu-id="f81cc-191">**फ़ंक्शन** प्रविष्टि में, पूर्वानुमान मॉडल ID के नाम के साथ **O\_forecast** को बदलें जिसका उपयोग एकीकरण के साथ किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="f81cc-191">In the **Function** entry, replace **O\_forecast** with the name of the forecast model ID that should be used with the integration.</span></span> <span data-ttu-id="f81cc-192">डिफॉल्ट टेम्पलेट में डेमो डेटा से पूर्वानुमान मॉडल ID है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-192">The default template has a forecast model ID from the demo data.</span></span>
- <span data-ttu-id="f81cc-193">यदि आप एक नया टेम्पलेट बना रहे हैं, तो आपको यह कॉलम जोड़ना होगा.</span><span class="sxs-lookup"><span data-stu-id="f81cc-193">If you're creating a new template, you must add this column.</span></span> <span data-ttu-id="f81cc-194">Power Query में, **सशर्त कॉलम जोड़ें** का चयन करें और नए कॉलम के लिए एक नाम दर्ज करें, जैसे **ModelID**.</span><span class="sxs-lookup"><span data-stu-id="f81cc-194">In Power Query, select **Add Conditional Column**, and enter a name for the new column, such as **ModelID**.</span></span> <span data-ttu-id="f81cc-195">स्तंभ के लिए स्थिति दर्ज करें, जहां, अगर अनुमानित पंक्ति ID अमान्य नहीं है, तो \<enter the forecast model ID\>; अन्यथा अमान्य.</span><span class="sxs-lookup"><span data-stu-id="f81cc-195">Enter the condition for the column, where, if Estimate line ID is not null, then \<enter the forecast model ID\>; else null.</span></span>

#### <a name="transform-the-billing-types"></a><span data-ttu-id="f81cc-196">बिलिंग प्रकार बदलें</span><span class="sxs-lookup"><span data-stu-id="f81cc-196">Transform the billing types</span></span>

<span data-ttu-id="f81cc-197">प्रोजेक्ट व्यय अनुमान (Fin और Ops पर PSA) टेम्पलेट में प्रतिबंधी स्तंभ शामिल करता है जिसका उपयोग इंटीग्रेश के दौरान Project Service Automation से प्राप्त बिलिंग प्रकारों को बदलने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-197">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the billing types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="f81cc-198">यदि आप अपना टेम्पलेट बनाते हैं, तो आपको यह सशर्त कॉलम जोड़ना होगा.</span><span class="sxs-lookup"><span data-stu-id="f81cc-198">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="f81cc-199">**उन्नतक्वेरी और फिल्टरिंग** लिंक का चयन करें और फिर **प्रतिबंधी स्तंभ जोड़ें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f81cc-199">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="f81cc-200">नए स्तंभ के लिए एक नाम दर्ज करें, जैसे **बिलिंग प्रकार**.</span><span class="sxs-lookup"><span data-stu-id="f81cc-200">Enter a name for the new column, such as **BillingType**.</span></span> <span data-ttu-id="f81cc-201">फिर निम्नलिखित शर्त दर्ज करें:</span><span class="sxs-lookup"><span data-stu-id="f81cc-201">Then enter the following condition:</span></span>

<span data-ttu-id="f81cc-202">और अगर **msdyn\_billingtype** = 192350000, तब **प्रभार्य**</span><span class="sxs-lookup"><span data-stu-id="f81cc-202">If **msdyn\_billingtype** = 192350000, then **NonChargeable**</span></span>  
<span data-ttu-id="f81cc-203">और अगर **msdyn\_billingtype** = 192350001, तब **प्रभार्य**</span><span class="sxs-lookup"><span data-stu-id="f81cc-203">else if **msdyn\_billingtype** = 192350001, then **Chargeable**</span></span>  
<span data-ttu-id="f81cc-204">और अगर **msdyn\_billingtype** = 192350002, तब **कॉम्प्लिमेंट्री**</span><span class="sxs-lookup"><span data-stu-id="f81cc-204">else if **msdyn\_billingtype** = 192350002, then **Complimentary**</span></span>  
<span data-ttu-id="f81cc-205">अन्य **उपलब्ध नहीं है**</span><span class="sxs-lookup"><span data-stu-id="f81cc-205">else **NotAvailable**</span></span>

#### <a name="transform-the-transaction-types"></a><span data-ttu-id="f81cc-206">लेन-देन के प्रकारों को बदलना</span><span class="sxs-lookup"><span data-stu-id="f81cc-206">Transform the transaction types</span></span>

<span data-ttu-id="f81cc-207">परियोजना व्यय अनुमान (Fin और Ops के लिए PSA) टेम्पलेट में एक सशर्त स्तंभ शामिल है जिसका उपयोग एकीकरण के दौरान Project Service Automation से प्राप्त बिलिंग प्रकारों को बदलने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="f81cc-207">The Project expense estimates (PSA to Fin and Ops) template includes a conditional column that is used to transform the transaction types that are received from Project Service Automation during the integration.</span></span> <span data-ttu-id="f81cc-208">यदि आप अपना टेम्पलेट बनाते हैं, तो आपको यह सशर्त कॉलम जोड़ना होगा.</span><span class="sxs-lookup"><span data-stu-id="f81cc-208">If you create your own template, you must add this conditional column.</span></span> <span data-ttu-id="f81cc-209">**उन्नतक्वेरी और फिल्टरिंग** लिंक का चयन करें और फिर **प्रतिबंधी स्तंभ जोड़ें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f81cc-209">Select the **Advanced Query and Filtering** link and then select **Add Conditional Column**.</span></span> <span data-ttu-id="f81cc-210">नए कॉलम के लिए एक नाम दर्ज करें, जैसे **TransactionType**.</span><span class="sxs-lookup"><span data-stu-id="f81cc-210">Enter a name for the new column, such as **TransactionType**.</span></span> <span data-ttu-id="f81cc-211">फिर निम्नलिखित शर्त दर्ज करें:</span><span class="sxs-lookup"><span data-stu-id="f81cc-211">Then enter the following condition:</span></span>

<span data-ttu-id="f81cc-212">अगर **msdyn\_transactiontypecode** = 192350000, तब **लागत**</span><span class="sxs-lookup"><span data-stu-id="f81cc-212">If **msdyn\_transactiontypecode** = 192350000, then **Cost**</span></span>  
<span data-ttu-id="f81cc-213">और अगर **msdyn\_transactiontypecode** = 192350005, तब **विक्रय**</span><span class="sxs-lookup"><span data-stu-id="f81cc-213">else if **msdyn\_transactiontypecode** = 192350005, then **Sales**</span></span>  
<span data-ttu-id="f81cc-214">अन्य **शून्य**</span><span class="sxs-lookup"><span data-stu-id="f81cc-214">else **null**</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="f81cc-215">डेटा इंटीग्रेशन में टेम्पलेट मैपिंग</span><span class="sxs-lookup"><span data-stu-id="f81cc-215">Template mapping in Data integration</span></span>

<span data-ttu-id="f81cc-216">निम्नलिखित चित्र डेटा एकीकरण में टेम्पलेट कार्य मानचित्रण का उदाहरण प्रदर्शित करते हैं.</span><span class="sxs-lookup"><span data-stu-id="f81cc-216">The following illustrations show examples of the template task mappings in Data integration.</span></span> <span data-ttu-id="f81cc-217">मानचित्रण फील्ड की जानकारी को प्रदर्शित करता है जिसे Project Service Automation से Finance तक सिन्क्रोनाइज्ड किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="f81cc-217">The mapping shows the field information that will be synchronized from Project Service Automation to Finance.</span></span>

<span data-ttu-id="f81cc-218">[![व्यय अनुमान लेन-देन की टेम्पलेट मैपिंग](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="f81cc-218">[![Template mapping of expense estimate transactions](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)](./media/ExpenseEstimateTransactionRelationshipsMapping.jpg)</span></span>

<span data-ttu-id="f81cc-219">[![व्यय अनुमानों की टेम्पलेट मैपिंग](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="f81cc-219">[![Template mapping of expense estimates](./media/ExpenseEstimatesMapping.jpg)](./media/ExpenseEstimatesMapping.jpg)</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]