---
title: मूल्य निर्धारण आयाम बंद करना
description: यह विषय मूल्य निर्धारण पैमानों को बंद करने के बारे में जानकारी देता है.
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
ms.openlocfilehash: 54e02726138f7306481ca50d5204ee29a3b68549
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896508"
---
# <a name="turning-off-a-pricing-dimension"></a>मूल्य निर्धारण आयाम बंद करना

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

आपको कुछेक वर्षों बाद अपनी प्राइस निर्धारण रणनीति की समीक्षा और इसे अपडेट करने की आवश्यकता हो सकती है। आपके द्वारा किए गए किसी भी अपडेट के लिए आपका किसी मौजूदा प्राइस निर्धारण आयाम को बंद कर नया आयाम बनाना आवश्यक हो सकता है। उदाहरण के लिए आपने पहले **भूमिका** के हिसाब से प्राइसिंग हो हो लेकिन अब आपने **कार्य अनुभव** के हिसाब से प्राइस तय करना है। ऐसा करने के लिए आपको मूल्य निर्धारण पैमानों के रूप में **रोल** को बंद करके **कार्य अनुभव** को नया मूल्य निर्धारण पैमाना बनाना होगा. 

किसी प्राइस-निर्धारण आयाम को बंद करने हेतु, भले ही वह आउट-ऑफ-द-बॉक्स या कस्टम हो, प्राइस निर्धारण के **लागत पर लागू** और **बिक्री पर लागू** फ़ील्ड को **नहीं** पर सेट करें।

यद्यपि, जब आप ऐसा करते हैं तो आपको त्रुटि संदेश प्राप्त हो सकता है, **यदि संबंधित मूल्य रिकॉर्ड हैं, तो मूल्य निर्धारण पैमाना को अद्यतन या मिटाया नहीं जा सकता है.**

यह त्रुटि संदेश इंगित करता है कि जिस आयाम को बंद किया जा रहा है, उसके लिए पहले तय किये गए प्राइस रिकॉर्ड हैं। किसी आयाम पर लागू होने की शर्त को **नहीं** पर सेट करने से पहले आयाम को दर्शाने वाले सभी **रोल प्राइस** और **रोल प्राइस मार्कअप** रिकॉर्ड को हटा दिया जाना चाहिए। यह नियम आउट-ऑफ-द-बॉक्स प्राइस निर्धारण आयामों और आपके द्वारा बनाए गए कस्टम प्राइस निर्धारण आयामों पर लागू होता है। इस सत्यापन का कारण यह है कि प्रत्येक **रोल प्राइस** रिकॉर्ड में पैमानों का विशिष्ट संयोजन होना चाहिए. उदाहरण के लिए किसी **US लागत रेट 2018** नामक प्राइस सूची में निम्न **रोल प्राइस** पंक्ति हैं। 

| स्टेंडर्ड टाइटल         | संगठन इकाई    |इकाई   |मूल्य  |मुद्रा  |
| -----------------------|-------------|-------|-------|----------|
| सिस्ट्म्स इंजीनियर|Contoso US|Hour| 100|USD|
| वरिष्ठ सिस्ट्म्स इंजीनियर|Contoso US|Hour| 150| USD|


जब आप मूल्य निर्धारण पैमानों के तौर पर **मानक शीर्षक** को बंद कर देते हैं और मूल्य निर्धारण इंजन रोल के लिए मूल्य की खोज करता है, तो केवल इनपुट संदर्भ से **संगठन इकाई** मान का उपयोग करता है. यदि इनपुट संदर्भ की **संगठनात्मक इकाई** “Contoso US” है, तो कोई भी परिणाम नहीं निकल सकेंगे क्योंकि दोनों पंक्तियों का मिलान हो जाएगा। इस परिदृश्य से बचने के लिए, जब आप **रोल प्राइस** रिकॉर्ड बनाते हैं, तो सिस्टम यह पुष्टि करता है कि पैमानों का संयोजन विशिष्ट है. यदि **भूमिका मू्ल्य** रिकॉर्ड बनने के बाद आयाम बंद कर दिया जाता है, तो इस सीमा का उल्लंघन किया जा सकता है। इसलिए आयाम बंद करने से पहले आवश्यक है कि आप सभी **भूमिका मू्ल्य** और **भूमिका मू्ल्य मार्कअप** पंक्तियों को हटा दें, जिनमें आयामों के मान दर्ज हैं।