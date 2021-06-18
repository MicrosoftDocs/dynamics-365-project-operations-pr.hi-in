---
title: ख़र्च रसीद संसाधित करना
description: यह विषय रसीदों के लिए ऑप्टिकल कैरेक्टर रिकॉग्निशन (OCR) प्रक्रिया के बारे में जानकारी देता है. जब Microsoft Dynamics 365 Finance में ख़र्च रिपोर्ट बनाई जाती है तो यह सुविधा उपयोगकर्ता के अनुभव को बेहतर बनाने के लिए डिज़ाइन की गई है.
author: stsporen
ms.date: 05/14/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Operations, Core
ms.search.region: Global
ms.author: stsporen
ms.search.validFrom: 2019-11-20
ms.dyn365.ops.version: 10.0.8
ms.openlocfilehash: ed9c97ba9cc505106599c2896dc2112358d0c408
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993508"
---
# <a name="expense-receipt-processing"></a><span data-ttu-id="9de40-104">ख़र्च रसीद संसाधित करना</span><span class="sxs-lookup"><span data-stu-id="9de40-104">Expense receipt processing</span></span>

<span data-ttu-id="9de40-105">रसीदों के लिए ऑप्टिकल कैरेक्टर रिकॉग्निशन (OCR) प्रक्रिया शुरू करने के माध्यम से व्यय प्रविष्टि का विस्तार किया गया है.</span><span class="sxs-lookup"><span data-stu-id="9de40-105">Expense entry has been enhanced through the introduction of optical character recognition (OCR) processing for receipts.</span></span> <span data-ttu-id="9de40-106">यह सुविधा ख़र्च रिपोर्ट बनाए जाने पर उपयोगकर्ता के अनुभव को बेहतर बनाने के लिए डिज़ाइन की गई है.</span><span class="sxs-lookup"><span data-stu-id="9de40-106">This feature is designed to improve the user experience when expense reports are created.</span></span>

## <a name="key-features"></a><span data-ttu-id="9de40-107">मुख्य सुविधाएँ</span><span class="sxs-lookup"><span data-stu-id="9de40-107">Key features</span></span>

- <span data-ttu-id="9de40-108">व्यापारी का नाम, तिथि और कुल राशि रसीदों से निकाली जाती है.</span><span class="sxs-lookup"><span data-stu-id="9de40-108">The merchant name, date, and total amount are extracted from receipts.</span></span>
- <span data-ttu-id="9de40-109">यह सुविधा असंबद्ध रसीदों की असंबद्ध ख़र्च लेनदेन से मिलान करने की कोशिश करती है.</span><span class="sxs-lookup"><span data-stu-id="9de40-109">The feature tries to match unattached receipts to unattached expense transactions.</span></span>
- <span data-ttu-id="9de40-110">उपयोगकर्ता रसीदों से मैन्युअल रूप से दर्ज किए गए ख़र्च लेनदेन बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="9de40-110">Users can create manually entered expense transactions from receipts.</span></span>

## <a name="usage-examples"></a><span data-ttu-id="9de40-111">उपयोग उदाहरण</span><span class="sxs-lookup"><span data-stu-id="9de40-111">Usage examples</span></span>

<span data-ttu-id="9de40-112">ख़र्च रिपोर्ट के बनने पर क्रेडिट कार्ड लेनदेन को शामिल करने वाली रसीदों को अपने आप संलग्न करने के लिए, निम्‍न कार्य करें:</span><span class="sxs-lookup"><span data-stu-id="9de40-112">To automatically attach receipts that include credit card transactions when an expense report is created, do the following:</span></span>

  1. <span data-ttu-id="9de40-113">**व्यय प्रबंधन** कार्यक्षेत्र खोलें.</span><span class="sxs-lookup"><span data-stu-id="9de40-113">Open the **Expense management** workspace.</span></span>
  2. <span data-ttu-id="9de40-114">**रसीद** टैब पर सत्यापित करें कि असंबद्ध रसीदें मौजूद हैं.</span><span class="sxs-lookup"><span data-stu-id="9de40-114">On the **Receipts** tab, verify that unattached receipts exist.</span></span> <span data-ttu-id="9de40-115">**रसीद** टैब पर आप रसीदें अपलोड कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="9de40-115">You can also upload receipts on the **Receipts** tab.</span></span>
  3. <span data-ttu-id="9de40-116">**व्यय** टैब पर सत्यापित करें कि असंबद्ध व्यय मौजूद हैं.</span><span class="sxs-lookup"><span data-stu-id="9de40-116">On the **Expenses** tab, verify that unattached expenses exist.</span></span> <span data-ttu-id="9de40-117">आमतौर पर, व्यय व्यवस्थापक क्रेडिट कार्ड प्रदाता से इन खर्चों को आयात करते हैं.</span><span class="sxs-lookup"><span data-stu-id="9de40-117">Typically, the expense administrator imports these expenses from the credit card provider.</span></span>
  4. <span data-ttu-id="9de40-118">**नई व्यय रिपोर्ट** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9de40-118">Select **New expense report**.</span></span> <span data-ttu-id="9de40-119">ध्यान दें कि आप व्यय रिपोर्ट बनाते समय, व्यय और रसीदों को भी शामिल कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="9de40-119">Notice that you can include expenses, and receipts, now as well, when you create an expense report.</span></span> <span data-ttu-id="9de40-120">यदि आप व्यय और रसीद दोनों जोड़ते हैं, तो व्यय के सापेक्ष रसीदों का मिलान अपने आप शुरू हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="9de40-120">If you add both expenses and receipts, automatic matching of the receipts against the expenses is triggered.</span></span>

<span data-ttu-id="9de40-121">एक ख़र्च बनाने के लिए या एक रसीद से ख़र्च का मिलान करने के लिए, निम्‍न कार्य करें:</span><span class="sxs-lookup"><span data-stu-id="9de40-121">To create an expense, or match an expense from a receipt, do the following:</span></span>

  1. <span data-ttu-id="9de40-122">व्यय रिपोर्ट में **रसीद** टैब पर, **रसीद जोड़ें** चुनकर रसीद संलग्न करें.</span><span class="sxs-lookup"><span data-stu-id="9de40-122">On an expense report, on the **Receipts** tab, attach a receipt by selecting **Add receipts**.</span></span>
  2. <span data-ttu-id="9de40-123">रसीद की अपलोड की गई छवि के अंतर्गत, **बनाएं** और **मिलान करें** विकल्प देखें.</span><span class="sxs-lookup"><span data-stu-id="9de40-123">Under the uploaded image of the receipt, notice the **Create** and **Match** options.</span></span>

      - <span data-ttu-id="9de40-124">मैन्युअल रूप से दर्ज व्यय लेनदेन बनाने के लिए **बनाएं** चुनें और वो मान भरें जो रसीद से निकाले जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="9de40-124">Select **Create** to create a manually entered expense transaction and fill in the values that are extracted from the receipt.</span></span>
      - <span data-ttu-id="9de40-125">यदि आप **मिलान करें** चुनते हैं, तो सिस्टम रसीद के लिए मौजूद व्यय का मिलान करने की कोशिश करता है.</span><span class="sxs-lookup"><span data-stu-id="9de40-125">If you select **Match**, the system tries to match an existing expense to the receipt.</span></span>

## <a name="installation"></a><span data-ttu-id="9de40-126">स्थापना</span><span class="sxs-lookup"><span data-stu-id="9de40-126">Installation</span></span>

<span data-ttu-id="9de40-127">यह सुविधा ख़र्च अनुभव को सरल बनाने में मदद करने के लिए **पुनर्कल्पित ख़र्च रिपोर्ट** के साथ मेल से कार्य करती है.</span><span class="sxs-lookup"><span data-stu-id="9de40-127">This feature works in combination with the **Expense reports re-imagined** feature to help simplify the expense experience.</span></span> <span data-ttu-id="9de40-128">यह सुविधा केवल टियर 2 + परिवेश के लिए उपलब्ध है, जो Sandbox और Production हैं.</span><span class="sxs-lookup"><span data-stu-id="9de40-128">This feature is only available for Tier 2+ environments, which are Sandbox and Production.</span></span>

<span data-ttu-id="9de40-129">इन उन्नत व्यय क्षमताओं को इस्तेमाल करने के लिए Microsoft Dynamics 365 Finance के लिए Expense Management Service ऐड-इन इंस्टॉल करें, और और अपने इंस्टेंस में फ़ीचर चालू करें.</span><span class="sxs-lookup"><span data-stu-id="9de40-129">To use these advanced expense capabilities, install the Expense Management Service add-in for Microsoft Dynamics 365 Finance, and turn on the features in your instance.</span></span> <span data-ttu-id="9de40-130">आप Microsoft Dynamics Lifecycle Services (LCS) में अपनी परियोजना से ऐड-इन में प्रवेश कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="9de40-130">You can access the add-in from your project in Microsoft Dynamics Lifecycle Services (LCS).</span></span>

1. <span data-ttu-id="9de40-131">LCS में साइन इन करें और वांछित परिवेश खोलें.</span><span class="sxs-lookup"><span data-stu-id="9de40-131">Sign in to LCS, and open the desired environment.</span></span>
2. <span data-ttu-id="9de40-132">**पूर्ण विवरण** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="9de40-132">Go to **Full details**.</span></span>
3. <span data-ttu-id="9de40-133">**बनाए रखें** चुनें या **परिवेश ऐड-इन** FastTab तक स्क्रॉल डाउन करें.</span><span class="sxs-lookup"><span data-stu-id="9de40-133">Select **Maintain**, or scroll down to the **Environment add-ins** FastTab.</span></span>
4. <span data-ttu-id="9de40-134">**नए ऐड-इन इंस्टॉल करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9de40-134">Select **Install a new add-in**.</span></span>
5. <span data-ttu-id="9de40-135">**Expense Management Service** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9de40-135">Select **Expense Management Service**.</span></span>
6. <span data-ttu-id="9de40-136">इंस्टॉलेशन गाइड के निर्देशों का पालन करें और नियम और शर्तों से सहमत हों.</span><span class="sxs-lookup"><span data-stu-id="9de40-136">Follow the installation guide, and agree to the terms and conditions.</span></span>
7. <span data-ttu-id="9de40-137">**स्थापित करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="9de40-137">Select **Install**.</span></span>

<span data-ttu-id="9de40-138">**फ़ीचर प्रबंधन** कार्यक्षेत्र में, निम्न फ़ीचर चालू करें:</span><span class="sxs-lookup"><span data-stu-id="9de40-138">In the **Feature management** workspace, turn on the following features:</span></span>

- <span data-ttu-id="9de40-139">व्यय रिपोर्ट पुनर्कल्पित</span><span class="sxs-lookup"><span data-stu-id="9de40-139">Expense reports re-imagined</span></span>
- <span data-ttu-id="9de40-140">स्वत: मिलान करे और रसीद से व्यय बनाएं</span><span class="sxs-lookup"><span data-stu-id="9de40-140">Auto-match and create expense from receipt</span></span>

<span data-ttu-id="9de40-141">जब आप इन फ़ीचर चालू करते हैं तो निम्नांकित कार्रवाइयां होती हैं:</span><span class="sxs-lookup"><span data-stu-id="9de40-141">When you turn on these features the following actions occur:</span></span>

- <span data-ttu-id="9de40-142">मौजूद **व्यय प्रबंधन** कार्यक्षेत्र को नए कार्यक्षेत्र से बदल दिया गया है.</span><span class="sxs-lookup"><span data-stu-id="9de40-142">The existing **Expense management** workspace is replaced with the new workspace.</span></span>
- <span data-ttu-id="9de40-143">व्यय फ़ील्ड दृश्यता के लिए नया मेनू आइटम जोड़ा गया है.</span><span class="sxs-lookup"><span data-stu-id="9de40-143">A new menu item for expense field visibility is added.</span></span>
- <span data-ttu-id="9de40-144">आप अब भी **व्यय प्रबंधन > मेरे व्यय > व्यय रिपोर्ट** पर जाकर पिछली **व्यय रिपोर्ट** खोल सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="9de40-144">You can still open the former **Expense reports** page by going to **Expense management > My expenses > Expense reports**.</span></span>
- <span data-ttu-id="9de40-145">कार्यप्रवाह और स्वीकृतियां अब भी आपको मौजूदा व्यय रिपोर्ट पृष्ठ पर ले जाती हैं.</span><span class="sxs-lookup"><span data-stu-id="9de40-145">Workflows and any approvals still take you to the existing expense reports page.</span></span>
- <span data-ttu-id="9de40-146">Microsoft Azure Cognitive Services के माध्यम से रसीद संसाधित की जाएंगा और मेटाडेटा को निकाला और जोड़ा जाएगा.</span><span class="sxs-lookup"><span data-stu-id="9de40-146">Receipts will be processed through Microsoft Azure Cognitive Services, and metadata will be extracted and added.</span></span>
- <span data-ttu-id="9de40-147">विकल्प जोड़ा गया है जो आपको व्यय रिपोर्ट बनाने की अनुमति देता है जिसमें मिलान की गयी असंबद्ध रसीदें शामिल होती हैं.</span><span class="sxs-lookup"><span data-stu-id="9de40-147">An option is added that lets you create an expense report that includes matched unattached receipts.</span></span>
- <span data-ttu-id="9de40-148">व्यय रिपोर्ट में जोड़ा गया विकल्प आपको रसीद से व्यय पद्धति बनाने की सुविधा देता है या किसी मौजूद रसीद का मौजूद व्यय पद्धति से मिलान करने की कोशिश करता है.</span><span class="sxs-lookup"><span data-stu-id="9de40-148">An option that is added to expense reports lets you create an expense line from a receipt, or attempts to match an existing receipt to an existing expense line.</span></span>

<span data-ttu-id="9de40-149">पुनर्कल्पित ख़र्च रिपोर्ट सुविधा के बारे में अधिक जानकारी के लिए, देखें [ख़र्च रिपोर्ट पुनर्कल्पित](ExpenseWorkspaceNew.md).</span><span class="sxs-lookup"><span data-stu-id="9de40-149">For more information about the Expense reports re-imagined feature, see [Expense reports reimagined](ExpenseWorkspaceNew.md).</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="9de40-150">सामान्य प्रश्‍न</span><span class="sxs-lookup"><span data-stu-id="9de40-150">Frequently asked questions</span></span>

<span data-ttu-id="9de40-151">**क्या Microsoft अपने मॉडल के लिए मेरा डेटा इस्तेमाल करता है?**</span><span class="sxs-lookup"><span data-stu-id="9de40-151">**Does Microsoft use my data for its models?**</span></span>

<span data-ttu-id="9de40-152">नहीं, Microsoft ने अपनी रसीद संसाधित करने की सेवा के लिए सामान्य मशीन लर्निंग मॉडल बनाया है.</span><span class="sxs-lookup"><span data-stu-id="9de40-152">No, Microsoft has built a general machine learning model for its receipt processing service.</span></span> <span data-ttu-id="9de40-153">यह मॉडल आपके द्वारा अपलोड की जाने वाली रसीदों पर आधारित नहीं है.</span><span class="sxs-lookup"><span data-stu-id="9de40-153">This model isn't based on the receipts that you upload.</span></span>

<span data-ttu-id="9de40-154">**यह फ़ीचर कहां उपलब्ध है और संसाधित किया जाता है?**</span><span class="sxs-lookup"><span data-stu-id="9de40-154">**Where is this feature available and processed?**</span></span>

<span data-ttu-id="9de40-155">मौजूदा समय में, संयुक्त राज्य अमेरिका समर्थित है.</span><span class="sxs-lookup"><span data-stu-id="9de40-155">Currently, the United States is supported.</span></span>

<span data-ttu-id="9de40-156">**मेरी रसीदें कहाँ जाती हैं?**</span><span class="sxs-lookup"><span data-stu-id="9de40-156">**Where do my receipts go?**</span></span>

<span data-ttu-id="9de40-157">फ़ील्ड डेटा निकालने के लिए Finance, Cognitive Services से संपर्क करेगा.</span><span class="sxs-lookup"><span data-stu-id="9de40-157">Finance will contact Cognitive Services to extract the field data.</span></span> <span data-ttu-id="9de40-158">Cognitive Services इसे संसाधित करने के दौरान अपने पास 24 घंटे तक आपकी रसीद की प्रति रखेगी.</span><span class="sxs-lookup"><span data-stu-id="9de40-158">Cognitive Services will retain a copy of your receipt for up to 24 hours while processing occurs.</span></span> <span data-ttu-id="9de40-159">संसाधित करने के बाद Cognitive Services रसीद को हटा देंगी.</span><span class="sxs-lookup"><span data-stu-id="9de40-159">After processing is completed, Cognitive Services will remove the receipt.</span></span> <span data-ttu-id="9de40-160">रसीदें अब भी Finance में संग्रहीत हैं.</span><span class="sxs-lookup"><span data-stu-id="9de40-160">Receipts are still stored in Finance.</span></span>

<span data-ttu-id="9de40-161">और जानकारकी के लिए [प्रपत्र पहचानकर्ता की नई क्षमता के साथ रसीद की समझ को सक्षम करें](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/) देखें.</span><span class="sxs-lookup"><span data-stu-id="9de40-161">For more information, see [Enable receipt understanding with Form Recognizer's new capability](https://azure.microsoft.com/blog/enable-receipt-understanding-with-form-recognizer-s-new-capability/).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]