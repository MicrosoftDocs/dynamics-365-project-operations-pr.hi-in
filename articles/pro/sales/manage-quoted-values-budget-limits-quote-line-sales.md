---
title: परियोजना-आधारित कोट पंक्तियाँ ओवरव्यू - लाइट
description: यह विषय परियोजना कार्य के लिए परियोजना-आधारित कोटेशन लाइनों का उपयोग करने के बारे में जानकारी प्रदान करता है. (प्रो)
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: be1663c0d226fa19fe4b9df566e16d215f1fc08e
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181094"
---
# <a name="project-based-quote-lines-overview---lite"></a>परियोजना-आधारित कोट पंक्तियाँ ओवरव्यू - लाइट

_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_

परियोजना-आधारित कोटेशन लाइनों को एक सगाई पर परियोजना के काम का अनुमान लगाने में मदद करने के लिए डिज़ाइन कर रहे हैं. परियोजना-आधारित कोटेशन लाइन की संरचना को निम्नलिखित अवधारणाओं के साथ परियोजना अनुमानों के लिए बढ़ाया गया है:

- बिलिंग विधि
- प्रोजेक्ट और टास्क मैपिंग
- शामिल लेनदेन कक्षाएं
- सीमा-में रखें सीमा
- प्रभार्यता सेटअप
- कोटेशन लाइन विवरणों का उपयोग करके अनुमान लगाना
- कोट पंक्ति ग्राहक

निम्नलिखित तालिका परियोजना-आधारित कोटेशन लाइन के **सामान्य** टैब पर फ़ील्ड के बारे में जानकारी प्रदान करती है. ये फ़ील्ड परियोजना कार्य के लिए विस्तृत, बुनियादी अनुमान के आधार सेट करने में मदद करते हैं.

| **फ़ील्ड** | **वर्णन** | **डाउनस्ट्रीम प्रभाव** |
| --- | --- | --- |
| नाम | कोटेशन लाइन का नाम जिससे आपको अनुमानित किए जा रहे कोटेशन के अलग घटक की पहचान करने में मदद मिलनी चाहिए. | कोटेशन जीतने के बाद इस कोटेशन लाइन से बनाए गए परियोजना अनुबंध लाइन में कॉपी किया गया. |
| बिलिंग विधि | एक अवसर से बनाई गई कोटेशन पर, इस मूल्य को अवसर लाइन पर संबंधित फ़ील्ड से कॉपी किया जाता है. इस फ़ील्ड में Dynamics 365 Project Operations द्वारा समर्थित दो मुख्य अनुबंध मॉडल शामिल हैं:</br>- निश्चित मूल्य</br>- समय और सामग्री.| इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है. |
| Project | इस वैकल्पिक फ़ील्ड का उपयोग परियोजना की पहचान करने में करें जिसका उपयोग इस अनुबंध पर कार्य निष्पादन के लिए किया जाएगा. जब किसी परियोजना का कोटेशन लाइन में मानचित्रण किया जाता है, तो यह देय योग्य कार्यों को सेट करने और कोटेशन लाइन विवरणों के रूप में कोटेशन लाइन पर परियोजना-आधारित अनुमान को उत्पन्न करने में भी मदद करता है. जब किसी परियोजना का परियोजना-आधारित कोटेशन लाइन पर मानचित्रण नहीं किया जाता है, तो प्रत्येक कोटेशन लाइन विवरण बनाकर मैन्युअल रूप से अनुमान बनाया जाना चाहिए. | इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है.|
| शामिल कार्य | इंगित करता है कि क्या इस कोटेशन लाइन का उपयोग चयनित परियोजना के लिए सभी या कुछ परियोजना कार्यों के लिए किया जाता है. इस फ़ील्ड में निम्नलिखित संभावित मान हैं:</br>- सभी परियोजना कार्य</br>- केवल चयनित परियोजना कार्य</br>इस फ़ील्ड में एक खाली मान **सभी परियोजना कार्य** विकल्प के समान है. | जब **केवल चयनित परियोजना कार्य** को चुना जाता है तो परियोजना पृष्ठ पर, **कार्य बिलिंग सेटअप** टैब आपको इस कोटेशन लाइन से संबद्ध करने के लिए विशिष्ट कार्यों का चयन करने की अनुमति देता है. इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है. |
| समय शामिल करें | एक **हाँ**/**नहीं** निशान इंगित करता है कि क्या चयनित परियोजना पर समय की लेनदेन या श्रम लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा. एक **नहीं** मान इंगित करता है कि समय की लेनदेन या श्रम लागत इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा. एक **हाँ** मान इंगित करता है कि समय की लेनदेन या श्रम लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा. | इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है. |
| व्यय शामिल करें | एक **हाँ**/**नहीं** निशान इंगित करता है कि क्या चयनित परियोजना पर ख़र्च लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा. एक **नहीं** मान इंगित करता है कि ख़र्च लागत इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा. एक **हाँ** मान इंगित करता है कि ख़र्च लागत इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा. | इस फ़ील्ड मान को परियोजना अनुबंध लाइन पर कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है. |
| शुल्क शामिल करें | एक **हाँ**/**नहीं** निशान इंगित करता है कि क्या चयनित परियोजना पर शुल्क इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा. एक **नहीं** मान इंगित करता है कि शुल्क को इस कोटेशन लाइन पर अनुमान में शामिल नहीं किया जाएगा. एक **हाँ** मान इंगित करता है कि शुल्क को इस कोटेशन लाइन पर अनुमान में शामिल किया जाएगा. | इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है. |
| कोट की गई राशि | यह वह राशि है जिसे इस परियोजना-आधारित कोटेशन लाइन पर पूर्वानुमानित सभी कार्यों के लिए ग्राहक को प्रस्तुत किया जाएगा. एक अवसर से बनाई गई कोटेशन पर, इस मान को अवसर लाइन पर **ग्राहक बजट** फ़ील्ड से कॉपी किया जाता है. जब परियोजना-आधारित कोटेशन लाइन में लाइन विवरण होते हैं, तो इस फ़ील्ड को संपादन के लिए लॉक कर दिया जाता है और कोटेशन लाइन विवरणों पर दर्ज राशि से संक्षेपित किया जाता है. | इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है. |
| अनुमानित कर | यह उपयोगकर्ता के लिए कोटेशन लाइन पर अनुमानित कर राशि जोड़ने के लिए एक संपादन योग्य फ़ील्ड है. जब किसी परियोजना-आधारित कोटेशन लाइन में लाइन विवरण होते हैं, तो इस फ़ील्ड को संपादन के लिए लॉक कर दिया जाता है और कोटेशन लाइन विवरणों पर दर्ज कर राशि से संक्षेपित किया जाता है. | इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है. |
| कर के बाद कोट की गई राशि | कर के बाद यह फ़ील्ड कोटेशन लाइन राशि है और केवल पढ़ी जाती है. इस फ़ील्ड में राशि की गणना *क्वोट की गई राशि + कर* के रूप में की जाती है. | इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है. |
| सीमा-में रखें सीमा | यह फ़ील्ड संपादन योग्य है और केवल परियोजना-आधारित कोटेशन लाइनों पर उपलब्ध है जिसमें **समय और सामग्री** बिलिंग विधि है. | इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है. |
| ग्राहक बजट | यह फ़ील्ड संपादन योग्य है और यदि कोटेशन एक अवसर से बनाया गया था तो अवसर लाइन पर संबंधित फ़ील्ड से कॉपी किया जाता है. | इस फ़ील्ड मान को परियोजना अनुबंध लाइन में कॉपी किया जाता है जो कोटेशन जीतने पर इस कोटेशन लाइन से बनाया जाता है. |


## <a name="validation-rules-for-fields-on-the-general-tab-of-project-based-quote-lines"></a>परियोजना-आधारित कोटेशन लाइनों के सामान्य टैब पर फ़ील्डों के लिए सत्यापन नियम

**नियम 1**: यदि **शामिल किए गए कार्य** फ़ील्ड खाली है, या यदि यह **सभी परियोजना कार्य** के लिए सेट है, तो कोटेशन लाइन में एक परियोजना शामिल की जाती है.

**नियम 2**: यदि **शामिल किए गए कार्य** फ़ील्ड खाली है, या यदि यह **सभी परियोजना कार्य** के लिए सेट है, तो केवल कोटेशन की परियोजना-आधारित एक कोटेशन लाइन पर एक परियोजना और एक निश्चित लेनदेन वर्ग को शामिल किया जा सकता है.

**नियम 3**: यदि **शामिल किए गए कार्य** फ़ील्ड को **केवल चयनित परियोजना कार्य** के लिए सेट किया गया है, तो एक परियोजना और एक निश्चित लेनदेन वर्ग को कोटेशन की परियोजना-आधारित कई कोटेशन लाइनों पर शामिल किया जा सकता है.

**नियम 4**: यदि किसी अवसर में कई कोटेशन हैं, तो विभिन्न कोटेशनों से कोटेशन लाइनें हो सकती हैं जो सभी एक ही परियोजना का संदर्भ देती हैं और एक ही लेनदेन वर्ग को शामिल करती हैं.

**नियम 5**: यदि कोटेशन उसी समान अवसर से संबंधित नहीं हैं, तो वे समान परियोजना और लेनदेन वर्ग को शामिल नहीं कर सकते हैं.

<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td width="61" valign="top">
                <p>
                    <strong>अवसर</strong>
                </p>
            </td>
            <td width="41" valign="top">
                <p>
                    <strong>कोट</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>कोट पंक्ति</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>Project</strong>
                </p>
            </td>
            <td width="90" valign="top">
                <p>
                    <strong>शामिल कार्य</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>समय शामिल करें</strong>
                </p>
            </td>
            <td width="48" valign="top">
                <p>
                    <strong>व्यय शामिल करें</strong>
                </p>
            </td>
            <td width="42" valign="top">
                <p>
                    <strong>शामिल करें</strong>
                </p>
                <p>
                    <strong>शुल्क</strong>
                </p>
            </td>
            <td width="54" valign="top">
                <p>
                    <strong>मान्य/ मान्य नहीं</strong>
                </p>
            </td>
            <td width="308" valign="top">
                <p>
                    <strong>कारण</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
रिक्त </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="42" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
मान्य नहीं है </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
नियम #2 का उल्लंघन. P1 परियोजना पर समय, ख़र्च और शुल्क कोटेशन लाइनों QL1 और QL2 पर शामिल हैं.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
रिक्त </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="42" valign="top">
                <p>
हाँ </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
रिक्त </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="48" valign="top">
                <p>
No </p>
            </td>
            <td width="42" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
मान्य नहीं है </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
नियम #2 का उल्लंघन. P1 प्रोजेक्ट पर समय और शुल्क उद्धरण लाइनों QL1 और QL2 पर शामिल हैं।
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
रिक्त </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="42" valign="top">
                <p>
हाँ </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
रिक्त </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="48" valign="top">
                <p>
No </p>
            </td>
            <td width="42" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
मान्य </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                  <p>
P1 परियोजना पर समय और शुल्क QL1 पर शामिल हैं.
P1 परियोजना पर ख़र्च QL2 पर शामिल है.
प्रत्येक कोटेशन लाइन पर जो भी शामिल किया जा रहा है उनमें ओवरलैप नहीं है और मान्य है.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
रिक्त </p>
            </td>
            <td width="48" valign="top">
                <p>
No </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="42" valign="top">
                <p>
No </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
केवल चयनित कार्य </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="42" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
मान्य नहीं है </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
नियम #2 ऊपर का उल्लंघन </p>
                <p>
Q1 में परियोजना P1 पर कार्यों के सबसेट पर समय, ख़र्च और शुल्क शामिल हैं.
                </p>
                <p>
QL2 में संपूर्ण परियोजना P1 के लिए समय, ख़र्च और शुल्क शामिल हैं और Q1 पर जो भी शामिल है उसके साथ ओवरलैप करती है.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
रिक्त </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="42" valign="top">
                <p>
हाँ </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="108" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
केवल चयनित कार्य </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="42" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="54" rowspan="2" valign="top">
                <p>
मान्य </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
ऊपर कहे गए नियम #3 के अनुकूल, </p>
                <p>
Q1 में परियोजना P1 पर कार्यों के सबसेट पर समय, ख़र्च और शुल्क शामिल हैं.
                </p>
                <p>
QL2 में परियोजना P1 पर कार्यों के सबसेट के लिए समय, ख़र्च और शुल्क शामिल हैं.
                </p>
                <p>
एकमात्र अतिरिक्त सत्यापन QL1 पर कार्यों के सबसेट के आसपास है जो QL2 पर कार्यों के सबसेट से अलग है. यह सुनिश्चित करता है कि कोई ओवरलैप नहीं हैं. यह सिस्टम द्वारा किया जाता है जब कार्य संबध्द होते हैं.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL2 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
केवल चयनित कार्य </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="42" valign="top">
                <p>
हाँ </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
सभी परियोजना कार्य या रिक्त </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="42" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="54" valign="top">
                <p>
मान्य </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
नियम #5 के आधार पर, Q1 और Q2 एक ही अवसर पर दो उद्धरण हैं, इसलिए वे दोनों एक परियोजना के समान घटकों के लिए अनुमान लगा सकते हैं.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
तिमाही 2 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
सभी परियोजना कार्य या रिक्त </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="42" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="54" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
            </td>
            <td width="41" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="90" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="48" valign="top">
            </td>
            <td width="42" valign="top">
            </td>
            <td width="54" valign="top">
            </td>
            <td width="308" valign="top">
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O1 </p>
            </td>
            <td width="41" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
सभी परियोजना कार्य या रिक्त </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="42" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="54" valign="top">
                <p>
मान्य </p>
            </td>
            <td width="308" rowspan="2" valign="top">
                <p>
नियम #4 पर आधारित, Q1 और Q2 विभिन्न अवसरों पर दो कोटेशन हैं, इसलिए वे एक ही परियोजना के समान घटकों के लिए अनुमान नहीं लगा सकते हैं.
                </p>
            </td>
        </tr>
        <tr>
            <td width="61" valign="top">
                <p>
O2 </p>
            </td>
            <td width="41" valign="top">
                <p>
तिमाही 1 </p>
            </td>
            <td width="42" valign="top">
                <p>
QL1 </p>
            </td>
            <td width="42" valign="top">
                <p>
P1 </p>
            </td>
            <td width="90" valign="top">
                <p>
सभी परियोजना कार्य या रिक्त </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="48" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="42" valign="top">
                <p>
हाँ </p>
            </td>
            <td width="54" valign="top">
                <p>
मान्य नहीं है </p>
            </td>
        </tr>
    </tbody>
</table>

