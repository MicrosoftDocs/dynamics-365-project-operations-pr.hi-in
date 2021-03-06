---
title: स्वचालित इनवॉइस निर्माण कॉन्फ़िगर करें
description: यह विषय स्वचालित रूप से इनवॉइस बनाने के लिए सिस्टम को कॉन्फ़िगर करने के लिए हॉट के बारे में जानकारी देता है.
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
ms.openlocfilehash: 764fd4568619e4f5676ee3cbf7fce14ffb069548
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898128"
---
# <a name="configure-automated-invoice-creation"></a>स्वचालित इनवॉइस निर्माण कॉन्फ़िगर करें

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

Project Operations में स्वचालित इनवॉइस चलाने को कॉन्फ़िगर करने के लिए निम्न चरणों को पूरा करें.

1. **सेटिंग्स** \> **बैच जॉब** पर जाएँ.
2. एक बैच जॉब तैयार करें और उसे **परियोजना संचालन क्रिएट इनवॉयस** नाम दें. बैच जॉब के नाम में "क्रिएट इनवॉयस" शब्द होना ज़रूरी है.
3. **जॉब प्रकार** फील्ड में, **कुछ नहीं** चुनें। **रोज़ की आवॉत्ति** और **सक्रिय है** विकल्प अपने आप **हाँ** में सेट होते हैं।
4. **वर्कफ्लो चलाएँ** चुनें। **लुक अप रिकार्ड** डॉयलॉग बॉक्स में, आपको तीन वर्कफ्लो दिखेंगे:

    - ProcessRunCaller
    - ProcessRunner
    - UpdateRoleUtilization

5. **ProcessRunCaller** चुनें, फिर **Add** चुनें।
6. अगले डॉयलॉग बॉक्स में,**ओके** चुनें। **प्रोसेस** वर्कफ्लो के बाद एक **स्लीप** वर्कफ्लो आएगा।

    आप **ProcessRunner** को 5 चरणों में चुन सकते हैं। इसके बाद, जब आप **OK** चुनते हैं, तो **स्लीप** वर्कफ्लो के बाद **प्रोसेस** वर्कफ्लो आएगा।

**ProcessRunCaller** और **ProcessRunner** वर्कफ्लो बीजक तैयार करेंगे। **ProcessRunCaller** कॉल **ProcessRunner**। **ProcessRunner** वह वर्कफ्लो होता है जो वास्तव में बीजक तैयार करता है। यह बीजक तैयार करने के लिए आवश्यक सभी संविदा लाइनों से गुजरता है और उन लाइनों के लिए बीजक तैयार करता है। बीजक के लिए आवश्यक संविदा लाइनें तय करने के लिए, जॉब में संविदा लाइनों के लिए बीजक चलाने की तारीखें देखी जाती हैं। यदि किसी एक संविदा से संबंधित संविदा लाइनों की बीजक चलाने की तारीखें समान हैं तो दो बीजक लाइनों वाले एक बीजक में लेनदेन संयोजित कर दिए जाते हैं। यदि बीजक तैयार करने के लिए कोई लेनदेन न हों तो जॉब बीजक तैयार करना छोड़ देता है।

**ProcessRunner** चलने का काम पूरा होने के बाद, यह **ProcessRunCaller** को बुलाता है और अंतिम समय देता है और बंद हो जाता है। इसके बाद **ProcessRunCaller** टाइमर शुरु करता है जो निर्दिष्ट अंतिम समय से 24 घंटों तक चलते रहता है। टाइमर के अंत में, **ProcessRunCaller** बंद हो जाएगा।

बीजक तैयार करने के लिए बैच प्रोसेस जॉब आवर्ती जॉब है। यदि बैच प्रोसेस कई बार चलाया जाता है तो जॉब कई बार किया जाएगा और त्रुटियाँ होंगी। इसलिए, आपको केवल एक बार बैच प्रोसेस शुरु करना चाहिए और इसके बंद होने पर ही दोबारा चालू करना चाहिए।

> [!NOTE]
> बैच इनवॉइसिंग केवल परियोजना अनुबंध लाइनों के लिए चलती है जो इनवॉइस शेड्यूल से कॉन्फ़िगर किए गए हैं. निश्चित मूल्य बिलिंग विधि वाली अनुबंध पंक्ति में माइलस्टोन कॉन्फ़िगर होने चाहिए. समय और सामग्री बिलिंग विधि वाली परियोजना अनुबंध पंक्ति को दिनांक-आधारित इनवॉइस शेड्यूल सेट अप की आवश्यकता होगी. यही बात परियोजना-आधारित अनुबंध पंक्ति पर लागू होती है.     
