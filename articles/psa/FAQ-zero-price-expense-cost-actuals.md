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
# <a name="why-is-the-price-defaulting-to-zero-on-expense-cost-actuals"></a>व्यय लागत वास्तविक पर मूल्य को शून्य पर डिफ़ॉल्ट क्यों बनाया गया है

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

यह सामान्य प्रश्न उन व्यय वास्तविक के लिए लागू होता है जहाँ लेनदेन श्रेणी व्यय पर और लेनदेन प्रकार लागत पर सेट है.

## <a name="troubleshooting-cost-rates-on-expense-cost-actuals"></a>व्यय लागत वास्तविक पर लागत दर से जुड़ी समस्या का निवारण

संबंधित व्यय प्रविष्टि पर जाएँ और सुनिश्चित करें कि व्यय प्रविष्टि फ़ील्ड में कोई राशि है. यदि व्यय प्रविष्टि के लिए मात्रा फ़ील्ड भरी नहीं गई है, तो आपने समस्या का पता लगा लिया है.
 
इस समस्या को हल करने के लिए, एक मान्य राशि दे कर व्यय प्रविष्टि को फिर से बनाएँ और इसे स्वीकृति दें.