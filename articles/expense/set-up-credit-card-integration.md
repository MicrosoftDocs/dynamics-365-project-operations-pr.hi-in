---
title: क्रेडिट कार्ड एकीकरण सेटअप करें
description: यह विषय बताता है कि व्यय-संबंधित क्रेडिट कार्ड लेनदेन को कैसे आयात किया जाए और बनाए रखा जाए.
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
ms.openlocfilehash: 483775e1334a281026dbfaf214d06d235255f13e
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896823"
---
# <a name="set-up-credit-card-integration"></a><span data-ttu-id="8a59a-103">क्रेडिट कार्ड एकीकरण सेटअप करें</span><span class="sxs-lookup"><span data-stu-id="8a59a-103">Set up credit card integration</span></span>

<span data-ttu-id="8a59a-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="8a59a-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8a59a-105">व्यय से संबंधित क्रेडिट कार्ड लेनदेन को सेट किया जा सकता है ताकि वे आवर्ती शेड्यूल पर अपने आप आयात किये जा सकें.</span><span class="sxs-lookup"><span data-stu-id="8a59a-105">Expense-related credit card transactions can be set up so that they are automatically imported on a recurring schedule.</span></span> <span data-ttu-id="8a59a-106">विकल्प रूप से, लेनदेन को मैन्युअल रूप से आयात किया जा सकता है क्योंकि उनकी ज़रूरत है.</span><span class="sxs-lookup"><span data-stu-id="8a59a-106">Alternatively, the transactions can be manually imported as they are required.</span></span> <span data-ttu-id="8a59a-107">क्रेडिट कार्ड लेनदेन को क्रेडिट कार्ड लेनदेन डेटा निकाय के माध्यम से आयात किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8a59a-107">The credit card transactions are imported through the Credit card transactions data entity.</span></span>

## <a name="import-credit-card-transactions"></a><span data-ttu-id="8a59a-108">क्रेडिट कार्ड लेनदेन आयात करें</span><span class="sxs-lookup"><span data-stu-id="8a59a-108">Import credit card transactions</span></span>

1. <span data-ttu-id="8a59a-109">**क्रेडिट कार्ड लेनदेन** पृष्ठ पर, **लेनदेन आयात करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="8a59a-109">On the **Credit card transactions** page, select **Import transactions**.</span></span> <span data-ttu-id="8a59a-110">यदि आप पहली बार डेटा प्रबंधन खोल रहे हैं, तो सिस्टम को जारी रखने से पहले डेटा निकायों की सूची को अद्यतन करना होगा.</span><span class="sxs-lookup"><span data-stu-id="8a59a-110">If you’re opening data management for the first time, the system must update the list of data entities before you can continue.</span></span>
2. <span data-ttu-id="8a59a-111">**नाम** फ़ील्ड में, आयात कार्य का विशिष्ट विवरण दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="8a59a-111">In the **Name** field, enter a unique description of the import job.</span></span>
3. <span data-ttu-id="8a59a-112">**स्रोत डेटा प्रारूप** फ़ील्ड में, उस फ़ाइल के प्रारूप को चुने जिसमें आयात करने के लिए क्रेडिट कार्ड लेनदेन शामिल है.</span><span class="sxs-lookup"><span data-stu-id="8a59a-112">In the **Source data format** field, select the format of the file that contains the credit card transactions to import.</span></span>
4. <span data-ttu-id="8a59a-113">**अपलोड करें** चुनें, और फिर आयात करने के लिए फ़ाइल ढूंढें और चुनें.</span><span class="sxs-lookup"><span data-stu-id="8a59a-113">Select **Upload**, and then find and select the file to import.</span></span>
5. <span data-ttu-id="8a59a-114">फ़ाइल अपलोड होने के बाद, टाइल पर **मानचित्र देखें** लिंक चुनकर, क्रेडिट कार्ड लेनदेन फ़ाइल और क्रेडिट कार्ड लेनदेन डेटा निकाय के स्तंभ को सत्यापित करें.</span><span class="sxs-lookup"><span data-stu-id="8a59a-114">After the file has been uploaded, validate the mapping of the credit card transaction file and the columns of the Credit card transactions data entity by selecting the **View map** link on the tile.</span></span> <span data-ttu-id="8a59a-115">यदि मैपिंग त्रुटियां हैं, या अगर आपको मैपिंग को बदलना है, तो **मैपिंग विज़ुअलाइज़ेशन** टैब या **मैपिंग विवरण** टैब से मैंपिग परिवर्तन करें.</span><span class="sxs-lookup"><span data-stu-id="8a59a-115">If there are mapping errors, or if you must change the mapping, make the mapping changes from either the **Mapping visualization** tab or the **Mapping details** tab.</span></span>
6. <span data-ttu-id="8a59a-116">क्रेडिट कार्ड लेनदेन को स्वचालित करने के लिए, **आवर्ती डेटा कार्य बनाएं** चुनें.</span><span class="sxs-lookup"><span data-stu-id="8a59a-116">To automate the credit card transactions, select **Create recurring data job**.</span></span> <span data-ttu-id="8a59a-117">फिर आप पुनरावृत्ति सेट कर सकते हैं जो बताती है कि क्रेडिट कार्ड लेनदेन को कितनी बार आयात किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="8a59a-117">You can then set the recurrence that defines how often credit card transactions should be imported.</span></span> <span data-ttu-id="8a59a-118">जब आप अपना काम समाप्त कर लें, तो **ठीक** चुनें.</span><span class="sxs-lookup"><span data-stu-id="8a59a-118">When you’ve finished, select **OK**.</span></span>
7. <span data-ttu-id="8a59a-119">अब चुनी गई फ़ाइल को आयात करने के लिए, **आयात करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="8a59a-119">To import the selected file now, select **Import**.</span></span>
8. <span data-ttu-id="8a59a-120">यदि आयात के दौरान त्रुटियां होती हैं, तो आप त्रुटियों को देखने के लिए निष्पादन लॉग या स्टेजिंग डेटा देख सकते हैं, जो आपको सफल आयात की गारंटी देने में मदद करने के लिए ठीक करना होगा.</span><span class="sxs-lookup"><span data-stu-id="8a59a-120">If errors occur during the import, you can view the execution log or staging data to see the errors that you must fix to help guarantee a successful import.</span></span>

> [!NOTE]
> <span data-ttu-id="8a59a-121">यदि आपको एक से अधिक फ़ाइल प्रारूप आयात करने होंगे, तो आपको प्रत्येक प्रारूप प्रकार के लिए अलग आयात कार्य बनाने होंगे.</span><span class="sxs-lookup"><span data-stu-id="8a59a-121">If you must import more than one file format, you must create separate import jobs for each format type.</span></span>

## <a name="reassign-the-credit-card-transactions-for-terminated-employees"></a><span data-ttu-id="8a59a-122">निलम्बित कर्मचारियों के लिए क्रेडिट कार्ड के लेनदेन को फिर से असाइन करें</span><span class="sxs-lookup"><span data-stu-id="8a59a-122">Reassign the credit card transactions for terminated employees</span></span>

<span data-ttu-id="8a59a-123">कर्मचारी रिकॉर्ड समाप्त होने के बाद, कर्मचारी का एक्टिव डायरेक्ट्री डोमेन सर्विस (AD DS) खाता निष्क्रिय हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="8a59a-123">After an employee record is terminated, the employee’s Active Directory Domain Services (AD DS) account is disabled.</span></span> <span data-ttu-id="8a59a-124">हालांकि, सक्रिय क्रेडिट कार्ड लेनदेन हो सकते हैं जिन्हें अब भी खर्च किया जाना चाहिए और प्रतिपूर्ति की जानी चाहिए.</span><span class="sxs-lookup"><span data-stu-id="8a59a-124">However, there might be active credit card transactions that must still be expensed and reimbursed.</span></span> <span data-ttu-id="8a59a-125">**क्रेडिट कार्ड लेनदेन** पृष्ठ, आप किसी भी क्रेडिट कार्ड लेनदेन के लिए कर्मचारी को फिर से असाइन कर सकते हैं जहां संबद्ध कर्मचारी को निलम्बित कर दिया गया हो.</span><span class="sxs-lookup"><span data-stu-id="8a59a-125">From the **Credit card transactions** page, you can reassign the employee for any credit card transaction where the associated employee has been terminated.</span></span>

<span data-ttu-id="8a59a-126">एक या अधिक क्रेडिट कार्ड लेनदेन चुनें और फिर **लेनदेन पुन: असाइन करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="8a59a-126">Select one or more credit card transactions, and then select **Reassign transactions**.</span></span> <span data-ttu-id="8a59a-127">फिर आप क्रेडिट कार्ड लेनदेन को असाइन करने के लिए किसी अन्य कर्मचारी को चुन सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="8a59a-127">You can then select another employee to assign the credit card transactions to.</span></span> <span data-ttu-id="8a59a-128">क्रेडिट कार्ड के लेनदेन के बाद फिर से असाइन किया गया है तो उन्हें व्यय रिपोर्ट के लिए चुना जा सकता है और व्यय रिपोर्ट प्रतिपूर्ति के लिए सामान्य प्रक्रिया के माध्यम से भुगतान किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8a59a-128">After the credit card transactions have been reassigned, they can be selected for an expense report and paid through the usual process for expense report reimbursement.</span></span>
