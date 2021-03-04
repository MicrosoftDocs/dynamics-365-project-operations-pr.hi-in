---
title: व्यय लागत वास्तविक पर मूल्य को शून्य पर डिफ़ॉल्ट क्यों बनाया जा रहा है?
description: इस समस्या का निवारण करना कि व्यय लागत वास्तविक पर मूल्य को 0 पर डिफ़ॉल्ट क्यों बनाया जा रहा है.
author: rumant
manager: kfend
ms.service: project-operations
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
ms.openlocfilehash: f6ea664f9f38621ce5d1b0dd033d7df491f845ff
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/10/2021
ms.locfileid: "5146350"
---
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a><span data-ttu-id="8c5b9-103">व्यय लागत वास्तविक पर मूल्य को शून्य पर डिफ़ॉल्ट क्यों बनाया गया है</span><span class="sxs-lookup"><span data-stu-id="8c5b9-103">Why is the price defaulting to zero on expense cost actuals</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="8c5b9-104">यह सामान्य प्रश्न उन व्यय वास्तविक के लिए लागू होता है जहाँ लेनदेन श्रेणी व्यय पर और लेनदेन प्रकार लागत पर सेट है.</span><span class="sxs-lookup"><span data-stu-id="8c5b9-104">This FAQ applies to expense actuals where the transaction class is set to Expense and transaction type is Cost.</span></span>

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a><span data-ttu-id="8c5b9-105">व्यय लागत वास्तविक पर लागत दर से जुड़ी समस्या का निवारण</span><span class="sxs-lookup"><span data-stu-id="8c5b9-105">Troubleshooting cost rates on expense cost actuals</span></span>

<span data-ttu-id="8c5b9-106">संबंधित व्यय प्रविष्टि पर जाएँ और सुनिश्चित करें कि व्यय प्रविष्टि फ़ील्ड में कोई राशि है.</span><span class="sxs-lookup"><span data-stu-id="8c5b9-106">Go to the related expense entry and make sure that there’s an amount in the expense entry field.</span></span> <span data-ttu-id="8c5b9-107">यदि व्यय प्रविष्टि के लिए मात्रा फ़ील्ड भरी नहीं गई है, तो आपने समस्या का पता लगा लिया है.</span><span class="sxs-lookup"><span data-stu-id="8c5b9-107">If the originating expense entry didn’t have the amount field filled, then you have isolated the problem.</span></span>
 
<span data-ttu-id="8c5b9-108">इस समस्या को हल करने के लिए, एक मान्य राशि दे कर व्यय प्रविष्टि को फिर से बनाएँ और इसे स्वीकृति दें.</span><span class="sxs-lookup"><span data-stu-id="8c5b9-108">To solve this problem, recreate the expense entry with a valid amount and approve it.</span></span>
