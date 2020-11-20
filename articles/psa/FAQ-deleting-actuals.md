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
ms.openlocfilehash: b9b45e3ae0cd9273af4d2a5cd9cce30502c0aa78
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127160"
---
# <a name="why-cant-i-delete-records-from-the-actuals-entity"></a>मैं वास्तविक निकाय से रिकॉर्ड क्यों नहीं हटा सकता?

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Project Service Automation (PSA) आपको वास्तविक को हटाने की अनुमति नहीं देता है क्योंकि वे लेन-देन के लिए सच्चाई के स्रोत के रूप में कार्य करते हैं, जिनका डाउनस्ट्रीम सिस्टम में वित्तीय प्रभाव होता है, जैसे कि सामान्य खाता-बही। अगर वास्तविक को हटाया जा सकता है, तो वित्तीय रिपोर्टिंग लेन-देन की ईमानदारी पर सवाल उठाया जा सकता है। ऑडिट ट्रेल स्थापित करने के लिए, ग्राहकों को क्षतिपूर्ति लेन-देन बनाने के लिए जर्नल का उपयोग करना चाहिए।

