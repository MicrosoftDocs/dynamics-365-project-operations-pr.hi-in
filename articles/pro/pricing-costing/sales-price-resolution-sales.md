---
title: अनुमानों और वास्तविक के लिए विक्रय मूल्यों का समाधान करें - लाइट
description: य विषय विक्रय मूल्य संबंधी अनुमानित और वास्तविक को लेकर समाधान प्रस्तुत करता है.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 92cebbe851c3cface86d0580e7e060134295e8c2
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/30/2020
ms.locfileid: "4176748"
---
# <a name="resolve-sales-prices-for-estimates-and-actuals---lite"></a>अनुमानों और वास्तविक के लिए विक्रय मूल्यों का समाधान करें - लाइट

_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_

जब अनुमानित और वास्तविक विक्रय मूल्यों को Dynamics 365 प्रकल्प परिचालन के द्वारा हल किया जाता है, तब सिस्टम द्वारा पहले तारीख और मुद्रा को लिया जाता है जो संबद्ध प्रकल्प की हो अथवा विक्रय मूल्य सूची के अनुबंध को आधार माना जाता है. विक्रय मूल्य सूची संबंधी स्थिति हल होने पर, सिस्टम द्वारा विक्रय या बिल की दर को हल किया जाता है.

## <a name="resolve-sales-rates-on-actual-and-estimate-lines-for-time"></a>विक्रय दरों को वास्तविक और अनुमानित समय रेखा के अनुसार हल किया जाता है

प्रकल्प परिचाल मे, अनुमानित समय संबंधी रेखाओं का उपयोग कोट रेखा को दर्शाने के लिये और अनुबंध रेखा संबंधी जानकारी समय और स्रोत संबंधी प्रकल्प के कार्यों के लिये होता है.

विक्रय की मूल्य सूची संबंधी स्थिति के हल होने पर, सिस्टम द्वारा निम्न चरणों में बिल दर के डिफॉल्ट हेतु पूरा किया जाता है.

1. सिस्टम द्वारा **रोल** और **स्रोत इकाई** फील्ड्स को समय के अनुमानित रेखाओं के फील्ड्स पर रखा जाता है, जिससे उन्हे मूल्य सूची संबंधी रोल मूल्य के साथ इसे हल करने के लिये लिया जा सके. इस मिलान में यह अनुमान लगाया जाता है कि बिल दर के लिये पूरी तरह से अलग मूल्य का उपयोग किया गया है. यदि आपने मूल्यों को अन्य फील्ड्स के आधार पर कॉन्फिगर किया है, न कि या फिर साथ में **रोल** और **स्रोत इकाई** के, तब यह संयोजन है, जिसका उपयोग रोल मूल्य रेखा के मिलान हेतु किया जाएगा.
2. यदि सिस्टम द्वारा रोल मूल्य रेखा को बिल दर पर पाया जाता है जो कि **रोल** और **स्रोत इकाई** फील्ड संयोजन के लिये है, तब वह बिल दर डिफॉल्ट है.
3. यदि सिस्टम **रोल** और **स्रोत इकाई** फील्ड मूल्यों का मिलान नही कर पाता है, तब वह रोल मूल्य रेखा प्राप्त करता है जो रोल के साथ मिलान करती है परंतु उसमें **स्रोत इकाई** के लिये कोई मूल्य नही होता है. सिस्टम द्वारा मिलान रोल मूल्य रेकॉर्ड को पा लिया जाता है, यह उस रेकॉर्ड से बिल दर को डिफॉल्ट रुप में ले आता है. इस मिलान में एक पूरी तरह से अलग कॉन्फिगरेशन है जो कि **रोल** संबंधी एकदम अलग प्राथमिकता विरुद्ध **स्रोत इकाई** में विक्रय मूल्य आयामों के अनुरुप होती है.

> [!NOTE]
> यदि आपने **रोल** और **स्रोत इकाई** में से कुछ अलग प्राथमिकता कॉन्फिगर की है, अथवा आपके पास उच्च प्राथमिकता को लेकर कोई और आयाम है, तब यह व्यवहार भी उसी के अनुरुप बदल जाएगा. सिस्टम द्वारा रोल मूल्य रेकॉर्ड्स को मिलान मूल्य के साथ निकाला जाता है जिसमें समान मूल्य आयाम होते हैं जिससे प्राथमिकता के क्रम पर रेखाओं के साथ काम किया जा सकें, जिनमें इन आयामों के लिये जो अंत में आ रहे हैं, शून्य मूल्य है.

## <a name="resolve-sales-rates-on-actual-and-estimate-lines-for-expense"></a>खर्च हेतु विक्रय दर को वास्तविक व अनुमानित के मध्य हल कीजिये

प्रकल्प परिचालन में, व्यय की अनुमानित रेखाओं का उपयोग कोट रेखा के लिये और अनुबंध रेखा के विस्तार को व्यय के अनुमानित रुप में प्रकल्प हेतु किया जाता है.

जब विक्रय हेतु मूल्य सूची का हल निकल आता है, सिस्टम द्वारा निम्न चरणों के साथ इकाई विक्रय मूल्य को पूरा किया जाता है.

1. सिस्टम द्वारा **श्रेणी** और **इकाई** फील्ड के संयोजन को अनुमानित खर्च रेखा के लिये उपयोग में लाया जाता है और इसे श्रेणी मूल्य रेखा के साथ मिलान का प्रयत्न किया जाता है जिसकी मूल्य सूची हल हो चुकी है.
2. यदि सिस्टम द्वारा मूल्य रेखा की श्रेणी को विक्रय दर के साथ पाया जाता है जिसमें **श्रेणी** और **इकाई** फील्ड का संयोजन है, तब विक्रय दर डिफॉल्ट होता है.
3. यदि सिस्टम द्वारा मिलान श्रेणी की मूल्य रेखा पाई जाती है, तब मूल्य पद्धति का उपयोग विक्रय मूल्य को डिफॉल्ट करने के लिये किया जाता है. निम्न तालिका खर्च मूल्य के डिफॉल्ट व्यवहार को प्रकल्प परिचालन में दर्शाती है.

    | संदर्भ | मूल्य निर्धारण विधि | डिफ़ॉल्ट मूल्य |
    | --- | --- | --- |
    | अनुमान | मूल्य प्रति इकाई | श्रेणी मूल्य रेखा के आधार पर |
    | &nbsp; | लागत के बराबर | 0.00 |
    | &nbsp; | लागत पर मार्कअप | 0.00 |
    | वास्तविक | मूल्य प्रति इकाई | श्रेणी मूल्य रेखा के आधार पर |
    | &nbsp; | लागत के बराबर | संबंधित वास्तविक लागत के आधार पर |
    | &nbsp; | लागत पर मार्कअप | श्रेणी मूल्य रेखा के अनुसार परिभाषित मार्क अप को लागू करें जो कि इकाई लागत दर को संबद्ध वास्तविक लागत के अनुरुप रखे |

4. यदि सिस्टम **श्रेणी** और **इकाई** फील्ड के मूल्यों में मिलान में सक्षम नही है, तब विक्रय दर डिफॉल्ट शून्य (0) पर रहेगा.