---
title: परियोजना आगड़न और वास्तविकों का एकीकरण
description: यह विषय परियोजना आगड़न और वास्तविकों के लिए Project Operations ड्यूल-राइट एकीकरण के बारे में जानकारी प्रदान करता है.
author: sigitac
ms.date: 4/26/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: d8aa1541a3560db175acead1d000895312b299db
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000033"
---
# <a name="project-estimates-and-actuals-integration"></a><span data-ttu-id="c1ce9-103">परियोजना आगड़न और वास्तविकों का एकीकरण</span><span class="sxs-lookup"><span data-stu-id="c1ce9-103">Project estimates and actuals integration</span></span>

<span data-ttu-id="c1ce9-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations_</span><span class="sxs-lookup"><span data-stu-id="c1ce9-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="c1ce9-105">यह विषय परियोजना आगड़न और वास्तविकों के लिए Project Operations ड्यूल-राइट एकीकरण के बारे में जानकारी प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-105">This topic provides information about Project Operations dual-write integration for project estimates and actuals.</span></span>

## <a name="project-estimates"></a><span data-ttu-id="c1ce9-106">परियोजना अनुमान</span><span class="sxs-lookup"><span data-stu-id="c1ce9-106">Project estimates</span></span>

<span data-ttu-id="c1ce9-107">परियोजना श्रम, व्यय, और सामग्री आगड़न Microsoft Dataverse में बनाए और संभाले जाते हैं और लेखांकन उद्देश्यों के लिए Finance and Operations ऐप्स से सिंक्रनाइज़ किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-107">Project labor, expense, and material estimates are created and maintained in Microsoft Dataverse and synchronized to Finance and Operations apps for accounting purposes.</span></span> <span data-ttu-id="c1ce9-108">ऑपरेशन्स बनाना, अपडेट करना और हटाना Finance and Operations ऐप्स के माध्यम से समर्थित नहीं हैं.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-108">Create, update, and delete operations aren't supported through the Finance and Operations apps.</span></span>

<span data-ttu-id="c1ce9-109">आगड़न बनाने को परियोजना के लिए वैध लेखांकन विन्यास की आवश्यकता होती है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-109">Creating estimates requires a valid accounting configuration for the project.</span></span> <span data-ttu-id="c1ce9-110">जो परियोजनाएं अनुबंध लाइनों से जुड़ी होती हैं, उनकी परियोजना लागत और राजस्व प्रोफ़ाइल नियमों में परिभाषित परियोजना लागत और राजस्व प्रोफ़ाइल होनी चाहिए.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-110">Projects that are associated with contract lines must have a valid project cost and revenue profile defined in the Project cost and revenue profile rules.</span></span> <span data-ttu-id="c1ce9-111">अधिक जानकारी के लिए, [बिल करने योग्य परियोजनाओं के लिए लेखांकन कॉन्फ़िगर करें](../project-accounting/configure-accounting-billable-projects.md#configure-project-cost-and-revenue-profile-rules) देखें.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-111">For more information, see [Configure accounting for billable projects](../project-accounting/configure-accounting-billable-projects.md#configure-project-cost-and-revenue-profile-rules).</span></span>

## <a name="labor-estimates"></a><span data-ttu-id="c1ce9-112">श्रम के आगड़न</span><span class="sxs-lookup"><span data-stu-id="c1ce9-112">Labor estimates</span></span>

<span data-ttu-id="c1ce9-113">श्रम के आगड़न परियोजना प्रबंधक या संसाधन प्रबंधक द्वारा बनाये जाते हैं जो परियोजना कार्य को एक सामान्य या नामित संसाधन भी देता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-113">Labor estimates are created by the Project Manager or Resource manager who also assigns a generic or named resource to the project task.</span></span> <span data-ttu-id="c1ce9-114">संसाधन असाइनमेंट रिकॉर्ड की समीक्षा Dataverse में **परियोजना विवरण** पेज पर **संसाधन असाइनमेंट्स** टैब पर की जा सकती है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-114">Resource assignment records can be reviewed on the **Resource Assignments** tab on the **Project Details** page in Dataverse.</span></span> <span data-ttu-id="c1ce9-115">Dataverse के संसाधन असाइनमेंट रिकॉर्ड्स **घंटे के आगड़नों के लिए Project Operations एकीकरण निकाय (msdyn\_resourceassignments)** का उपयोग करते हुए Finance and Operations में घंटे के पूर्वानुमान रिकॉर्ड्स बनाते हैं.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-115">Resource assignment records in Dataverse create hour forecast records in Finance and Operations apps using **Project Operations integration entity for hour estimates (msdyn\_resourceassignments)**.</span></span>

   ![श्रम आगड़न का एकीकरण](./Media/DW4LaborEstimates.png)

<span data-ttu-id="c1ce9-117">ड्यूल-राइट संसाधन असाइनमेंट रिकॉर्ड्स को स्टेजिंग तालिका (**ProjCDSEstimateHoursImport**) से सिंक्रनाइज़ करता है, और फिर घंटे के पूर्वानुमान रिकॉर्ड्स (**ProjForecastEmpl**) बनाने और अपडेट करने के लिए व्यवसाय तर्क का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-117">Dual-write synchronizes resource assignment records to the staging table (**ProjCDSEstimateHoursImport**), and then uses business logic to create and update hour forecast records (**ProjForecastEmpl**).</span></span>

<span data-ttu-id="c1ce9-118">परियोजना लेखाकार **परियोजना प्रबंधन और लेखांकन** > **सभी परियोजनाएं** > **योजना** > **घंटे का पूर्वानुमान** पर जाकर Finance and Operations ऐप्स में बनाए गए पूर्वानुमान घंटे के रिकॉर्ड्स की समीक्षा करता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-118">The Project accountant reviews forecast hour records created in Finance and Operations apps by going to **Project management and accounting** > **All projects** > **Plan** > **Hour forecasts**.</span></span>

## <a name="expense-estimates"></a><span data-ttu-id="c1ce9-119">व्यय अनुमान</span><span class="sxs-lookup"><span data-stu-id="c1ce9-119">Expense estimates</span></span>

<span data-ttu-id="c1ce9-120">व्यय आगड़न परियोजना प्रबंधक द्वारा Dataverse में **परियोजना विवरण** पेज पर **व्यय आगड़न** टैब पर बनाए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-120">Expense estimates are created by the Project manager on the **Expense Estimates** tab on the **Project Details** page in Dataverse.</span></span> <span data-ttu-id="c1ce9-121">व्यय आगड़न रिकॉर्ड्स Dataverse में **आगड़न लाइन** निकाय में संग्रहीत किये जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-121">Expense estimate records are stored in the **Estimate Line** entity in Dataverse.</span></span> <span data-ttu-id="c1ce9-122">इन आगड़न रिकॉर्ड्स में लेनदेन वर्ग, **व्यय** होता है और इन्हें **व्यय आगड़नों के लिए Project Operations एकीकरण निकाय (msdyn\_estimatelines)** का उपयोग करते हुए Finance and Operations ऐप्स में व्यय पूर्वानुमान रिकॉर्ड्स से सिंक्रनाइज़ किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-122">These estimate records have transaction class, **Expense** and are synchronized to expense forecast records in Finance and Operations apps using **Project Operations integration entity for expense estimates (msdyn\_estimatelines)**.</span></span>

   ![व्यय आगड़न एकीकरण](./Media/DW4ExpenseEstimates.png)

<span data-ttu-id="c1ce9-124">ड्यूल-राइट व्यय आगड़न रिकॉर्ड्स को स्टेजिंग तालिका **(ProjCDSEstimateExpenseImport)** से सिंक्रनाइज़ करता है और फिर व्यय पूर्वानुमान रिकॉर्ड्स (**ProjForecastCost**) बनाने और अपडेट करने के लिए व्यवसाय तर्क का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-124">Dual-write synchronizes expense estimate records to the staging table, **ProjCDSEstimateExpenseImport)** and then uses business logic to create and update expense forecast records (**ProjForecastCost**).</span></span> <span data-ttu-id="c1ce9-125">आगड़न लाइनें बिक्री आगड़न और लागत आगड़न रिकॉर्ड्स को अलग-अलग संग्रहीत करती हैं.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-125">Estimate lines store sales estimate and cost estimate records separately.</span></span> <span data-ttu-id="c1ce9-126">Finance and Operations ऐप्स में बिजनेस लॉजिक स्टेजिंग टेबल में इस डिटेल का इस्तेमाल करते हुए सिंगल एक्सपेंस पूर्वानुमान रिकॉर्ड को पॉप्युलेट करता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-126">The business logic in Finance and Operations apps populates a single Expense forecast record using this detail in the staging table.</span></span>

<span data-ttu-id="c1ce9-127">परियोजना लेखाकार **परियोजना प्रबंधन और लेखांकन** > **सभी परियोजनाएं** > **योजना** > **व्यय पूर्वानुमान** पर जाकर Finance and Operations ऐप्स में बनाए गए व्यय पूर्वानुमान के रिकॉर्ड्स की समीक्षा कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-127">The Project accountant can review expense forecast records in Finance and Operations apps by going to **Project management and accounting** > **All projects** > **Plan** > **Expense forecasts**.</span></span>

## <a name="material-estimates"></a><span data-ttu-id="c1ce9-128">सामग्री अनुमान</span><span class="sxs-lookup"><span data-stu-id="c1ce9-128">Material estimates</span></span>

<span data-ttu-id="c1ce9-129">सामग्री के आगड़न परियोजना प्रबधंक द्वारा Dataverse में **परियोजना विवरण** पेज पर **सामग्री आगड़न** टैब में बनाये जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-129">Material estimates are created by the Project manager on the **Material Estimates** tab on the **Project Details** page in Dataverse.</span></span> <span data-ttu-id="c1ce9-130">सामग्री आगड़न के रिकॉर्ड्स Dataverse में **आगड़न लाइन** निकाय में संग्रहीत किये जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-130">Material estimate records are stored in the **Estimate Line** entity in Dataverse.</span></span> <span data-ttu-id="c1ce9-131">इन आगड़न रिकॉर्ड्स में लेनदेन वर्ग, **सामग्री** होता है और इन्हें **सामग्री आगड़नों के लिए परियोजना एकीकरण तालिका (msdyn\_estimatelines)** का उपयोग करते हुए Finance and Operations वित्त और ऑपरेशन्स ऐप्स में आइटम पूर्वानुमान रिकॉर्ड्स से सिंक्रनाइज़ किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-131">These estimate records have the transaction class, **Material** and are synchronized to item forecast records in Finance and Operations apps using **Project integration table for material estimates (msdyn\_estimatelines)**.</span></span>

   ![सामग्री अनुमान एकीकरण](./Media/DW4MaterialEstimates.png)

<span data-ttu-id="c1ce9-133">ड्यूल-राइट सामग्री आगणन रिकॉर्ड्स को स्टेजिंग टेबल **ProjForecastSalesImpor** में सिंक्रनाइज़ करता है, और फिर आइटम पूर्वानुमान रिकॉर्ड्स को बनाने और उनका अद्यतन करने के लिए व्यावसायिक तर्क का उपयोग करता है (**ForecastSale**).</span><span class="sxs-lookup"><span data-stu-id="c1ce9-133">Dual-write synchronizes material estimate records to the staging table **ProjForecastSalesImpor**, and then uses business logic to create and update item forecast records (**ForecastSales**).</span></span> <span data-ttu-id="c1ce9-134">आगड़न लाइनें बिक्री आगड़न और लागत आगड़न रिकॉर्ड्स को अलग-अलग संग्रहीत करती हैं.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-134">Estimate lines store sales estimate and cost estimate records separately.</span></span> <span data-ttu-id="c1ce9-135">Finance and Operations एप्स में व्यावसायिक तर्क स्टेजिंग टेबल में इस विवरण का उपयोग करके एकल आइटम पूर्वानुमान रिकॉर्ड को पॉप्युलेट करता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-135">The business logic in Finance and Operations apps populates a single Item forecast record using this detail in the staging table.</span></span>

<span data-ttu-id="c1ce9-136">परियोजना लेखाकार **परियोजना प्रबंधन और लेखांकन** > **सभी परियोजनाएं** > **योजना** > **आइटम र्वानुमान** पर जाकर Finance and Operations एप्स में आइटम पूर्वानुमान रिकॉर्ड्स की समीक्षा कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-136">The Project accountant can review item forecast records in Finance and Operations apps by going to **Project management and accounting** > **All projects** > **Plan** > **Item forecasts**.</span></span>

## <a name="project-actuals"></a><span data-ttu-id="c1ce9-137">परियोजना वास्तविक</span><span class="sxs-lookup"><span data-stu-id="c1ce9-137">Project actuals</span></span>

<span data-ttu-id="c1ce9-138">समय, व्यय, सामग्री, और बिलिंग गतिविधि के आधार पर Dataverse में परियोजना वास्तविक बनाए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-138">Project actuals are created in Dataverse, based on time, expense, material, and billing activity.</span></span> <span data-ttu-id="c1ce9-139">मात्रा, लागत मूल्य, बिक्री मूल्य, और परियोजना सहित इन लेनदेन के सभी परिचालन गुण इस Dataverse इकाई में कैप्चर किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-139">All operational attributes of these transactions including quantity, cost price, sales price, and project are captured in this Dataverse entity.</span></span> <span data-ttu-id="c1ce9-140">अधिक जानकारी के लिए, [वास्तविक](../actuals/actuals-overview.md) देखें.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-140">For more information, see [Actuals](../actuals/actuals-overview.md).</span></span> <span data-ttu-id="c1ce9-141">डाउनस्ट्रीम लेखांकन के लिए वास्तविक रिकॉर्ड को Finance and Operations एप्लिकेशन के लिए से सिंक्रनाइज़ किए जाते हैं ड्यूल-राइट तालिका मानचित्र **Project Operations एकीकरण वास्तविक (msdyn\_actuals)**.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-141">Actual records are synchronized to Finance and Operations apps using the dual-write table map **Project Operations integration actuals (msdyn\_actuals)** for downstream accounting.</span></span>

   ![वास्तविक एकीकरण](./Media/DW4Actuals.png)

<span data-ttu-id="c1ce9-143">**Project Operations एकीकरण वास्तविक** तालिका मानचित्र, विशेषता **स्किप सिंक (केवल आंतरिक उपयोग)** **गलत** पर सेट के साथ Dataverse में  **वास्तविक** इकाई के सभी रिकॉर्ड्स को सिंक्रोनाइज़ करता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-143">The **Project Operations integration actuals** table map synchronizes all the records from the **Actuals** entity in Dataverse, with the attribute **Skip Sync (internal use only)** set to **False**.</span></span> <span data-ttu-id="c1ce9-144">जब रिकॉर्ड बनाया जाता है तब यह विशेषता मान Dataverse में स्वचालित रूप से सेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-144">This attribute value is set in Dataverse automatically when the record is created.</span></span> <span data-ttu-id="c1ce9-145">उदाहरण जहां यह विशेषता **सही** पर सेट है:</span><span class="sxs-lookup"><span data-stu-id="c1ce9-145">Examples where this attribute is set to **True** are:</span></span>

  - <span data-ttu-id="c1ce9-146">इंटरकंपनी लेनदेन के लिए परियोजना लागत के वास्तविक आंकड़े.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-146">Project cost actuals for intercompany transactions.</span></span> <span data-ttu-id="c1ce9-147">अधिक जानकारी के लिए, [इंटरकंपनी लेनदेन बनाएं](../project-accounting/create-intercompany-transactions.md) देखें.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-147">For more information, see [Create intercompany transactions](../project-accounting/create-intercompany-transactions.md).</span></span> <span data-ttu-id="c1ce9-148">इन रिकॉर्ड्स को छोड़ दिया जाता है क्योंकि प्रणाली इंटरकंपनी विक्रेता चालान पोस्ट होने पर Finance and Operations ऐप्स में परियोजना लागत का वास्तविक आंकड़ा पुनः निर्मित करती है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-148">These records are skipped because the system recreates the project cost actual in Finance and Operations apps when the intercompany vendor invoice is posted.</span></span>
  - <span data-ttu-id="c1ce9-149">प्रोफार्मा चालान की पुष्टि होने पर नकारात्मक बिल नहीं किये गए बिक्री रिकॉर्ड निर्मित होते हैं.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-149">Negative unbilled sales records created when the proforma invoice is confirmed.</span></span> <span data-ttu-id="c1ce9-150">इन रिकॉर्ड्स को छोड़ दिया जाता है क्योंकि Finance and Operations ऐप्स में परियोजना सबलेजर चालान बनाने पर बिल नहीं किये गए बिक्री रिकॉर्ड को उल्टा नहीं करता है, बल्कि पूरे चालानों की स्थिति को बदल देता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-150">These records are skipped because the project subledger in Finance and Operations apps doesn't reverse the unbilled sales record at invoicing but changes the status to fully invoiced.</span></span>

<span data-ttu-id="c1ce9-151">ड्यूल-राइट तालिका मानचित्र वास्तविक रिकॉर्ड्स को स्टेजिंग तालिका, **ProjCDSActualsImport** से सिंक्रनाइज़ करता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-151">The dual-write table map synchronizes the actuals records to the staging table, **ProjCDSActualsImport**.</span></span> <span data-ttu-id="c1ce9-152">इन रिकॉर्ड्स को आवधिक प्रक्रिया, **स्टेजिंग तालिका से आयात करें** द्वारा Project Operations एकीकरण पत्रिका लाइनों और परियोजना चालान प्रस्ताव लाइनों को बनाते समय उपयोग किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-152">These records are processed by the periodic process **Import from staging table** when creating Project Operations integration journal lines and project invoice proposal lines.</span></span> <span data-ttu-id="c1ce9-153">अधिक जानकारी के लिए, [Project Operations में एकीकरण पत्रिका](../project-accounting/project-operations-integration-journal.md) देखें.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-153">For more information, see [Integration journal in Project Operations](../project-accounting/project-operations-integration-journal.md).</span></span>

<span data-ttu-id="c1ce9-154">Dataverse **लेन-देन कनेक्शन** निकाय में परियोजना के वास्तविक लेनदेन के बीच के लिंक को भी कैप्चर करता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-154">Dataverse also captures the links between the project actual transactions in the **Transaction connection** entity.</span></span> <span data-ttu-id="c1ce9-155">अधिक जानकारी के लिए, [वास्तविक आंकड़ों को मूल रिकॉर्ड से लिंक करें](../actuals/linkingactuals.md) देखें.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-155">For more information, see [Link actuals to original records](../actuals/linkingactuals.md).</span></span> <span data-ttu-id="c1ce9-156">वास्तविक लेनदेन के बीच लिंक्स ड्यूल-राइट तालिका मानचित्र, **परियोजना लेनदेन संबंधों के लिए एकीकरण निकाय (msdyn\_transactionconnections)** का उपयोग करते हुए Finance and Operations ऐप्स से भी सिंक्रनाइज़ किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-156">Links between actual transactions are also synchronized to Finance and Operations apps using the dual-write table map, **Integration entity for project transaction relationships (msdyn\_transactionconnections)**.</span></span> <span data-ttu-id="c1ce9-157">इन रिकॉर्ड्स को आवधिक प्रक्रिया, **स्टेजिंग तालिका से आयात करें** द्वारा Project Operations एकीकरण पत्रिका लाइनों और परियोजना चालान प्रस्ताव लाइनों को बनाते समय उपयोग किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-157">These records are used by the periodic process, **Import from staging table** when creating Project Operations integration journal lines and Project invoice proposal lines.</span></span>

<span data-ttu-id="c1ce9-158">एक Project Operations एकीकरण पत्रिका और एक परियोजना चालान प्रस्ताव पोस्ट करने से स्टेजिंग तालिका **ProjCDSActualsImport** में संबंधित रिकॉर्ड में एक अद्यतन ट्रिगर हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-158">Posting a Project Operations integration journal and a project invoice proposal triggers an update in respective records in the staging table, **ProjCDSActualsImport**.</span></span> <span data-ttu-id="c1ce9-159">प्रणाली वास्तविक लेनदेनों के लिए निम्नलिखित लेखांकन विशेषताओं को कैप्चर और रिकॉर्ड करती है:</span><span class="sxs-lookup"><span data-stu-id="c1ce9-159">The system captures and records the following accounting attributes for actuals transactions:</span></span>

- <span data-ttu-id="c1ce9-160">लेखांकन मुद्रा राशि</span><span class="sxs-lookup"><span data-stu-id="c1ce9-160">Accounting currency amount</span></span>
- <span data-ttu-id="c1ce9-161">विनिमय दर</span><span class="sxs-lookup"><span data-stu-id="c1ce9-161">Exchange rate</span></span>
- <span data-ttu-id="c1ce9-162">वाउचर संख्या</span><span class="sxs-lookup"><span data-stu-id="c1ce9-162">Voucher number</span></span>
- <span data-ttu-id="c1ce9-163">विक्रय कर राशि</span><span class="sxs-lookup"><span data-stu-id="c1ce9-163">Sales tax amount</span></span>

<span data-ttu-id="c1ce9-164">**Project Operations एकीकरण वास्तविक आकड़े** टेबल नक्शा संबंधित वास्तविक आकड़ों के रिकॉर्ड्स को Dataverse में इस जानकारी के साथ अपडेट करता है.</span><span class="sxs-lookup"><span data-stu-id="c1ce9-164">The **Project Operations integration actuals** table map updates respective actuals records in Dataverse with this information.</span></span>