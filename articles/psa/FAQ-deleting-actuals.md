---
title: मैं वास्तविक निकाय से रिकॉर्ड क्यों नहीं हटा सकता?
description: यह विषय इस बारे में जानकारी प्रदान करता है कि आप वास्तविक इकाई से रिकॉर्ड क्यों नहीं हटा सकते।
author: JPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: f47e7ccd46642dc6129fbb3beac3c9490160d046
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077826"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a>मैं वास्तविक निकाय से रिकॉर्ड क्यों नहीं हटा सकता?

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Project Service Automation (PSA) आपको वास्तविक को हटाने की अनुमति नहीं देता है क्योंकि वे लेन-देन के लिए सच्चाई के स्रोत के रूप में कार्य करते हैं, जिनका डाउनस्ट्रीम सिस्टम में वित्तीय प्रभाव होता है, जैसे कि सामान्य खाता-बही। अगर वास्तविक को हटाया जा सकता है, तो वित्तीय रिपोर्टिंग लेन-देन की ईमानदारी पर सवाल उठाया जा सकता है। ऑडिट ट्रेल स्थापित करने के लिए, ग्राहकों को क्षतिपूर्ति लेन-देन बनाने के लिए जर्नल का उपयोग करना चाहिए।

