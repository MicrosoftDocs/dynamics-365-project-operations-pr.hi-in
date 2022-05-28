---
title: लेन-देन कनेक्शन - विभिन्न प्रकार के लेन-देन के वास्तविक लिंक
description: यह विषय बताता है कि लाभप्रदता, बिलिंग बैकलॉग, और बिल बनाम बिल न किए गए राजस्व गणनाओं को ट्रैक करने में मदद करने के लिए विभिन्न प्रकार के वास्तविक लिंक के लिए लेनदेन कनेक्शन का उपयोग कैसे किया जाता है।
author: rumant
ms.date: 03/25/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: rumant
ms.openlocfilehash: 2e8d75a69e27619e6a21f0fe61e2c656e94017b0
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/14/2022
ms.locfileid: "8580780"
---
# <a name="transaction-connections---link-actuals-of-different-transaction-types"></a>लेन-देन कनेक्शन - विभिन्न प्रकार के लेन-देन के वास्तविक लिंक

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

लेन-देन कनेक्शन रिकॉर्ड विभिन्न प्रकार के वास्तविक समय को जोड़ने के लिए बनाए जाते हैं, जैसे समय, व्यय, या सामग्री का उपयोग इसके जीवन चक्र में उद्धरण या पूर्व-बिक्री चरण से अनुबंध चरण, अनुमोदन और/या याद, चालान, और संभावित रूप से क्रेडिट या सुधारात्मक चालान तक चलता है। .

निम्न उदाहरण एक Project Operations परियोजना जीवनचक्र में समय प्रविष्टियों के विशिष्ट प्रसंस्करण को दर्शाता है.

> ![परियोजना संचालन में प्रसंस्करण समय प्रविष्टियाँ।](media/basic-guide-17.png)

प्रोजेक्ट ऑपरेशंस प्रोजेक्ट जीवनचक्र में समय प्रविष्टियों का प्रसंस्करण इन चरणों का पालन करता है: 

1. एक समय प्रविष्टि प्रस्तुत करने से दो जर्नल लाइनें बन जाती हैं: एक लागत के लिए और एक बिल न की गई बिक्री के लिए। 
2. समय प्रविष्टि की अंतिम स्वीकृति के कारण दो वास्तविक बन जाते हैं: एक लागत के लिए और एक बिल न की गई बिक्री के लिए। ये 2 वास्तविक लेन-देन कनेक्शन का उपयोग करके जुड़े हुए हैं।
3. जब उपयोगकर्ता एक परियोजना इनवॉइस बनाता है, तो बिल न की गई बिक्री वास्तविक से डेटा का उपयोग करके इनवॉइस पंक्ति लेन-देन बनाया जाता है.
4. जब इनवॉइस की पुष्टि हो जाती है, तो यह दो नए वास्तविक बनाता है: एक बिल न किया गया विक्रय उत्क्रमण और एक वास्तविक बिल की गई बिक्री। बिल न किए गए विक्रय उत्क्रमण और वास्तविक बिल न किए गए विक्रय वास्तविक लेन-देन कनेक्शन का उपयोग करके जुड़े हुए हैं। बिल की गई बिक्री और बिना बिल की गई वास्तविक बिक्री के वास्तविक आंकड़े भी एक समय बैकलॉग या वर्क इन प्रोग्रेस (डब्ल्यूआईपी) राजस्व के बीच के लिंक को दिखाने के लिए जुड़े हुए हैं जो अब बिल राजस्व है।   

प्रसंस्करण कार्यप्रवाह में प्रत्येक घटना रिकॉर्ड के निर्माण को ट्रिगर करती है **लेन-देन कनेक्शन** टेबल। यह समय प्रविष्टि, जर्नल लाइन, वास्तविक और इनवॉइस लाइन विवरण में बनाए गए रिकॉर्ड के बीच संबंध का एक ट्रेस बनाने में मदद करता है।

निम्न तालिका में अभिलेखों को दिखाया गया है: **लेन-देन कनेक्शन** पिछले कार्यप्रवाह के लिए निकाय।

|ईवेंट                   |लेनदेन 1                 |लेन-देन 1 भूमिका |लेनदेन 1 प्रकार       |लेनदेन 2          |लेन-देन 2 भूमिका |लेनदेन 2 प्रकार |
|------------------------|------------------------------|---------------|-----------------------------|-----------------------------|-------------------|-------------------|
|समय प्रविष्टि सबमिशन   |जर्नल पंक्ति (बिक्री) GUID     |बिना बिल की गई विक्रय |msdyn_journalline            |जर्नल पंक्ति (लागत) GUID     |लागत            |msdyn_journalline  |
|समय स्वीकृति           |बिल न की गई वास्तविक (बिक्री) GUID  |बिना बिल की गई विक्रय |msdyn_actual                 |लागत वास्तविक (लागत) GUID       |लागत            |msdyn_actual       |
|इनवॉइस निर्माण        |इनवॉइस पंक्ति डिटेल GUID      |बिल की गई विक्रय   |msdyn_invoicelinetransaction |बिल न की गई बिक्री वास्तविक GUID   |बिना बिल की गई विक्रय  |msdyn_actual       |
|इनवॉइस की पुष्टि    |वास्तविक GUID को उलटना         |उलटना      |msdyn_actual                 |मूल निर्बाध बिक्री GUID |मूल        |msdyn_actual       |
|                        |बिल की बिक्री GUID             |बिल की गई विक्रय   |msdyn_actual                 |बिल न की गई बिक्री वास्तविक GUID   |बिना बिल की गई विक्रय  |msdyn_actual       |
|ड्राफ्ट इनवॉइस सुधार |इनवॉइस पंक्ति लेन-देन GUID|बदलना      |msdyn_invoicelinetransaction |बिल की बिक्री GUID            |मूल        |msdyn_actual       |
|इनवॉइस सुधार की पुष्टि करें|बिल की बिक्री उलटना GUID  |उलटना      |msdyn_actual                 |बिल की बिक्री GUID            |मूल        |msdyn_actual       |
|                        |नई बिल न की गई बिक्री GUID |बदलना            |msdyn_actual                 |बिल की बिक्री GUID            |मूल        |msdyn_actual       |


निम्नलिखित उदाहरण प्रोजेक्ट संचालन में समय प्रविष्टियों के उदाहरण का उपयोग करके विभिन्न घटनाओं में विभिन्न प्रकार के वास्तविक के बीच बनाए गए लिंक दिखाता है।

> ![परियोजना संचालन में विभिन्न प्रकार के वास्तविक एक दूसरे से कैसे जुड़े हैं।](media/TransactionConnections.png)

[!INCLUDE[footer-include](../includes/footer-banner.md)]