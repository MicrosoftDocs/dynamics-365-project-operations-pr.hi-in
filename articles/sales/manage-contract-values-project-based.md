---
title: परियोजना-आधारित अनुबंध पंक्तियों के साथ कार्य करें
description: यह विषय परियोजना-आधारित अनुबंध पंक्तियों के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/28/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 14d880eccd5547c122ebe37b63022e64fa2fb6fe
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181723"
---
# <a name="work-with-projectbased-contract-lines"></a>परियोजना-आधारित अनुबंध पंक्तियों के साथ कार्य करें

Dynamics 365 Project Operations में परियोजना-आधारित अनुबंध पंक्तियाँ किसी सहभागिता पर परियोजना कार्य के विशिष्ट घटकों के लिए अनुमान और बिलिंग समझौतों को होल्ड करने के लिए डिज़ाइन की गई हैं. निम्न अवधारणाओं के साथ परियोजना अनुमानों और बिलिंग परिदृश्यों के लिए परियोजना-आधारित अनुबंध पंक्ति की संरचना को विस्तृत किया गया है:

- बिलिंग विधि
- परियोजना और कार्य मैपिंग
- शामिल ट्रांज़ैक्शन श्रेणियाँ
- सीमा-में रखें सीमा
- प्रभार्यता सेटअप
- अनुबंध पंक्ति विवरण का उपयोग करके अनुमान लगाता है
- अनुबंध पंक्ति ग्राहक

निम्न फ़ील्ड को परियोजना-आधारित अनुबंध पंक्ति के **सामान्य** टैब पर शामिल किया गया है. ये फ़ील्ड विस्तृत, जमीनी अनुमान और परियोजना-आधारित कार्य के लिए बिलिंग व्यवस्था हेतु आधार स्थापित करने में मदद करती हैं.

| क्षेत्र | विवरण | डाउनस्ट्रीम प्रभाव |
| --- | --- | --- |
| **नाम** | उस अनुबंध पंक्ति का नाम, जो अनुमान लगाए जा रहे अनुबंध के असतत घटक की पहचान करती है. किसी कोट से बनाए गए परियोजना अनुबंध के लिए, यह मान परियोजना-आधारित कोट पंक्ति के संगत मान से कॉपी किया जाता है. | इस फ़ील्ड मान को उस परियोजना इनवॉइस पंक्ति पर कॉपी किया गया है, जो इनवॉइस के बनाए जाने पर इस अनुबंध पंक्ति से बनाई गई है. |
| **बिलिंग विधि** | किसी कोट से बनाए गए परियोजना अनुबंध पर, यह मान संगत फ़ील्ड से कोट पंक्ति पर कॉपी किया जाता है. यह एक विकल्प सेट है, जो Project Operations द्वारा समर्थित दो मुख्य अनुबंध मॉडल का प्रतिनिधित्व करता है:</br>- **निश्चित मूल्य**</br>- **समय और सामग्री** | संदर्भित अनुबंध पंक्ति की बिलिंग पद्धति के आधार पर, वास्तविक ट्रांज़ैक्शन संसाधित किया जाएगा. यदि वास्तविक द्वारा संदर्भित अनुबंध पंक्ति में समय और सामग्री बिलिंग विधि होती है, तो लागत और बिल न किए गए विक्रय वास्तविक रिकॉर्ड बनाए जाते हैं. यदि वास्तविक द्वारा संदर्भित अनुबंध पंक्ति में एक निश्चित मूल्य बिलिंग विधि होती है, तो केवल वास्तविक लागत बनाई जाती है. |
| **Project** | इस फ़ील्ड का उपयोग उस परियोजना की पहचान करने के लिए करें, जिसका उपयोग इस सहभागिता पर कार्य वितरित करने के लिए किया जाएगा. | वास्तविक या अनुमान पंक्ति रिकॉर्ड पर अनुबंध पंक्ति संदर्भ को हल करने के लिए इस फ़ील्ड के मान का उपयोग **शामिल कार्य** और **शामिल ट्रांज़ैक्शन श्रेणियाँ** फ़ील्ड के संयोजन में किया जाता है. |
| **समय शामिल करें** | एक ध्वज इंगित करता है कि इस अनुबंध पंक्ति पर चयनित परियोजना पर समय ट्रांज़ैक्शन या लेबर लागत शामिल होगी या नहीं. **नहीं** मान इंगित करता है कि इस अनुबंध पंक्ति पर समय ट्रांज़ैक्शन या लेबर लागतें शामिल नहीं होंगी. **हाँ** मान इंगित करता है कि वह शामिल होगी. | वास्तविक या अनुमान पंक्ति रिकॉर्ड पर अनुबंध पंक्ति संदर्भ को हल करने के लिए इस फ़ील्ड मान का उपयोग परियोजना के संयोजन में किया जाता है. |
| **व्यय शामिल करें** | एक ध्वज इंगित करता है कि इस अनुबंध पंक्ति पर चयनित परियोजना पर व्यय लागत शामिल होगी या नहीं. **नहीं** मान इंगित करता है कि इस अनुबंध पंक्ति पर व्यय लागत शामिल नहीं होगी. **हाँ** मान इंगित करता है कि वह शामिल होगी. | वास्तविक या अनुमान पंक्ति रिकॉर्ड पर अनुबंध पंक्ति संदर्भ को हल करने के लिए इस फ़ील्ड मान का उपयोग परियोजना के संयोजन में किया जाता है. |
| **शुल्क शामिल करें** | एक ध्वज इंगित करता है कि इस अनुबंध पंक्ति पर चयनित परियोजना पर शुल्क शामिल होगा या नहीं. **नहीं** मान इंगित करता है कि इस अनुबंध पंक्ति पर शुल्क शामिल नहीं होगा. **हाँ** मान इंगित करता है कि वह शामिल होगी. | वास्तविक या अनुमान पंक्ति रिकॉर्ड पर अनुबंध पंक्ति संदर्भ को हल करने के लिए इस फ़ील्ड मान का उपयोग परियोजना के संयोजन में किया जाता है. |
| **अनुबंधित राशि** | एक निश्चित मूल्य अनुबंध पंक्ति पर, यह राशि वह सहमत मूल्य है, जो ग्राहक को इस अनुबंध पंक्ति से संबद्ध सभी कार्य घटकों के लिए इनवॉइस किया जाएगा. समय और सामग्री अनुबंध पंक्ति पर, यह राशि वह अनुमानित मूल्य है, जो ग्राहक को इस अनुबंध पंक्ति से संबद्ध सभी कार्य घटकों के लिए इनवॉइस किया जाएगा. किसी कोट से बनाए गए परियोजना अनुबंध पर, यह मान संगत फ़ील्ड से कोट पंक्ति पर कॉपी किया जाता है. जब किसी परियोजना-आधारित अनुबंध पंक्ति में पंक्ति विवरण होता है, तो यह फ़ील्ड संपादन के लिए लॉक हो जाती है और अनुबंध पंक्ति विवरण पर राशि से सारांशित होती है. | जब अनुबंध पंक्ति में पंक्ति विवरण होता है, तो यह मान पंक्ति विवरण पर राशि को बदलकर संशोधित किया जा सकता है. एक निश्चित मूल्य अनुबंध पंक्ति पर, इस मान का उपयोग आवधिक बिलिंग माइलस्टोन पर कर से पहले राशि जनरेट करने के लिए किया जाता है. |
| **अनुमानित कर** | उपयोगकर्ता अनुबंध पंक्ति पर अनुमानित कर राशि इनपुट करने के लिए इस फ़ील्ड को संपादित कर सकता है. जब किसी परियोजना-आधारित अनुबंध पंक्ति में पंक्ति विवरण होता है, तो यह फ़ील्ड संपादन के लिए लॉक हो जाती है और अनुबंध पंक्ति विवरण पर कर राशि से सारांशित होती है. | जब अनुबंध पंक्ति में पंक्ति विवरण होता है, तो यह मान पंक्ति विवरण पर कर राशि को बदलकर संशोधित किया जा सकता है. एक निश्चित मूल्य अनुबंध पंक्ति पर, इस मान का उपयोग आवधिक बिलिंग माइलस्टोन पर कर को जनरेट करने के लिए किया जाता है. |
| **कर के बाद अनुबंधित राशि** | कर के बाद अनुबंध पंक्ति राशि. यह फ़ील्ड केवल पढ़ने के लिए है और इसकी गणना **अनुबंधित राशि + कर** के रूप में की जाती है. | एक निश्चित मूल्य अनुबंध पंक्ति पर, इस मान का उपयोग आवधिक बिलिंग माइलस्टोन को जनरेट करने के लिए किया जाता है. |
| **सीमा-में-रखें सीमा** | उपयोगकर्ता इस फ़ील्ड को संपादित कर सकता है और यह केवल उन परियोजना-आधारित अनुबंध पंक्तियों पर उपलब्ध है, जिनमें समय और सामग्री बिलिंग पद्धति होती है. | उपयोगकर्ता इस फ़ील्ड को संपादित कर सकता है. जब समय और सामग्री के लिए कोई समय या व्यय वास्तविक इस अनुबंध पंक्ति को संदर्भित करता है, तो पहले से खर्च और प्रतिबद्ध राशियों के लिए लेखांकन करने के बाद वास्तविक पर राशि का मूल्यांकन अनुबंध पंक्ति पर सीमा-में-रखें सीमा के विरुद्ध किया जाता है. |
| **ग्राहक बजट** | यह फ़ील्ड संपादन योग्य है और यदि अनुबंध को कोट से बनाया गया था, तो उसे संगत फ़ील्ड से कोट पंक्ति पर कॉपी किया जाता है. | इस फ़ील्ड का उपयोग केवल जानकारी के लिए किया जाता है और इसका कोई महत्व नहीं है. |

## <a name="validation-rule-for-the-options-on-the-general-tab-of-project-based-contract-lines"></a>परियोजना-आधारित अनुबंध पंक्तियों के सामान्य टैब पर विकल्पों के लिए सत्यापन नियम

नियम: परियोजना और एक निश्चित ट्रांज़ैक्शन श्रेणी को अनुबंध में केवल एक परियोजना-आधारित अनुबंध पंक्ति पर शामिल किया जा सकता है.

| अनुबंध | अनुबंध पंक्ति | Project | समय शामिल करें | व्यय शामिल करें | शुल्क शामिल करें | मान्य/मान्य नहीं | कारण                                                                                                                                                                                                  |
|----------|---------------|---------|--------------|-----------------|-------------|-----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| C1       | CL1           | P1      | हाँ          | हाँ             | हाँ         | मान्य नहीं है       | नियम का उल्लंघन करता है. परियोजना P1 पर समय, व्यय और शुल्क को दोनों अनुबंध पंक्तियों, CL1 और CL2 पर शामिल किया जाता है.                                                                                       |
| C1       | CL2           | P1      | हाँ          | हाँ             | हाँ         | मान्य नहीं है       | नियम का उल्लंघन करता है. परियोजना P1 पर समय, व्यय और शुल्क को दोनों अनुबंध पंक्तियों, CL1 और CL2 पर शामिल किया जाता है.                                                                                       |
| C1       | CL1           | P1      | हाँ          | No              | हाँ         | मान्य नहीं है       | नियम का उल्लंघन करता है. परियोजना P1 पर समय और शुल्क को दोनों अनुबंध पंक्तियों, CL1 और CL2 पर शामिल किया जाता है.                                                                                                   |
| C1       | CL2           | P1      | हाँ          | हाँ             | हाँ         | मान्य नहीं है       | नियम का उल्लंघन करता है. परियोजना P1 पर समय और शुल्क को दोनों अनुबंध पंक्तियों, CL1 और CL2 पर शामिल किया जाता है.                                                                                                   |
| C1       | CL1           | P1      | हाँ          | No              | हाँ         | मान्य           | परियोजना P1 पर समय और शुल्क को CL1 पर शामिल किया जाता है. परियोजना P1 पर व्यय को CL2 पर शामिल किया गया है. </br>   प्रत्येक अनुबंध पंक्ति पर जो शामिल किया जा रहा है उसमें कोई ओवरलैप नहीं है और इसलिए मान्य है.  |
| C1       | CL2           | P1      | No           | हाँ             | No          | मान्य           | परियोजना P1 पर समय और शुल्क को CL1 पर शामिल किया जाता है. परियोजना P1 पर व्यय को CL2 पर शामिल किया गया है. </br>   प्रत्येक अनुबंध पंक्ति पर जो शामिल किया जा रहा है उसमें कोई ओवरलैप नहीं है और इसलिए मान्य है.  |
| C1       | CL1           | P1      | हाँ          | हाँ             | हाँ         | मान्य नहीं है       | नियम का उल्लंघन करता है. परियोजना P1 पर समय, व्यय और शुल्क को दो अनुबंधों की पंक्तियों पर शामिल किया जाता है.                                                                                               |
| CL2      | CL2           | P1      | हाँ          | हाँ             | हाँ         | मान्य नहीं है       | नियम का उल्लंघन करता है. परियोजना P1 पर समय, व्यय और शुल्क को दो अनुबंधों की पंक्तियों पर शामिल किया जाता है.                                                                                               |