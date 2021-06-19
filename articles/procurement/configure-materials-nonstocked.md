---
title: स्टॉक-नहीं की गयी सामग्री और लंबित विक्रेता चालान कॉन्फ़िगर करें
description: यह विषय बताता है कि स्टॉक-नहीं की गयी सामग्री और लंबित विक्रेता चालान को कैसे सक्षम किया जाए.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 24418f3aad8356bd209eef7487a47a3870bce10f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993913"
---
# <a name="configure-non-stocked-materials-and-pending-vendor-invoices"></a><span data-ttu-id="b2b59-103">स्टॉक-नहीं की गयी सामग्री और लंबित विक्रेता चालान कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="b2b59-103">Configure non-stocked materials and pending vendor invoices</span></span>

<span data-ttu-id="b2b59-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations_</span><span class="sxs-lookup"><span data-stu-id="b2b59-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

## <a name="minimum-version-requirement"></a><span data-ttu-id="b2b59-105">आवश्यक न्यूनतम संस्करण</span><span class="sxs-lookup"><span data-stu-id="b2b59-105">Minimum version requirement</span></span>

<span data-ttu-id="b2b59-106">Dynamics 365 Project Operations के लिए स्टॉक-नहीं की गयी सामग्री और लंबित विक्रेता चालान का उपयोग करने के लिए स्टॉक-नहीं की गयी / संसाधन आधारित परिदृश्यों के निम्न संस्करणों की आवश्यकता है:</span><span class="sxs-lookup"><span data-stu-id="b2b59-106">Using non-stocked materials and pending vendor invoices for Dynamics 365 Project Operations non-stocked/resource based scenarios requires the following versions:</span></span>

<span data-ttu-id="b2b59-107">Dynamics 365 Dataverse समाधान:</span><span class="sxs-lookup"><span data-stu-id="b2b59-107">Dynamics 365 Dataverse solutions:</span></span>

- <span data-ttu-id="b2b59-108">Project Operations - 4.9.0.221 या उच्चतर</span><span class="sxs-lookup"><span data-stu-id="b2b59-108">Project Operations – 4.9.0.221 or higher</span></span>
- <span data-ttu-id="b2b59-109">ड्यूल-राइट एप्लिकेशन Orchestration समाधान - 2.2.2.23 या उच्चतर</span><span class="sxs-lookup"><span data-stu-id="b2b59-109">Dual-write application orchestration solution - 2.2.2.23 or higher</span></span>

<span data-ttu-id="b2b59-110">Dynamics 365 Finance:</span><span class="sxs-lookup"><span data-stu-id="b2b59-110">Dynamics 365 Finance:</span></span>
- <span data-ttu-id="b2b59-111">10.0.18 (10.0.793.52) या उच्चतर.</span><span class="sxs-lookup"><span data-stu-id="b2b59-111">10.0.18 (10.0.793.52) or higher.</span></span> <span data-ttu-id="b2b59-112">सुनिश्चित करें कि आपका वित्त वातावरण वर्तमान है और न्यूनतम संस्करण आवश्यकताओं को पूरा करने के लिए सभी गुणवत्ता अद्यतन लागू किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="b2b59-112">Make sure that your Finance environment is current and all quality updates are applied to meet the minimum version requirements.</span></span>

## <a name="run-dual-write-maps-for-non-stocked-materials-and-vendor-invoice-integration"></a><span data-ttu-id="b2b59-113">स्टॉक-नहीं की गयी सामग्री और विक्रेता चालान एकीकरण के लिए ड्यूल-राइट मानचित्र चलाएँ</span><span class="sxs-lookup"><span data-stu-id="b2b59-113">Run Dual-write maps for non-stocked materials and vendor invoice integration</span></span>

<span data-ttu-id="b2b59-114">यह अनुभाग स्टॉक-नहीं की गयी सामग्री और विक्रेता के चालान के लिए आवश्यक नक्शों के बारे में जानकारी देता है.</span><span class="sxs-lookup"><span data-stu-id="b2b59-114">This section provides information about specific the maps required for non-stocked materials and vendor invoices.</span></span> <span data-ttu-id="b2b59-115">यह जांच लें कि [नए वातावरण प्रावधान](../environment/resource-provision-new-environment.md#run-project-operations-dual-write-maps) विषय में सूचीबद्ध पूर्वापेक्षित मानचित्र आपके पर्यावरण पर चल रहे हैं.</span><span class="sxs-lookup"><span data-stu-id="b2b59-115">Verify that the prerequisite maps listed in the [Provision a new environment](../environment/resource-provision-new-environment.md#run-project-operations-dual-write-maps) topic are running on your environment.</span></span>

1. <span data-ttu-id="b2b59-116">Lifecycle Services (LCS) पर जाएं, अपने LCS प्रोजेक्ट पर जाएं, और **पर्यावरण विवरण** पृष्ठ पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="b2b59-116">Go to Lifecycle Services (LCS), navigate to your LCS project, and go to the **Environment details** page.</span></span>
2. <span data-ttu-id="b2b59-117">**Common Data Service पर्यावरण जानकारी** अनुभाग में, **ऐप्स के लिए CDS से लिंक करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-117">In the **Common Data Service Environment Information** section, select **Link to CDS for Apps**.</span></span> <span data-ttu-id="b2b59-118">आपके द्वारा लिंक चुनने के बाद, आप मैपिंग में निकायों की सूची पर रिडायरेक्ट हो जाएंगे।</span><span class="sxs-lookup"><span data-stu-id="b2b59-118">After you select the link, you will be redirected to the list of entities in the mappings.</span></span>
3. <span data-ttu-id="b2b59-119">सुनिश्चित करें कि निम्नलिखित मानचित्र चल रहे हैं.</span><span class="sxs-lookup"><span data-stu-id="b2b59-119">Make sure the following maps are running.</span></span> <span data-ttu-id="b2b59-120">यदि वे नहीं चल रहे हैं, तो उन्हें शुरू करें और सभी संबंधित तालिका मानचित्रों को शामिल करना सुनिश्चित करें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-120">If they aren't running, start them and make sure to include all related table maps.</span></span>

    - <span data-ttu-id="b2b59-121">CDS द्वारा जारी अलग-अलग उत्पाद (उत्पाद)</span><span class="sxs-lookup"><span data-stu-id="b2b59-121">CDS released distinct products (products)</span></span>
    - <span data-ttu-id="b2b59-122">विक्रेता v2 (msdyn_vendors)</span><span class="sxs-lookup"><span data-stu-id="b2b59-122">Vendors v2 (msdyn_vendors)</span></span>
    - <span data-ttu-id="b2b59-123">सामग्री आगणन के लिए Project Operations तालिका (msdyn_estimatelines)</span><span class="sxs-lookup"><span data-stu-id="b2b59-123">Project Operations table for material estimates (msdyn_estimatelines)</span></span>
    - <span data-ttu-id="b2b59-124">Project Operations एकीकरण परियोजना विक्रेता चालान निर्यात इकाई (msdyn_projectvendorinvoices)</span><span class="sxs-lookup"><span data-stu-id="b2b59-124">Project Operations integration project vendor invoice export entity (msdyn_projectvendorinvoices)</span></span>
    - <span data-ttu-id="b2b59-125">Project Operations एकीकरण परियोजना विक्रेता चालान लाइन निर्यात इकाई (msdyn_projectvendorinvoicelines)</span><span class="sxs-lookup"><span data-stu-id="b2b59-125">Project Operations integration project vendor invoice line export entity (msdyn_projectvendorinvoicelines)</span></span>
    - <span data-ttu-id="b2b59-126">Project Operations एकीकरण वास्तविक (msdyn_actuals).</span><span class="sxs-lookup"><span data-stu-id="b2b59-126">Project Operations integration actuals (msdyn_actuals).</span></span> <span data-ttu-id="b2b59-127">सुनिश्चित करें कि आप मानचित्र संस्करण 1.0.0.14 या उससे उच्चतर चला रहे हैं.</span><span class="sxs-lookup"><span data-stu-id="b2b59-127">Make sure you are running map version 1.0.0.14 or higher.</span></span> <span data-ttu-id="b2b59-128">आप **ड्यूअल-राइट** पृष्ठ पर **संस्करण** कॉलम में मानचित्र का सक्रिय संस्करण देख सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="b2b59-128">You can see the active version of the map in the **Version** column on the **Dual Write** page.</span></span> <span data-ttu-id="b2b59-129">**टेबल मैप संस्करण** का चयन करके मैप का एक नया संस्करण सक्रिय कर सकते हैं और फिर चयनित संस्करण को सहेज सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="b2b59-129">You can activate a new version of the map by selecting **Table map version** and then saving the selected version.</span></span>

<span data-ttu-id="b2b59-130">यदि आप मानक डेमो डेटा का उपयोग कर रहे हैं, तो आपको प्रारंभिक सिंक के साथ निम्नलिखित इकाई मानचित्र को रोककर पुनः आरंभ करने की आवश्यकता भी हो सकती है:</span><span class="sxs-lookup"><span data-stu-id="b2b59-130">If you are using standard demo data, you might also need to stop and restart the following entity maps with initial sync:</span></span>
  - <span data-ttu-id="b2b59-131">भुगतान के दिन CDS V2 (msdyn_paymentdays)</span><span class="sxs-lookup"><span data-stu-id="b2b59-131">Payment days CDS V2 (msdyn_paymentdays)</span></span>
  - <span data-ttu-id="b2b59-132">भुगतान शड्यूल (msdyn_paymentschedules)</span><span class="sxs-lookup"><span data-stu-id="b2b59-132">Payment schedule (msdyn_paymentschedules)</span></span>
  - <span data-ttu-id="b2b59-133">भुगतान की शर्तें (msdyn_paymentterms)</span><span class="sxs-lookup"><span data-stu-id="b2b59-133">Terms of payment (msdyn_paymentterms)</span></span>
  - <span data-ttu-id="b2b59-134">विक्रेता समूह (msdyn_vendorgroups)</span><span class="sxs-lookup"><span data-stu-id="b2b59-134">Vendor groups (msdyn_vendorgroups)</span></span>
  - <span data-ttu-id="b2b59-135">इकाइयाँ (uom)</span><span class="sxs-lookup"><span data-stu-id="b2b59-135">Units (uom)</span></span>

> [!NOTE]
> <span data-ttu-id="b2b59-136">मौजूदा डेमो डेटा सेट में कुछ रिकॉर्ड्स के लिए विक्रेता समूहों और इकाइयों के लिए प्रारंभिक सिंक विफल हो सकता है.</span><span class="sxs-lookup"><span data-stu-id="b2b59-136">The initial sync for vendor groups and units might fail for a few records in the existing demo data set.</span></span> <span data-ttu-id="b2b59-137">आप विफलताओं को अनदेखा कर सकते हैं क्योंकि वे आपको Project Operations के साथ डेमो डेटा का उपयोग करने से नहीं रोकेंगे.</span><span class="sxs-lookup"><span data-stu-id="b2b59-137">You can ignore the failures as they won't prevent you from using demo data with Project Operations.</span></span>

## <a name="configure-prerequisites-in-dataverse"></a><span data-ttu-id="b2b59-138">Dataverse में पूर्वापेक्षाएँ कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="b2b59-138">Configure prerequisites in Dataverse</span></span>

### <a name="activate-workflow-to-create-accounts-based-on-vendor-entity"></a><span data-ttu-id="b2b59-139">विक्रेता इकाई के आधार पर खाते बनाने के लिए वर्कफ़्लो सक्रिय करें</span><span class="sxs-lookup"><span data-stu-id="b2b59-139">Activate workflow to create accounts based on vendor entity</span></span>

<span data-ttu-id="b2b59-140">Dual Write Orchestration समाधान [विक्रेता मास्टर एकीकरण](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/vendor-mapping.md) प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="b2b59-140">The Dual Write Orchestration solution provides [Vendors master integration](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/vendor-mapping.md).</span></span> <span data-ttu-id="b2b59-141">इस सुविधा के लिए एक पूर्व शर्त के रूप में, विक्रेता डेटा को **खाते** इकाई में बनाया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="b2b59-141">As a prerequisite for this feature, vendor data must be created in the **Accounts** entity.</span></span> <span data-ttu-id="b2b59-142">[विक्रेता डिजाइनों के बीच स्विच करें](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/vendor-switch.md#use-the-extended-vendor-design-for-vendors-of-the-organization-type) में दिए गए विवरण के अनुसार **खाता** तालिका में विक्रेता बनाने के लिए एक टेम्पलेट वर्कफ़्लो प्रक्रिया को सक्रिय करें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-142">Activate a template workflow process to create vendors in the **Accounts** table as described in [Switch between vendor designs](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/vendor-switch.md#use-the-extended-vendor-design-for-vendors-of-the-organization-type).</span></span>

### <a name="set-products-to-be-created-as-active"></a><span data-ttu-id="b2b59-143">उत्पादों को सक्रिय के रूप में बनाए जाने के लिए सेट करें</span><span class="sxs-lookup"><span data-stu-id="b2b59-143">Set products to be created as active</span></span>

<span data-ttu-id="b2b59-144">स्टॉक-नहीं की गयी सामग्री को वित्त में **जारी किए गए उत्पाद** के रूप में कॉन्फ़िगर किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="b2b59-144">Non-stocked materials must be configured as **Released products** in Finance.</span></span> <span data-ttu-id="b2b59-145">Dual Write Orchestration सॉल्यूशन एक आउट-ऑफ-द-बॉक्स प्रदान करता है [Dataverse उत्पाद कैटलॉग के लिए उत्पादों का एकीकरण](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/product-mapping.md).</span><span class="sxs-lookup"><span data-stu-id="b2b59-145">The Dual Write Orchestration solution provides an out-of-the-box [Released products integration to Dataverse Product catalog](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/product-mapping.md).</span></span> <span data-ttu-id="b2b59-146">डिफ़ॉल्ट रूप से, वित्त से उत्पादों को एक ड्राफ्ट स्थिति में Dataverse से सिंक्रनाइज़ किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="b2b59-146">By default, products from Finance are synchronized to Dataverse in a draft state.</span></span> <span data-ttu-id="b2b59-147">उत्पाद को एक सक्रिय स्थिति से सिंक्रनाइज़ करने के लिए, ताकि इसका उपयोग सीधे सामग्री उपयोगिता दस्तावेजों या लंबित विक्रेता चालानों में किया जा सके,**System**  > **Administration** >  **System administration** >  **System settings**, and on the **Sales** tab, set **Create products in active state** to **Yes** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="b2b59-147">To synchronize the product to an active state so that it can be directly used in material usage documents or pending vendor invoices, go to **System** > **Administration** > **System administration** > **System settings**, and on the **Sales** tab, set **Create products in active state** to **Yes**.</span></span>

## <a name="configure-prerequisites-in-finance"></a><span data-ttu-id="b2b59-148">वित्त में पूर्व आवश्यक शर्तें कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="b2b59-148">Configure prerequisites in Finance</span></span>

### <a name="enable-the-feature-key-for-pending-vendor-invoices"></a><span data-ttu-id="b2b59-149">लंबित विक्रेता चालानों के लिए सुविधा को सक्षम करें</span><span class="sxs-lookup"><span data-stu-id="b2b59-149">Enable the feature key for pending vendor invoices</span></span>

<span data-ttu-id="b2b59-150">लंबित विक्रेता चालान लाइनों पर परियोजना विवरण जोड़ने के लिए कार्यक्षमता को सक्षम करने के लिए निम्न चरणों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-150">Complete the following steps to enable functionality to add project details on pending vendor invoice lines.</span></span>

1. <span data-ttu-id="b2b59-151">वित्त में, **सुविधा प्रबंधन** कार्यक्षेत्र पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="b2b59-151">In Finance, go to the **Feature Management** workspace.</span></span>
2. <span data-ttu-id="b2b59-152">सुविधा सूची में, **संसाधन आधारित/स्टॉक-नहीं किए गए परिदृश्यों के लिए Project Operations पर लंबित विक्रेता चालानों को ढूंढें** और **सक्षम करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-152">In the feature list, find **Enable pending vendor invoices on Project Operations for resource based/non-stocked scenarios** feature and select **Enable**.</span></span>

### <a name="define-category-groups-and-project-categories-for-items"></a><span data-ttu-id="b2b59-153">आइटम्स के लिए श्रेणी समूहों और परियोजना श्रेणियों को परिभाषित करें</span><span class="sxs-lookup"><span data-stu-id="b2b59-153">Define category groups and project categories for items</span></span>

<span data-ttu-id="b2b59-154">**आइटम** लेनदेन प्रकार के लिए कम से कम एक श्रेणी समूह और इस समूह का उपयोग करके कम से कम एक परियोजना श्रेणी कॉन्फ़िगर करें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-154">Configure at least one category group for the **Item** transaction type , and at least one project category using this group.</span></span> <span data-ttu-id="b2b59-155">अधिक जानकारी के लिए, [Configure project categories](../project-accounting/configure-project-categories.md#category-groups) देखें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-155">For more information, see [Configure project categories](../project-accounting/configure-project-categories.md#category-groups).</span></span>

<span data-ttu-id="b2b59-156">परियोजना लागत और राजस्व प्रोफाइल की समीक्षा करें, और आइटम लेनदेन के लिए लेज़र पोस्टिंग सेटअप को कॉन्फ़िगर करें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-156">Review the project cost and revenue profiles, and configure ledger posting setup for item transactions.</span></span> <span data-ttu-id="b2b59-157">अधिक जानकारी के लिए, [Configure accounting for billable projects](../project-accounting/configure-accounting-billable-projects.md) देखें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-157">For more information, see [Configure accounting for billable projects](../project-accounting/configure-accounting-billable-projects.md).</span></span>

### <a name="set-up-a-write-in-product"></a><span data-ttu-id="b2b59-158">राइट-इन उत्पाद सेट करें</span><span class="sxs-lookup"><span data-stu-id="b2b59-158">Set up a write-in product</span></span>

<span data-ttu-id="b2b59-159">Project Operations में, आप रिलीज़ किए गए उत्पाद कैटलॉग में और राइट-इन उत्पादों के लिए कॉन्फ़िगर किए गए कैटलॉग उत्पादों के लिए सामग्री आगणन और उपयोगिता रिकॉर्ड कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="b2b59-159">In Project Operations, you can record material estimates and usage for catalog products that are configured in the released product catalog and for write-in products.</span></span> <span data-ttu-id="b2b59-160">राइट-इन उत्पादों का उपयोग करने के लिए एक एकल जारी उत्पाद की आवश्यकता होती है जो इस उद्देश्य के लिए वित्त में कॉन्फ़िगर किया गया हो.</span><span class="sxs-lookup"><span data-stu-id="b2b59-160">Using write-in products requires a single released product that's configured in Finance for this purpose.</span></span> <span data-ttu-id="b2b59-161">राइट-इन उत्पाद को कॉन्फ़िगर करने के लिए निम्न चरणों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-161">Complete the following steps to configure a write-in product.</span></span> <span data-ttu-id="b2b59-162">संसाधन/स्टॉक-नहीं किए गए परिदृश्यों के लिए Project Operations का उपयोग कर रहे प्रत्येक कानूनी इकाई में इन चरणों को दोहराएं.</span><span class="sxs-lookup"><span data-stu-id="b2b59-162">Repeat these steps in each legal entity that is using Project Operations for resource/non-stocked scenarios.</span></span>

1. <span data-ttu-id="b2b59-163">वित्त में, **उत्पाद जानकारी प्रबंधन** >  **उत्पाद** >  **जारी किए गए उत्पादों** पर जाएं, और **नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-163">In Finance, go to **Product Information Management** > **Products** > **Released products**, and select **New**.</span></span>
2. <span data-ttu-id="b2b59-164">**उत्पाद प्रकार** फ़ील्ड में, **आइटम** चुनें और **उत्पाद उपप्रकार** फ़ील्ड में, **उत्पाद** चुनें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-164">In the **Product type** field, select **Item** and in the **Product subtype** field, select **Product**.</span></span>
3. <span data-ttu-id="b2b59-165">उत्पाद का नंबर (WRITEIN) और उत्पाद का नाम (राइट-इन उत्पाद) दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-165">Enter the product number (WRITEIN) and the product name (Write-in Product).</span></span>
4. <span data-ttu-id="b2b59-166">आइटम मॉडल समूह का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-166">Select  the item model group.</span></span> <span data-ttu-id="b2b59-167">सुनिश्चित करें कि आपके द्वारा चुने गए आइटम मॉडल समूह में **इन्वेंटरी पॉलिसी स्टॉक किए गए उत्पाद** फ़ील्ड **गलत** पर सेट है.</span><span class="sxs-lookup"><span data-stu-id="b2b59-167">Make sure that the item model group you select has the **Inventory policy Stocked product** field set to **False**.</span></span>
5. <span data-ttu-id="b2b59-168">**आइटम समूह**, **संग्रहण आयाम समूह**, और **ट्रैकिंग आयाम समूह** फ़ील्ड्स में मानों का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-168">Select values in the **Item group**, **Storage dimension group**, and **Tracking dimension group** fields.</span></span> <span data-ttu-id="b2b59-169">केवल **साइट** के लिए **संग्रहण आयाम** का उपयोग करें, और कोई ट्रैकिंग आयाम सेट न करें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-169">Use the **Storage dimension** for **Site** only, and do not set any tracking dimensions.</span></span>
6. <span data-ttu-id="b2b59-170">**इन्वेंटरी यूनिट**, **खरीद यूनिट**, और **विक्रय यूनिट** फ़ील्ड में मानों का चयन करें, और फिर अपने परिवर्तनों को सहेजें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-170">Select values in the **Inventory unit**, **Purchase unit**, and **Sales unit** field, and then save your changes.</span></span>
7. <span data-ttu-id="b2b59-171">**योजना** टैब में, डिफ़ॉल्ट ऑर्डर सेटिंग्स सेट करें, और **इन्वेंटरी** टैब पर, डिफ़ॉल्ट साइट और वेयरहाउस सेट करें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-171">In the **Plan** tab, set the default order settings, and on the **Inventory** tab, set the default site and warehouse.</span></span>
8. <span data-ttu-id="b2b59-172">**परियोजना प्रबंधन और लेखांकन** > **सेटअप** > **परियोजना प्रबंधन और लेखांकन मापदंड** पर जाएं और **Dynamics 365 Dataverse पर Project Operations** खोलें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-172">Go to **Project management and accounting** > **Setup** > **Project management and accounting parameters** and open **Project Operations on Dynamics 365 Dataverse**.</span></span> 
9. <span data-ttu-id="b2b59-173">**सामग्री**  टैब पर, **राइट-इन उत्पाद** फ़ील्ड में, आपके द्वारा बनाए गए उत्पाद का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-173">On the **Materials** tab, in the **Write-in product** field, select the product you created.</span></span>
10. <span data-ttu-id="b2b59-174">आपके Dataverse परिवेश में, साइट मानचित्र में, **उत्पाद** इकाई खोलें और राइट-इन उत्पाद रिकॉर्ड ढूंढें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-174">In your Dataverse environment, in the site map, open the **Products** entity and find the write-in product record.</span></span> 
11. <span data-ttu-id="b2b59-175">रिकॉर्ड विवरण खोलें और उत्पाद स्थिति को **सेवामुक्त** पर सेट करें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-175">Open the record details and set product state to **Retired**.</span></span> <span data-ttu-id="b2b59-176">यह उत्पाद स्थिति किसी को भी गलती से इस रिकॉर्ड को सीधे सामग्री आगणन और उपयोगिता दस्तावेजों में उपयोग करने से रोकती है.</span><span class="sxs-lookup"><span data-stu-id="b2b59-176">This product state prevents anyone from accidentally using this record directly in material estimates and usage documents.</span></span>

### <a name="set-up-a-procurement-integration-account"></a><span data-ttu-id="b2b59-177">एक खरीद एकीकरण खाता सेट अप करें</span><span class="sxs-lookup"><span data-stu-id="b2b59-177">Set up a procurement integration account</span></span>

<span data-ttu-id="b2b59-178">किसी परियोजना से संबन्धित लाइन्स के साथ लंबित विक्रेता चालान पोस्ट करते समय खरीद एकीकरण खाते को क्लियरिंग खाते की तरह इस्तेमाल किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="b2b59-178">The procurement integration account is used as a clearing account when posting a pending vendor invoice with lines attributed to a project.</span></span>

<span data-ttu-id="b2b59-179">जब सिस्टम लंबित विक्रेता चालान पोस्ट करता है, तो इस खाते का उपयोग परियोजना लागत राशि के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="b2b59-179">When the system posts a pending vendor invoice, this account is used for the project cost amount.</span></span> <span data-ttu-id="b2b59-180">विक्रेता चालान विवरण को Dataverse में संसाधित किया जाता है, और तदनुरूपी एक परियोजना वास्तविक बनाई जाती है.</span><span class="sxs-lookup"><span data-stu-id="b2b59-180">The vendor invoice details are processed in Dataverse, and a corresponding project actual is created.</span></span> <span data-ttu-id="b2b59-181">परियोजना वास्तविक से प्राप्त जानकारी को Project Operations एकीकरण जरनल में जोड़ा जाता है.</span><span class="sxs-lookup"><span data-stu-id="b2b59-181">The information from the project actual is added to the Project Operations Integration journal.</span></span> <span data-ttu-id="b2b59-182">जब आप एकीकरण जरनल पोस्ट करते हैं, तो खरीद एकीकरण खाते से राशि दे दी जाती है और परियोजना लागत में दर्ज की जाती है.</span><span class="sxs-lookup"><span data-stu-id="b2b59-182">When you post the integration journal, the amount is cleared from the procurement integration account and recorded to the project cost.</span></span>

1. <span data-ttu-id="b2b59-183">खरीद एकीकरण खाता सेट करने के लिए, **परियोजना प्रबंधन और लेखांकन** > **सेटअप** > **परियोजना प्रबंधन और लेखा मापदंड** पर जाएं, और **Dynamics 365 Dataverse पर Project Operations** खोलें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-183">To set up the procurement integration account, go to **Project management and accounting** > **Setup** > **Project management and accounting parameters**, and open **Project Operations on Dynamics 365 Dataverse**.</span></span> 
2. <span data-ttu-id="b2b59-184">**सामग्री** टैब का चयन करें, और **खरीद एकीकरण खाते** फील्ड में एक मान का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-184">Select the **Materials** tab, and select a value in the **Procurement integration account** field.</span></span>

#### <a name="set-up-project-category-defaults-for-an-item"></a><span data-ttu-id="b2b59-185">किसी आइटम के लिए परियोजना श्रेणी डिफ़ॉल्ट सेट करें</span><span class="sxs-lookup"><span data-stu-id="b2b59-185">Set up project category defaults for an item</span></span>

1. <span data-ttu-id="b2b59-186">वित्त में, **परियोजना प्रबंधन और लेखांकन** > **सेटअप** > **परियोजना प्रबंधन और लेखा मापदंडों** पर जाएं, और **Dynamics 365 Dataverse पर Project Operations** खोलें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-186">In Finance, go to **Project management and accounting** > **Setup** > **Project management and accounting parameters**, and open **Project Operations on Dynamics 365 Dataverse**.</span></span> 
2. <span data-ttu-id="b2b59-187">**परियोजना श्रेणी डिफॉल्ट** टैब पर, **आइटम**  फ़ील्ड में, एक मान चुनें.</span><span class="sxs-lookup"><span data-stu-id="b2b59-187">On the **Project category defaults** tab, in the **Item** field, select a value.</span></span> <span data-ttu-id="b2b59-188">यदि परियोजना श्रेणी को परियोजना वास्तविक रिकॉर्ड पर सेट नहीं किया गया था, तो इस परियोजना श्रेणी का उपयोग सामग्री लेनदेन के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="b2b59-188">This project category is used for material transactions if the project category wasn't set on the project actuals record.</span></span>