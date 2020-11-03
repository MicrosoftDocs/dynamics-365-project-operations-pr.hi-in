---
title: Microsoft Project Client एकीकरण
description: परियोजना शेड्यूल की योजना बनाना और उसे बनाए रखना जटिल हो सकता है, इसीलिए परियोजना प्रबन्धकों को ऐसे उपकरणों/साधनों का उपयोग करना होगा जो उन्हें इस कार्य को प्रबन्धित करने में सहायक हों. Microsoft Project Client के साथ एकीकरण, परियोजना कार्य विश्लेषण संरचना को खोलने और प्रबन्धित करने के लिए समर्थन प्रदान करता है.
author: Yowelle
manager: AnnBe
ms.date: 12/11/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjWbsTemplate
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2017-12-04
ms.dyn365.ops.version: 7.2999999999999998
ms.openlocfilehash: 732b72d9819fc149c4b2c783b3dc7f7eec3f0393
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077761"
---
# <a name="microsoft-project-client-integration"></a><span data-ttu-id="bacee-104">Microsoft Project Client एकीकरण</span><span class="sxs-lookup"><span data-stu-id="bacee-104">Microsoft Project client integration</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="bacee-105">परियोजना शेड्यूल की योजना बनाना और उसे बनाए रखना जटिल हो सकता है, इसीलिए परियोजना प्रबन्धकों को ऐसे उपकरणों/साधनों का उपयोग करना होगा जो उन्हें इस कार्य को प्रबन्धित करने में सहायक हों.</span><span class="sxs-lookup"><span data-stu-id="bacee-105">Planning and maintaining a project schedule can be complex, so project managers need to use tools that help them manage this task.</span></span> <span data-ttu-id="bacee-106">Microsoft Project Client के साथ एकीकरण, परियोजना कार्य विश्लेषण संरचना को खोलने और प्रबन्धित करने के लिए समर्थन प्रदान करता है.</span><span class="sxs-lookup"><span data-stu-id="bacee-106">Integration with Microsoft Project Client provides support to open and manage a project work breakdown structure.</span></span> <span data-ttu-id="bacee-107">परियोजना प्रबन्धक Dynamics 365 Finance परियोजना कार्य विश्लेषण संरचना में किसी भी परिवर्तन को वापस प्रकाशित कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="bacee-107">The project manager can publish any changes back to the Dynamics 365 Finance project work breakdown structure.</span></span>

> [!NOTE]
> <span data-ttu-id="bacee-108">यदि आप जुलाई अपडेट (संस्करण 10.0.4) का उपयोग कर रहे हैं, तो आपको KB 4054797 और 4055884 इंस्टॉल करना होगा.</span><span class="sxs-lookup"><span data-stu-id="bacee-108">If you are using the July update (version 10.0.4), you must install KB 4054797 and 4055884.</span></span>

## <a name="configure-the-microsoft-project-client-add-in"></a><span data-ttu-id="bacee-109">Microsoft Project Client ऐड-इन को कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="bacee-109">Configure the Microsoft Project Client add-in</span></span>
<span data-ttu-id="bacee-110">Microsoft Project Client के साथ एकीकरण सक्षम करने के लिए, Microsoft Dynamics 365 ऐड-इन को उपयोगकर्ता के क्लाइंट Microsoft परियोजना अनुप्रयोग में इंस्टॉल करना आवश्यक है.</span><span class="sxs-lookup"><span data-stu-id="bacee-110">To enable the integration with Microsoft Project Client, a Microsoft Dynamics 365 add-in is required to be installed in the user’s client Microsoft Project application.</span></span> <span data-ttu-id="bacee-111">यह **परियोजना प्रबंधन कार्यक्षेत्र** को खोलकर किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="bacee-111">This is done by opening the **Project management workspace**.</span></span>

<span data-ttu-id="bacee-112">•   कार्यक्षेत्र के **लिंक्स** > **सेटअप** खंड से **परियोजना क्लाइंट ऐड-इन कॉन्फ़िगर करें** को क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="bacee-112">•   Click **Configure project client add-in** from the **Links** > **Setup** section of the workspace.</span></span>

<span data-ttu-id="bacee-113">•   **खोलें** पर क्लिक करें, और फिर अनुबोध कराए जाने पर **चलाएं** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="bacee-113">•   Click **Open** , then click **Run** when prompted.</span></span>

## <a name="open-and-edit-an-existing-draft-work-breakdown-structure-in-microsoft-project-client"></a><span data-ttu-id="bacee-114">Microsoft Project Client में मौजूदा प्रारूप कार्य विश्लेषण संरचना को खोलें और संपादित करें</span><span class="sxs-lookup"><span data-stu-id="bacee-114">Open and edit an existing draft work breakdown structure in Microsoft Project Client</span></span>
<span data-ttu-id="bacee-115">यदि Dynamics 365 Finance की किसी परियोजना में पहले से ही एक कार्य विश्लेषण संरचना है, तो कार्य विश्लेषण संरचना को Microsoft Project Client अनुप्रयोग में खोला जा सकता है, यदि कार्य-विश्लेषण संरचना एक प्रारूप स्थिति में है.</span><span class="sxs-lookup"><span data-stu-id="bacee-115">If a project in Dynamics 365 Finance already has a work breakdown structure created, the work breakdown structure can be opened in the Microsoft Project Client application if the work breakdown structure is in a draft status.</span></span> <span data-ttu-id="bacee-116">**परियोजना** पृष्ठ से खोलने के लिए, **योजना** टैब से **Microsoft Project में खोलें** को क्लिक करें. इस पृष्ठ को Microsoft Project Client अनुप्रयोग के भीतर ही **Microsoft Dynamics 365** टैब में **खोलें** पर क्लिक करके भी खोला जा सकता है. सूची से **विधिक निकाय** और **परियोजना** चुनें.</span><span class="sxs-lookup"><span data-stu-id="bacee-116">To open from the **Project** page, click **Open in Microsoft Project** link from the **Plan** tab. This page can also be opened from within the Microsoft Project Client application by clicking **Open** in the **Microsoft Dynamics 365** tab. Select the **Legal entity** and **Project** from the list.</span></span>

> [!NOTE]
> <span data-ttu-id="bacee-117">यदि आप अपने ब्राउज़र के रूप में Internet Explorer का उपयोग कर रहे हैं, तो आपको फ़ाइल के डाउनलोड होने वाले स्थान से मैन्युअल रूप से खोलने के लिए **सहेजें** पर क्लिक करना होगा.</span><span class="sxs-lookup"><span data-stu-id="bacee-117">If you're using Internet Explorer as your browser, you will need to click **Save** to manually open from the location that the file is downloaded to.</span></span> <span data-ttu-id="bacee-118">अथवा, Microsoft Project Client में फ़ाइल खोलने के लिए **सहेजें और खोलें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="bacee-118">Or, click **Save and open** to open the file in Microsoft Project Client.</span></span> <span data-ttu-id="bacee-119">सहेजते समय फ़ाइल का नाम न बदलें.</span><span class="sxs-lookup"><span data-stu-id="bacee-119">Do not rename the file name when saving.</span></span>

<span data-ttu-id="bacee-120">Microsoft Project Client का उपयोग करके फ़ाइल में कोई भी संपादन करने से पहले, आपको इसे चेक आउट करने की आवश्यकता होती है. **Microsoft Dynamics 365** टैब में **चेक आउट** पर क्लिक करें. यह अन्य उपयोगकर्ताओं को वित्त के भीतर से कार्य विश्लेषण संरचना को एक ही समय में संपादित करने से रोकेगा.</span><span class="sxs-lookup"><span data-stu-id="bacee-120">Before making any edits to the file using Microsoft Project Client, you need to check it out. Click **Check out** in the **Microsoft Dynamics 365** tab. This will prevent other users from editing the work breakdown structure from within Finance at the same time.</span></span> <span data-ttu-id="bacee-121">किसी भी संपादन को पूरा करने के बाद कार्य-विश्लेषण संरचना को प्रकाशित करने के लिए, **Microsoft Dynamics 365** टैब पर **चेक इन** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="bacee-121">To publish the work breakdown structure after completing any edits, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

<span data-ttu-id="bacee-122">यदि किसी परियोजना टीम को पहले से ही वित्त में परियोजना से जोड़ा गया है, तो संसाधन सूची टीम के सदस्यों के साथ पॉप्युलेट होगी.</span><span class="sxs-lookup"><span data-stu-id="bacee-122">If a project team has already been added to the project in Finance, the resource list will be populated with the team members.</span></span> <span data-ttu-id="bacee-123">यदि किसी परियोजना टीम को अभी तक परियोजना से नहीं जोड़ा गया है, तो आप **Microsoft Dynamics 365** टैब पर **संसाधन** बटन पर क्लिक करके संसाधनों को चुन सकते हैं और Microsoft Project Client के भीतर टीम निर्मित कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="bacee-123">If a project team has not yet been added to the project, you can select resources and build the team within Microsoft Project Client by clicking the **Resources** button on the **Microsoft Dynamics 365** tab.</span></span> 

<span data-ttu-id="bacee-124">निम्नलिखित डेटा को चेक-इन प्रक्रिया के भाग के रूप में वित्त में वापस सिंक किया जाएगा:</span><span class="sxs-lookup"><span data-stu-id="bacee-124">The following data will be synced back to Finance as part of the check-in process:</span></span>

<span data-ttu-id="bacee-125">•   कार्य का नाम</span><span class="sxs-lookup"><span data-stu-id="bacee-125">•   Task name</span></span>

<span data-ttu-id="bacee-126">•   प्रारंभ तिथि</span><span class="sxs-lookup"><span data-stu-id="bacee-126">•   Start date</span></span>

<span data-ttu-id="bacee-127">•   समाप्ति दिनांक</span><span class="sxs-lookup"><span data-stu-id="bacee-127">•   Finish date</span></span>

<span data-ttu-id="bacee-128">•   पूर्वगामी</span><span class="sxs-lookup"><span data-stu-id="bacee-128">•   Predecessors</span></span>

<span data-ttu-id="bacee-129">•   संसाधन के नाम</span><span class="sxs-lookup"><span data-stu-id="bacee-129">•   Resource names</span></span>

<span data-ttu-id="bacee-130">•   श्रेणी</span><span class="sxs-lookup"><span data-stu-id="bacee-130">•   Category</span></span>

<span data-ttu-id="bacee-131">•   संसाधन श्रेणी</span><span class="sxs-lookup"><span data-stu-id="bacee-131">•   Resource category</span></span>

<span data-ttu-id="bacee-132">•   कार्य घंटे</span><span class="sxs-lookup"><span data-stu-id="bacee-132">•   Work hours</span></span>

<span data-ttu-id="bacee-133">•   नोट्स</span><span class="sxs-lookup"><span data-stu-id="bacee-133">•   Notes</span></span>

<span data-ttu-id="bacee-134">•   प्राथमिकता</span><span class="sxs-lookup"><span data-stu-id="bacee-134">•   Priority</span></span>

> [!NOTE]
> <span data-ttu-id="bacee-135">यदि आप अपने Microsoft Project Client फ़ाइल में कोई अन्य कॉलम जोड़ते हैं, तो वे फ़ाइल में सहेजे नहीं जाएंगे और फ़ाइल को दोबारा खोलने पर प्रदर्शित नहीं किये जाएंगे.</span><span class="sxs-lookup"><span data-stu-id="bacee-135">If you add any other columns to your Microsoft Project Client file, they will not be saved to the file and will not be displayed when the file is opened again.</span></span>

## <a name="create-the-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="bacee-136">Microsoft Project Client का उपयोग करके किसी मौजूदा परियोजना के लिए कार्य विश्लेषण संरचना बनाएं</span><span class="sxs-lookup"><span data-stu-id="bacee-136">Create the work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="bacee-137">Microsoft Project Client का उपयोग करके एक नयी कार्य विश्लेषण संरचना बनाने के लिए, इन चरणों का पालन करें:</span><span class="sxs-lookup"><span data-stu-id="bacee-137">To create a new work breakdown structure using Microsoft Project Client, follow these steps:</span></span>


1.  <span data-ttu-id="bacee-138">Microsoft Project Client खोलें.</span><span class="sxs-lookup"><span data-stu-id="bacee-138">Open Microsoft Project Client.</span></span>

2.  <span data-ttu-id="bacee-139">**Microsoft Dynamics 365** टैब पर, **खोलें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="bacee-139">On the **Microsoft Dynamics 365** tab, click **Open**.</span></span>

3.  <span data-ttu-id="bacee-140">परियोजना के लिए **विधिक निकाय** चुनें.</span><span class="sxs-lookup"><span data-stu-id="bacee-140">Select the **Legal entity** for the project.</span></span>

4.  <span data-ttu-id="bacee-141">**प्रोजेक्ट** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="bacee-141">Select the **Project**.</span></span>

5.  <span data-ttu-id="bacee-142">**Microsoft Dynamics 365** टैब पर **चेक आउट** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="bacee-142">Click **Check out** on the **Microsoft Dynamics 365** tab.</span></span>

6.  <span data-ttu-id="bacee-143">वित्त में प्रकाशित होने के लिए तैयार होने पर, **Microsoft Dynamics 365** टैब पर **चेक इन** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="bacee-143">When ready to publish to Finance, click **Check in** on the **Microsoft Dynamics 365** tab.</span></span>

## <a name="replace-the-existing-work-breakdown-structure-for-an-existing-project-using-microsoft-project-client"></a><span data-ttu-id="bacee-144">Microsoft Project Client का उपयोग करके मौजूदा परियोजना के लिए मौजूदा कार्य विश्लेषण संरचना को प्रतिस्थापित करें</span><span class="sxs-lookup"><span data-stu-id="bacee-144">Replace the existing work breakdown structure for an existing project using Microsoft Project Client</span></span>
<span data-ttu-id="bacee-145">Microsoft Project Client का उपयोग करके एक नयी कार्य विश्लेषण संरचना बनाने और मौजूदा परियोजना के लिए मौजूदा कार्य विश्लेषण संरचना को प्रतिस्थापित करने के लिए, इन चरणों का पालन करें:</span><span class="sxs-lookup"><span data-stu-id="bacee-145">To create a new work breakdown structure using Microsoft Project Client and replace an existing work breakdown structure for an existing project, follow these steps:</span></span>

1.  <span data-ttu-id="bacee-146">Microsoft Project Client खोलें.</span><span class="sxs-lookup"><span data-stu-id="bacee-146">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="bacee-147">Microsoft Project Client में शेड्यूल बनाएं.</span><span class="sxs-lookup"><span data-stu-id="bacee-147">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="bacee-148">**Microsoft Dynamics 365** टैब पर, **परिवर्तन सहेजें** > **मौजूदा परियोजना प्रतिस्थापित करें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="bacee-148">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Replace existing project**.</span></span>

4.  <span data-ttu-id="bacee-149">परियोजना के लिए **विधिक निकाय** चुनें.</span><span class="sxs-lookup"><span data-stu-id="bacee-149">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="bacee-150">**प्रोजेक्ट** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="bacee-150">Select the **Project**.</span></span>

6.  <span data-ttu-id="bacee-151">**ठीक** क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="bacee-151">Click **OK**.</span></span>

## <a name="create-a-new-project-from-within-microsoft-project-client"></a><span data-ttu-id="bacee-152">Microsoft Project Client से इसके भीतर एक नयी परियोजना बनाएं</span><span class="sxs-lookup"><span data-stu-id="bacee-152">Create a new project from within Microsoft Project Client</span></span>


1.  <span data-ttu-id="bacee-153">Microsoft Project Client खोलें.</span><span class="sxs-lookup"><span data-stu-id="bacee-153">Open the Microsoft Project Client.</span></span>

2.  <span data-ttu-id="bacee-154">Microsoft Project Client में शेड्यूल बनाएं.</span><span class="sxs-lookup"><span data-stu-id="bacee-154">Create the schedule in Microsoft Project Client.</span></span>

3.  <span data-ttu-id="bacee-155">**Microsoft Dynamics 365** टैब पर, **परिवर्तन सहेजें** > **नयी परियोजना में सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="bacee-155">On the **Microsoft Dynamics 365** tab, click **Save changes** > **Save to new Project**.</span></span>

4.  <span data-ttu-id="bacee-156">परियोजना के लिए **विधिक निकाय** चुनें.</span><span class="sxs-lookup"><span data-stu-id="bacee-156">Select the **Legal entity** for the project.</span></span>

5.  <span data-ttu-id="bacee-157">यदि आवश्यक हो तो **परियोजना ID** दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="bacee-157">Enter the **Project ID** , if necessary.</span></span>

6.  <span data-ttu-id="bacee-158">**प्रोजेक्ट नाम** दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="bacee-158">Enter the **Project name**.</span></span>

7.  <span data-ttu-id="bacee-159">**परियोजना प्रकार** , **परियोजना समूह** और **परियोजना अनुबंध ID** चुनें.</span><span class="sxs-lookup"><span data-stu-id="bacee-159">Select the **Project type** , **Project group** and the **Project contract ID**.</span></span> <span data-ttu-id="bacee-160">वैकल्पिक रूप से, आप **नया** पर क्लिक करके एक नया परियोजना अनुबंध बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="bacee-160">Alternatively, you can create a new project contract by clicking **New**.</span></span>

8.  <span data-ttu-id="bacee-161">संसाधनीकरण के लिए उपयोग किए जाने वाला **कैलेंडर** चुनें.</span><span class="sxs-lookup"><span data-stu-id="bacee-161">Select the **Calendar** to be used for resourcing.</span></span>

11. <span data-ttu-id="bacee-162">**ठीक** क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="bacee-162">Click **OK**.</span></span>
