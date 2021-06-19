---
title: प्रोजेक्ट कोटेशन का विश्लेषण
description: यह विषय प्रोजेक्ट कोटेशन के विश्लेषण के बारे में जानकारी प्रदान करता है।
author: rumant
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
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
ms.openlocfilehash: acb3f1a2020cfd59f60f828e9092bd7ccde00077
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6012453"
---
# <a name="analysis-of-project-quotes"></a>प्रोजेक्ट कोटेशन का विश्लेषण

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

Dynamics 365 Project Service Automation लाभप्रदता का अनुमान लगाने के लिए प्रोजेक्ट कोटेशन का विश्लेषण करता है। यह भी विश्लेषण करता है कि डिलीवरी की तारीख या पूर्णता तिथि और बजट के बारे में ग्राहकों की अपेक्षाओं के साथ कोटेशन कितनी अच्छी तरह से मेल खाता है।

## <a name="profitability-analysis"></a>लाभप्रदता का विश्लेषण

Project Service Automation सकल मार्जिन और समायोजित सकल मार्जिन का उपयोग करके लाभप्रदता का विश्लेषण करता है।

- सकल मार्जिन की गणना निम्न सूत्र का उपयोग करके की जाती है:

  `
    (Sum of estimated chargeable sales value – Sum of estimated chargeable costs) x 100
  `
- समायोजित सकल मार्जिन की गणना निम्न सूत्र का उपयोग करके की जाती है:

  `
    (Sum of estimated chargeable sales value – Sum of all estimated costs) x 100
  `

यदि सकल मार्जिन और समायोजित सकल मार्जिन के लिए मान एक विस्तृत मार्जिन से भिन्न होते हैं, तो कोटेशन में अधिकांश काम गैर-प्रभार्य के रूप में वर्गीकृत किया जाता है।

## <a name="analysis-of-customer-expectations"></a>ग्राहक की उम्मीदों का विश्लेषण

यदि आप निम्न फ़ील्ड के लिए मान दर्ज करते हैं, तो शेड्यूल और बजट के बारे में ग्राहकों की अपेक्षाओं के लिए आप कोटेशन का विश्लेषण और चार्ट तैयार कर सकते हैं:

- कोटेशन हेडर पर **अनुरोधित डिलीवरी की तिथि** फ़ील्ड.
- **ग्राहक बजट** प्रत्येक कोटेशन लाइन (प्रोजेक्ट-आधारित लाइनों और उत्पाद-आधारित लाइनों के लिए)।

शेड्यूल के बारे में ग्राहकों की अपेक्षाओं का विश्लेषण कोटेशन लाइन की नवीनतम अंतिम तिथि को कोटेशन में सभी कोटेशन लाइनों में अनुरोधित डिलीवरी तिथि के साथ तुलना करके किया जाता है।

बजट के बारे में ग्राहकों की अपेक्षाओं का विश्लेषण कुल ग्राहक बजट के योग की तुलना में सभी कोटेशन लाइनों में कोटेशन की राशि के साथ किया जाता है।


[!INCLUDE[footer-include](../includes/footer-banner.md)]