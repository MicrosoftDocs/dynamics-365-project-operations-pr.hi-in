---
title: परियोजना अनुबंधों पर एकाधिक ग्राहकों को प्रबंधित करें - लाइट
description: यह विषय परियोजना अनुबंधों पर एकाधिक ग्राहकों को प्रबंधित करने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/27/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b248dabdbd5239b140da7c99d3f38609facfe75e
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181319"
---
# <a name="manage-multiple-customers-on-project-contracts---lite"></a>परियोजना अनुबंधों पर एकाधिक ग्राहकों को प्रबंधित करें - लाइट

_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_

Dynamics 365 Project Operations में परियोजना अनुबंध उस परिदृश्य का समर्थन करते हैं, जहां एक संविदाजन्य करार में ऐसे कई ग्राहकों को शामिल किया जाता है, जो एक सौदे का वित्तपोषण कर रहे हैं. **परियोजना अनुबंध** पृष्ठ के **सारांश** टैब में **ग्राहक** फ़ील्ड शामिल है. यह फ़ील्ड सौदे के प्राथमिक ग्राहक की पहचान करती है. सौदे के लिए अन्य ग्राहकों को **परियोजना अनुबंध** पृष्ठ के **ग्राहक** टैब पर सेट अप किया जा सकता है.

परियोजना अनुबंध पर सूचीबद्ध सभी अनुबंध ग्राहक, परियोजना अनुबंध के लिए बनाई गई नई परियोजना-आधारित अनुबंध पंक्तियों पर अनुबंध पंक्ति ग्राहकों के रूप में डिफ़ॉल्ट होते हैं. मौजूदा परियोजना-आधारित अनुबंध पंक्तियाँ नए अनुबंध ग्राहकों को इनहेरिट नहीं करती हैं, क्योंकि नए रिकॉर्ड बनाए जाते हैं.

उत्पाद-आधारित अनुबंध पंक्तियाँ स्वचालित रूप से प्राथमिक ग्राहक से संबद्ध होती हैं.

अनुबंध हासिल किए जाने से पहले अनुबंध ग्राहक और अनुबंध पंक्ति ग्राहक किसी भी समय जोड़े, अद्यतन या हटाए जा सकते हैं.

## <a name="primary-customer"></a>प्राथमिक ग्राहक

परियोजना अनुबंध के **सारांश** टैब पर संभावित ग्राहक के रूप में सूचीबद्ध ग्राहक अनुबंध का प्राथमिक ग्राहक होता है. जब आप अनुबंध की ग्राहक सूची से प्राथमिक ग्राहक को हटाने का प्रयास करेंगे, तो आपको एक त्रुटि संदेश प्राप्त होगा कि अनुबंध पर प्राथमिक ग्राहक रिकॉर्ड को हटाया नहीं जा सकता है.

अनुबंध ग्राहक सूची से प्राथमिक ग्राहक अद्यतन नहीं किया जा सकता है. इसके बजाय, अनुबंध के **सारांश** टैब पर संभावित ग्राहक को बदलें. जब इस फ़ील्ड को **अनुबंध सारांश** पृष्ठ पर अद्यतन किया जाता है, तो **प्राथमिक** ध्वज सेट के साथ नए ग्राहक को एक नए अनुबंध ग्राहक के रूप में जोड़ा जाता है. पिछला प्राथमिक ग्राहक अभी भी अनुबंध का एक ग्राहक रहेगा.

## <a name="create-update-or-delete-a-contract-customer-record"></a>अनुबंध ग्राहक रिकॉर्ड बनाएं, अद्यतन करें या हटाएं

**परियोजना अनुबंध** पृष्ठ के **ग्राहक** टैब से अनुबंध ग्राहक को बनाया, अद्यतन या हटाया जा सकता है. निम्न तालिका में फ़ील्ड परियोजना अनुबंध के अनुबंध ग्राहक रिकॉर्ड पर हैं और अनुबंध के साथ कार्य करने के दौरान ध्यान में रखी जानी चाहिए.

| क्षेत्र | स्थान | विवरण | डाउनस्ट्रीम प्रभाव |
| --- | --- | --- | --- |
| **खाता** | **अनुबंध ग्राहक** टैब और अनुबंध ग्राहक के लिए **मुख्य** और **त्वरित निर्माण** प्रपत्र पर ग्रिड संपादित की जा सकती है. | सभी सक्रिय खातों को सूचीबद्ध करता है. रिकॉर्ड बनने के बाद इस फील्ड को लॉक कर दिया जाता है. खाता अद्यतन करने के लिए, रिकॉर्ड हटाएं और उसे पुनः बनाएँ. यदि आपने वास्तविक रिकॉर्ड किए हैं या यदि अनुबंध ग्राहक रिकॉर्ड प्राथमिक ग्राहक है, तो आप रिकॉर्ड को हटा नहीं सकते. | अनुबंध पंक्ति बनाए जाने पर, अनुबंध ग्राहकों को अनुबंध पंक्ति ग्राहकों के रूप में कॉपी किया जाता है. |
| **बिलिंग स्प्लिट प्रतिशत** | **अनुबंध ग्राहक** टैब और अनुबंध ग्राहक के लिए **मुख्य** और **त्वरित निर्माण** प्रपत्र पर ग्रिड संपादित की जा सकती है. | उन प्रत्येक बिल न किए गए विक्रय ट्रांज़ैक्शन के प्रतिशत का प्रतिनिधित्व करती है, जिसे इस अनुबंध ग्राहक के लिए एट्रिब्यूट किया गया है. | नई अनुबंध पंक्तियों पर और नई परियोजना अनुबंध पंक्तियों पर परियोजना अनुबंध पंक्ति ग्राहकों पर कॉपी किया जाता है. |
| **बिल प्रेषण संपर्क नाम** | **अनुबंध ग्राहक** टैब और अनुबंध ग्राहक के लिए **मुख्य** और **त्वरित निर्माण** प्रपत्र पर ग्रिड संपादित की जा सकती है. | इस पाठ फ़ील्ड का उपयोग इस ग्राहक के लिए इंवॉयस देने वाले संपर्क व्यक्ति की पहचान के लिए किया जाना चाहिए. यह फ़ील्ड संबंधित खाता रिकॉर्ड से डिफ़ॉल्ट है. | इस ग्राहक के लिए जनरेट की गई इनवॉइस पर **अनुबंध नाम को बिल करें** फ़ील्ड पर कॉपी किया जाता है. |
| **इस नाम से बिल करें** | **अनुबंध ग्राहक** टैब और अनुबंध ग्राहक के लिए **मुख्य** और **त्वरित निर्माण** प्रपत्र पर ग्रिड संपादित की जा सकती है | इस पाठ फ़ील्ड का उपयोग इस ग्राहक के लिए इंवॉयस देने वाले संपर्क व्यक्ति की पहचान के लिए किया जाना चाहिए. यह फ़ील्ड संबंधित खाता रिकॉर्ड से डिफ़ॉल्ट है. | इस ग्राहक के लिए जनरेट की गई इनवॉइस पर **अनुबंध नाम को बिल करें** फ़ील्ड पर कॉपी किया जाता है. |
| **भुगतान शर्तें** | **अनुबंध ग्राहक** टैब और अनुबंध ग्राहक के लिए **मुख्य** और **त्वरित निर्माण** प्रपत्र पर ग्रिड संपादित की जा सकती है. | मान संबंधित खाता रिकॉर्ड से डिफ़ॉल्ट हैं. | इस ग्राहक के लिए जनरेट की गई इनवॉइस पर **अनुबंध नाम को बिल करें** फ़ील्ड पर कॉपी किया जाता है. |
| **राउंडिंग है** | **अनुबंध ग्राहक** टैब और अनुबंध ग्राहक के लिए **मुख्य** और **त्वरित निर्माण** प्रपत्र पर ग्रिड संपादित की जा सकती है. | इंगित करता है कि क्या यह ग्राहक इस समझौते के लिए एक डिफ़ॉल्ट पूर्ण ग्राहक है. परियोजना अनुबंध पर केवल एक राउंडिंग ग्राहक हो सकता है. | जब मात्रा पर विभाजित लागत और बिल न की गई विक्रय के कारण राउंडिंग अंतर होता है, तो वह अंतर इस ग्राहक पर मैप किए गए वास्तविक पर लागू होता है. |
| **सीमा-में-रखें सीमा** | **अनुबंध ग्राहक** टैब और अनुबंध ग्राहक के लिए **मुख्य** और **त्वरित निर्माण** प्रपत्र पर ग्रिड संपादित की जा सकती है | इंगित करता है कि उस समस्त राशि के लिए कोई निगोशिएट की गई सीमा या कैप होगी या नहीं, जो इस सहभागिता के लिए ग्राहक को इनवॉइस की जाएगी. | अनुबंध ग्राहक स्तर पर सेट अप की गई **सीमा-में-रखें सीमा** उन **बिल न किए गए विक्रय वास्तविक** पर मूल्यांकित की जाएगी, जो इस अनुबंध ग्राहक को संदर्भित करते हैं. |

## <a name="edit-billing-split-percentages"></a>बिलिंग विभाजन प्रतिशत संपादित करें

इन-लाइन ग्रिड संपादन अनुभव का उपयोग करके बिलिंग विभाजन प्रतिशत को संपादित किया जा सकता है. जब बिलिंग विभाजन प्रतिशत का योग 100 प्रतिशत नहीं होगा, तो एक त्रुटि प्राप्त होगी. बिलिंग विभाजन प्रतिशत संपादित करने के बाद, त्रुटि को खारिज करने के लिए पृष्ठ को रीफ़्रेश करें.

सभी अनुबंध ग्राहकों को समान रूप से बिलिंग विभाजन आवंटित करने के लिए आप **अनुबंध ग्राहक** सबग्रिड पर **समान रूप से वितरित करें**  भी चुन सकते हैं. यदि कोई राउंडिंग फ़ैक्टर मौजूद है, तो उसे राउंडिंग ग्राहक में जोड़ा जाएगा. अनुबंध ग्राहकों में से एक को हमेशा **राउंडिंग** ग्राहक के रूप में टैग किया जाता है, जिसका अर्थ है कि अनुबंध ग्राहक रिकॉर्ड में राउंडिंग ध्वज **हाँ** पर सेट है. आमतौर पर, यह अनुबंध का प्राथमिक ग्राहक है, लेकिन इसे भी बदला जा सकता है.