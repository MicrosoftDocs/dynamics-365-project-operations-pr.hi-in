---
title: एक रिटेनर या एडवांस को इनवॉइस दें
description: यह विषय Project Operations में एक रिटेनर या एडवांस को इनवॉइस देने के तरीके के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/20/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 12bf3822227badcf8c83d84d6aef6c0fdc7a972a
ms.sourcegitcommit: 250270409412ba4cad95fbd4c345a80d3d2b3e53
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/21/2020
ms.locfileid: "4596194"
---
# <a name="invoice-a-retainer-or-an-advance"></a>एक रिटेनर या एडवांस को इनवॉइस करें

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

Dynamics 365 Project Operations रिटेनर-आधारित अनुबंधों और वन-टाइम एडवांस का समर्थन करता है. परियोजना अनुबंध पर, आप रिटेनरों या एकबारी एडवांस का शेड्यूल रिकॉर्ड कर सकते हैं. हालांकि, परियोजना अनुबंध स्तर पर रिकॉर्डिंग एक रिटेनर या एडवांस को उपयोग के लिए तुरंत उपलब्ध नहीं करता है. एक रिटेनर या एडवांस का एक इनवॉइस पर उपयोग करने के लिए सबसे पहले रिटेनर या एडवांस को इनवॉइस दिया जाना चाहिए जो वास्तव में ग्राहक को चार्ज किया जाता है.

रिटेनर या एडवांस को इनवॉइस देने के लिए निम्नलिखित चरणों को पूरा करें.

1. **बिक्री** > **बिलिंग** > **रिटेनर और एडवांस** चुनें. 
2. **एडवांस और रिटेनर** पृष्ठ पर, विशिष्ट रिटेनर या एडवांस को इनवॉइस देने हेतु चुनने के लिए फ़िल्टर का उपयोग करें और इसे **इनवॉइस के लिए तैयार** के रूप में चिह्नित करें.
3. **परियोजना अनुबंध** सूची या विवरण पृष्ठ से मैन्युअल रूप से भी इनवॉइस बनाएं. **इनवॉइस** पृष्ठ पर **एडवांस और रिटेनर** अनुभाग में ड्राफ्ट इनवॉइस पर रिटेनर या एडवांस को दिखाया गया है.
4. इनवॉइस की पुष्टि करें. इससे रिटेनर या एडवांस इस्तेमाल के लिए उपलब्ध हो जाएगा. आप **रिटेनर और एडवांस** सूची पृष्ठ पर इनवॉइस सत्यापित कर सकते हैं. इनवॉइस दिए जा चुके एडवांस या रिटेनर के लिए, उपलब्ध राशि ग्रिड में दिखाई जाती है.

## <a name="create-a-retainer-or-advance-from-the-invoice-grid"></a>इनवॉइस ग्रिड से रिटेनर या एडवांस बनाएं

आप इनवॉइस पर सीधे रिटेनर या एडवांस बना सकते हैं.

1. एक ड्राफ्ट इनवॉइस पर, **एडवांस और रिटेनर** सबग्रिड पर, एक नया रिटेनर या एडवांस बनाने के लिए **नया** का चयन करें. 
2. **त्वरित बनाएं** पृष्ठ पर, आवश्यक जानकारी जोड़ें, और फिर **सहेजें** चुनें. इनवॉइस से संबंधित परियोजना अनुबंध पर रिटेनर या एडवांस बनाया जाता है. रिटेनर या एडवांस को स्वचालित रूप से **इनवॉइस के लिए तैयार** के रूप में चिह्नित किया जाता है और फिर **इनवॉइस** पृष्ठ पर **एडवांस और रिटेनर** सबग्रिड में जोड़ा जाता है.

## <a name="reconcile-an-invoiced-retainer-or-advance"></a>इनवॉइस दिए गए रिटेनर या एडवांस का मिलान करें

रिटेनर या एडवांस को इनवॉइस दिए जाने के बाद, समय, ख़र्च, उपलब्धि या अन्य परियोजना-आधारित शुल्कों के साथ इनवॉइस पर उनका उपयोग या मिलान किया जा सकता है. ग्राहक अपनी इनवॉइस राशि को रिटेनर या इस इनवॉइस पर इस्तेमाल की गई एडवांस राशि से कम देखेंगे.

किसी परियोजना अनुबंध के लिए बनने वाले हर इनवॉइस पर, जिसमें इनवॉइस दिए गए रिटेनर या एडवांस हैं, Project Operation अपने आप रिटेनर या एडवांस को इनवॉइस पर लागू करता है.

इसे **लागू किए गए रिटेनर और एडवांस** ग्रिड में **इनवॉइस** पृष्ठ पर देखा जा सकता है. निम्नलिखित तालिका **परियोजना इनवॉइस** पृष्ठ के **लागू किए गए रिटेनर और अग्रिम** ग्रिड पर फ़ील्ड के बारे में जानकारी प्रदान करती है.

| क्षेत्र | स्थान | विवरण | डाउनस्ट्रीम प्रभाव |
| --- | --- | --- | --- |
| विवरण | **परियोजना इनवॉइस** पृष्ठ पर **लागू किए गए एडवांस और रिटेनर** ग्रिड |यह केवल-पढ़ने योग्य फ़ील्ड इस इनवॉइस पर उपयोग किए जाने वाले रिटेनर या एडवांस का विवरण प्रदान करता है. इस मान को इनवॉइस पर नहीं बदला जा सकता. इस मान को **परियोजना अनुबंध** पृष्ठ पर सबग्रिड पर अपडेट किया जा सकता है. | इस फ़ील्ड को मुद्रित इनवॉइस पर ग्राहक को प्रदर्शित किया जा सकता है ताकि यह इंगित किया जा सके कि इनवॉइस पर कौन सा रिटेनर या एडवांस लागू किया गया है. |
| वितरण दिनांक | **परियोजना इनवॉइस** पृष्ठ पर **लागू किए गए एडवांस और रिटेनर** ग्रिड  | यह केवल-पढ़ने योग्य फ़ील्ड इस इनवॉइस पर उपयोग किए जाने वाले रिटेनर या एडवांस की इनवॉइस तिथि प्रदान करता है. इस मान को इनवॉइस पर नहीं बदला जा सकता. इस मान को **परियोजना अनुबंध** पृष्ठ पर सबग्रिड पर अपडेट किया जा सकता है. | इस फ़ील्ड को मुद्रित इनवॉइस पर ग्राहक को प्रदर्शित किया जा सकता है ताकि उस तारीख को इंगित किया जा सके जब रिटेनर या एडवांस को पहले ग्राहक को इनवॉइस दिया गया था. |
| राशि | **परियोजना इनवॉइस** पृष्ठ पर **लागू किए गए एडवांस और रिटेनर** ग्रिड  | यह केवल-पढ़ने योग्य फ़ील्ड इस इनवॉइस पर उपयोग किए जाने वाले रिटेनर या एडवांस की राशि प्रदान करता है. इस मान को इनवॉइस पर नहीं बदला जा सकता. इस मान को **परियोजना अनुबंध** पृष्ठ पर सबग्रिड पर अपडेट किया जा सकता है. | इस फ़ील्ड को मुद्रित इनवॉइस पर ग्राहक को प्रदर्शित किया जा सकता है ताकि ग्राहक द्वारा भुगतान किए गए रिटेनर या एडवांस की मूल राशि को इंगित किया जा सके. |
| उपयोग की गई राशि | **परियोजना इनवॉइस** पृष्ठ पर **लागू किए गए एडवांस और रिटेनर** ग्रिड  | यह केवल-पढ़ने योग्य फ़ील्ड गणना की गई मान प्रदान करता है जो संक्षेपित करता है कि रिटेनर या एडवांस का कितना उपयोग किया गया है. | इस फ़ील्ड को मुद्रित इनवॉइस पर ग्राहक को प्रदर्शित किया जा सकता है ताकि इस रिटेनर या एडवांस से राशि का संकेत मिल सके जो पहले से उपयोग किया गया था. |
| विस्तारित राशि | **परियोजना इनवॉइस** पृष्ठ पर **लागू किए गए एडवांस और रिटेनर** ग्रिड  | यह संपादन योग्य फ़ील्ड इस परियोजना इनवॉइस पर उपयोग किए जा रहे रिटेनर या एडवांस की राशि प्रदान करता है. यह राशि एडवांस पर उपलब्ध राशि से अधिक नहीं हो सकती है. सिस्टम स्वचालित रूप से ग्रिड पर **राशि** और **उपयोग की गई राशि** फ़ील्डों के बीच के अंतर के रूप में इसकी गणना करता है. आप इस राशि को उपलब्ध से कम उपयोग करने के लिए घटा सकते हैं लेकिन आप उपलब्ध राशि से अधिक उपयोग करने के लिए राशि नहीं बढ़ा सकते हैं. | इस फ़ील्ड को मुद्रित इनवॉइस पर ग्राहक को प्रदर्शित किया जा सकता है ताकि इनवॉइस पर उपयोग की जा रही इस रिटेनर या एडवांस से राशि का पता चल सके. |
| शेष रिटेनर राशि. | **परियोजना इनवॉइस** पृष्ठ पर **लागू किए गए एडवांस और रिटेनर** ग्रिड  | यह केवल-पढ़ने योग्य फ़ील्ड इस बात का मान प्रदान करता है कि इनवॉइस की पुष्टि होने के बाद रिटेनर या एडवांस का कितना छोड़ा दिया जाएगा. | इस फ़ील्ड को मुद्रित इनवॉइस पर ग्राहक को प्रदर्शित किया जा सकता है ताकि इनवॉइस की पुष्टि और भुगतान के बाद इस रिटेनर या अग्रिम से छोड़ दी गई राशि को इंगित किया जा सके. |