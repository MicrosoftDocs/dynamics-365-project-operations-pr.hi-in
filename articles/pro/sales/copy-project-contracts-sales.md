---
title: परियोजना अनुबंधों की प्रतिलिपि बनाएँ - लाइट
description: इस विषय में Project Operations में परियोजना संपर्क की प्रतिलिपि बनाने की जानकारी दी गई है.
author: rumant
manager: Annbe
ms.date: 10/07/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 4137fc400c7fdd8fecd9d8349bf7f57f3470b51f
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181409"
---
# <a name="copy-project-contracts---lite"></a>परियोजना अनुबंधों की प्रतिलिपि बनाएँ - लाइट

_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_

आप आसानी से मौजूदा अनुबंधों की कॉपी को दो तरीके में से किसी एक में बनाकर नए परियोजना अनुबंधों को तैयार कर सकते हैं: 

  - **परियोजना अनुबंध** सूची पृष्ठ पर, एक/किसी परियोजना अनुबंध को चुनें और फिर **कॉपी** चुनें.
  - **परियोजना अनुबंध** विवरण पृष्ठ पर, **कॉपी** चुनें.

एक संवाद पृष्ठ खुलेगा, जहां आप कॉपी किए अनुबंध से मापदंडों को चुन सकते हैं. निम्न क्षेत्र संवाद में शामिल हैं. इस संवाद में चुने गए मूल्यों के आधार पर, कॉपी करने की प्रक्रिया बदल सकती है.

| **फ़ील्ड** | **वर्णन** | **डाउनस्ट्रीम प्रभाव** |
| --- | --- | --- |
| विषय | लक्ष्य अनुबंध के लिए विषय को दर्ज़ करें. जब संवाद पृष्ठ खुलता है, तो सिस्टम इस फ़ील्ड को स्रोत अनुबंध के नाम के साथ सेट कर देगा जिसमें **कॉपी** संलग्न होगी. | इस फील्ड का प्रवाह की दिशा में कोई प्रभाव नहीं होता है. |
| ग्राहक | ग्राहक की कंपनी या खाता रिकॉर्ड का संदर्भ. जब संवाद खुलता है, तो सिस्टम इस क्षेत्र को स्रोत अनुबंध पर खाता के लिए सेट कर देगा. | यह क्षेत्र अनुबंध पर प्राथमिक ग्राहक है. |
| अनुबंध इकाई | संगठन इकाई जो इस समझौते से जुड़ी परियोजना(ओं) की डिलीवरी के लिए जिम्मेदार है. जब संवाद पृष्ठ खुलता है, तो सिस्टम इसे स्रोत अनुबंध की अनुबंध इकाई के लिए सेट कर देगा. | करार इकाई कंपनी का डिवीजन है जो समझौता पूरा होने के बाद परियोजनाओं को निष्पादित करेगा. हर अनुबंध इकाई के पास एक मुद्रा है. इस मुद्रा का उपयोग परियोजना के दौरान हुए अनुमानित और वास्तविक लागत को दर्ज़ करने के लिए किया जाता है. |
| मुद्रा | इस सौदे में जिस मुद्रा का लेन-देन होता है. जब संवाद पृष्ठ खुलता है, तो सिस्टम क्षेत्र को स्रोत अनुबंध की मुद्रा के लिए सेट कर देगा. मुद्रा को बदला जा सकता है. यदि ऐसा है तो, **मूल्य निर्धारण को कॉपी करें** क्षेत्र हमेशा **नहीं** पर सेट रहता है क्योंकि स्रोत अनुबंधों पर मूल्य सूचियां अब प्रासंगिक नहीं हैं. | अनुबंध पर वित्तीय अनुमानों को बनाने के लिए, और जब सौदे को जीत लिया जाता है तो ग्राहक को इनवॉइस करने के लिए, मुद्रा का उपयोग मूल्य सूचियों को डिफ़ॉल्ट करने के लिए किया जाता है. |
| अनुरोधित वितरण तिथि | ग्राहक द्वारा अनुरोध की गई डिलीवरी तारीख. | जब आप किसी विशेष आवृत्ति के साथ इनवॉइस करने के लिए तारीख बनाते हैं तो इस तारीख का उपयोग अंतिम तारीख के रूप में किया जाता है. |
| मूल्य-निर्धारण की प्रतिलिपि बनाएँ | इंगित करता है कि अनुबंध पर निर्धारित मूल्य को स्रोत अनुबंध से कॉपी करना चाहिए या नहीं. | यदि क्षेत्र को **हां** पर सेट किया जाता है, तो परियोजना और उत्पाद मूल्य सूची प्राथमिकताओं को स्रोत से कॉपी करके लक्ष्य अनुबंध पर किया जाता है. यदि **नहीं** को चुना जाता है, तो खाता या परियोजना मापदंड के नवीनतम मूल्य सूचियों के आधार पर मूल्य सूचियां डिफ़ॉल्ट होती हैं. |

जब आप संवाद पृष्ठ पर **ओके** को चुनते हैं, तो सिस्टम चयनित मापदंडों के आधार पर अनुबंध की कॉपी बनाता है. नया अनुबंध खुल जाएगा.

निम्न जानकारी **स्रोत** से **लक्ष्य अनुबंध** में कॉपी नहीं की गई है:

  - इनवॉइस शेड्यूल
  - अनुबंध और अनुबंध पंक्ति ग्राहक
  - परियोजना-आधारित अनुबंध पंक्तियों पर परियोजना का सन्दर्भ
  - ग्राहक के बजट की जानकारी

क्योंकि यह जानकारी प्रत्येक अनुबंध के लिए विशेष है, ये क्षेत्र और रिकॉर्ड्स कॉपी नहीं किए गए हैं. परियोजना और उत्पादों के लिए अनुबंध पंक्तियां, अनुबंध पंक्ति विवरणों पर अनुमान, और अनुबंध स्तर पर इससे अधिक मूल्यों को कॉपी नहीं किया गया है. मूल्य और लागत दर डिफ़ॉल्ट रूप से **मापदंड कॉपी करें** संवाद पृष्ठ पर **मूल्य निर्धारण कॉपी करें** क्षेत्र के चयन पर निर्भर करते हैं.