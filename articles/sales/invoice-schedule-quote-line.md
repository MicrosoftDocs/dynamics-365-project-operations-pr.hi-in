---
title: परियोजना-आधारित कोटेशन लाइनों पर इंवॉयस शेड्यूल
description: यह विषय कोट लाइन के लिए इनवॉयस शेड्यूल और उपलब्धि के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 2b69742915fe79ee59e7fdcf317000cea79c5929
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/31/2020
ms.locfileid: "4180824"
---
# <a name="invoice-schedules-on-project-based-quote-lines"></a>परियोजना-आधारित कोटेशन लाइनों पर इंवॉयस शेड्यूल

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

एक परियोजना-आधारित कोट लाइन एक इनवॉयस शेड्यूल व्यक्त करने की क्षमता देती है. यह कोट के चरण के दौरान वैकल्पिक है क्योंकि आवेदन जब एक कोट लाइन से सहबद्ध रहता है तो एक परियोजना की इनवॉयसिंग का समर्थन नहीं करता है. कोट प्राप्त करने के बाद ही इनवॉयसिंग की अनुमति दी जाती है. कोट के चरण के दौरान इनवॉयस शेड्यूल बनाने का एकमात्र डाउनस्ट्रीम प्रभाव यह है कि इस इनवॉयस शेड्यूल को परियोजना-आधारित अनुबंध लाइन पर कॉपी की जाती है. यदि आप कोट के चरण के दौरान इनवॉयस शेड्यूल नहीं बनाते/बनाती हैं, तो आप परियोजना-आधारित अनुबंध लाइन पर ऐसा करने में सक्षम होंगे/होंगी.

कुल मिलाकर, इनवॉयस शेड्यूल का उद्देश्य परियोजना-आधारित अनुबंध लाइन के लिए ड्राफ्ट इनवॉयस के स्वचालित निर्माण की अनुमति देना है. 

## <a name="create-a-time-and-material-invoice-schedule-for-a-project-based-quote-line"></a>परियोजना-आधारित कोट लाइन के लिए एक समय और सामग्री इनवॉयस शेड्यूल बनाएं

जब परियोजना-आधारित कोट लाइन के लिए बिलिंग विधि समय और सामग्री होती है, तो सिस्टम तिथि-आधारित इनवॉयस शेड्यूल उत्पन्न करता है. तिथि-आधारित इनवॉयस शेड्यूल को स्वचालित रूप से उत्पन्न करने के लिए, निम्नलिखित चरणों को पूरा करें.

1. **सेटिंग** > **इंवॉयस बारंबारता** पर जाएं और इनवॉइस बारंबारता सेट करें.
2. **कोटेशन** पृष्ठ पर, परियोजना कोटेशन खोलें और **सारांश** टैब पर, एक अनुरोध की गई डिलीवरी तिथि निर्धारित करें.
3. एक तिथि-आधारित इनवॉयस शेड्यूल को बनाने की अपनी जरूरत के लिए समय और सामग्री कोट लाइन खोलें. 
4. **इंवॉयस शेड्यूल** टैब पर, **बिलिंग शुरू** और **इंवॉयस बारंबारता** फ़ील्ड में मानों का चयन करें. 
5. सब-ग्रिड पर, **इंवॉयस शेड्यूल उत्पन्न करें** चुनें.
6. आवेदन इंवॉयस शेड्यूल को **इंवॉयस चालू की तिथि**, **लेन-देन की निर्दिष्ट तिथि**, और **चालू की स्थिति** फील्ड्स के साथ उत्पन्न करता है, जो निम्नलिखित तरीके से सेट किया गया है:

    - **इंवॉयस चालू की तिथि** इंवॉयस बारंबारता के आधार पर तय की गई तारीख के लिए निर्धारित है.
    - **लेन-देन की निर्दिष्ट तिथि** **इंवॉयस चालू की तिथि** से पहले दिन के लिए निर्धारित है.
    - **चालू की स्थिति** स्वचालित रूप से **चालू नहीं** के लिए सेट हो जाता है. जब स्वचालित इंवॉयस निर्माण कार्य एक निश्चित इंवॉयस चालू की तिथि के लिए चलती है, तो यह इस फ़ील्ड को या तो **चालू सफल** या **चालू असफल** में अपडेट करेगा.

## <a name="create-a-fixed-price-invoice-schedule-for-a-project-based-quote-line"></a>परियोजना-आधारित कोट लाइन के लिए तय कीमत का इनवॉइस शेड्यूल बनाएं

जब परियोजना-आधारित कोटेशन लाइन में **तय** बिलिंग विधि होती है, तो सिस्टम उपलब्धि आधारित इंवॉयस शेड्यूल बनाता है. कैलेंडर अवधि के लिए समान रूप से वितरित किए जाने वाले उपलब्धि के एक निश्चित सेट के लिए इस शेड्यूल को स्वचालित रूप से उत्पन्न करने हेतु निम्नलिखित चरणों को पूरा करें.

1. **सेटिंग** > **इंवॉयस बारंबारता** पर जाएं और इनवॉइस बारंबारता सेट करें.
2. **कोटेशन** पृष्ठ पर, परियोजना कोटेशन खोलें और **सारांश** टैब पर, एक अनुरोध की गई डिलीवरी तिथि निर्धारित करें.
3. तय कीमत की कोट लाइन खोलें जिसके लिए आपको एक उपलब्धि शेड्यूल बनाने की आवश्यकता है. 
4. **इंवॉयस शेड्यूल** टैब पर, **बिलिंग शुरू** और **इंवॉयस बारंबारता** फ़ील्ड में मानों का चयन करें. 
5. सब-ग्रिड पर, **आवधिक उपलब्धि उत्पन्न करें** का चयन करें.
6. आवेदन एक उपलब्धि नाम, तिथि, और राशि के साथ इनवॉयस शेड्यूल उत्पन्न करता है.

    - माइलस्टोन नाम उस तिथि पर सेट किया गया है जो इनवॉइस आवृत्ति के आधार पर तय किया गया है.
    - माइलस्टोन की तिथि उस तिथि के लिए निर्धारित की गई है जो इनवॉयस आवृत्ति के आधार पर तय होती है.
    - माइलस्टोन राशि की गणना परियोजना-आधारित कोट लाइन पर कोट राशि को आवृत्ति और बिलिंग चालू और अनुरोध की गई डिलीवरी तिथियों द्वारा तय उपलब्धि की संख्या से विभाजित कर की जाती है.
    - यदि कोट लाइन में अनुमानित कर राशि भी है, तो आवधिक उपलब्धियों को उत्पन्न करते समय यह मूल्य प्रत्येक उपलब्धि के बीच समान रूप से विभाजित होता है.

### <a name="manually-create-milestones"></a>मैन्युअल रूप से माइलस्टोन बनाएँ

तय कीमत के उपलब्धि भी मैन्युअल रूप से उत्पन्न किए जा सकते हैं जब वे आवधिक रूप से विभाजित नहीं होते हैं. मैन्युअल रूप से एक उपलब्धि बनाने के लिए:

तय कीमत की कोट लाइन खोलें जहां आपको उपलब्धि बनाने की जरूरत है. सबग्रिड पर, **इनवॉयस शेड्यूल** टैब पर, **+ नया कोट पंक्ति माइलस्टोन बनाएँ** का चयन करें और निम्न तालिका के आधार पर आवश्यक जानकारी दर्ज करें.

| **फ़ील्ड** | **स्थान** | **वर्णन** | **डाउनस्ट्रीम प्रभाव** |
| --- | --- | --- | --- |
| माइलस्टोन नाम | त्वरित बनाएँ | माइलस्टोन का नाम. | यह परियोजना अनुबंध लाइन उपलब्धि और इनवॉयस के लिए प्रचारित किया जाता है |
| परियोजना कार्य | त्वरित बनाएँ | यदि उपलब्धि परियोजना कार्य से सहबद्ध है, तो आप कार्य स्थिति के आधार पर अनुकूलित लॉजिक सेट को उपलब्धि स्थिति से जोड़ने के लिए इस संदर्भ का उपयोग कर सकते/सकती हैं. | आवेदन, एक कार्य के लिए इस संदर्भ का कोई डाउनस्ट्रीम प्रभाव नहीं है. |
| माइलस्टोन दिनांक | त्वरित बनाएँ | उस तिथि को निर्धारित करें जिस पर स्वचालित इनवॉयस निर्माण प्रक्रिया को इनवॉयसिंग के लिए इस उपलब्धि के स्थिति की तलाश करनी चाहिए. | यह परियोजना अनुबंध लाइन उपलब्धि और इनवॉयस के लिए प्रचारित किया जाता है. |
| इनवॉइस स्थिति | त्वरित बनाएँ | जब एक उपलब्धि बनायी जाती है, तो इस स्थिति को हमेशा **इंवॉयसिंग के लिए तैयार नहीं** पर सेट किया जाता है. | यह परियोजना अनुबंध लाइन उपलब्धि और इनवॉयस के लिए प्रचारित किया जाता है. |
| पंक्ति राशि | त्वरित बनाएँ | ग्राहक को इनवॉयस किए जाने वाली उपलब्धि की राशि या मूल्य. | यह परियोजना अनुबंध लाइन उपलब्धि और इनवॉयस के लिए प्रचारित किया जाता है. |
| कर | त्वरित बनाएँ | कर राशि जो उपलब्धि पर लागू होगी. | यह परियोजना अनुबंध लाइन उपलब्धि और इनवॉयस के लिए प्रचारित किया जाता है. |