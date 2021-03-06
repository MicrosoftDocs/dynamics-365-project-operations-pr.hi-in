---
title: परियोजना कोटेशन (Sales) पर सारांश जानकारी
description: यह विषय परियोजना कोटेशनों पर लागू होने वाली जानकारी और सेटिंग्स के बारे में जानकारी प्रदान करता है. (Sales)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: d050258ae457bb4392d5fa761442cfc7a444feb0
ms.sourcegitcommit: f6509f7d50de4d4ebb92c1bf2cfcdf09f17458eb
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/06/2020
ms.locfileid: "3966793"
---
# <a name="summary-information-on-a-project-quote-sales"></a>परियोजना कोटेशन (Sales) पर सारांश जानकारी

_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_

यह लेख उस जानकारी को बताता है जो किसी परियोजना कोटेशन पर लागू होती है. इसमें वो सेटिंग्स शामिल हैं जो सभी कोटेशन लाइनों को प्रभावित करती हैं, और परियोजना कोटेशन के KPIs को चलाने के लिए सभी लाइन आइटमों में संक्षेप में उद्धृत कोटेशन के बारे में जानकारी शामिल हैं.

निम्नलिखित तालिका में एक परियोजना कोटेशन पर सारांश जानकारी फ़ील्ड सूचीबद्ध की गई है जो Dynamics 365 Project Operations के लिए अद्वितीय हैं या जिसमें Dynamics 365 Sales कोटेशन से व्यवहार में कुछ महत्वपूर्ण बदलाव हैं.

| **फ़ील्ड** | **स्थान** | **प्रासंगिकता, उद्देश्य, और मार्गदर्शन** | **डाउनस्ट्रीम प्रभाव** |
| --- | --- | --- | --- |
| प्रकार | सारांश टैब (छिपा हुआ) | यह विकल्प सेट फ़ील्ड निम्नलिखित विकल्पों को छांटता है:</br>- कार्य-आधारित (केवल तभी उपलब्ध है जब परियोजना संचालन इंस्टॉल की जाती है)</br>- आइटम-आधारित (केवल तभी उपलब्ध है जब Project Operations और बिक्री इंस्टॉल की जाती है)</br>- सेवा रखरखाव-आधारित (तब उपलब्ध है जब Dynamics 365 Field Service इंस्टॉल की जाती है) | जब आप Project Operations एप्लिकेशन का उपयोग करते हैं, तो इस फ़ील्ड का मूल्य स्वचालित रूप से **कार्य-आधारित** पर सेट हो जाता है. यह कोटेशन को परियोजना आधारित कोटेशन के रूप में वर्गीकृत करता है. सभी परियोजना-विशिष्ट विस्तार और कार्यक्षमता को सक्षम करने के लिए एक कोटेशन परियोजना-आधारित होना चाहिए. |
| संभाव्य ग्राहक | सारांश टैब | ग्राहक की कंपनी या खाता रिकॉर्ड का संदर्भ. जब किसी अवसर से कोटेशन बनाया जाता है, तो इस फ़ील्ड को अवसर पर संबंधित फ़ील्ड से कॉपी किया जाता है. | परियोजना कोटेशन पर मुद्रा ग्राहक की मुद्रा के आधार पर डिफ़ॉल्ट है. हालांकि, कोटेशन को सहेजने से पहले इसे बदला जा सकता है. |
| खाता प्रबंधक | सारांश टैब | इस डील के लिए खाता प्रबंधक का नाम. जब किसी अवसर से कोटेशन बनाया जाता है, तो इस फ़ील्ड को अवसर पर संबंधित फ़ील्ड से कॉपी किया जाता है. | खाता प्रबंधक इस परियोजना के पूरा होने के माध्यम से ग्राहक के साथ संबंधों को प्रबंधित करने के लिए ज़िम्मेदार है. खाता प्रबंधक से सहबध्द बुक करने योग्य संसाधन रिकॉर्ड के आधार पर, अनुबंध इकाई परियोजना कोटेशन पर चूक करती है. |
| अनुबंध इकाई | सारांश टैब | संगठन इकाई जो इस कोटेशन से जुड़ी परियोजना या परियोजनाओं की डिलीवरी के लिए ज़िम्मेदार है. जब किसी अवसर से कोटेशन बनाया जाता है, तो इस फ़ील्ड को अवसर पर संबंधित फ़ील्ड से कॉपी किया जाता है. | करार इकाई कंपनी का डिवीजन है जो समझौता पूरा होने के बाद परियोजनाओं को निष्पादित करेगा. प्रत्येक अनुबंध इकाई में एक मुद्रा होती है, और इस मुद्रा का उपयोग परियोजना के निष्पादन के दौरान किए गए अनुमानित और वास्तविक लागतों की रिपोर्ट करने के लिए किया जाता है. |
| उत्पाद मूल्य सूची | सारांश टैब | यह मूल्य सूची है जिसका उपयोग उत्पाद-आधारित कोटेशन लाइनों पर कीमतों को डिफ़ॉल्ट करने के लिए किया जाता है. इस फ़ील्ड के लिए विकल्पों की सूची मूल्य सूचियों की एक सूची प्रदर्शित करती है जहां मूल्य सूची मुद्रा कोटेशन पर मुद्रा से मेल खाती है. जब किसी अवसर से कोटेशन बनाया जाता है, तो इस फ़ील्ड को अवसर पर संबंधित फ़ील्ड से कॉपी किया जाता है. अवसर पर यह फ़ील्ड खाता रिकॉर्ड से चूक जाता है लेकिन बदला जा सकता है. | जब एक कोटेशन जीत जाता है, तो बनाए गए फील्ड मान को परियोजना अनुबंध में कॉपी किया जाता है. |
| मुद्रा | सारांश टैब | यह उस मुद्रा को इंगित करता है जिसका उपयोग इस डील के मूल्य को रिपोर्ट करने के लिए किया जाएगा. यह वह मुद्रा भी है, जिसमें समझौता जीतने पर ग्राहक को इनवॉइस दिया जाएगा. जब किसी अवसर से कोटेशन बनाया जाता है, तो इस फ़ील्ड को अवसर पर संबंधित फ़ील्ड से कॉपी किया जाता है. अवसर पर यह फ़ील्ड खाता रिकॉर्ड से चूक करता है लेकिन उपयोगकर्ता द्वारा बदला जा सकता है. | कोटेशन सहेजे जाने के बाद, यह फ़ील्ड अब संपादन योग्य नहीं है. इसका उपयोग कोटेशन पर उत्पाद और परियोजना मूल्य सूचियों को डिफ़ॉल्ट करने के लिए किया जाता है. कोटेशन पर मुद्रा का उपयोग मूल्य सूची पर मुद्रा से मिलान करने के लिए किया जाता है. |
| सीमा-में रखें सीमा | सारांश टैब | यह अंतिम मूल्य पर मोल भाव की ऊपरी सीमा को इंगित करता है जिसपर ग्राहक इस समझौते के लिए सहमत हो रहे हैं. | इस ऊपरी सीमा का मूल्यांकन निष्पादन के दौरान किया जाता है और इस समझौते से जुड़ी सभी लाइन वस्तुओं और परियोजनाओं में लागू होता है. |
| अनुरोधित वितरण तिथि | सारांश टैब | जब किसी अवसर से कोटेशन बनाया जाता है, तो इस फ़ील्ड को अवसर पर संबंधित फ़ील्ड से कॉपी किया जाता है. | इस तिथि का उपयोग इनवॉइस शेड्यूल जनरेट करने के लिए अंतिम तिथि के रूप में किया जाता है. |

नीचे एक परियोजना कोटेशन पर उपलब्ध टैब और KPIs दिए गए हैं जो Project Operations के लिए अद्वितीय हैं या जिनमें Sales कोटेशन से व्यवहार में कुछ महत्वपूर्ण बदलाव हैं:

| **फ़ील्ड** | **स्थान** | **प्रासंगिकता, उद्देश्य और मार्गदर्शन** |
| --- | --- | --- |
| लाभप्रदता का विश्लेषण | कोटेशन पर टैब करें | टैब निम्नलिखित मेट्रिक्स दिखाता है:</br>- कुल चार्ज करने योग्य लागत</br></br>- कुल चार्ज नहीं करने योग्य लागत</br>- कुल राजस्व</br>- कुल राजस्व (आधार)</br>- कुल मुनाफ़ा</br>- कुल समायोजित मुनाफ़ा|
| ग्राहक अपेक्षाओं से तुलना | कोटेशन पर टैब करें | यह टैब निम्नलिखित मेट्रिक्स दिखाता है:</br>- अनुमानित समापन</br>- अनुरोध किया गया समापन</br>- ग्राहक बजट</br>- कोटेशन मान |
| कोटेशन विश्लेषण | कोटेशन पर टैब करें | यह टैब एक परियोजना कोटेशन के लिए निम्नलिखित शीर्ष KPIs का सारांश देता है</br>- बजट और शेड्यूल के लिए ग्राहकों की अपेक्षाओं से तुलना</br>- कुल मुनाफ़ा</br>- कुल समायोजित मुनाफ़ा |
