---
title: एक कोट पंक्ति पर अनुमान बनाएँ
description: यह विषय किसी परियोजना के लिए क्वोटेशन लाइन पर अनुमान बनाने के तरीके के बारे में जानकारी देता है.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: e841ab7c37e0b348a4d1570123a5aea00ede0047
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898489"
---
# <a name="create-estimates-on-a-quote-line"></a>एक कोट पंक्ति पर अनुमान बनाएँ

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

परियोजना-आधारित क्वोट पर, आप परियोजना को डिलीवर करने के लिए आवश्यक कार्य का अनुमान लगाने हेतु लाइन विवरण क्वोट करें निकाय का उपयोग कर सकते हैं. फिर आप उस अनुमान को ग्राहक के साथ साझा कर सकते हैं।

प्रोजेक्ट-आधारित कोट लाइनों का कोई कोट लाइन विवरण नहीं होना चाहिए। वैकल्पिक रूप से, उनके पास कई कोट लाइन विवरण हो सकते हैं। समय, खर्च या शुल्क का अनुमान लगाने के लिए कोट लाइन विवरण का उपयोग किया जाता है। Dynamics 365 Project Operations कोट लाइन विवरण पर सामग्री अनुमानों की अनुमति नहीं देता है. इन्हें लेन-देन वर्ग कहा जाता है। अनुमानित कर राशि लेन-देन वर्ग में भी दर्ज की जा सकती है।

लेन-देन वर्गों के अलावा, कोट लाइन विवरण में एक लेन-देन प्रकार होता है। क्वोटेशन लाइन विवरण के लिए दो लेनदेन प्रकार हैं, **लागत** और **परियोजना अनुबंध**.

## <a name="estimate-by-using-a-contract"></a>एक अनुबंध का उपयोग करके अनुमान करें

यदि आपने प्रोजेक्ट-आधारित अनुबंध बनाते समय Project Operations कोट का उपयोग किया है, तो कोट पर प्रत्येक कोट लाइन के लिए आपने जो अनुमान लगाया है, वह प्रोजेक्ट अनुबंध में कॉपी किया गया है. एक प्रोजेक्ट अनुबंध की संरचना प्रोजेक्ट कोट की संरचना की तरह है जिसमें लाइनें, लाइन विवरण और इनवॉइस शेड्यूल हैं।

अनुमान सीधे एक प्रोजेक्ट अनुबंध में किया जा सकता है, जैसा कि एक प्रोजेक्ट कोट में है। एक प्रोजेक्ट कोट के लिए, अनुबंध लाइनों और अनुबंध लाइन विवरण का उपयोग करके अनुमान किया जाता है। अनुबंध लाइन का विवरण एक प्रोजेक्ट प्लान से भी उत्पन्न किया जा सकता है जिसे बॉटम-अप अनुमान दृष्टिकोण का उपयोग करके बनाया गया था।

अनुबंध लाइन के विवरण का उपयोग समय, खर्च या शुल्क का अनुमान लगाने के लिए किया जा सकता है। अनुमानित कर राशि को अनुबंध लाइन विवरण पर भी दर्ज किया जा सकता है।

क्वोट लाइन विवरण में सामग्री अनुमानों की अनुमति नहीं है.

प्रोजेक्ट अनुबंध पर समर्थित प्रक्रियाएं इनवॉइस निर्माण और पुष्टिकरण हैं। इनवॉइस निर्माण प्रोजेक्ट-आधारित इनवॉइस का ड्राफ्ट तैयार करता है, जिसमें वर्तमान तारीख तक सभी बिल न की गई बिक्री वास्तविक शामिल होती हैं।

पुष्टिकरण अनुबंध को केवल पढ़ने योग्य बनाता है और इसकी स्थिति को **ड्राफ़्ट** से **पुष्टि की गई** में बदल देता है। यह कार्रवाई करने के बाद, आप इसे पूर्ववत नहीं कर सकते। क्योंकि यह कार्रवाई स्थायी है, इसलिए अनुबंध को **ड्राफ़्ट** स्थिति में रखना सबसे अच्छा अभ्यास है।

ड्राफ्ट अनुबंधों और पुष्टि किए गए अनुबंधों के बीच एकमात्र अंतर उनकी स्थिति है और तथ्य यह है कि ड्राफ्ट अनुबंधों को संपादित किया जा सकता है जबकि पुष्टि किए गए अनुबंधों को नहीं किया जा सकता। ड्राफ्ट अनुबंधों और पुष्टि किए गए अनुबंधों दोनों पर इनवॉइस बनाना और ट्रैकिंग वास्तविक हो सकते हैं।

परिवर्तन आदेश अनुबंधों या परियोजनाओं पर समर्थित नहीं हैं.

## <a name="estimating-projects"></a>प्रोजेक्ट का अनुमान लगाना

आप परियोजनाओं के समय और व्यय का अनुमान लगा सकते हैं लेकिन सामग्री या शुल्क का नहीं.

समय अनुमान तब उत्पन्न होते हैं जब आप कोई कार्य बनाते हैं और कार्य करने के लिए आवश्यक सामान्य संसाधन की विशेषताओं की पहचान करते हैं। समय का अनुमान शेड्यूल कार्यों से उत्पन्न होता है। यदि आप शेड्यूल के संदर्भ में सामान्य टीम सदस्य बनाते हैं तो समय का अनुमान नहीं लगाया जाता है।

**अनुमान** पृष्ठ पर ग्रिड में खर्च का अनुमान लगाया जाता है।

## <a name="understand-estimation"></a>अनुमानों को समझना

अनुमान चरण में व्यावसायिक तर्क को समझने के लिए एक गाइड के रूप में निम्न तालिका का उपयोग करें।

| परिदृश्य                                                                                                                                                                                                                                                                                                                                          | इकाई रिकॉर्ड                                                                                                                                                                                                       | लेन-देन का प्रकार | लेनदेन वर्ग | अतिरिक्त जानकारी                                                            |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------|-------------|-----------------------------------------------------------------------------------|
| जब आपको किसी कोट पर समय के बिक्री मूल्य का अनुमान लगाने की आवश्यकता होती है                                                                                                                                                                                                                                                                                    | कोट लाइन विवरण (QLD) रिकॉर्ड बनाया जाता है                                                                                                                                                                               | प्रोजेक्ट अनुबंध | Time        | बिक्री पक्ष QLD पंक्ति पर लेन-देन का मूल फ़ील्ड, लागत पक्ष QLD का संदर्भ देता है |
|                                                                                                                                                                                                                                                                                     | इसी लागत मूल्यों को स्टोर करने के लिए सिस्टम द्वारा एक दूसरा QLD रिकॉर्ड बनाया जाता है। सभी गैर-धन वाले फ़ील्ड को सिस्टम द्वारा बिक्री QLD से लागत QLD में कॉपी किया जाता है।                                                                                                                                                                               | लागत | Time        | विक्रय पक्ष कोट लाइन विवरण (QLD) लाइन पर लेन-देन का मूल फ़ील्ड, लागत पक्ष QLD का संदर्भ देता है |
| जब आपको अनुबंध पर समय के बिक्री मूल्य का अनुमान लगाने की आवश्यकता होती है                                                                                                                                                                                                                                                                                 | प्रोजेक्ट अनुबंध लाइन विवरण (CLD) रिकॉर्ड बनाया जाता है                                                                                                                                                                    | प्रोजेक्ट अनुबंध | Time        | बिक्री पक्ष CLD पंक्ति पर लेन-देन मूल फ़ील्ड लागत CLD का संदर्भ देता है      |
|                                                                                                                                                                                                                                                                                  | इसी लागत मूल्यों को स्टोर करने के लिए सिस्टम द्वारा एक दूसरा CLD रिकॉर्ड बनाया जाता है। सभी गैर-धन वाले फ़ील्ड को सिस्टम द्वारा बिक्री CLD से लागत CLD में कॉपी किया जाता है।                                                                                                                                                                    | लागत | Time        | बिक्री पक्ष CLD पंक्ति पर लेन-देन मूल फ़ील्ड लागत CLD का संदर्भ देता है      |
| जब उपयोगकर्ता प्रोजेक्ट कार्य पर एक संसाधन का वर्णन करता है                                                                                                                                                                                                                                                                                            | कार्य के बिक्री मूल्य को दिखाने के लिए अनुमानित लाइन रिकॉर्ड तब बनाया जाता है जब किसी कार्य को सभी आवश्यक मूल्य निर्धारण आयामों के साथ बनाया जाता है। भूमिका और संगठनात्मक इकाइयां मूल्य निर्धारण के पैमाने हैं | परियोजना अनुबंध | समय        |                                                                                   |
|     | कार्य की लागत मूल्य दिखाने के लिए अनुमान लाइन रिकॉर्ड तब बनाया जाता है जब किसी कार्य को सभी आवश्यक मूल्य निर्धारण आयामों के साथ बनाया जाता है। सभी गैर-धन वाले फ़ील्ड को सिस्टम द्वारा बिक्री अनुमान लाइन से लागत अनुमान लाइन तक कॉपी किया जाता है। भूमिका और संगठनात्मक इकाई लागत और बिल दर दोनों के लिए मूल्य निर्धारण के पैमाने हैं.                                                                                                                                                                                                                | लागत             | समय           |                                                                                   |



## <a name="customize-the-quote-line-detail-and-contract-line-detail-entities"></a>क्वोट लाइन विवरण और अनुबंध लाइन विवरण निकायों को अनुकूलित करें

यदि आपने कोट लाइन विवरण पर एक कस्टम फ़ील्ड जोड़ा है और चाहते हैं कि सिस्टम संबंधित मूल्य लाइन पर डिफ़ॉल्ट मान के रूप में फ़ील्ड के उस मूल्य को दर्ज करे जिसे यह बनाता है, तो PreOperationContractLineDetailUpdate और PreOperationQuoteLineDetailUpdate प्लग-इन पंजीकरण टूल का उपयोग करें. इन प्लग-इन को फिर से कोट लाइन विवरण या अनुबंध लाइन विवरण बदलने के बाद पंजीकृत किया जाना चाहिए। प्रक्रिया को पूरा करने के लिए इन चरणों का पालन करें।

1. PluginRegistrationTool खोलें, और अपने ऑनलाइन उदाहरण से कनेक्ट करें।
2. **खोज** का चयन करें और अपडेट करने के लिए प्लग-इन को खोजें।
3. प्लग-इन का चयन करें और फिर, मुख्य पृष्ठ पर, **चुनें** का चयन करें।
4. अपडेट करने के लिए प्लग-इन का चरण चुनें, राइट-क्लिक करें और फिर **अपडेट** चुनें।
5. **मौजूदा चरण अपडेट** संवाद बॉक्स में, **फ़िल्टरिंग विशेषताएं** फ़ील्ड में, दीर्घवृत्त बटन (**।।।**) का चयन करें:
6. **चयन विशेषताएं** संवाद बॉक्स में, कस्टम विशेषताओं के लिए चेक बॉक्स का चयन करें।
7. संवाद बॉक्स बंद करने के लिए **ठीक** चुनें और फिर **चरण अपडेट** चुनें।
8. दूसरे प्लग-इन के लिए चरण 1 को 7 से दोहराएं।
9. PluginRegistrationTool को बंद करें।