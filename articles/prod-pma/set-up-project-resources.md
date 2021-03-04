---
title: प्रोजेक्ट संसाधन सेट अप करना
description: यह विषय परियोजना संसाधनों को सेट करने या अनुरोध के बारे में जानकारी प्रदान करता है.
author: Yowelle
manager: AnnBe
ms.date: 09/01/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 82022
ms.assetid: bd2fb375-84c6-428a-8e54-f0f719045898
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 7eec8ad5d78019219b2e04ca75eeaa5a3c8a748f
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077872"
---
# <a name="set-up-project-resources"></a>प्रोजेक्ट संसाधन सेट अप करना

[!include [banner](../includes/banner.md)]

आपको एक कैलेंडर व्यवस्थित करना होगा और इसे किसी कर्मचारी या कामगार के साथ जोड़ना होगा. कैलेंडर का उपयोग परियोजना को शेड्यूल करने तथा उन संसाधनों के कार्य समय के लिए किया जाता है जो परियोजना के लिए आरक्षित होते हैं. कैलेंडर व्यवस्थापन के दौरान परियोजना प्रबंधक के द्वारा संसाधन अनुकूलन के भाग के रूप में संसाधन समतलन किया जा सकता है. कैलेंडर शेड्यूल के आधार पर, संसाधनों पर प्रतिबंध लगाया जा सकता है. आप **कैलेंडर** पृष्ठ पर एक कैलेंडर सेट कर सकते हैं.

जब आप एक श्रमिक को एक परियोजना संसाधन के रूप में सेट करते हैं, तो आप उन श्रमिकों में से जो कंपनी में काम करते हैं जिनके लिए आप संसाधन सेट कर रहे हैं उन्हें चुन सकते हैं. वैकल्पिक रूप से, आप अपने संगठन में अन्य कंपनियों से श्रमिकों का चयन कर सकते हैं. इन श्रमिकों को कंपनियों के बीच के संसाधन के रूप में जाना जाता है.

निम्नलिखित प्रक्रियाएं समझाती हैं कि आपकी कंपनी में एक परियोजना संसाधन के रूप में एक श्रमिक को कैसे सेट किया जाए और कंपनियों के बीच के एक परियोजना संसाधन को कैसे सेट किया जाए.

## <a name="set-up-a-worker-as-a-project-resource"></a>एक परियोजना संसाधन के रूप में एक श्रमिक को सेट करें

1. **श्रमिक** पृष्ठ पर, **श्रमिक** सूची में, उस श्रमिक का चयन करें जिसे आप एक परियोजना संसाधन के रूप में जोड़ रहे हैं, और श्रमिक रिकॉर्ड खोलें.
2. क्रिया-कलाप फलक पर, **परियोजना** &gt; **सेटअप** &gt; **परियोजना सेटअप** चुनें .
3. कैलेंडर का चयन करें, और उसके बाद पृष्ठ बंद करें.

आप पूर्व-कार्यभार के एक प्रकार के रूप में संसाधन के लिए डिफ़ॉल्ट परियोजनाओं को भी निर्दिष्ट कर सकते हैं. जब संसाधन प्रबंधक या परियोजना प्रबंधक जानता है कि संसाधन पहले से किन परियोजनाओं पर काम कर रहा होगा, तो पूर्व-कार्यभार का उपयोग किया जा सकता है. पूर्व-कार्यभार किसी परियोजना प्रायोजक या ग्राहक के अनुरोध पर भी आधारित हो सकते हैं. एक परियोजना को पहले से नियत करने के लिए, **परियोजनाओं को नियत करें** पृष्ठ पर, **परियोजनाएं** टैब पर, **शेष परियोजनाएं** सूची में, उपयुक्त परियोजना का चयन करें.

## <a name="set-up-an-intercompany-resource"></a>एक इंटरकंपनी संसाधन सेट करें

जब आप कंपनियों के बीच के एक संसाधन के रूप में एक श्रमिक को सेट करते हैं, तो आपको ऋण देने वाली कंपनी और लेने वाली कंपनी दोनों में सेटअप पूरा करना होगा.

### <a name="in-the-lending-company"></a>ऋण देने वाली कंपनी में

1. फाइनैन्स में, सत्यापित करें कि ऋण देने वाली कंपनी का चयन किया जाता है, और फिर पिछले अनुभाग में प्रक्रिया पूरी करें, "एक परियोजना संसाधन के रूप में एक श्रमिक को सेट करें."
2. **कंपनियों के बीच लेखांकन** पृष्ठ पर, **नया** चुनें.
3. **कानूनी निकाय ID** फ़ील्ड में, ऋण देने वाली कंपनी का चयन करें. उपयुक्त के रूप में शेष फ़ील्ड में भरें, और फिर **सहेजें** का चयन करें.
4. **स्थानांतरण मूल्य** पृष्ठ पर **नया** का चयन करें.
5. **ऋण लेने वाली कानूनी निकाय** फ़ील्ड में, उपयुक्त कंपनी का चयन करें.
6. ऋण लेने वाली कंपनी को केवल उस संसाधन को ऋण देने के लिए जो आपने इस अनुभाग की शुरुआत में बनाया, **संसाधन** फ़ील्ड में, आपके द्वारा बनाए गए संसाधन का नाम चुनें. ऋण देने वाली कंपनी में सभी संसाधनों को ऋण लेने वाली कंपनी को उपलब्ध कराने के लिए, **संसाधन** फील्ड खाली छोड़ दें.
7. **परियोजना प्रबंधन और लेखांकन मापदंड** पृष्ठ पर **इंटरकंपनी** टैब पर, **कंपनियों के बीच संसाधन शेड्यूलिंग और टाइमशीट सक्षम करें** विकल्प को **हां** पर सेट करें.

### <a name="in-the-borrowing-company"></a>ऋण लेने वाली कंपनी में

- **संसाधन सूची** पृष्ठ पर, खोज फ़िल्टर में, आपके द्वारा ऋण देने वाली कंपनी के लिए बनाए गए संसाधन का नाम दर्ज करें, यह सत्यापित करने के लिए कि नाम ऋण लेने वाली कंपनी के लिए संसाधन सूची में शामिल है.

## <a name="request-project-resources"></a>प्रोजेक्ट संसाधनों अनुरोध
परियोजना संसाधन शेड्यूलिंग के लिए कार्यक्षमता केवल संसाधन प्रबंधकों को काम या परियोजना में कर्मचारी संसाधनों को वितरित करने देती है. इस कार्यक्षमता को सक्षम करने के लिए निम्नलिखित कार्य पूरा करें या सत्यापित करें कि वो पूरे हो गए हैं:

- संख्या क्रम सेट करें.
- परियोजना प्रबंधन और लेखांकन कार्यप्रवाह सेट करें.
- संसाधन अनुरोध वर्कफ़्लोज़ सक्षम करें.

पूर्ववर्ती कार्य पूरे होने के बाद, आप अपनी ज़रूरत के अनुसार निम्नांकित कार्यों को पूरा कर सकते हैं:

- सॉफ्ट-बुक किए गए कर्मचारी संसाधन से संसाधन अनुरोध बनाएं.
- संसाधन अनुरोधों की निगरानी करें.
- पूर्णता संसाधन अनुरोध.
- WBS से कर्मचारी संसाधन का अनुरोध करें.
- कर्मचारी संसाधन के लिए अनुरोध के बिना परियोजना के लिए संसाधन बुक करें.