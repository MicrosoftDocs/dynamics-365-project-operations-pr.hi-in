---
title: परियोजना अनुबंध सेटिंग - लाइट
description: यह विषय उन फ़ील्ड के बारे में जानकारी देता है जो अनुबंध पंक्ति और अनुबंध के बारे में जानकारी को प्रभावित करती हैं, जो सभी लाइन आइटम भर में सारांशित है.
author: rumant
manager: Annbe
ms.date: 10/20/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 28dfb256eb75ca9484161f053969c205fcd60965
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/31/2020
ms.locfileid: "4180914"
---
# <a name="project-contract-settings---lite"></a>परियोजना अनुबंध सेटिंग - लाइट

_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_

यह विषय उन फ़ील्ड्स के बारे में जानकारी देती है, जो पूरे परियोजना अनुबंध पर लागू होती हैं, इसमें सेटिंग शामिल हैं जो सभी अनुबंध पंक्तियों को प्रभावित करती हैं. प्रोजेक्ट अनुबंध के KPI को चलाने के लिए सभी पंक्ति वस्तुओं में संक्षेपित अनुबंध के बारे में जानकारी भी शामिल है.

निम्न तालिका परियोजना अनुबंध पर फ़ील्ड को सूचीबद्ध करती है जो Dynamics 365 Project Operations के लिए अद्वितीय हैं या Dynamics 365 Sales में बिक्री के आदेश से व्यवहार में कुछ महत्वपूर्ण परिवर्तन हैं.

| क्षेत्र | स्थान | विवरण | डाउनस्ट्रीम प्रभाव |
| --- | --- | --- | --- |
| प्रकार | **सारांश** टैब (छिपा हुआ) | यह निम्नांकित विकल्पों के साथ विकल्प सेट फ़ील्ड है:</br>- **कार्य-आधारित** (केवल तभी उपलब्ध है जब परियोजना संचालन इंस्टॉल की जाती है)</br>- **आइटम-आधारित** (केवल तभी उपलब्ध है जब Project Operations और बिक्री इंस्टॉल की जाती है)</br>- **सेवा रखरखाव-आधारित** (तब उपलब्ध है जब Dynamics 365 Field Service इंस्टॉल की जाती है) | Project Operations में, इस फील्ड का मान **कार्य-आधारित** में डिफॉल्ट करता है और अनुबंध को परियोजना-आधारित अनुबंध के रूप में वर्गीकृत करता है. सभी परियोजना-विशिष्ट विस्तारों और कार्यक्षमता को सक्षम करने के लिए अनुबंध परियोजना-आधारित होना चाहिए. |
| संभाव्य ग्राहक | **सारांश** टैब | ग्राहक कंपनी या खाता रिकॉर्ड का संदर्भ. जब अनुबंध कोटेशन से बनाया जाता है, तो इस फ़ील्ड को कोटेशन रिकॉर्ड पर संबंधित फ़ील्ड से कॉपी किया जाता है. | परियोजना अनुबंध पर मुद्रा, ग्राहक की मुद्रा के आधार पर डिफ़ॉल्ट होती है. अनुबंध को सहेजने से पहले इसे बदला जा सकता है. |
| खाता प्रबंधक | **सारांश** टैब | इस डील के लिए खाता प्रबंधक का नाम. जब अनुबंध कोटेशन से बनाया जाता है, तो इस फ़ील्ड को कोटेशन रिकॉर्ड पर संबंधित फ़ील्ड से कॉपी किया जाता है. | परियोजना के पूरा होने तक ग्राहक के साथ संबंध के प्रबंधन के लिए खाता प्रबंधक जिम्मेदार है. खाता प्रबंधक से सहबद्ध बुक करने योग्य संसाधन रिकॉर्ड के आधार पर, अनुबंध इकाई परियोजना अनुबंध पर डिफ़ॉल्ट करती है. |
| अनुबंध इकाई | **सारांश** टैब | इस अनुबंध से जुड़ी परियोजनाओं के वितरण के लिए उत्तरदायी संगठन इकाई. जब अनुबंध कोटेशन से बनाया जाता है, तो इस फ़ील्ड को कोटेशन रिकॉर्ड पर संबंधित फ़ील्ड से कॉपी किया जाता है. | अनुबंध इकाई कंपनी की भाग है, जो परियोजनाओं को निष्पादित करती है. हर अनुबंधकारी इकाई के पास एक मुद्रा है, और इस मुद्रा का उपयोग परियोजना के दौरान किए गए अनुमानित और वास्तविक लागत की रिपोर्ट करने के लिए किया जाता है. |
| उत्पाद मूल्य सूची | **सारांश** टैब | इस मूल्य सूची का उपयोग उत्पाद-आधारित अनुबंध पंक्तियों पर कीमतों को डिफ़ॉल्ट करने के लिए किया जाता है. इस फ़ील्ड के लिए ड्रॉप-डाउन विकल्पों की सूची मूल्य सूची की सूची दिखाती है, जहां मूल्य सूची मुद्रा अनुबंध पर मुद्रा से मेल खाती है. जब अनुबंध कोटेशन से बनाया जाता है, तो इस फ़ील्ड को कोटेशन रिकॉर्ड पर संबंधित फ़ील्ड से कॉपी किया जाता है. परियोजना अनुबंध पर, यह फ़ील्ड खाता रिकॉर्ड से डिफ़ॉल्ट है लेकिन इसे बदला जा सकता है. | इस फ़ील्ड के लिए कोई डाउनस्ट्रीम संबद्धता नहीं है. |
| मुद्रा | **सारांश** टैब | मुद्रा इस सौदे के मूल्य और उस मुद्रा की रिपोर्ट करती हैं, जिसमें ग्राहक का इनवॉइस किया जाएगा. जब अनुबंध कोटेशन से बनाया जाता है, तो इस फ़ील्ड को कोटेशन रिकॉर्ड पर संबंधित फ़ील्ड से कॉपी किया जाता है. परियोजना अनुबंध पर, यह फ़ील्ड खाता रिकॉर्ड से डिफ़ॉल्ट है, लेकिन इसे बदला जा सकता है. | अनुबंध सहेजे जाने के बाद, यह फ़ील्ड अब संपादन योग्य नहीं है. इस फ़ील्ड का इस्तेमाल अनुबंध पर उत्पाद और परियोजना मूल्य सूचियों को डिफ़ॉल्ट करने के लिए किया जाता है. अनुबंध पर मुद्रा का इस्तेमाल मूल्य सूची पर मुद्रा से मिलान के लिए किया जाता है. |
| सीमा-में रखें सीमा | **सारांश** टैब | यह फ़ील्ड अंतिम मान पर तय उच्चतम सीमा को इंगित करती है, जिस पर ग्राहक इस सौदे के लिए सहमत हो गया है. | उच्चतम सीमा का मूल्यांकन निष्पादन के दौरान किया जाता है और यह इस सौदे से जुड़ी सभी लाइन वस्तुओं और परियोजनाओं पर लागू होता है. |
| अनुरोधित वितरण तिथि | **सारांश** टैब | जब किसी प्रोजेक्ट कोटे से कोई कॉन्ट्रैक्ट बनाया जाता है, तो फील्ड को प्रोजेक्ट कोटे पर संबंधित फील्ड से कॉपी किया जाता है. | इस तिथि का इस्तेमाल इनवॉइस शेड्यूल बनाने के लिए अंतिम तिथि के रूप में किया जाता है. |

निम्नलिखित KPI प्रोजेक्ट अनुबंध के **अनुबंध प्रदर्शन** टैब पर उपलब्ध हैं.

| क्षेत्र | स्थान | विवरण |
| --- | --- | --- |
| अनुबंध मान | पूरा अनुबंध | परियोजना अनुबंध का कुल मूल्य. |
| बिल की गई राशि | पूरा अनुबंध | इस अनुबंध के सापेक्ष सभी इनवॉइस पर राशियों का योग. |
| व्यय की गई लागत | पूरा अनुबंध | अनुबंध पर मैप की जाने वाली सभी परियोजनाओं पर लॉग्ड ऑन सभी लागत वास्तविक आंकड़ों का योग. |
| सकल मार्जिन | पूरा अनुबंध | बिल की राशि - अब तक लगने वाली लागत / बिल की गई राशि |
| अपेक्षित मार्जिन | पूरा अनुबंध | (अनुबंध मूल्य - अनुमानित लागत) / अनुबंध मूल्य अनुमानित लागत = सभी परियोजनाओं पर अनुमानित लागत का योग अनुबंध पर मैप किया गया.|
| अनुबंध मान | परियोजना-आधारित पंक्तियाँ | अनुबंध पंक्ति का मूल्य. |
| बिल की गई राशि | परियोजना-आधारित पंक्तियाँ | नियत कीमत अनुबंध पंक्ति के लिए: इस अनुबंध पर बनाए गए विभिन्न इनवॉइस पर इस अनुबंध पंक्ति के सापेक्ष सभी वास्तविक आंकड़ो की बिल बिक्री राशियों का योग. समय और सामग्री अनुबंध पंक्ति के लिए: इस अनुबंध के लिए बनाए गए विभिन्न इनवॉइस पर इस अनुबंध पंक्ति के सापेक्ष सभी प्रभारित वास्तविक बिल बिक्री राशियों का योग. |
| व्यय की गई लागत | परियोजना-आधारित पंक्तियाँ | अनुबंध पंक्ति पर मैप की गई सभी परियोजनाओं पर सभी लाग्ड वास्तविक आंकड़ों की लागत का योग. |
| सकल मार्जिन | परियोजना-आधारित पंक्तियाँ | (बिल की राशि - अब तक लगने वाली लागत) / बिल की गई राशि |
| अपेक्षित मार्जिन | परियोजना-आधारित पंक्तियाँ | (आधार मुद्रा में अनुबंध लाइन राशि - आधार मुद्रा में अनुबंध लाइन के लिए अनुमानित लागत) / आधार मुद्रा में अनुबंध लाइन राशि |
| व्यय की गई लागत | परियोजना-आधारित पंक्ति का विवरण | समय: अनुबंध पंक्ति में मैप की गई परियोजना पर इस भूमिका के लिए लॉग्ड समय लागत वास्तविक आंकड़ों की राशि का योग. व्यय: इस श्रेणी के लिए अनुबंध पंक्ति पर मैप की गई सभी लॉग्ड व्यय लागत वास्तविक आंकड़ों की राशि का योग. |
| लॉग की गई मात्रा | परियोजना-आधारित पंक्ति का विवरण | समय: कुल समय पर मात्रा इस अनुबंध पंक्ति पर मैप की गई परियोजना की भूमिका के लिए लागत के वास्तविक आंकड़े होते हैं. व्यय: परियोजना पर व्यय लागत वास्तविक आंकड़ो पर इस व्यय श्रेणी के लिए सभी मात्रा इस अनुबंध पंक्ति में मैप की जाती हैं. |
| बिल की गई राशि | परियोजना-आधारित पंक्ति का विवरण | नियत कीमत अनुबंध पंक्ति के लिए, इस फील्ड को विवरण स्तर पर खाली छोड़ दिया जाता है और केवल अनुबंध पंक्ति स्तर पर दिखाया जाता है. समय और सामग्री अनुबंध पंक्ति के लिए, गणना विवरण स्तर पर पूरी की जाती है. विवरण इस अनुबंध पंक्ति के सापेक्ष सभी बिल की गयी राजस्व पंक्तियों पर राशि का योग दिखाते हैं जो आदेय हैं. |
| बिल की गई मात्रा | परियोजना-आधारित पंक्ति का विवरण | नियत कीमत अनुबंध पंक्ति के लिए, इस फील्ड को विवरण स्तर पर खाली छोड़ दिया जाता है और केवल अनुबंध पंक्ति स्तर पर दिखाया जाता है. समय और सामग्री अनुबंध पंक्ति के लिए, गणना समय और खर्च के लिए विवरण स्तर पर पूरी की जाती है. समय: इस अनुबंध पंक्ति के सापेक्ष इस भूमिका के लिए सभी बिल की गयी आय पंक्तियों पर घंटों का योग है जो कि आदेय है. व्यय: परियोजना पर व्यय लागत वास्तविक आंकड़ो पर इस व्यय श्रेणी के लिए सभी मात्रा इस अनुबंध पंक्ति में मैप की जाती हैं. |
| अनुबंध मान | उत्पाद-आधारित पंक्तियाँ | इस उत्पाद-आधारित अनुबंध पंक्ति का अनुबंध पंक्ति मान. |
| बिल की गई राशि | उत्पाद-आधारित पंक्तियाँ | इस अनुबंध के लिए बनाए गए विभिन्न इनवॉइस पर उत्पाद आधारित अनुबंध पंक्ति के सापेक्ष सभी इनवॉइस पंक्तियों पर राशियों का योग. |
| व्यय की गई लागत | उत्पाद-आधारित पंक्तियाँ | उत्पाद-आधारित अनुबंध पंक्ति के लिए लॉग की गयी सभी लागत वास्तविक आंकड़ों की राशि का योग. |
| सकल मार्जिन | परियोजना-आधारित पंक्तियाँ | बिल की राशि - अब तक लगने वाली लागत / बिल की गई राशि |
| अपेक्षित मार्जिन | उत्पाद-आधारित पंक्तियाँ | (अनुबंध पंक्ति मूल्य - अनुबंध पंक्ति के लिए अनुमानित लागत) / अनुबंध पंक्ति मान |