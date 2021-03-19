---
title: मैं वास्तविक निकाय से रिकॉर्ड क्यों नहीं हटा सकता?
description: यह विषय इस बारे में जानकारी प्रदान करता है कि आप वास्तविक इकाई से रिकॉर्ड क्यों नहीं हटा सकते।
author: JPBurrows
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 11/6/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: e3122c5d9495b3ff9a683f477e719ce0c228a84d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5286070"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a><span data-ttu-id="ef1bf-103">मैं वास्तविक निकाय से रिकॉर्ड क्यों नहीं हटा सकता?</span><span class="sxs-lookup"><span data-stu-id="ef1bf-103">Why can’t I delete records from the Actuals entity?</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="ef1bf-104">Project Service Automation (PSA) आपको वास्तविक को हटाने की अनुमति नहीं देता है क्योंकि वे लेन-देन के लिए सच्चाई के स्रोत के रूप में कार्य करते हैं, जिनका डाउनस्ट्रीम सिस्टम में वित्तीय प्रभाव होता है, जैसे कि सामान्य खाता-बही।</span><span class="sxs-lookup"><span data-stu-id="ef1bf-104">Project Service Automation (PSA) doesn't allow you to delete actuals because they serve as the source of truth for transactions that have financial implications to downstream systems, such as the general ledger.</span></span> <span data-ttu-id="ef1bf-105">अगर वास्तविक को हटाया जा सकता है, तो वित्तीय रिपोर्टिंग लेन-देन की ईमानदारी पर सवाल उठाया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="ef1bf-105">If actuals could be deleted, the integrity of the financial reporting transactions could be questioned.</span></span> <span data-ttu-id="ef1bf-106">ऑडिट ट्रेल स्थापित करने के लिए, ग्राहकों को क्षतिपूर्ति लेन-देन बनाने के लिए जर्नल का उपयोग करना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="ef1bf-106">To establish an audit trail, customers should use journals to create compensating transactions.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]