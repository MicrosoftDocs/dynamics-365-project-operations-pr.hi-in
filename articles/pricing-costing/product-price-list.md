---
title: उत्पाद मूल्य सूचियाँ
description: यह विषय परियोजना कोटेशन और अनुबंधों में इस्तेमाल किए जाने वाले कैटलॉग मूल्य निर्धारण में मूल्य सूचियों के बारे में जानकारी देता है.
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
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 3570aeb78804e9b267caa55a27e02d6c8df9a5c6
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898173"
---
# <a name="product-price-lists"></a>उत्पाद मूल्य सूचियाँ

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

मूल्य सूची और मूल्य सूची आइटम एंटिटी उत्पाद सूची मूल्य निर्धारण का समर्थन करती हैं। ज्यादातर, इस फंक्शन का इस्तेमाल प्रोजेक्ट के कोट्स और प्रोजेक्ट की संविदाओं पर कैटेलॉग-आधारित लाइनों के लिए किया जाता है।

प्रोजेक्ट-आधारित लाइनों के लिए, संविदा प्राप्त आदेश को दर्शाती है। क्योंकि आम तौर पर आदेश प्राप्त होने से पहले ही सौदे की वार्ता की जाती है, कीमत निर्धारण जो कोट के साथ की जाती है, हमेशा नई कीमत सूची की अनुलिपि होती है और संविदा से संबद्ध होती है। इस नई कीमत सूची को संविदा की परिधि से बाहर परिवर्तित नहीं किया जा सकता। यह सीमा मास्टर कीमत सूची में होने वाले कीमत परिवर्तन से वार्ता द्वारा निर्धारित दर कार्ड को सुरक्षित रखने में मदद करती है।

प्रॉडक्ट निर्धारित होने चाहिए ताकि प्रॉडक्ट कैटेलॉग में उनकी डिफाल्ट लागत और कीमत सूची हो। डिफ़ॉल्ट कीमत और सूची मूल्यों को कॉन्फ़िगर करने के लिए सूची मूल्य, मानक लागत और वर्तमान लागत का इस्तेमाल करें. इन डिफाल्ट सूची की कीमतों का इस्तेमाल केवल कोट लाइन या प्रोजेक्ट कांट्रेक्ट लाइन के लिए किया जाता है जब सिस्टम को किसी कोट या प्रोजेक्ट कांट्रेक्ट के लिए प्रॉडक्ट कीमत लाइन में उस प्रॉडक्ट की कीमत सूची लाइन नहीं मिल पाती है।

प्रॉडक्ट कैटेलॉग लाइनों की लागत कीमत को कोट के बीच परिवर्तित किया जा सकता है। यह सक्षमता महत्वपूर्ण है क्योंकि यदि आप सटीक ढंग से लागतों का पता नहीं लगा सकते हैं तो आप प्रोजेक्ट के प्रचालनीय लाभ को भी निर्धारित नहीं कर सकते हैं। डिफ़ॉल्ट रूप से, उत्पाद की मानक लागत का इस्तेमाल लागत कीमत के रूप में किया जाता है। हालांकि, डिफाल्ट लागत कीमत को कोट लाइन पर अपडेट किया जा सकता है यदि उस कोट के लिए अलग लागत कीमत हो।

## <a name="price-list-items"></a>कीमत सूची के आइटम

आप एक प्रॉडक्ट कैटेलॉग से दूसरी कीमत सूचियों में उत्पाद जोड़ सकते हैं। प्रॉडक्ट की कीमत सूची लाइनें एक विशेष यूनिट को बताती हैं। कीमत सूची मदों पर प्रॉडक्ट के कीमत निर्धारण को मुद्रा की राशि के रूप में कॉन्फ़िगर किया जा सकता है। वैकल्पिक रूप स, इसे कीमत सूची, चालू लागत या मानक लागत के कार्य के रूप में कॉन्फ़िगर किया जा सकता है।

जब कीमतों को कीमत सूची, मानक लागत या चालू लागत के कार्य के रूप में कन्फीगर किया जाता है तो PSA विभिन्न राउंडिंग विकल्पों का समर्थन करता है। एक से अधिक कीमत निर्धारण विधियों और राउंडिंग विकल्पों का लाभ लेने के अलावा, आप डिस्काउंट सूची को कीमत सूची की मदों के साथ जोड़ सकते हैं। 

जब आप **परियोजना कोटेशन** पृष्ठ पर **कस्टम मूल्य निर्धारण बनाएं** चुनकर कोटेशन के लिए नई कस्टम मूल्य सूची बनाते हैं तो मूल्य सूची की प्रतिलिपि बनाई जाती है, और नई मूल्य सूची के शीर्ष पर **इकाई** फ़ील्ड को **बिक्री इकाई** पर सेट किया जाता है. नई कीमत सूची का नाम कोट और टाइमस्टैम्प के नाम के साथ लगाया जाता है। कस्टम कीमत निर्धारण का इस्तेमाल करने वाले कोट के लिए अतिरिक्त रिव्यू और अनुमोदन करने के लिए आप कस्टम वर्कफ्लो में नई कीमत सूची और कोट के नाम का भी इस्तेमाल कर सकते हैं।

 
## <a name="default-product-price-list"></a>डिफाल्ट प्रॉडक्ट कीमत सूची
प्रत्येक ग्राहक रिकार्ड में **डिफॉल्ट मूल्य लिस्ट** फील्ड होता है जहाँ आप ग्राहक की मुद्रा से मेल करने वाली कीमत सूची को निर्दिष्ट कर सकते हैं। डिफाल्ट मूल्य इस फील्ड में अपने आप दर्ज नहीं होता है. जब किसी विशेष ग्राहक के साथ कस्टम कीमत निर्धारण करार मौजूद होता है तो आप इस फील्ड का इस्तेमाल उस ग्राहक के साथ कीमत सूची से जोड़ सकते हैं।

अवसर, कोट और प्रोजेक्ट कांट्रेक्ट एंटिटी डिफाल्ट प्रॉडक्ट कीमत सूचियों को दर्ज करने के लिए निम्नलिखित क्रम का इस्तेमाल करते हैं। इसी क्रम का इस्तेमाल प्रोजेक्ट कीमत सूचियों के लिए किया जाता है।

1.  भाव प्रस्ताव
2.  अवसर
3.  ग्राहक
4.  ग्लोबल सेटिंग 

डिफाल्ट द्वारा, कोट लाइन पर **प्रॉडक्ट** फील्ड कोट की प्रॉडक्ट कीमत सूची में सभी सक्रिय प्रॉडक्ट की सूची बनाता है। यदि कोई प्रॉडक्ट निष्क्रिय किया गया हो यो यदि वह ड्राफ्ट प्रॉडक्ट हो तो कीमत की सूची में होने पर भी उसे सूचीबद्ध नहीं किया जाता। 

प्रोजेक्ट कांट्रेक्ट के लिए बनाए गए पहले इनवॉइस पर इनवॉइस लाइनों के रूप में प्रॉडक्ट कैटेलॉग लाइनों को जोड़ा जाता है। ड्राफ्ट इनवॉइस में, ऐसी इनवॉइस लाइनों को हटाया जा सकता है। ऐसे मामले में, ये लाइनें इनवॉइस बनाए जाने तक या इनवॉइस ग्राहक को भेजे जाने तक, बाद की इनवॉइस में दिखता रहेगा। आप प्रॉडक्ट इनवॉइस लाइन की आंशिक मात्रा का बीजक नहीं बना सकते. जब प्रोजेक्ट कांट्रेक्ट से प्रॉडक्ट लाइनों का इनवॉइस बनाया जाता है, तो वास्तविक इनवॉइस बनाया जाता है। हालांकि, ऐसे वास्तविक इनवॉइस संबंधित प्रोजेक्ट एंटिटी से जोड़े नहीं जाते। दूसरे शब्दों में, प्रॉडक्ट-आधारित प्रोजेक्ट कांट्रेक्ट लाइनें किसी प्रोजेक्ट-आधारित इस्तेमाल से स्वतंत्र होती हैं। परियोजनाओं में सामग्री के उपभोग पर नज़र नहीं रखी गयी है.