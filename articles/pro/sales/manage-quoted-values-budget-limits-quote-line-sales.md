---
title: परियोजना-आधारित कोट पंक्तियाँ ओवरव्यू
description: यह विषय परियोजना कार्य के लिए परियोजना-आधारित कोटेशन लाइनों का उपयोग करने के बारे में जानकारी प्रदान करता है.
author: rumant
ms.date: 03/30/2021
ms.topic: overview
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 0a9661d9b91ffeece4c66b129846632b30ebebc8
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/14/2022
ms.locfileid: "8591084"
---
# <a name="project-based-quote-lines-overview"></a>परियोजना-आधारित कोट पंक्तियाँ ओवरव्यू 

लाइट तैनाती _**पर लागू होता है:** प्रोफार्मा इनवॉइस करने के लिए - डील, संसाधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations_

परियोजना-आधारित कोटेशन लाइनों को एक सगाई पर परियोजना के काम का अनुमान लगाने में मदद करने के लिए डिज़ाइन कर रहे हैं. परियोजना-आधारित कोटेशन लाइन की संरचना को निम्नलिखित अवधारणाओं के साथ परियोजना अनुमानों के लिए बढ़ाया गया है:

- बिलिंग विधि
- प्रोजेक्ट और टास्क मैपिंग
- शामिल लेनदेन कक्षाएं
- सीमा-में रखें सीमा
- प्रभार्यता सेटअप
- कोटेशन लाइन विवरणों का उपयोग करके अनुमान लगाना
- कोट पंक्ति ग्राहक

निम्नलिखित तालिका परियोजना-आधारित कोटेशन लाइन के **सामान्य** टैब पर फ़ील्ड के बारे में जानकारी प्रदान करती है. ये फ़ील्ड परियोजना कार्य के लिए विस्तृत, बुनियादी अनुमान के आधार सेट करने में मदद करते हैं.

| **फ़ील्ड** | **विवरण** | **डाउनस्ट्रीम प्रभाव** |
| --- | --- | --- |
| नाम | कोट लाइन का नाम जो आपको अनुमान लगाए गए कोट के अलग घटक की पहचान करने में मदद करता है. | कोटेशन जीतने के बाद इस कोटेशन लाइन से बनाए गए परियोजना अनुबंध लाइन में कॉपी किया गया. |
| बिलिंग विधि | एक अवसर से बनाई गई कोटेशन पर, इस मूल्य को अवसर लाइन पर संबंधित फ़ील्ड से कॉपी किया जाता है. इस फ़ील्ड में Dynamics 365 Project Operations समर्थित दो मुख्य अनुबंध मॉडल शामिल हैं:</br>- निश्चित मूल्य</br>- समय और सामग्री.| इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है. |
| Project | इस वैकल्पिक फ़ील्ड का उपयोग परियोजना की पहचान करने में करें जिसका उपयोग इस अनुबंध पर कार्य निष्पादन के लिए किया जाएगा. जब किसी परियोजना का कोटेशन लाइन में मानचित्रण किया जाता है, तो यह देय योग्य कार्यों को सेट करने और कोटेशन लाइन विवरणों के रूप में कोटेशन लाइन पर परियोजना-आधारित अनुमान को उत्पन्न करने में भी मदद करता है. जब किसी परियोजना का परियोजना-आधारित कोटेशन लाइन पर मानचित्रण नहीं किया जाता है, तो प्रत्येक कोटेशन लाइन विवरण बनाकर मैन्युअल रूप से अनुमान बनाया जाना चाहिए. | इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है.|
| शामिल कार्य | इंगित करता है कि क्या इस कोटेशन लाइन का उपयोग चयनित परियोजना के लिए सभी या कुछ परियोजना कार्यों के लिए किया जाता है. इस फ़ील्ड में निम्नलिखित संभावित मान हैं:</br>- सभी परियोजना कार्य</br>- केवल चयनित परियोजना कार्य</br>इस फ़ील्ड में एक खाली मान **सभी परियोजना कार्य** विकल्प के समान है. | जब **केवल चयनित परियोजना कार्य** को परियोजना पेज पर चुना जाता है, तो **कार्य बिलिंग सेटअप** टैब आपको इस कोट लाइन से संबद्ध करने के लिए विशिष्ट कार्यों का चयन करने की अनुमति देता है. इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है. |
| समय शामिल करें | यदि इस कोट लाइन पर अनुमान में लेन-देन या श्रम की लागत को चुनी गई परियोजना में शामिल किया जाएगा तो **हां**/**नहीं** मान इंगित होता है. एक **नहीं** मान इंगित करता है कि समय की लेनदेन या श्रम लागत इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा. एक **हाँ** मान इंगित करता है कि समय की लेनदेन या श्रम लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा. | इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है. |
| व्यय शामिल करें | यदि इस कोट लाइन पर अनुमान में लेन-देन या व्यय की लागत को चुनी गई परियोजना में शामिल किया जाएगा तो **हां**/**नहीं** मान इंगित होता है. एक **नहीं** मान इंगित करता है कि ख़र्च लागत इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा. एक **हाँ** मान इंगित करता है कि ख़र्च लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा. | इस मान को परियोजना कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है. |
| सामग्री शामिल करें | यदि इस कोट लाइन पर अनुमान में लेन-देन या सामग्री लागत को चुनी गई परियोजना में शामिल किया जाएगा तो **हां**/**नहीं** मान इंगित होता है. **नहीं** मान इंगित करता है कि सामग्री की लागत को इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा. एक **हां** मान इंगित करता है कि सामग्री की लागत को इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा. | इस मान को परियोजना कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है. |
| शुल्क शामिल करें | यदि इस कोट लाइन पर अनुमान में लेन-देन या शुल्क को चुनी गई परियोजना में शामिल किया जाएगा तो **हां**/**नहीं** मान इंगित होता है. एक **नहीं** मान इंगित करता है कि शुल्क को इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा. एक **हाँ** मान इंगित करता है कि शुल्क को इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा. | इस मान को परियोजना कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है. |
| कोट की गई राशि | यह वह राशि है जिसे इस परियोजना-आधारित कोट लाइन पर पूर्वानुमानित सभी कार्यों के लिए ग्राहक को कोट किया जाएगा. एक अवसर से बनाई गई कोटेशन पर, इस मान को अवसर लाइन पर **ग्राहक बजट** फ़ील्ड से कॉपी किया जाता है. जब परियोजना-आधारित कोटेशन लाइन में लाइन विवरण होते हैं, तो इस फ़ील्ड को संपादन के लिए लॉक कर दिया जाता है और कोटेशन लाइन विवरणों पर दर्ज राशि से संक्षेपित किया जाता है. | इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है. |
| अनुमानित कर | यह उपयोगकर्ता के लिए कोटेशन लाइन पर अनुमानित कर राशि जोड़ने के लिए एक संपादन योग्य फ़ील्ड है. जब किसी परियोजना-आधारित कोटेशन लाइन में लाइन विवरण होते हैं, तो इस फ़ील्ड को संपादन के लिए लॉक कर दिया जाता है और कोटेशन लाइन विवरणों पर दर्ज कर राशि से संक्षेपित किया जाता है. | इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है. |
| कर के बाद कोट की गई राशि | कर के बाद यह फ़ील्ड कोटेशन लाइन राशि है और केवल पढ़ी जाती है. इस फ़ील्ड में राशि की गणना *क्वोट की गई राशि + कर* के रूप में की जाती है. | इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है. |
| सीमा-में रखें सीमा | यह फ़ील्ड संपादन योग्य है और केवल परियोजना-आधारित कोटेशन लाइनों पर उपलब्ध है जिसमें **समय और सामग्री** बिलिंग विधि है. | इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है. |
| ग्राहक बजट | यह फ़ील्ड संपादन योग्य है और यदि कोटेशन एक अवसर से बनाया गया था तो अवसर लाइन पर संबंधित फ़ील्ड से कॉपी किया जाता है. | इस मान को परियोजना के कॉन्ट्रैक्ट लाइन में कॉपी किया जाता है जो कोट के जीते जाने पर इस कोट लाइन से बनाया जाता है. |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a>परियोजना-आधारित कोटेशन लाइनों के सामान्य टैब पर फ़ील्डों के लिए सत्यापन नियम

**नियम 1**: यदि **शामिल किए गए कार्य** फ़ील्ड खाली है, या यदि यह **सभी परियोजना कार्य** के लिए सेट है, तो कोटेशन लाइन में एक परियोजना शामिल की जाती है.

**नियम 2**: यदि **शामिल किए गए कार्य** फ़ील्ड खाली है, या यदि यह **सभी परियोजना कार्य** के लिए सेट है, तो केवल कोटेशन की परियोजना-आधारित एक कोटेशन लाइन पर एक परियोजना और एक निश्चित लेनदेन वर्ग को शामिल किया जा सकता है.

**नियम 3**: यदि **शामिल किए गए कार्य** फ़ील्ड को **केवल चयनित परियोजना कार्य** के लिए सेट किया गया है, तो एक परियोजना और एक निश्चित लेनदेन वर्ग को कोटेशन की परियोजना-आधारित कई कोटेशन लाइनों पर शामिल किया जा सकता है.

**नियम 4**: यदि किसी अवसर में कई कोटेशन हैं, तो विभिन्न कोटेशनों से कोटेशन लाइनें हो सकती हैं जो सभी एक ही परियोजना का संदर्भ देती हैं और एक ही लेनदेन वर्ग को शामिल करती हैं.

**नियम 5**: यदि कोटेशन उसी समान अवसर से संबंधित नहीं हैं, तो वे समान परियोजना और लेनदेन वर्ग को शामिल नहीं कर सकते हैं.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="59" valign="top">
                <p>
                    <strong>अवसर</strong>
                </p>
            </td>
            <td width="39" valign="top">
                <p>
                    <strong>कोट</strong>
                </p>
            </td>
            <td width="40" valign="top">
                <p>
                    <strong>कोट पंक्ति</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>Project</strong>
                </p>
            </td>
            <td width="77" valign="top">
                <p>
                    <strong>शामिल कार्य</strong>
                </p>
            </td>
            <td width="45" valign="top">
                <p>
                    <strong>समय शामिल करें</strong>
                </p>
            </td>
            <td width="46" valign="top">
                <p>
                    <strong>व्यय शामिल करें</strong>
                </p>
            </td>
            <td width="43" valign="top">
                <p>
                    <strong>सामग्री शामिल करें</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>शामिल करें</strong>
                </p>
                <p>
                    <strong>शुल्क</strong>
                </p>
            </td>
            <td width="49" valign="top">
                <p>
                    <strong>मान्य/ मान्य नहीं</strong>
                </p>
            </td>
            <td width="200" valign="top">
                <p>
                    <strong>कारण</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
रिक्त </p>
            </td>
            <td width="45" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="46" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="43" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="41" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
मान्य नहीं है </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
नियम #2 का उल्लंघन. P1 परियोजना पर समय, ख़र्च और शुल्क कोटेशन लाइनों QL1 और QL2 पर शामिल हैं </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
रिक्त </p>
            </td>
            <td width="45" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="46" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="43" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="41" valign="top">
                <p>
हाँ </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
रिक्त </p>
            </td>
            <td width="45" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="46" valign="top">
                <p>
No </p>
            </td>
            <td width="43" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="41" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
मान्य नहीं है </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
नियम #2 का उल्लंघन. P1 परियोजना पर समय, सामग्री और शुल्क कोटेशन लाइनों QL1 और QL2 पर शामिल हैं </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
रिक्त </p>
            </td>
            <td width="45" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="46" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="43" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="41" valign="top">
                <p>
हाँ </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
रिक्त </p>
            </td>
            <td width="45" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="46" valign="top">
                <p>
No </p>
            </td>
            <td width="43" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="41" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
मान्य </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
P1 परियोजना पर समय, सामग्री और शुल्क QL1 पर शामिल हैं <br>
P1 परियोजना पर ख़र्च QL2 पर शामिल है <br>
प्रत्येक कोट लाइन पर जो कुछ भी शामिल किया जा रहा है उनमें ओवरलैप नहीं है और इसलिए मान्य है.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
रिक्त </p>
            </td>
            <td width="45" valign="top">
                <p>
No </p>
            </td>
            <td width="46" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="43" valign="top">
                <p>
No </p>
            </td>
            <td width="41" valign="top">
                <p>
No </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
केवल चयनित कार्य </p>
            </td>
            <td width="45" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="46" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="43" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="41" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
मान्य नहीं है </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
नियम #2 का उल्लंघन </p>
                <p>
Q1 परियोजना P1 पर कार्यों के सबसेट पर समय, सामग्री, व्यय और शुल्क को शामिल करता है. </p>
                <p>
QL2 में पूरे परियोजना P1 के लिए समय, व्यय और शुल्क शामिल है और इसलिए Q1 में जो भी शामिल है, उसके साथ ओवरलैप होता है.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
रिक्त </p>
            </td>
            <td width="45" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="46" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="43" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="41" valign="top">
                <p>
हाँ </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
केवल चयनित कार्य </p>
            </td>
            <td width="45" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="46" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="43" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="41" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
मान्य </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
प्रति नियम #3, </p>
                <p>
Q1 परियोजना P1 पर कार्यों के सबसेट पर समय, सामग्री, व्यय और शुल्क को शामिल करता है.
                </p>
                <p>
QL2 में परियोजना P1 पर कार्यों के सबसेट के लिए समय, सामग्री, व्यय और शुल्क शामिल हैं.
                </p>
                <p>
एकमात्र अतिरिक्त सत्यापन QL1 पर कार्यों के सबसेट के आसपास है जो QL2 पर कार्यों के सबसेट से अलग है ताकि यह सुनिश्चित किया जा सके कि कोई ओवरलैप नहीं है. यह सिस्टम द्वारा किया जाता है जब कार्य संबध्द होते हैं.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
केवल चयनित कार्य </p>
            </td>
            <td width="45" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="46" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="43" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="41" valign="top">
                <p>
हाँ </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
सभी परियोजना कार्य या रिक्त </p>
            </td>
            <td width="45" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="46" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="43" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="41" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
मान्य </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
नियम #5 के अनुसार, Q1 और Q2 एक ही अवसर पर दो कोट हैं, इसलिए वे दोनों एक परियोजना के एक जैसे घटकों के लिए अनुमान लगा सकते हैं.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
तिमाही 2 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
सभी परियोजना कार्य या रिक्त </p>
            </td>
            <td width="45" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="46" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="43" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="41" valign="top">
                <p>
हाँ </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
            </td>
            <td width="39" valign="top">
            </td>
            <td width="40" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="77" valign="top">
            </td>
            <td width="45" valign="top">
            </td>
            <td width="46" valign="top">
            </td>
            <td width="43" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="49" valign="top">
            </td>
            <td width="200" valign="top">
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O1 </p>
            </td>
            <td width="39" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
सभी परियोजना कार्य या रिक्त </p>
            </td>
            <td width="45" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="46" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="43" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="41" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="49" rowspan="2" valign="top">
                <p>
मान्य नहीं है </p>
            </td>
            <td width="200" rowspan="2" valign="top">
                <p>
नियम #4 के अनुसार, Q1 और Q2 विभिन्न अवसरों पर दो कोटेशन हैं, इसलिए वे एक ही परियोजना के एक जैसे घटकों के लिए अनुमान नहीं लगा सकते हैं.
                </p>
            </td>
        </tr>
        <tr>
            <td width="59" valign="top">
                <p>
O2 </p>
            </td>
            <td width="39" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="40" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="41" valign="top">
                <p>
P1 </p>
            </td>
            <td width="77" valign="top">
                <p>
सभी परियोजना कार्य या रिक्त </p>
            </td>
            <td width="45" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="46" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="43" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="41" valign="top">
                <p>
हाँ </p>
            </td>
        </tr>
    </tbody>
</table>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
