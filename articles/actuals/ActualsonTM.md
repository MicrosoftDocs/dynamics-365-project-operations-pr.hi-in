---
title: एक समय और सामग्री जुड़ाव में वास्तविक प्रभाव
description: यह विषय Microsoft में एक समय और सामग्री सहभागिता के जीवनचक्र के दौरान विभिन्न घटनाओं पर वास्तविक तालिका पर प्रभाव के बारे में जानकारी प्रदान करता है।Dynamics 365 Project Operations
author: rumant
ms.date: 02/22/2022
ms.topic: overview
ms.prod: ''
audience: Application User
ms.reviewer: johnmichalak
ms.search.scope: ''
ms.assetid: ''
ms.search.region: ''
ms.search.industry: ''
ms.author: rumant
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: a4ea3f9cf74d8a67447571001b75065b8cde5c00
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/14/2022
ms.locfileid: "8580826"
---
# <a name="actuals-impact-in-a-time-and-materials-engagement"></a>एक समय और सामग्री जुड़ाव में वास्तविक प्रभाव

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

निम्न तालिका विभिन्न प्रकार के लेन-देन के वास्तविक को सूचीबद्ध करती है जो एक समय और सामग्री जुड़ाव में विभिन्न घटनाओं में बनाए जाते हैं।

| ईवेंट | वास्तविक लागत | वास्तविक अनबिल्ड बिक्री | बिल की गई बिक्री वास्तविक | उदाहरण |
|---|---|---|---|---|
| समय बनाया गया है। | लागू नहीं | लागू नहीं | लागू नहीं | <p>फ़ैब्रिकम यूएस संगठनात्मक इकाई से बॉब कोज़ैक, जिसकी लागत दर 100 यूएस डॉलर (यूएसडी 100) प्रति घंटा है, एक प्रोजेक्ट पर काम कर रहा है जिसका नाम "आर्म इंस्टालेशन एट एडैटम" है। इस परियोजना के लिए उनकी अनुबंधित बिल दर USD 200 प्रति घंटा है। बॉब कोज़ाक से नमूना समय प्रविष्टि यहां दी गई है:</p><p>बॉब कोज़ैक, 8 घंटे</p> |
| समय प्रस्तुत किया गया है। | लागू नहीं | लागू नहीं | लागू नहीं | समय प्रविष्टि के लिए एक लागत जर्नल लाइन और बिल न किए गए विक्रय जर्नल बनाए जाते हैं। जर्नल प्रविष्टि में डिफ़ॉल्ट मूल्य और लागत दर दर्ज की जाती है। |
| स्वीकृत होने से पहले समय प्रविष्टि को वापस बुला लिया जाता है। | लागू नहीं | लागू नहीं | लागू नहीं | |
| समय स्वीकृत है: सबमिट किए गए घंटे बराबर बिल योग्य घंटे। | एक वास्तविक लागत बनाई जाती है। | एक बिल न की गई वास्तविक बिक्री बनाई जाती है। | लागू नहीं | <p>नए वास्तविक जो बनाए गए हैं:</p><ul><li>**वास्तविक लागत:** बॉब कोज़ैक, 8 घंटे, USD 800</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 8 घंटे, USD 1,600</li></ul> |
| समय स्वीकृत है: बिल करने योग्य घंटे सबमिट किए गए घंटों से कम कर दिए गए हैं। | एक वास्तविक लागत बनाई जाती है। | <p>दो बिल न किए गए वास्तविक विक्रय बनाए जाते हैं:</p><ul><li>बिल करने योग्य घंटों के लिए वास्तविक बिल न की गई बिक्री प्रभार्य</li><li>शेष मात्रा के लिए वास्तविक गैर-प्रभार्य बिल न की गई बिक्री</li></ul> | लागू नहीं | <p>नए वास्तविक जो बनाए गए हैं:</p><ul><li>**वास्तविक लागत:** बॉब कोज़ैक, 8 घंटे, USD 800</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 6 घंटे, USD 2,000, *प्रभार्य*</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 2 घंटा, USD 400, *गैर प्रभार्य*</li></ul> |
| समय स्वीकृत है: बिल करने योग्य घंटे सबमिट किए गए घंटों से ऊपर बढ़ा दिए गए हैं। | एक वास्तविक लागत बनाई जाती है। | एक बिल न की गई वास्तविक बिक्री बनाई जाती है। | लागू नहीं | <p>नए वास्तविक जो बनाए गए हैं:</p><ul><li>**वास्तविक लागत:** बॉब कोज़ैक, 8 घंटे, USD 800</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 10 घंटे, USD 2,000</li></ul> |
| समय अनुमोदन रद्द कर दिया गया है। | <p>वास्तविक वास्तविक लागत की समायोजन स्थिति को अपडेट किया जाता है **समायोजित।**</p><p>एक वास्तविक प्रतिवर्ती लागत बनाई जाती है जिसकी समायोजन स्थिति होती है **समायोज्य।**</p> | <p>वास्तविक बिल न की गई वास्तविक बिक्री की समायोजन स्थिति को अपडेट किया जाता है **समायोजित**.</p><p>एक रिवर्सल बिल न की गई वास्तविक बिक्री बनाई जाती है जिसमें समायोजन की स्थिति होती है **समायोज्य**.</p> | लागू नहीं | <p>मौजूदा वास्तविक जो अद्यतन किए गए हैं:</p><ul><li>**वास्तविक लागत:** बॉब कोज़ैक, 8 घंटे, USD 800, *समायोजित*</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 8 घंटा, USD 1,600, *समायोजित*</li></ul><p>नए वास्तविक जो पिछले वित्तीय प्रभाव को उलटने के लिए बनाए गए हैं:</p><ul><li>**वास्तविक लागत:** बॉब कोज़ैक, (8 घंटा), (यूएसडी 800), *समायोज्य*</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, (8 घंटा), (1,600 अमरीकी डालर), *समायोज्य*</li></ul> |
| स्वीकृत होने के बाद समय प्रविष्टि को वापस बुला लिया जाता है। | <p>वास्तविक वास्तविक लागत की समायोजन स्थिति को अपडेट किया जाता है **समायोजित।**</p><p>एक वास्तविक प्रतिवर्ती लागत बनाई जाती है जिसकी समायोजन स्थिति होती है **समायोज्य।**</p> | <p>वास्तविक बिल न की गई वास्तविक बिक्री की समायोजन स्थिति को अपडेट किया जाता है **समायोजित**.</p><p>एक रिवर्सल बिल न की गई वास्तविक बिक्री बनाई जाती है जिसमें समायोजन की स्थिति होती है **समायोज्य**.</p> | लागू नहीं | <p>मौजूदा वास्तविक जो अद्यतन किए गए हैं:</p><ul><li>**वास्तविक लागत:** बॉब कोज़ैक, 8 घंटे, USD 800, *समायोजित*</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 8 घंटा, USD 1,600, *समायोजित*</li></ul><p>नए वास्तविक जो पिछले वित्तीय प्रभाव को उलटने के लिए बनाए गए हैं:</p><ul><li>**वास्तविक लागत:** बॉब कोज़ैक, (8 घंटा), (यूएसडी 800), *समायोज्य*</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, (8 घंटा), (1,600 अमरीकी डालर), *समायोज्य*</li></ul> |
| अनुबंध की पुष्टि की है। | <p>वास्तविक वास्तविक लागत की समायोजन स्थिति को अपडेट किया जाता है **समायोजित**.</p><p>रिवर्सल कॉस्ट वास्‍तविक बनाए जाते हैं जिनकी समायोजन स्थिति होती है **समायोज्य**.</p><p>संविदात्मक नियमों के पुनर्मूल्यांकन के बाद नई लागत वास्तविक बनाई जाती है।</p> | <p>पुराने बिल न किए गए वास्तविक बिक्री की समायोजन स्थिति को अपडेट किया जाता है **समायोजित**.</p><p>रिवर्सल बिल न किए गए वास्तविक बिक्री वास्तविक बनाए जाते हैं जिनकी समायोजन स्थिति होती है **समायोज्य**.</p><p>संविदात्मक नियमों के पुनर्मूल्यांकन के बाद नए बिल न किए गए वास्तविक वास्तविक बनाए जाते हैं।</p> | लागू नहीं | <p>मौजूदा वास्तविक जो अद्यतन किए गए हैं:</p><ul><li>**वास्तविक लागत:** बॉब कोज़ैक, 8 घंटे, USD 800, *समायोजित*</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 8 घंटा, USD 1,600, *समायोजित*</li></ul><p>नए वास्तविक जो पिछले वित्तीय प्रभाव को उलटने के लिए बनाए गए हैं:</p><ul><li>**वास्तविक लागत:** बॉब कोज़ैक, (8 घंटा), (यूएसडी 800), *समायोज्य*</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, (8 घंटा), (1,600 अमरीकी डालर), *समायोज्य*</li></ul><p>नए वास्तविक जो पुनर्मूल्यांकन किए गए वित्तीय प्रभाव के लिए बनाए गए हैं:</p><ul><li>**वास्तविक लागत:** बॉब कोज़ैक, 8 घंटे, USD 800</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 8 घंटे, USD 1,600</li></ul> |
| एक चालान बनाया जाता है। | लागू नहीं | लागू नहीं | लागू नहीं | |
| चालान की पुष्टि हो गई है। बिल न की गई बिक्री की वास्तविक मात्रा से इनवॉइस लाइन विवरण पर मात्रा में कोई परिवर्तन नहीं हुआ है। | लागू नहीं | <p>पुरानी बिल न की गई वास्तविक बिक्री की इनवॉइस स्थिति अद्यतन की जाती है।</p><p>रिवर्सल बिल न किए गए वास्तविक बिक्री वास्तविक बनाए जाते हैं जिनकी समायोजन स्थिति होती है **समायोज्य**. | एक वास्तविक बिल की गई बिक्री बनाई जाती है। | <p>मौजूदा वास्तविक जो अपरिवर्तित रहता है:</p><ul><li>**वास्तविक लागत:** बॉब कोज़ैक, 8 घंटे, USD 800</li></ul><p>मौजूदा वास्तविक जो अद्यतन किया गया है:</p><ul><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 8 घंटा, USD 1,600, *ग्राहक चालान पोस्ट किया गया*</li></ul>नया वास्तविक जो वित्तीय कार्य प्रगति पर है (WIP) को उलटने के लिए बनाया गया है:</p><ul><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, (8 घंटे), (1,600 अमरीकी डालर)</li></ul><p>नया वास्तविक जो बिल किए गए बिक्री मूल्यों को रिकॉर्ड करने के लिए बनाया गया है:</p><ul><li>**बिल की गई बिक्री वास्तविक:** बॉब कोज़ैक, 8 घंटे, USD 1,600</li></ul> |
| इनवॉइस की पुष्टि तब की जाती है जब इनवॉइस लाइन विवरण की मात्रा बिल न की गई बिक्री की वास्तविक मात्रा से कम हो जाती है। | लागू नहीं | <p>वास्तविक बिल न की गई वास्तविक बिक्री की समायोजन स्थिति को अपडेट किया जाता है **समायोजित**.</p><p>बिल न किए गए वास्तविक बिक्री वास्तविक उलट वास्तविक बिल न किए गए वास्तविक बिक्री के लिए बनाए जाते हैं। उनके पास समायोजन की स्थिति है **समायोज्य**.</p><p>दो नए बिल न किए गए वास्तविक विक्रय बनाए गए हैं:</p><ul><li>बिल करने योग्य घंटों के लिए वास्तविक बिल न की गई बिक्री प्रभार्य</li><li>शेष मात्रा के लिए वास्तविक गैर-प्रभार्य बिल न की गई बिक्री</li></ul><p>दो नए बिल न किए गए वास्तविक बिक्री के लिए रिवर्सल बिल न किए गए वास्तविक वास्तविक बनाए जाते हैं।</p> | <p>दो वास्तविक बिक्री बिल बनाए गए हैं:</p><ul><li>बिल करने योग्य बिल की बिक्री बिल करने योग्य घंटों के लिए वास्तविक है</li><li>शेष मात्रा के लिए वास्तविक गैर-प्रभार्य बिल बिक्री</li></ul> | <p>मौजूदा वास्तविक जो अपरिवर्तित रहता है:</p><ul><li>**वास्तविक लागत:** बॉब कोज़ैक, 8 घंटे, USD 800</li></ul><p>मौजूदा वास्तविक जो अद्यतन किया गया है:</p><ul><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 8 घंटा, USD 1,600, *समायोजित*</li></ul><p>नया वास्तविक जो पिछले वित्तीय WIP को उलटने के लिए बनाया गया है:</p><ul><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, (8 घंटा), (1,600 अमरीकी डालर), *समायोज्य*</li></ul><p>नए वास्तविक जो अद्यतन बिक्री WIP को रिकॉर्ड करने के लिए बनाए गए हैं:</p><ul><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 6 घंटे, USD 2,000, *प्रभार्य*</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 2 घंटा, USD 400, *गैर प्रभार्य*</li></ul><p>नए वास्तविक जो अद्यतन बिक्री WIP को उलटने के लिए बनाए गए हैं:</p><ul><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, (6 घंटा), (USD 1,200), *प्रभार्य*</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, (2 घंटा), (USD 400), *गैर प्रभार्य*</li></ul><p>नए वास्तविक जो बिल किए गए बिक्री मूल्यों को रिकॉर्ड करने के लिए बनाए गए हैं:</p><ul><li>**बिल की गई बिक्री वास्तविक:** बॉब कोज़ैक, 6 घंटे, USD 1,200, *प्रभार्य*</li><li>**बिल की गई बिक्री वास्तविक:** बॉब कोज़ैक, 2 घंटा, USD 400, *गैर प्रभार्य*</li></ul> |
| इनवॉइस की पुष्टि की जाती है जब इनवॉइस लाइन विवरण पर मात्रा को अनबिल की गई बिक्री की वास्तविक मात्रा से बढ़ा दिया जाता है। | लागू नहीं | <p>वास्तविक बिल न की गई वास्तविक बिक्री की समायोजन स्थिति को अपडेट किया जाता है **समायोजित**.</p><p>बिल न किए गए वास्तविक बिक्री वास्तविक उलट वास्तविक बिल न किए गए वास्तविक बिक्री के लिए बनाए जाते हैं। उनके पास समायोजन की स्थिति है **समायोज्य**.</p><p>नई मात्रा के लिए बिल न किए गए वास्तविक बिक्री वास्तविक बनाए जाते हैं।</p><p>बिल न किए गए वास्तविक बिक्री वास्तविक नए बिल न किए गए वास्तविक बिक्री के लिए बनाए जाते हैं।</p> | बिल की गई वास्तविक बिक्री नई मात्रा के लिए बनाई जाती है। | <p>मौजूदा वास्तविक जो अपरिवर्तित रहता है:</p><ul><li>**वास्तविक लागत:** बॉब कोज़ैक, 8 घंटे, USD 800</li></ul><p>मौजूदा वास्तविक जो अद्यतन किया गया है:</p><ul><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 8 घंटा, USD 1,600, *समायोजित*</li></ul><p>नया वास्तविक जो पिछले वित्तीय WIP को उलटने के लिए बनाया गया है:</p><ul><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, (8 घंटा), (1,600 अमरीकी डालर), *समायोज्य*</li></ul><p>नया वास्तविक जो अद्यतन बिक्री WIP रिकॉर्ड करने के लिए बनाया गया है:</p><ul><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 10 घंटा, USD 2,000, *प्रभार्य*</li></ul><p>नया वास्तविक जो अद्यतन बिक्री WIP को उलटने के लिए बनाया गया है:</p><ul><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, (10 घंटा), (USD 2,000), *प्रभार्य*, *ायोज्य*</li></ul><p>नया वास्तविक जो बिल किए गए बिक्री मूल्यों को रिकॉर्ड करने के लिए बनाया गया है:</p><ul><li>**बिल की गई बिक्री वास्तविक:** बॉब कोज़ैक, 10 घंटा, USD 1,200z, *प्रभार्य*</li></ul> |
| प्रभार्य मात्रा या कीमत को कम करने के लिए चालान को सही किया जाता है। | लागू नहीं | <p>दो बिल न किए गए वास्तविक विक्रय बनाए जाते हैं:</p><ul><li>सुधारात्मक इनवॉइस पर मात्रा के लिए वास्तविक प्रभार्य बिल न की गई बिक्री</li><li>शेष मात्रा के लिए प्रभार्य बिना बिल की बिक्री वास्तविक</li></ul><p>दो नए बिल न किए गए वास्तविक बिक्री के लिए रिवर्सल बिल न किए गए वास्तविक वास्तविक बनाए जाते हैं।</p> | <p>रिवर्सल बिल बिक्री वास्तविक बनाए जाते हैं।</p><p>नई मात्रा के लिए नए बिल किए गए बिक्री वास्तविक बनाए जाते हैं। | <p>मौजूदा वास्तविक जो अपरिवर्तित रहते हैं:</p><ul><li>**वास्तविक लागत:** बॉब कोज़ैक, 8 घंटे, USD 800</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 8 घंटा, USD 1,600, *ग्राहक चालान पोस्ट किया गया*</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, (8 घंटे), (1,600 अमरीकी डालर)</li></ul><p>मौजूदा वास्तविक जो अद्यतन किया गया है:</p><ul><li>**बिल की गई बिक्री वास्तविक:** बॉब कोज़ैक, (8 घंटे), (1,600 अमरीकी डालर) *समायोजित*</li></ul><p>नया वास्तविक जो पिछले बिल किए गए बिक्री मूल्यों को उलटने के लिए बनाया गया है:</p><ul><li>**बिल की गई बिक्री वास्तविक:** बॉब कोज़ैक, (8 घंटे), (1,600 अमरीकी डालर) *समायोज्य*</li></ul><p>सही बिक्री WIP रिकॉर्ड करने के लिए बनाए गए नए वास्तविक:</p><ul><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 6 घंटा, USD 1,200, *प्रभार्य*, *ाहक चालान पोस्ट किया गया*</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 2 घंटा, USD 400, *प्रभार्य*</li></ul><p>नया वास्तविक जो सही बिक्री WIP को उलटने के लिए बनाया गया है:</p><ul><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, (6 घंटा), (USD 1,200), *प्रभार्य*, *ायोज्य*</li></ul><p>नया वास्तविक जो सही बिल किए गए बिक्री मूल्यों को रिकॉर्ड करने के लिए बनाया गया है:</p><ul><li>**बिल की गई बिक्री वास्तविक:** बॉब कोज़ैक, 6 घंटे, USD 1,200, *प्रभार्य*</li></ul> |
| प्रभार्य मात्रा या कीमत बढ़ाने के लिए चालान को सही किया जाता है। | लागू नहीं | <p>नए बिल न किए गए वास्तविक बिक्री वास्तविक नई मात्रा के लिए बनाए जाते हैं।</p> <p>बिल न किए गए वास्तविक बिक्री वास्तविक नए बिल न किए गए वास्तविक बिक्री के लिए बनाए जाते हैं।</p> | <p>रिवर्सल बिल बिक्री वास्तविक बनाए जाते हैं।</p>नई मात्रा के लिए नए बिल किए गए बिक्री वास्तविक बनाए जाते हैं।</p> | <p>मौजूदा वास्तविक जो अपरिवर्तित रहते हैं:</p><ul><li>**वास्तविक लागत:** बॉब कोज़ैक, 8 घंटे, USD 800</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 8 घंटा, USD 1,600, *ग्राहक चालान पोस्ट किया गया*</li><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, (8 घंटे), (1,600 अमरीकी डालर)</li></ul><p>मौजूदा वास्तविक जो अद्यतन किया गया है:</p><ul><li>**बिल की गई बिक्री वास्तविक:** बॉब कोज़ैक, (8 घंटे), (1,600 अमरीकी डालर) *समायोजित*</li></ul><p>नया वास्तविक जो पिछले बिल किए गए बिक्री मूल्यों को उलटने के लिए बनाया गया है:</p><ul><li>**बिल की गई बिक्री वास्तविक:** बॉब कोज़ैक, (8 घंटे), (1,600 अमरीकी डालर) *समायोज्य*</li></ul><p>नया वास्तविक जो सही बिक्री WIP रिकॉर्ड करने के लिए बनाया गया है:</p><ul><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, 10 घंटा, USD 2,000, *प्रभार्य*, *ाहक चालान पोस्ट किया गया*</li></ul><p>नया वास्तविक जो सही बिक्री WIP को उलटने के लिए बनाया गया है:</p><ul><li>**बिल न की गई बिक्री वास्तविक:** बॉब कोज़ैक, (10 घंटा), (USD 2,000), *प्रभार्य*</li></ul><p>नया वास्तविक जो सही बिल किए गए बिक्री मूल्यों को रिकॉर्ड करने के लिए बनाया गया है:</p><ul><li>**बिल की गई बिक्री वास्तविक:** बॉब कोज़ैक, 10 घंटा, USD 1,200z, *प्रभार्य*</li></ul> |

[!INCLUDE[footer-include](../includes/footer-banner.md)]