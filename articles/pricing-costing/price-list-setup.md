---
title: मूल्य सूची सेटअप करें
description: यह विषय लागत और बिक्री मूल्य सूची सेट करने के तरीके के बारे में जानकारी देता है.
author: rumant
manager: Annbe
ms.date: 10/20/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 000c22944b187b6250f2e982d73020028093fde6
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/31/2020
ms.locfileid: "4180194"
---
# <a name="set-up-price-lists"></a>मूल्य सूची सेटअप करें

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

Dynamics 365 Project Operations में मूल्य सूचियां दरों का कैटलॉग दिखाती हैं. दरें लागत, बिक्री और बिल दरें प्रकट करती हैं. मूल्य सूची लागत दरों या बिक्री और बिल दरों को प्रकट करती है, इसके आधार पर मूल्य सूची का संदर्भ **बिक्री** या **लागत** होता है.

निम्नलिखित विस्तार Project Operations के लिए विशिष्ट हैं और Dynamics 365 Sales से मूल्य सूची में लागू होते हैं.

- **संदर्भ**: इस फ़ील्ड में समर्थित मान **लागत** और **बिक्री** हैं. मान, **खरीद** समर्थित नहीं है. लागत मूल्य सूची बनाने के लिए **लागत** का संदर्भ सेट करें या बिक्री मूल्य सूची के लिए **बिक्री** का संदर्भ सेट करें. लागत मूल्य सूचियां अनुमान और वास्तविक रिकॉर्ड पर लागत प्रकार के लिए मूल्य स्पष्ट करती हैं. बिक्री मूल्य सूचियां, बिना बिल किए गए और बिल किए गए बिक्री प्रकारों के अनुमानित और वास्तविक रिकॉर्ड पर मूल्य को स्पष्ट करती हैं.
- **समय इकाई**: यह उस समय की डिफ़ॉल्ट इकाई है, जिसके लिए मूल्य इस मूल्य सूची के लिए संबंधित **भूमिका मूल्य** तालिका में सेट किया गया है.
- **मूल्य सूची निकाय**: यह छिपी हुई फ़ील्ड हुआ Project Operations द्वारा उन मूल्य सूचियों में अंतर करने के लिए है, वो कोटेशन या अनुबंध-विशिष्ट हैं जो मानक हैं और विश्व स्तर पर लागू हैं.

## <a name="price-list-header"></a>मूल्य सूची शीर्षलेख

निम्न तालिका में मूल्य सूची के **सामान्य** टैब पर फ़ील्ड शामिल हैं जो Project Operations के लिए अद्वितीय हैं या बिक्री में मूल्य सूची से व्यवहार में महत्वपूर्ण परिवर्तन हैं.

| क्षेत्र | स्थान | विवरण | डाउनस्ट्रीम प्रभाव |
| --- | --- | --- | --- |
| नाम | **सामान्य** टैब और **त्वरित बनाएँ** प्रपत्र | मूल्य सूची की पहचान. | मूल्य सूची को सभी सूची पृष्ठों और ड्रॉप-डाउन विकल्पों पर इस मूल्य के साथ दिखाया गया है.|
| संदर्भ | **सामान्य** टैब और **त्वरित बनाएँ** प्रपत्र | यह फ़ील्ड **लागत** या **बिक्री** पर सेट की जा सकती है. | **मूल्य** के लिए सेट की गई मूल्य सूची का इस्तेमाल लागत अनुमान और लागत वास्तविक आंकड़ों के मान देखने के लिए किया जाता है. **बिक्री** के लिए सेट की गई मूल्य सूची का इस्तेमाल बिक्री अनुमानों और बिक्री वास्तविक आकड़ों के मान देखने के लिए किया जाता है. केवल **बिक्री** के संदर्भ वाली मूल्य सूची को ग्राहकों, परियोजना कोटेशन और परियोजना अनुबंधों के लिए परियोजना मूल्य सूचियों से जोड़ा जा सकता है. |
| प्रारंभ तिथि | **सामान्य** टैब और **त्वरित बनाएँ** प्रपत्र | उस अवधि की शुरुआती तारीख जिसमें मूल्य सूची प्रभावी है. | **अंतिम तिथि** फ़ील्ड के साथ, इस फ़ील्ड का इस्तेमाल यह निर्धारित करने के लिए किया जाता है कि कौन सी मूल्य सूची निश्चित अनुमान या वास्तविक रेखा के लिए लागू है. |
| समाप्ति तिथि | **सामान्य** टैब और **त्वरित बनाएँ** प्रपत्र | उस अवधि की समाप्ति तारीख जिसमें मूल्य सूची प्रभावी है. | **प्रारंभ तिथि** फ़ील्ड के साथ, यह फ़ील्ड यह निर्धारित करने के लिए उपयोग की जाती है कि कौन सी मूल्य सूची किसी निश्चित अनुमान या वास्तविक क्षेत्र के लिए लागू है. |
| मुद्रा | **सामान्य** टैब और **त्वरित बनाएँ** प्रपत्र | इस फ़ील्ड का इस्तेमाल इस मूल्य सूची से संबंधित प्रत्येक भूमिका, श्रेणी या मूल्य सूची आइटम लाइन पर मुद्रा को डिफ़ॉल्ट करने के लिए किया जाता है. | **बिक्री** पर मूल्य सूची, भूमिकाएं, श्रेणियां, या मूल्य सूची आइटम लाइन इस मुद्रा के अलावा किसी भी मुद्रा में नहीं बनाई जा सकती हैं. **लागत** मूल्य सूचियों पर, आप किसी भी मुद्रा में भूमिका मूल्य सीमा बना सकते हैं. यहां स्पष्ट की गई मुद्रा डिफ़ॉल्ट के रूप में इस्तेमाल की जाती है. उपयोगकर्ता सेटअप जो संबंधित भूमिका मूल्य है, वह किसी भी मुद्रा में श्रम लागत दर सेटअप को सक्षम करने के लिए इस मूल्य को ओवरराइड कर सकता है. श्रेणी लागत दर और मूल्य सूची आइटम लागत केवल यहां स्पष्ट की गई मुद्रा में सेट की जा सकती हैं. |
| समय इकाई | **सामान्य** टैब और **त्वरित बनाएँ** प्रपत्र | इस फ़ील्ड का उपयोग इस मूल्य सूची से संबंधित प्रत्येक भूमिका क्षेत्र में समय इकाई को डिफ़ॉल्ट करने के लिए किया जाता है. | यह फ़ील्ड मान केवल संबंधित भूमिका मूल्य सेटअप में इस्तेमाल होता है. **लागत** और **बिक्री** मूल्य सूचियों पर, आप समय की किसी भी इकाई में भूमिका मूल्य क्षेत्र बना सकते हैं. यहां स्पष्ट की गई टाइम यूनिट को डिफ़ॉल्ट के रूप में इस्तेमाल किया जाता है. उपयोगकर्ता सेटअप संबंधी भूमिका मूल्य इस मूल्य को ओवरराइड कर सकते हैं ताकि किसी भी समय में श्रम लागत और बिल दर सेटअप को सक्रिय किया जा सके. |
| विवरण | **सामान्य** टैब और **त्वरित बनाएँ** प्रपत्र | यह पाठ फ़ील्ड आपको मूल्य सूची का बहु-पंक्ति विवरण देने की अनुमति देता है. | यह क्षेत्र विभिन्न निकायों में मूल्य सूची पर **संबंधित** विचार में दिखाए गए हैं, जिनके संबंधित मूल्य सूची है. |