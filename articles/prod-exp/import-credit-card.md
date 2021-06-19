---
title: क्रेडिट कार्ड लेनदेन आयात करें और कायम करें
description: यह विषय बताता है कि व्यय-संबंधित क्रेडिट कार्ड लेनदेन को कैसे आयात किया जाए और बनाए रखा जाए. इन लेनदेन को सेट किया जा सकता है ताकि वे स्वचालित रूप से बार-बार आने वाले शेड्यूल पर आयात हो सकें, या उन्हें आवश्यकतानुसार मैन्युअल रूप से आयात किया जा सके.
author: KimANelson
ms.date: 01/12/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.search.form: TrvPbsMainDataLines
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.custom: 274023
ms.assetid: 3605eda1-a7ed-4675-8031-5279c5a8f5e4
ms.search.region: Global
ms.author: suvaidya
ms.dyn365.ops.version: Version 1611
ms.search.validFrom: 2016-11-30
ms.openlocfilehash: edeab157aa2fa6cf518ad086b4c1f22c5b45fa04
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005163"
---
# <a name="import-and-maintain-credit-card-transactions"></a><span data-ttu-id="61c6a-104">क्रेडिट कार्ड लेनदेन आयात करें और कायम करें</span><span class="sxs-lookup"><span data-stu-id="61c6a-104">Import and maintain credit card transactions</span></span>

<span data-ttu-id="61c6a-105">व्यय से संबंधित क्रेडिट कार्ड लेनदेन को सेट किया जा सकता है ताकि वे आवर्ती शेड्यूल पर अपने आप आयात किये जा सकें.</span><span class="sxs-lookup"><span data-stu-id="61c6a-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="61c6a-106">विकल्प रूप से, लेनदेन को मैन्युअल रूप से आयात किया जा सकता है क्योंकि उनकी ज़रूरत है.</span><span class="sxs-lookup"><span data-stu-id="61c6a-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="61c6a-107">क्रेडिट कार्ड लेनदेन को क्रेडिट कार्ड लेनदेन डेटा निकाय के माध्यम से आयात किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="61c6a-107">The credit card transactions are imported through the Credit card transactions data entity.</span></span>

<span data-ttu-id="61c6a-108">डेटा निकायों के बारे में अधिक जानकारी के लिए, [डेटा निकाय](/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities) देखें.</span><span class="sxs-lookup"><span data-stu-id="61c6a-108">For more information about data entities, see [Data entities](/dynamics365/fin-ops-core/dev-itpro/data-entities/data-entities).</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="61c6a-109">क्रेडिट कार्ड लेनदेन आयात करें</span><span class="sxs-lookup"><span data-stu-id="61c6a-109">Import credit card transactions</span></span>

1. <span data-ttu-id="61c6a-110">**क्रेडिट कार्ड लेनदेन** पृष्ठ पर, **लेनदेन आयात करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="61c6a-110">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="61c6a-111">यदि आप पहली बार डेटा प्रबंधन खोल रहे हैं, तो सिस्टम को जारी रखने से पहले डेटा निकायों की सूची को अद्यतन करना होगा.</span><span class="sxs-lookup"><span data-stu-id="61c6a-111">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="61c6a-112">**नाम** फ़ील्ड में, आयात कार्य का विशिष्ट विवरण दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="61c6a-112">In the **Name** field, enter a unique description of the import job.</span></span>
3. <span data-ttu-id="61c6a-113">**स्रोत डेटा प्रारूप** फ़ील्ड में, उस फ़ाइल के प्रारूप को चुने जिसमें आयात करने के लिए क्रेडिट कार्ड लेनदेन शामिल है.</span><span class="sxs-lookup"><span data-stu-id="61c6a-113">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="61c6a-114">**अपलोड करें** चुनें, और फिर आयात करने के लिए फ़ाइल ढूंढें और चुनें.</span><span class="sxs-lookup"><span data-stu-id="61c6a-114">Select **Upload**, and then find and select the file to import.</span></span>
5. <span data-ttu-id="61c6a-115">फ़ाइल अपलोड होने के बाद, टाइल पर **मानचित्र देखें** लिंक चुनकर, क्रेडिट कार्ड लेनदेन फ़ाइल और क्रेडिट कार्ड लेनदेन डेटा निकाय के स्तंभ को सत्यापित करें.</span><span class="sxs-lookup"><span data-stu-id="61c6a-115">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the Credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="61c6a-116">यदि मैपिंग त्रुटियां हैं, या अगर आपको मैपिंग को बदलना है, तो **मैपिंग विज़ुअलाइज़ेशन** टैब या **मैपिंग विवरण** टैब से मैंपिग परिवर्तन करें.</span><span class="sxs-lookup"><span data-stu-id="61c6a-116">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="61c6a-117">क्रेडिट कार्ड लेनदेन को स्वचालित करने के लिए, **आवर्ती डेटा कार्य बनाएं** चुनें.</span><span class="sxs-lookup"><span data-stu-id="61c6a-117">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="61c6a-118">फिर आप पुनरावृत्ति सेट कर सकते हैं जो बताती है कि क्रेडिट कार्ड लेनदेन को कितनी बार आयात किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="61c6a-118">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="61c6a-119">जब आप अपना काम समाप्त कर लें, तो **ठीक** चुनें.</span><span class="sxs-lookup"><span data-stu-id="61c6a-119">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="61c6a-120">अब चुनी गई फ़ाइल को आयात करने के लिए, **आयात करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="61c6a-120">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="61c6a-121">यदि आयात के दौरान त्रुटियां होती हैं, तो आप त्रुटियों को देखने के लिए निष्पादन लॉग या स्टेजिंग डेटा देख सकते हैं, जो आपको सफल आयात की गारंटी देने में मदद करने के लिए ठीक करना होगा.</span><span class="sxs-lookup"><span data-stu-id="61c6a-121">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help guarantee a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="61c6a-122">यदि आपको एक से अधिक फ़ाइल प्रारूप आयात करने होंगे, तो आपको प्रत्येक प्रारूप प्रकार के लिए अलग आयात कार्य बनाने होंगे.</span><span class="sxs-lookup"><span data-stu-id="61c6a-122">If you must import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="61c6a-123">निलम्बित कर्मचारियों के लिए क्रेडिट कार्ड के लेनदेन को फिर से असाइन करें</span><span class="sxs-lookup"><span data-stu-id="61c6a-123">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="61c6a-124">कर्मचारी रिकॉर्ड समाप्त होने के बाद, कर्मचारी का एक्टिव डायरेक्ट्री डोमेन सर्विस (AD DS) खाता निष्क्रिय हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="61c6a-124">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="61c6a-125">हालांकि, सक्रिय क्रेडिट कार्ड लेनदेन हो सकते हैं जिन्हें अब भी खर्च किया जाना चाहिए और प्रतिपूर्ति की जानी चाहिए.</span><span class="sxs-lookup"><span data-stu-id="61c6a-125">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="61c6a-126">**क्रेडिट कार्ड लेनदेन** पृष्ठ, आप किसी भी क्रेडिट कार्ड लेनदेन के लिए कर्मचारी को फिर से असाइन कर सकते हैं जहां संबद्ध कर्मचारी को निलम्बित कर दिया गया हो.</span><span class="sxs-lookup"><span data-stu-id="61c6a-126">From the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="61c6a-127">एक या अधिक क्रेडिट कार्ड लेनदेन चुनें और फिर **लेनदेन पुन: असाइन करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="61c6a-127">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="61c6a-128">फिर आप क्रेडिट कार्ड लेनदेन को असाइन करने के लिए किसी अन्य कर्मचारी को चुन सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="61c6a-128">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="61c6a-129">क्रेडिट कार्ड के लेनदेन के बाद फिर से असाइन किया गया है तो उन्हें व्यय रिपोर्ट के लिए चुना जा सकता है और व्यय रिपोर्ट प्रतिपूर्ति के लिए सामान्य प्रक्रिया के माध्यम से भुगतान किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="61c6a-129">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]