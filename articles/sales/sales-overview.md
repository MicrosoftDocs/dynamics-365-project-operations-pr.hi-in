---
title: विक्रय प्रक्रिया अवलोकन
description: यह विषय बुनियादी बिक्री प्रक्रियाओं के बारे में जानकारी प्रदान करता है।
author: rumant
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 09/23/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app: ''
ms.openlocfilehash: e66d96a940f3b22d5d1f3372d2b6767a4482d925
ms.sourcegitcommit: 7750485f8685a2ca5e1b3c165ead24a3b583c447
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/25/2020
ms.locfileid: "3891442"
---
# <a name="sales-processes-overview"></a>विक्रय प्रक्रिया अवलोकन

प्रोजेक्ट-आधारित संगठन में उपयोग की जाने वाली विक्रय प्रक्रियाएं बिक्री-आधारित प्रक्रियाओं से भिन्न होती हैं जिनका उपयोग उत्पाद-आधारित संगठन में किया जाता है। ऐसा इसलिए है क्योंकि परियोजना-आधारित संगठनों के लिए बिक्री चक्र लंबे हैं और प्रत्येक डील के लिए कोटेशन का विश्लेषण और निर्माण करने के लिए अनुकूलित अनुमान तकनीकों की ज़रूरत होती है. Dynamics 365 Project Operations निम्नांकित कार्यक्षमता का इस्तेमाल करता है जिसका इस्तेमाल बिक्री प्रक्रिया में होता है:

- विक्रय प्रक्रिया की निगरानी करने के लिए एक लीड रिकॉर्ड का उपयोग किया जाता है.
- योग्य लीड्स को अवसरों के रूप में ट्रैक किया जाता है।
- अवसर के लिए सभी संबंधित पुरावशेष पहुंच योग्य हैं. इन आर्टिफ़ैक्ट में बिक्री टीम, हितधारक, संभाव्यता, रेटिंग, बिक्री चरण और व्यावसायिक प्रक्रियाएं शामिल हैं।
- एक अवसर के लिए कई कोट बनाए जाते हैं।
- कोटेशन को बिक्री ऑर्डर बनाने के लिए, **जीत के साथ बंद किया गया** का दर्जा दिया जाता है. Project Operations में, विक्रय आदेश को अनुकूलित किया जाता है और इसे प्रोजेक्ट अनुबंध कहा जाता है.

## <a name="estimate-a-sale"></a>बिक्री का अनुमान लगाना
बिक्री के मूल्य का अनुमान प्रोजेक्ट की जटिलता और उन प्रोजेक्ट के आधार पर लगाया जा सकता है जो पहले डिलीवर किए जा चुके हैं. उन प्रोजेक्ट के लिए जिनमें पिछले प्रोजेक्ट के विस्तार शामिल हैं या ऐसे प्रोजेक्ट जहां विक्रेता की विशेषज्ञता उच्च है और प्रसिद्ध कार्य टेम्पलेट्स का उपयोग किया जाता है, आप एक सरल आकलन प्रक्रिया का उपयोग कर सकते हैं। अधिक जटिल प्रोजेक्ट में आमतौर पर लंबी खरीद प्रक्रिया होती है। इसलिए, बिक्री अनुमान प्रक्रिया में अधिक चरण होते हैं। इस प्रक्रिया के आरंभ में, काम के प्रत्येक अलग हिस्से के लिए एक उच्च-स्तरीय अनुमान बनाना शुरू करने के लिए विक्रय टीम खाता प्रबंधकों और विषय वस्तु विशेषज्ञों (SME) के इनपुट का उपयोग करती है. काम के इन हिस्सों को कोट लाइनों द्वारा दर्शाया गया है. 

आप कोट का उच्च-स्तरीय अनुमान बना सकते हैं। आखिरकार, इस उच्च-स्तरीय अनुमान को एक अधिक विस्तृत अनुमान से बदल दिया जाएगा जो एक प्रोजेक्ट योजना पर आधारित है जिसे आप मानक प्रोजेक्ट टेम्पलेट्स का उपयोग करके बनाते हैं। ये टेम्प्लेट आपको एक शेड्यूल बनाने और कोट और उसके हिस्सों (कोट लाइनों) पर मौद्रिक मान निर्धारित करने में मदद करते हैं। 

आप एक प्रोजेक्ट के लिए कई कोट बना सकते हैं और उनका एकल अवसर रिकॉर्ड प्रकार के तहत समूह बना सकते हैं. आखिरकार, उन कोट में से एक को **जीते के रूप में बंद** चिह्नित किया और एक प्रोजेक्ट अनुबंध या काम का विवरण (SOW) बनाया जाता है. एक प्रोजेक्ट अनुबंध प्रत्येक हिस्से (अनुबंध लाइन) के लिए अनुबंधित मूल्य रखता है जिसे ग्राहक द्वारा डिलीवरी के लिए स्वीकार किया जाता है। एक SOW आमतौर पर Microsoft Word दस्तावेज़ के रूप में बनाया जाता है। प्रोजेक्ट की डिलीवरी के दौरान ग्राहक को भेजे गए सभी इनवॉइस, प्रोजेक्ट अनुबंध या SOW का संदर्भ देते हैं।

आप एक अवसर रिकॉर्ड के तहत वैकल्पिक कोट भी बना सकते हैं या सिस्टम इस तरह से सेट कर सकते हैं ताकि एक कोट पाने पर एक प्रोजेक्ट अनुबंध बनाया जाए. इस स्थिति में, आप एक Word दस्तावेज़ संलग्न कर सकते हैं जो प्रोजेक्ट अनुबंध रिकॉर्ड में SOW को दर्शाता है।

## <a name="configure-the-sales-process"></a>बिक्री प्रक्रिया को कॉन्फ़िगर करें
आप अपनी बिक्री प्रक्रिया को कॉन्फ़िगर करने के लिए व्यवसाय प्रक्रिया प्रवाह (BPF) का उपयोग कर सकते हैं. ये प्रवाह बिक्री प्रक्रिया के चरणों के माध्यम से सौदों को आगे बढ़ाने के लिए एक निर्देशित दृश्य इंटरफेस प्रदान करते हैं.

उदाहरण के लिए, आपकी कंपनी की बिक्री प्रक्रिया में निम्नलिखित छह चरण हो सकते हैं:

1. योग्य होना
2. अनुमान
3. आंतरिक समीक्षा
4. अनुबंध
5. डिलीवर करें
6. बंद करें
 
आपका संगठन एक ही डील को विकसित होने पर दर्शाने के लिए विभिन्न इकाइयों का उपयोग कर सकता है। बिक्री प्रक्रिया के आरंभ में, एक डील अवसर इकाई के द्वारा दर्शाया जाता है। जैसे-जैसे समय बीतता है और अधिक विवरण सामने आते हैं, आप एक या अधिक कोट बनाने के लिए उच्च-स्तरीय अनुमानों का उपयोग कर सकते हैं। यदि इन कोट में से एक की आंतरिक और ग्राहक हितधारकों द्वारा समीक्षा की जाती है, तो कोट इकाई डील को दर्शाती है। ग्राहक द्वारा कोट को स्वीकार करने के बाद, एक प्रोजेक्ट अनुबंध या SOW सौदे को दर्शाता है। इस व्यवहार का समर्थन करने के लिए, BPF को इस तरह से संरचित किया जाता है ताकि प्रक्रिया में प्रत्येक चरण एक अलग डेटाबेस तालिका से जुड़ा हो।

बिक्री प्रक्रिया में **योग्य** चरण को एक अवसर इकाई द्वारा समर्थित किया जा सकता है। **अनुमान** और **आंतरिक समीक्षा** चरणों को एक कोट इकाई द्वारा समर्थित किया जा सकता है। **कॉन्ट्रैक्ट**, **डिलीवरी** और **क्लोज़** चरणों को प्रोजेक्ट अनुबंध इकाई द्वारा समर्थित किया जा सकता है।

जब आप चरणों के बीच से डील को आगे बढ़ाते हैं, तो आपको प्रक्रिया के माध्यम से मदद करने और मार्गदर्शन करने के लिए उपयुक्त इकाई रिकॉर्ड बनाने के लिए कहा जाता है। चरण सशर्त हो सकते हैं। उदाहरण के लिए, यदि आपको किसी कोट की उस समय आंतरिक समीक्षा की आवश्यकता होती है जब कोट कस्टम मूल्य सूची का उपयोग करती है, तो आप उस स्थिति को व्यावसायिक प्रक्रिया के उपयुक्त चरण में कॉन्फ़िगर कर सकते हैं। **आंतरिक समीक्षा** चरण को तब केवल उन कोट के लिए दिखाया जाता है जो एक कस्टम मूल्य सूची का उपयोग करते हैं। अन्य सभी डील और कोट के लिए, **अनुमान** चरण के बाद **अनुबंध** चरण आता है।

> [!NOTE]
> Project Operation में अवसर, क्वोटेशन, आदेश और इनवॉइस निकाय रिकॉर्ड के लिए विशेष पृष्ठ हैं. आपको इन रिकॉर्डों को इन निकायों के लिए परियोजना जानकारी पृष्ठों का उपयोग करके बनाना चाहिए. नहीं तो, आप **परियोजना जानकारी** पृष्ठ से रिकॉर्ड को खोलने में सक्षम नहीं होंगे. यदि आप **परियोजना जानकारी** पृष्ठ से एक रिकॉर्ड खोलना चाहते हैं, तो आपको रिकॉर्ड को मिटाना होगा और **परियोजना जानकारी** पृष्ठ का उपयोग करके इसे फिर से बनाना होगा जहां इनमें से प्रत्येक निकाय प्रकार के लिए व्यावसायिक तर्क यह सुनिश्चित करता है कि रिकॉर्ड का **प्रकार** क्षेत्र सही ढंग से सेट किया गया है, और सभी अनिवार्य अवधारणाओं को ठीक से शुरू किया गया है.


## <a name="track-revisions-to-quotes-and-project-plans-in-the-sales-cycle"></a>विक्रय चक्र में कोट और प्रोजेक्ट की योजना के लिए संशोधन ट्रैक करें
Project Operations में, आप उन संशोधनों को ट्रैक नहीं कर सकते हैं जो एक कोट के लिए बनाए गए हैं. इसके बजाय, आपको मौजूदा कोट **गंवाए के रूप में बंद** के रूप में चिह्नित करना होगा और फिर एक नया कोट बनाना होगा। आप एक क्वोट को कॉपी कर सकते हैं या एक परियोजना-आधारित क्वोट क्लोन कर सकते हैं.

## <a name="track-comments-and-approvals-of-quotes-and-project-contracts"></a>क्वोट और परियोजना अनुबंधों की टिप्पणियों और अनुमोदनों को ट्रैक करें
आप रिकॉर्ड वॉल और पोस्ट का उपयोग करके कोट और प्रोजेक्ट अनुबंधों की समीक्षा और अनुमोदन का प्रबंधन कर सकते हैं। आपका संगठन कार्य आइटम असाइन करने, पुनर्निर्देशित करने, एस्कैलेट करने और सूचनाएं प्रबंधित करने और अनुमोदन करने के लिए कस्टम वर्कफ़्लो और प्लग-इन बना सकता है.
