---
title: OCR को इस्तेमाल करके व्यय से रसीद का मिलान करें
description: यह विषय रसीदों के लिए ऑप्टिकल कैरेक्टर रिकॉग्निशन (OCR) प्रक्रिया के बारे में जानकारी देता है.
author: suvaidya
manager: AnnBe
ms.date: 09/23/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 02c1bafbe907a657689b610ae792f88085320903
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897003"
---
# <a name="match-a-receipt-to-an-expense-using-ocr"></a><span data-ttu-id="c6f33-103">OCR को इस्तेमाल करके व्यय से रसीद का मिलान करें</span><span class="sxs-lookup"><span data-stu-id="c6f33-103">Match a receipt to an expense using OCR</span></span>

<span data-ttu-id="c6f33-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="c6f33-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c6f33-105">रसीदों के लिए ऑप्टिकल कैरेक्टर रिकॉग्निशन (OCR) प्रक्रिया शुरू करने के माध्यम से व्यय प्रविष्टि का विस्तार किया गया है.</span><span class="sxs-lookup"><span data-stu-id="c6f33-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="c6f33-106">यह कार्यक्षमता व्यय रिपोर्ट बनाते समय उपयोगकर्ता अनुभव को बेहतर बनाने के लिए डिज़ाइन की गई है.</span><span class="sxs-lookup"><span data-stu-id="c6f33-106">This functionality is designed to improve the user experience when creating expense reports.</span></span>

## <a name="key-features"></a><span data-ttu-id="c6f33-107">मुख्य सुविधाएँ</span><span class="sxs-lookup"><span data-stu-id="c6f33-107">Key features</span></span>

- <span data-ttu-id="c6f33-108">सिस्टम रसीद से व्यापारी का नाम, तिथि और कुल राशि निकालता है.</span><span class="sxs-lookup"><span data-stu-id="c6f33-108">The system extracts the merchant name, date, and total amount from receipts.</span></span>
- <span data-ttu-id="c6f33-109">सिस्टम असंबद्ध रसीदों को असंबद्ध व्यय लेनदेन से मिलान करने की कोशिश करेगा.</span><span class="sxs-lookup"><span data-stu-id="c6f33-109">The system will try to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="c6f33-110">आप रसीदों से मैन्युअल रूप से दर्ज किए गए व्यय लेनदेन बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="c6f33-110">You can create manually entered expense transactions from receipts.</span></span>

## <a name="attach-receipts-to-an-expense-report"></a><span data-ttu-id="c6f33-111">व्यय रिपोर्ट में रसीदें संलग्न करें</span><span class="sxs-lookup"><span data-stu-id="c6f33-111">Attach receipts to an expense report</span></span>

<span data-ttu-id="c6f33-112">व्यय रिपोर्ट बनने पर क्रेडिट कार्ड लेनदेन शामिल करने वाली रसीदों को अपने आप संलग्न करने के लिए, निम्नांकित चरणों का पालन करें.</span><span class="sxs-lookup"><span data-stu-id="c6f33-112">To automatically attach receipts that include credit card transactions when an expense report is created, complete the following steps.</span></span>

  1. <span data-ttu-id="c6f33-113">**व्यय प्रबंधन** कार्यक्षेत्र खोलें.</span><span class="sxs-lookup"><span data-stu-id="c6f33-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="c6f33-114">**रसीद** टैब पर सत्यापित करें कि असंबद्ध रसीदें मौजूद हैं.</span><span class="sxs-lookup"><span data-stu-id="c6f33-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="c6f33-115">**रसीद** टैब पर आप रसीदें अपलोड कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="c6f33-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="c6f33-116">**व्यय** टैब पर सत्यापित करें कि असंबद्ध व्यय मौजूद हैं.</span><span class="sxs-lookup"><span data-stu-id="c6f33-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="c6f33-117">आमतौर पर, व्यय व्यवस्थापक क्रेडिट कार्ड प्रदाता से इन खर्चों को आयात करते हैं.</span><span class="sxs-lookup"><span data-stu-id="c6f33-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="c6f33-118">**नई व्यय रिपोर्ट** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c6f33-118">Select **New expense report**.</span></span> <span data-ttu-id="c6f33-119">ध्यान दें कि आप व्यय रिपोर्ट बनाते समय, व्यय और रसीदों को भी शामिल कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="c6f33-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="c6f33-120">यदि आप व्यय और रसीद दोनों जोड़ते हैं, तो व्यय के सापेक्ष रसीदों का मिलान अपने आप शुरू हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="c6f33-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

## <a name="create-or-match-receipts-to-an-expense-report"></a><span data-ttu-id="c6f33-121">व्यय रिपोर्ट के लिए रसीद बनाएं या मिलान करें</span><span class="sxs-lookup"><span data-stu-id="c6f33-121">Create or match receipts to an expense report</span></span>
<span data-ttu-id="c6f33-122">व्यय बनाने के लिए या रसीद से व्यय का मिलान करने के लिए निम्नांकित चरणों का पालन करें.</span><span class="sxs-lookup"><span data-stu-id="c6f33-122">To create an expense, or match an expense from a receipt, complete the following steps.</span></span>

  1. <span data-ttu-id="c6f33-123">व्यय रिपोर्ट में **रसीद** टैब पर, **रसीद जोड़ें** चुनकर रसीद संलग्न करें.</span><span class="sxs-lookup"><span data-stu-id="c6f33-123">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="c6f33-124">रसीद की अपलोड की गई छवि के अंतर्गत, **बनाएं** और **मिलान करें** विकल्प देखें.</span><span class="sxs-lookup"><span data-stu-id="c6f33-124">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="c6f33-125">मैन्युअल रूप से दर्ज व्यय लेनदेन बनाने के लिए **बनाएं** चुनें और वो मान भरें जो रसीद से निकाले जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="c6f33-125">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="c6f33-126">यदि आप **मिलान करें** चुनते हैं, तो सिस्टम रसीद के लिए मौजूद व्यय का मिलान करने की कोशिश करता है.</span><span class="sxs-lookup"><span data-stu-id="c6f33-126">If you select **Match**, the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="c6f33-127">स्थापना</span><span class="sxs-lookup"><span data-stu-id="c6f33-127">Installation</span></span>

<span data-ttu-id="c6f33-128">इन उन्नत व्यय क्षमताओं को इस्तेमाल करने के लिए Microsoft Dynamics 365 Finance के लिए Expense Management Service ऐड-इन इंस्टॉल करें, और और अपने इंस्टेंस में फ़ीचर चालू करें.</span><span class="sxs-lookup"><span data-stu-id="c6f33-128">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="c6f33-129">आप Microsoft Dynamics Lifecycle Services (LCS) में अपनी परियोजना से ऐड-इन में प्रवेश कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="c6f33-129">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="c6f33-130">LCS में साइन इन करें और वांछित परिवेश खोलें.</span><span class="sxs-lookup"><span data-stu-id="c6f33-130">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="c6f33-131">**पूर्ण विवरण** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="c6f33-131">Go to **Full details**.</span></span>
3. <span data-ttu-id="c6f33-132">**बनाए रखें** चुनें या **परिवेश ऐड-इन** FastTab तक स्क्रॉल डाउन करें.</span><span class="sxs-lookup"><span data-stu-id="c6f33-132">Select **Maintain**, or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="c6f33-133">**नए ऐड-इन इंस्टॉल करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c6f33-133">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="c6f33-134">**Expense Management Service** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c6f33-134">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="c6f33-135">इंस्टॉलेशन गाइड के निर्देशों का पालन करें और नियम और शर्तों से सहमत हों.</span><span class="sxs-lookup"><span data-stu-id="c6f33-135">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="c6f33-136">**स्थापित करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="c6f33-136">Select **Install**.</span></span>

<span data-ttu-id="c6f33-137">**फ़ीचर प्रबंधन** कार्यक्षेत्र में, निम्न फ़ीचर चालू करें:</span><span class="sxs-lookup"><span data-stu-id="c6f33-137">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="c6f33-138">व्यय रिपोर्ट पुनर्कल्पित</span><span class="sxs-lookup"><span data-stu-id="c6f33-138">Expense reports re-imagined</span></span>
- <span data-ttu-id="c6f33-139">स्वत: मिलान करे और रसीद से व्यय बनाएं</span><span class="sxs-lookup"><span data-stu-id="c6f33-139">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="c6f33-140">जब आप इन फ़ीचर चालू करते हैं तो निम्नांकित कार्रवाइयां होती हैं:</span><span class="sxs-lookup"><span data-stu-id="c6f33-140">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="c6f33-141">मौजूद **व्यय प्रबंधन** कार्यक्षेत्र को नए कार्यक्षेत्र से बदल दिया गया है.</span><span class="sxs-lookup"><span data-stu-id="c6f33-141">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="c6f33-142">व्यय फ़ील्ड दृश्यता के लिए नया मेनू आइटम जोड़ा गया है.</span><span class="sxs-lookup"><span data-stu-id="c6f33-142">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="c6f33-143">आप अब भी **व्यय प्रबंधन > मेरे व्यय > व्यय रिपोर्ट** पर जाकर पिछली **व्यय रिपोर्ट** खोल सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="c6f33-143">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="c6f33-144">कार्यप्रवाह और स्वीकृतियां अब भी आपको मौजूदा व्यय रिपोर्ट पृष्ठ पर ले जाती हैं.</span><span class="sxs-lookup"><span data-stu-id="c6f33-144">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="c6f33-145">Microsoft Azure Cognitive Services के माध्यम से रसीद संसाधित की जाएंगा और मेटाडेटा को निकाला और जोड़ा जाएगा.</span><span class="sxs-lookup"><span data-stu-id="c6f33-145">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="c6f33-146">विकल्प जोड़ा गया है जो आपको व्यय रिपोर्ट बनाने की अनुमति देता है जिसमें मिलान की गयी असंबद्ध रसीदें शामिल होती हैं.</span><span class="sxs-lookup"><span data-stu-id="c6f33-146">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="c6f33-147">व्यय रिपोर्ट में जोड़ा गया विकल्प आपको रसीद से व्यय पद्धति बनाने की सुविधा देता है या किसी मौजूद रसीद का मौजूद व्यय पद्धति से मिलान करने की कोशिश करता है.</span><span class="sxs-lookup"><span data-stu-id="c6f33-147">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="c6f33-148">सामान्य प्रश्‍न</span><span class="sxs-lookup"><span data-stu-id="c6f33-148">Frequently asked questions</span></span>

<span data-ttu-id="c6f33-149">**क्या Microsoft अपने मॉडल के लिए मेरा डेटा इस्तेमाल करता है?**</span><span class="sxs-lookup"><span data-stu-id="c6f33-149">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="c6f33-150">नहीं, Microsoft ने अपनी रसीद संसाधित करने की सेवा के लिए सामान्य मशीन लर्निंग मॉडल बनाया है.</span><span class="sxs-lookup"><span data-stu-id="c6f33-150">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="c6f33-151">यह मॉडल आपके द्वारा अपलोड की जाने वाली रसीदों पर आधारित नहीं है.</span><span class="sxs-lookup"><span data-stu-id="c6f33-151">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="c6f33-152">**यह फ़ीचर कहां उपलब्ध है और संसाधित किया जाता है?**</span><span class="sxs-lookup"><span data-stu-id="c6f33-152">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="c6f33-153">मौजूदा समय में, संयुक्त राज्य अमेरिका समर्थित है.</span><span class="sxs-lookup"><span data-stu-id="c6f33-153">Currently, the United States is supported.</span></span>

<span data-ttu-id="c6f33-154">**मेरी रसीदें कहाँ जाती हैं?**</span><span class="sxs-lookup"><span data-stu-id="c6f33-154">**Where do my receipts go?**</span></span>

<span data-ttu-id="c6f33-155">फ़ील्ड डेटा निकालने के लिए Finance, Cognitive Services से संपर्क करेगा.</span><span class="sxs-lookup"><span data-stu-id="c6f33-155">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="c6f33-156">Cognitive Services इसे संसाधित करने के दौरान अपने पास 24 घंटे तक आपकी रसीद की प्रति रखेगी.</span><span class="sxs-lookup"><span data-stu-id="c6f33-156">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="c6f33-157">संसाधित करने के बाद Cognitive Services रसीद को हटा देंगी.</span><span class="sxs-lookup"><span data-stu-id="c6f33-157">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="c6f33-158">रसीदें अब भी Finance में संग्रहीत हैं.</span><span class="sxs-lookup"><span data-stu-id="c6f33-158">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="c6f33-159">और जानकारकी के लिए [प्रपत्र पहचानकर्ता की नई क्षमता के साथ रसीद की समझ को सक्षम करें](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/) देखें.</span><span class="sxs-lookup"><span data-stu-id="c6f33-159">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>
