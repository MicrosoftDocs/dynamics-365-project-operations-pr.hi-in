---
title: संसाधन का अनुमान
description: यह विषय परियोजना संचालन में संसाधन अनुमान की गणना के बारे में जानकारी देता है।
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 2ebde2b3c5bcfb5faa02ee476065ac34b1953432
ms.sourcegitcommit: f255b2cbf290973ce62fe2c1c121bd1df15a7392
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/01/2020
ms.locfileid: "3928572"
---
# <a name="resource-estimates"></a>संसाधन का अनुमान

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

संसाधन के अनुमान चरणबद्ध प्रयासों से आते हैं, जो लागू मूल्य निर्धारण आयामों के साथ-साथ काम के रुकने की संरचना में परिभाषित होते हैं। आमतौर पर, गणना **प्रत्येक भूमिका x घंटे के लिए दर/घंटा है।** प्रत्येक संसाधन के लिए चरणबद्ध प्रयास संसाधन को असाइनमेंट रिकॉर्ड में रखा जाता है। मूल्य निर्धारण को पूर्व-निर्धारित मूल्य सूची में रखा जाता है। लागू मूल्य सूची के आधार पर इकाई रूपांतरण लागू किया जाता है।

![संसाधन का अनुमान](./media/navigation12.png)

## <a name="default-cost-price-and-cost-currency"></a>डिफ़ॉल्ट लागत मूल्य और लागत मुद्रा

संगठनात्मक इकाई से लागत मूल्य डिफ़ॉल्ट हैं।

## <a name="default-bill-rate-and-sales-currency"></a>डिफ़ॉल्ट बिल दर और बिक्री मुद्रा

बिक्री मूल्य प्रति सौदा एक बार लागू होते हैं। बिक्री मूल्य सूची डिफ़ॉल्ट के लिए पदानुक्रम इस प्रकार है:

1. संगठन
2. ग्राहक
3. कोट/अनुबंध
