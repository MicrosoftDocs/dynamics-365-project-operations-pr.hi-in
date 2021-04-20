---
title: क्रेडिट कार्ड एकीकरण सेटअप करें
description: यह विषय बताता है कि खर्च से संबंधित क्रेडिट कार्ड लेनदेन के साथ कैसे काम करना है.
author: suvaidya
manager: AnnBe
ms.date: 04/02/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.search.form: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.search.region: ''
ms.author: shylaw
ms.search.validFrom: ''
ms.dyn365.ops.version: ''
ms.openlocfilehash: 72ff98f5985af4362cde3c9914e0d20247f1f09a
ms.sourcegitcommit: ca0fc078d1a12484eca193fe051b8442c0559db8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/07/2021
ms.locfileid: "5866685"
---
# <a name="set-up-credit-card-integration"></a><span data-ttu-id="9131f-103">क्रेडिट कार्ड एकीकरण सेटअप करें</span><span class="sxs-lookup"><span data-stu-id="9131f-103">Set up credit card integration</span></span>

<span data-ttu-id="9131f-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="9131f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="9131f-105">व्यय से संबंधित क्रेडिट कार्ड लेनदेन को सेट किया जा सकता है ताकि वे आवर्ती शेड्यूल पर अपने आप आयात किये जा सकें.</span><span class="sxs-lookup"><span data-stu-id="9131f-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="9131f-106">विकल्प रूप से, लेनदेन को मैन्युअल रूप से आयात किया जा सकता है क्योंकि उनकी ज़रूरत है.</span><span class="sxs-lookup"><span data-stu-id="9131f-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="9131f-107">क्रेडिट कार्ड लेनदेन को क्रेडिट कार्ड लेनदेन डेटा निकाय के माध्यम से आयात किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="9131f-107">The credit card transactions are imported through the credit card transactions data entity.</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="9131f-108">क्रेडिट कार्ड लेनदेन आयात करें</span><span class="sxs-lookup"><span data-stu-id="9131f-108">Import credit card transactions</span></span>

<span data-ttu-id="9131f-109">क्रेडिट कार्ड लेनदेन आयात करने के लिए, इन चरणों का पालन करें:</span><span class="sxs-lookup"><span data-stu-id="9131f-109">To import credit card transactions, follow these steps:</span></span>

1. <span data-ttu-id="9131f-110">**क्रेडिट कार्ड लेनदेन** पृष्ठ पर, **लेनदेन आयात करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9131f-110">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="9131f-111">यदि आप पहली बार डेटा प्रबंधन खोल रहे हैं, तो सिस्टम को जारी रखने से पहले डेटा निकायों की सूची को अद्यतन करना होगा.</span><span class="sxs-lookup"><span data-stu-id="9131f-111">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="9131f-112">**नाम** फ़ील्ड में, आयात नौकरी के लिए एक विशिष्ट विवरण दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="9131f-112">In the **Name** field, enter a unique description for the import job.</span></span>
3. <span data-ttu-id="9131f-113">**स्रोत डेटा प्रारूप** फ़ील्ड में, उस फ़ाइल के प्रारूप को चुने जिसमें आयात करने के लिए क्रेडिट कार्ड लेनदेन शामिल है.</span><span class="sxs-lookup"><span data-stu-id="9131f-113">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="9131f-114">**अपलोड करें** चुनें, और फिर आयात करने के लिए फ़ाइल ढूंढें और चुनें.</span><span class="sxs-lookup"><span data-stu-id="9131f-114">Select **Upload**, and then find and select the file to import.</span></span>
5. <span data-ttu-id="9131f-115">फ़ाइल अपलोड होने के बाद, टाइल पर **मानचित्र देखें** लिंक चुनकर, क्रेडिट कार्ड लेनदेन फ़ाइल और क्रेडिट कार्ड लेनदेन डेटा निकाय के स्तंभ को सत्यापित करें.</span><span class="sxs-lookup"><span data-stu-id="9131f-115">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="9131f-116">यदि मैपिंग त्रुटियां हैं, या अगर आपको मैपिंग को बदलना है, तो **मैपिंग विज़ुअलाइज़ेशन** टैब या **मैपिंग विवरण** टैब से मैंपिग परिवर्तन करें.</span><span class="sxs-lookup"><span data-stu-id="9131f-116">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="9131f-117">क्रेडिट कार्ड लेनदेन को स्वचालित करने के लिए, **आवर्ती डेटा कार्य बनाएं** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9131f-117">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="9131f-118">फिर आप पुनरावृत्ति सेट कर सकते हैं जो बताती है कि क्रेडिट कार्ड लेनदेन को कितनी बार आयात किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="9131f-118">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="9131f-119">जब आप अपना काम समाप्त कर लें, तो **ठीक** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9131f-119">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="9131f-120">अब चुनी गई फ़ाइल को आयात करने के लिए, **आयात करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9131f-120">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="9131f-121">यदि आयात के दौरान त्रुटियां होती हैं, तो आप एक सफल आयात सुनिश्चित करने में मदद करने के लिए आपको तय की जाने वाली त्रुटियों को देखने के लिए निष्पादन लॉग या स्टेज़िंग डेटा देख सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="9131f-121">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help ensure a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="9131f-122">यदि आपको एक से अधिक फ़ाइल प्रारूप आयात करने की आवश्यकता है, तो आपको प्रत्येक प्रारूप प्रकार के लिए अलग आयात जॉब पैदा करनी होंगी.</span><span class="sxs-lookup"><span data-stu-id="9131f-122">If you need to import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="9131f-123">निलम्बित कर्मचारियों के लिए क्रेडिट कार्ड के लेनदेन को फिर से असाइन करें</span><span class="sxs-lookup"><span data-stu-id="9131f-123">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="9131f-124">कर्मचारी रिकॉर्ड समाप्त होने के बाद, कर्मचारी का एक्टिव डायरेक्ट्री डोमेन सर्विस (AD DS) खाता निष्क्रिय हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="9131f-124">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="9131f-125">हालांकि, सक्रिय क्रेडिट कार्ड लेनदेन हो सकते हैं जिन्हें अब भी खर्च किया जाना चाहिए और प्रतिपूर्ति की जानी चाहिए.</span><span class="sxs-lookup"><span data-stu-id="9131f-125">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="9131f-126">**क्रेडिट कार्ड लेनदेन** पेज पर, आप किसी भी क्रेडिट कार्ड लेनदेन के लिए कर्मचारी को फिर से असाइन कर सकते हैं जहां संबंधित कर्मचारी को समाप्त कर दिया गया है.</span><span class="sxs-lookup"><span data-stu-id="9131f-126">On the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="9131f-127">एक या अधिक क्रेडिट कार्ड लेनदेन चुनें और फिर **लेनदेन पुन: असाइन करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9131f-127">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="9131f-128">फिर आप क्रेडिट कार्ड लेनदेन को असाइन करने के लिए किसी अन्य कर्मचारी को चुन सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="9131f-128">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="9131f-129">क्रेडिट कार्ड के लेनदेन के बाद फिर से असाइन किया गया है तो उन्हें व्यय रिपोर्ट के लिए चुना जा सकता है और व्यय रिपोर्ट प्रतिपूर्ति के लिए सामान्य प्रक्रिया के माध्यम से भुगतान किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="9131f-129">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>

## <a name="delete-credit-card-transactions"></a><span data-ttu-id="9131f-130">क्रेडिट कार्ड लेनदेन हटाएं</span><span class="sxs-lookup"><span data-stu-id="9131f-130">Delete credit card transactions</span></span> 

<span data-ttu-id="9131f-131">कभी-कभी, क्रेडिट कार्ड लेनदेन आयात किए जाने के बाद, कुछ लेनदेन को हटाने की आवश्यकता हो सकती है.</span><span class="sxs-lookup"><span data-stu-id="9131f-131">Sometimes, after credit card transactions are imported, certain transactions may need to be deleted.</span></span> <span data-ttu-id="9131f-132">ऐसा इसलिए हो सकता है क्योंकि लेन-देन डुप्लिकेट हैं या क्योंकि डेटा सटीक नहीं हो सकता है.</span><span class="sxs-lookup"><span data-stu-id="9131f-132">This could be because the transactions are duplicates or because the data might isn't accurate.</span></span> <span data-ttu-id="9131f-133">व्यवस्थापक क्रेडिट कार्ड लेनदेन का चयन करने और हटाने के लिए **क्रेडिट कार्ड लेनदेन हटाएं** सुविधा का उपयोग कर सकते हैं जो **खर्च रिपोर्ट** से संलग्न नहीं हैं.</span><span class="sxs-lookup"><span data-stu-id="9131f-133">Admins can use the **"Delete credit card transactions"** feature to select and delete credit card transactions that are **not attached** to an expense report.</span></span> 

1. <span data-ttu-id="9131f-134">**आवधिक कार्यों पर जाएं** > **क्रेडिट कार्ड लेनदेन मिटाएं**.</span><span class="sxs-lookup"><span data-stu-id="9131f-134">Go to **Periodic tasks** > **Delete credit card transactions**.</span></span>
2. <span data-ttu-id="9131f-135">**फ़िल्टर** चुनें और रिकॉर्ड को शामिल करने के लिए पहचान करने के लिए जानकारी प्रदान करें.</span><span class="sxs-lookup"><span data-stu-id="9131f-135">Select **Filter** and provide information to identify the records to include.</span></span>
3. <span data-ttu-id="9131f-136">रिकॉर्ड हटाने के लिए **ठीक** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9131f-136">Select **OK** to delete the records.</span></span> 

[!INCLUDE[footer-include](../includes/footer-banner.md)]
