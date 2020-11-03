---
title: व्यय लागत वास्तविक पर मूल्य को शून्य पर डिफ़ॉल्ट क्यों बनाया जा रहा है?
description: इस समस्या का निवारण करना कि व्यय लागत वास्तविक पर मूल्य को 0 पर डिफ़ॉल्ट क्यों बनाया जा रहा है.
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/22/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 9f4ff8a96250d675faeda3246c2d0a6c5bd83286
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077721"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="3e49a-103">व्यय लागत वास्तविक पर मूल्य को शून्य पर डिफ़ॉल्ट क्यों बनाया जा रहा है?</span><span class="sxs-lookup"><span data-stu-id="3e49a-103">Why is the price defaulting to zero on expense cost actuals?</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="3e49a-104">यह सामान्य प्रश्न उन व्यय वास्तविक के लिए लागू होता है जहाँ लेनदेन श्रेणी व्यय पर और लेनदेन प्रकार लागत पर सेट है.</span><span class="sxs-lookup"><span data-stu-id="3e49a-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="3e49a-105">व्यय लागत वास्तविक पर लागत दर से जुड़ी समस्या का निवारण</span><span class="sxs-lookup"><span data-stu-id="3e49a-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="3e49a-106">संबंधित व्यय प्रविष्टि पर जाएँ और सुनिश्चित करें कि व्यय प्रविष्टि फ़ील्ड में कोई राशि है.</span><span class="sxs-lookup"><span data-stu-id="3e49a-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="3e49a-107">यदि व्यय प्रविष्टि के लिए मात्रा फ़ील्ड भरी नहीं गई है, तो आपने समस्या का पता लगा लिया है.</span><span class="sxs-lookup"><span data-stu-id="3e49a-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="3e49a-108">इस समस्या को हल करने के लिए, एक मान्य राशि दे कर व्यय प्रविष्टि को फिर से बनाएँ और इसे स्वीकृति दें.</span><span class="sxs-lookup"><span data-stu-id="3e49a-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>
