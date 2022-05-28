---
title: संगठनात्मक इकाइयाँ
description: यह विषय संगठनात्मक इकाइयों की अवधारणा का वर्णन करता है, और बताता है कि Microsoft में संगठनात्मक इकाइयों को कैसे बनाया और बनाए रखा जाए।Dynamics 365 Project Operations
author: rumant
ms.date: 1/31/2022
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: 9a8c503dc6286f40c80ed9b7a8a04974ff7e50b4
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/14/2022
ms.locfileid: "8581378"
---
# <a name="organizational-units-overview"></a>संगठनात्मक इकाइयाँ सिंहावलोकन

माइक्रोसॉफ्ट में Dynamics 365 Project Operations, एक *संगठित इकाई* एक पेशेवर सेवा कंपनी में एक विशिष्ट समूह या प्रभाग है जो लागत दरों वाले बिल योग्य संसाधनों को नियोजित करता है।

पेशेवर सेवा कंपनियों के लिए जो विभिन्न अभ्यास क्षेत्रों या व्यावसायिक लाइनों में तकनीकी संसाधनों को नियोजित करती हैं, भूमिका भरने की लागत भिन्न हो सकती है, यह अभ्यास क्षेत्र या व्यवसाय लाइन पर निर्भर करता है जहां भूमिका भरी जाती है। इस परिदृश्य में, संगठनात्मक इकाइयों की अवधारणा एक कंपनी के एक डिवीजन में बिल योग्य भूमिकाओं के एक समूह को समूहित करने का एक तरीका प्रदान करने में मदद करती है, जिसमें उन भूमिकाओं के लिए एक अलग लागत संरचना होती है।

## <a name="the-concept-of-organizational-units-in-project-operations"></a>परियोजना संचालन में संगठनात्मक इकाइयों की अवधारणा

प्रोजेक्ट ऑपरेशंस में, एक संगठनात्मक इकाई में एक विशिष्ट मुद्रा और विशिष्ट लागत मूल्य सूचियां होती हैं।

एक संगठनात्मक इकाई की मुद्रा प्राथमिक मुद्रा है जिसका उपयोग लागतों पर नजर रखने के लिए किया जाता है।

प्रत्येक संगठनात्मक इकाई में एक या अधिक लागत मूल्य सूचियां जोड़ी जा सकती हैं। प्रोजेक्ट ऑपरेशंस निम्नलिखित सीमाएँ मूल्य सूचियों पर रखता है जिन्हें एक संगठनात्मक इकाई से जोड़ा जा सकता है:

- मूल्य सूचियां संगठनात्मक इकाई की मुद्रा में होनी चाहिए.
- मूल्य सूचियाँ लागत मूल्य सूचियाँ होनी चाहिए।

इसके अतिरिक्त, संसाधन निकाय में संगठनात्मक इकाई के लिए एक विशेषता शामिल होती है। प्रत्येक संसाधन को एक संगठनात्मक इकाई को सौंपा जा सकता है।

### <a name="roles-of-organizational-units"></a>संगठनात्मक इकाइयों की भूमिका

संगठनात्मक इकाई परियोजना संचालन में दो भूमिकाएँ निभाती है:

- **अनुबंध इकाई** - संगठनात्मक इकाई जो कंपनी समूह या उस डिवीजन का प्रतिनिधित्व करती है जो जो मुख्य रूप से बिक्री को पाने और ग्राहक को काम और सेवाओं की डिलीवरी का प्रबंधन करने के लिए जिम्मेदार है। अनुबंध करने वाली इकाई की पहचान **अवसर**, **कोट**, **प्रोजेक्ट अनुबंध** और **प्रोजेक्ट** पेज के हेडर अनुभाग में **कॉन्ट्रैक्टिंग यूनिट** फ़ील्ड द्वारा की जाती है।
- **रिसोर्सिंग यूनिट** - वह संगठनात्मक इकाई जो किसी संसाधन से संबंधित होती है या उसे सौंपी जाती है। यह संगठनात्मक इकाई काम के विवरण (SOW) और अनुबंध इकाई के स्वामित्व वाले प्रोजेक्टों पर कुछ भूमिकाओं के लिए अपने संसाधन प्रदान कर सकती है।

![कॉन्ट्रैक्टिंग इकाइयां और रिसोर्सिंग इकाइयां.](media/OrgUnits.png)

### <a name="organizational-unit-faq"></a>संगठनात्मक इकाई अक्सर पूछे जाने वाले प्रश्न

संगठनात्मक इकाइयों के बारे में अक्सर पूछे जाने वाले कुछ प्रश्न यहां दिए गए हैं।

#### <a name="how-is-the-organizational-unit-entity-in-project-operations-related-to-the-organization-entity-that-already-exists-in-dynamics-365"></a>प्रोजेक्ट ऑपरेशंस में संगठनात्मक इकाई इकाई संगठन इकाई से कैसे संबंधित है जो पहले से ही Dynamics 365 में मौजूद है?

Dynamics 365 में संगठन निकाय एक वैश्विक Dynamics 365 इंस्टेंस के नाम का प्रतिनिधित्व करता है। यह नाम आमतौर पर वैश्विक उद्यम का नाम है।

संगठनात्मक यूनिट इकाई वैश्विक उद्यम में एक समूह या डिवीजन का प्रतिनिधित्व करती है। इस समूह या डिवीजन में भूमिकाओं का एक समूह है और उन भूमिकाओं के लिए एक मूल्य सूची है और वे भूमिकाएं और मूल्य सूची उद्यम में अन्य समूहों या डिवीजनों की भूमिकाओं और मूल्य सूची से अलग हैं।

जब प्रोजेक्ट संचालन स्थापित होता है, तो संगठन के आधार पर एक डिफ़ॉल्ट संगठनात्मक इकाई बनाई जाती है। सभी मौजूदा संसाधनों को डिफ़ॉल्ट संगठनात्मक इकाई को सौंपा गया है। यदि कोई नया सक्रिय निर्देशिका उपयोगकर्ता या संसाधन Dynamics 365 में आयात किया जाता है, तो उपयोगकर्ता आयात प्रक्रिया उन्हें प्रोजेक्ट संचालन में डिफ़ॉल्ट संगठनात्मक इकाई को असाइन करती है।

#### <a name="how-does-the-organizational-unit-entity-differ-from-the-business-unit-entity"></a>संगठनात्मक इकाई इकाई व्यावसायिक इकाई इकाई से कैसे भिन्न है?

Dynamics 365 में, व्यावसायिक यूनिट इकाई एक सुरक्षा निर्माण है। व्यावसायिक यूनिट के साथ एक उपयोगकर्ता का सहयोग उन इकाइयों और इकाई रिकॉर्डों को निर्धारित करता है जो उपयोगकर्ता के पास हैं। यह उन अनुमतियों को भी निर्धारित करता है (बनाएं, पढ़ें, लिखें, हटाएं, जोड़ें, में जोडें, असाइन, या शेयर) जो उपयोगकर्ता के पास उन इकाई रिकॉर्डों के लिए हैं।

संगठनात्मक यूनिट इकाई एक कंपनी समूह या डिवीजन का प्रतिनिधित्व करती है जिसमें कर्मचारियों के लिए अलग-अलग लागत दरें होती हैं जो इसे सौंपी जाती हैं। एक संगठनात्मक इकाई वाले संसाधन का सहयोग प्रोजेक्ट के काम के लिए संसाधन की लागत निर्धारित करता है।

जब आप Dynamics 365 को कार्यान्वित करते हैं, तो व्यावसायिक इकाइयों के पदानुक्रम और व्यावसायिक इकाइयों के लिए उपयोगकर्ताओं के असाइनमेंट के लिए सुरक्षा प्राधिकरण का अनुकूलन करें। उन सभी उपयोगकर्ताओं को असाइन करें जिन्हें आम तौर पर उसी व्यावसायिक इकाई में रिकॉर्ड के समान सेट का उपयोग करना चाहिए। संगठनात्मक इकाई का सुरक्षा प्राधिकरण या पहुंच पर कोई प्रभाव नहीं है।

**उदाहरण जो संगठनात्मक इकाइयों और व्यावसायिक इकाइयों के मॉडलिंग में एक संभावित अंतर दिखाता है**

रैना, Ltd. के पास एक संपन्न Microsoft प्रौद्योगिकी अभ्यास है। दमयंती और दर्शन दोनों C\# डेवलपर्स हैं, लेकिन ट्रिसिया संयुक्त राज्य अमेरिका में है, जबकि दर्शन भारत में है। अधिकांश परियोजना कार्यों में Contoso India और Contoso US दोनों के संसाधनों की आवश्यकता होती है, और प्रकाश और ट्रिसिया को इस अभ्यास क्षेत्र में परियोजनाओं के लिए समान स्तर की सुरक्षा पहुंच की आवश्यकता होती है। हालांकि, रैना इंडिया के डेवलपर्स की लागत रैना यूएस के डेवलपर्स की लागत से काफी भिन्न है।

यहाँ Dynamics 365 और Project Operations का उपयोग करके इस परिदृश्य के लिए डिज़ाइन करने का एक इष्टतम तरीका दिया गया है।

1. Microsoft प्रौद्योगिकी अभ्यास को एक व्यावसायिक इकाई के रूप में बनाएँ, और इसके साथ दर्शन और दमयंती को संबद्ध करें। इस तरह, आप यह सुनिश्चित करने में मदद करते हैं कि दोनों कर्मचारियों के पास उस अभ्यास क्षेत्र में किसी भी परियोजना के लिए समान स्तर की सुरक्षा पहुंच है। वे दोनों प्रगति की जांच करने और समय, व्यय, सामग्री उपयोग और कार्य अपडेट की रिपोर्ट करने में सक्षम होंगे।
2. यह सुनिश्चित करने में सहायता के लिए दो संगठनात्मक इकाइयाँ बनाएँ कि परियोजना की लागत सही ढंग से परिलक्षित होती है।
3. ट्रिसिया को Contoso US से और प्रकाश को Contoso India से संबद्ध करें।
4. दोनों संगठनात्मक इकाई को उचित लागत मूल्य सूचियाँ सौंपें। इस तरह, आप यह सुनिश्चित करने में मदद करते हैं कि प्रकाश और ट्रिसिया के लिए परियोजना पर दर्ज की गई लागतें Contoso US और Contoso India के बीच लागत के अंतर को सटीक रूप से दर्शाती हैं।

#### <a name="are-organizational-units-related-to-sales-territories-in-dynamics-365"></a>क्या Dynamics 365 में बिक्री क्षेत्रों से संबंधित संगठनात्मक इकाइयां हैं?

बिक्री क्षेत्रों और संगठनात्मक इकाइयों के बीच कोई सहयोग या संबंध नहीं है। बिक्री क्षेत्र आमतौर पर एक भौगोलिक क्षेत्र होता है जहां बिक्री होती है। एक बिक्री मूल्य सूची प्रत्येक बिक्री क्षेत्र से जुड़ी हो सकती है।

एक संगठनात्मक इकाई कंपनी में एक आंतरिक समूह या डिवीजन है जो कि भूमिकाओं के एक सेट के लिए लागत को ट्रैक करता है जो इसे अन्य डिवीजनों या बाहरी ग्राहकों को बेचता है।

**उदाहरण जो संगठनात्मक इकाइयों और बिक्री क्षेत्रों के मॉडलिंग में एक संभावित अंतर दिखाता है**

Contoso, Ltd. के दो विकास केंद्र हैं: रैना US और रैना इंडिया। इन दो विकास केंद्रों के बीच संसाधनों की लागत काफी भिन्न होती है। Contoso लैटिन अमेरिका, उत्तरी अमेरिका, एशिया-प्रशांत, पश्चिमी यूरोप और मध्य पूर्व जैसे कई अंतरराष्ट्रीय बाजारों में अपनी सूचना प्रौद्योगिकी (आईटी) सेवाएं बेचता है। एक ही प्रोजेक्ट भूमिकाओं के लिए बिल की दरें इन बाजारों में व्यापक रूप से भिन्न हो सकती हैं। रैना यूएस और रैना इंडिया को संगठनात्मक इकाइयों के रूप में स्थापित किया जाना चाहिए, और प्रत्येक संगठनात्मक इकाई की अपनी लागत मूल्य सूची होनी चाहिए। एशिया-प्रशांत, लैटिन अमेरिका, उत्तरी अमेरिका, पश्चिमी यूरोप और मध्य पूर्व को बिक्री क्षेत्रों के रूप में स्थापित किया जाना चाहिए, और प्रत्येक बिक्री क्षेत्र की अपनी बिक्री मूल्य सूची होनी चाहिए।

#### <a name="why-is-there-a-restriction-on-the-association-of-price-lists-with-organizational-units"></a>संगठनात्मक इकाइयों के साथ मूल्य सूचियों के सहयोग पर प्रतिबंध क्यों है?

बिक्री मूल्य आमतौर पर भौगोलिक क्षेत्रों या बाजारों के लिए विशिष्ट है जहां सेवाएं बेची जाती हैं। एक कंपनी के आंतरिक डिवीजनों में आमतौर पर एक ही प्रकार की सेवाओं के लिए अपनी बिक्री मूल्य निर्धारण नहीं होता है। हालांकि, आंतरिक डिवीजनों में बेचे गए सामानों की एक अलग लागत होती है (COGS), उन लोगों के कौशल पर निर्भर करता है जो वे काम करते हैं और जिस क्षेत्र में वे काम करते हैं। क्योंकि संगठनात्मक इकाइयां किसी कंपनी के आंतरिक डिवीजनों के रूप में तैयार की जाती हैं, उनके पास केवल लागत मूल्य सूची हो सकती है।

#### <a name="why-cant-we-associate-sales-price-lists-with-organizational-units"></a>हम बिक्री मूल्य सूचियों को संगठनात्मक इकाइयों से संबद्ध क्यों नहीं कर सकते?

प्रोजेक्ट ऑपरेशंस में, बिक्री मूल्य सूचियों को ग्राहकों और बिक्री क्षेत्रों से जोड़ा जा सकता है। अवसर, कोट, परियोजना अनुबंध, और परियोजना जैसी लेन-देन वाली संस्थाएं बिक्री मूल्य सूचियों का उपयोग करती हैं जो परियोजना के जुड़ाव के लिए बिल दरों और संभावित राजस्व का निर्धारण करने के लिए ग्राहक खाते या बिक्री क्षेत्र से जुड़ी होती हैं।

लागत मूल्य सूची संगठनात्मक इकाइयों के साथ जुड़ी हुई हैं। अवसर, भाव, परियोजना अनुबंध, और परियोजना जैसी लेन-देन वाली इकाइयां लागत मूल्य सूचियों का उपयोग करती हैं जो एक परियोजना जुड़ाव के लिए लागत निर्धारित करने के लिए अनुबंध इकाई से जुड़ी होती हैं।

#### <a name="are-organizational-units-hierarchical-in-project-operations"></a>क्या संगठनात्मक इकाइयाँ पदानुक्रमित परियोजना संचालन में हैं?

नहीं. प्रोजेक्ट ऑपरेशंस की वर्तमान रिलीज़ में, संगठनात्मक इकाइयाँ पदानुक्रमित नहीं हैं। इसलिए, आप निम्न कार्य नहीं कर सकते:

- डिफ़ॉल्ट लागत मूल्य दर्ज करने के लिए एक पैटर्न कॉन्फ़िगर करें जो एक पदानुक्रम को पार करता है।
- रिपोर्ट आय या लागत जो संगठनात्मक इकाई पदानुक्रम के विभिन्न स्तरों पर लुढ़की है।

#### <a name="were-a-big-multinational-firm-that-has-a-complex-multilevel-hierarchy-of-cost-centers-divisions-and-billing-offices-how-can-we-best-use-the-concept-of-organizational-units-in-the-current-version-of-project-operations"></a>हम एक बड़ी बहुराष्ट्रीय फर्म हैं जिसके पास लागत केंद्रों, डिवीजनों और बिलिंग कार्यालयों का एक जटिल, बहुस्तरीय पदानुक्रम है। हम परियोजना संचालन के वर्तमान संस्करण में संगठनात्मक इकाइयों की अवधारणा का सर्वोत्तम उपयोग कैसे कर सकते हैं?

जब आपके पास लागत केंद्रों, डिवीजनों, बिलिंग कार्यालयों आदि का एक जटिल पदानुक्रम हो, तो उस पदानुक्रम के लीफ नोड्स को विशिष्ट संगठनात्मक इकाइयों के रूप में सेट करें।

निम्न उदाहरण एक विशिष्ट पदानुक्रम दिखाता है।

**रैना इंडिया**

- SAP अभ्यास

    - तकनीकी सलाहकार
    - कार्यात्मक सलाहकार

- Microsoft प्रौद्योगिकी अभ्यास

    - तकनीकी सलाहकार
    - कार्यात्मक सलाहकार

**रैना US**

- SAP अभ्यास

    - तकनीकी सलाहकार
    - कार्यात्मक सलाहकार

- Microsoft प्रौद्योगिकी अभ्यास

    - तकनीकी सलाहकार
    - कार्यात्मक सलाहकार

यदि आपका पदानुक्रम इस उदाहरण से मिलता-जुलता है, तो आपको इसे एक समतल सूची के रूप में सेट करना होगा, जैसा कि यहाँ दिखाया गया है:

- रैना इंडिया - SAP अभ्यास - तकनीकी सलाहकार
- रैना इंडिया - SAP अभ्यास - कार्यात्मक सलाहकार
- रैना इंडिया - Microsoft टेक्नोलॉजी प्रैक्टिकल कार्यात्मक सलाहकार
- रैना इंडिया - Microsoft टेक्नोलॉजी प्रैक्टिकल कार्यात्मक सलाहकार
- रैना यूएस - SAP अभ्यास - तकनीकी सलाहकार
- रैना यूएस - SAP अभ्यास - कार्यात्मक सलाहकार
- रैना यूएस - Microsoft टेक्नोलॉजी अभ्यास - तकनीकी सलाहकार
- रैना यूएस - Microsoft टेक्नोलॉजी अभ्यास - कार्यात्मक सलाहकार

#### <a name="were-a-small-professional-services-company-that-operates-as-only-one-division-how-can-we-best-use-the-concept-of-organizational-units-in-the-current-version-of-project-operations"></a>हम एक छोटी पेशेवर सेवा कंपनी हैं जो केवल एक डिवीजन के रूप में काम करती है। हम परियोजना संचालन के वर्तमान संस्करण में संगठनात्मक इकाइयों की अवधारणा का सर्वोत्तम उपयोग कैसे कर सकते हैं?

यदि आपकी कंपनी एक इकाई के रूप में काम करती है, जिसमें एक मूल्य मूल्य सूची है, तो आपको कोई संगठनात्मक इकाई स्थापित करने की आवश्यकता नहीं है। प्रोजेक्ट ऑपरेशंस की स्थापना एक डिफ़ॉल्ट संगठनात्मक इकाई बनाती है जिसका नाम संगठन के समान होता है। डिफ़ॉल्ट रूप से, सभी उपयोगकर्ताओं को इस संगठनात्मक इकाई को सौंपा गया है। जब भी सिस्टम को आवश्यकता होती है कि एक संगठनात्मक इकाई का चयन किया जाना है, तो यह संगठनात्मक इकाई डिफ़ॉल्ट रूप से चुनी जाती है।

#### <a name="when-a-project-is-created-from-a-quote-or-project-contract-line-the-default-contracting-unit-comes-from-the-quote-or-project-contract-what-is-the-default-contracting-unit-if-a-project-is-created-before-sales-entities-such-as-quote-or-project-contract"></a>जब कोई प्रोजेक्ट किसी कोटेशन या प्रोजेक्ट अनुबंध लाइन से बनाई जाती है, तो डिफ़ॉल्ट अनुबंध इकाई कोटेशन या प्रोजेक्ट अनुबंध से आती है। यदि कोई प्रोजेक्ट बिक्री संस्थाओं जैसे कोट या प्रोजेक्ट कॉन्ट्रैक्ट से पहले बनाया जाता है, तो डिफ़ॉल्ट अनुबंध इकाई क्या है?

जब कोई प्रोजेक्ट स्वयं बनाया जाता है, तो प्रोजेक्ट की डिफ़ॉल्ट अनुबंध इकाई उस उपयोगकर्ता पर आधारित होती है जो इसे बनाता है। वह उपयोगकर्ता डिफ़ॉल्ट प्रोजेक्ट मैनेजर भी है। यदि परियोजना को एक बिक्री इकाई जैसे कि उद्धरण या परियोजना अनुबंध के लिए मैप किया जाता है, तो परियोजना की अनुबंध इकाई इसके बजाय बिक्री इकाई पर आधारित होती है। इस मामले में, यदि अनुबंध इकाई को बदल दिया जाता है तो प्रोजेक्ट के अनुमानों की पुनर्गणना की जा सकती है, क्योंकि लागत मूल्य सूची का उपयोग लागत अनुमान परिवर्तनों की गणना करने के लिए किया जाता है। बिक्री मूल्य सूची का उपयोग उन बिक्री अनुमानों की गणना करने के लिए किया जाता है जिन्हें बदला जाएगा ताकि वे उद्धरण की परियोजना मूल्य सूची के साथ समन्वयित हों।

**अनुबंध इकाई** और **मुद्रा** परियोजना के क्षेत्रों को संपादन के लिए बंद कर दिया गया है, क्योंकि वे बिक्री इकाई (उद्धरण या परियोजना अनुबंध) के मूल्यों के साथ समन्वयित होना चाहिए जिससे परियोजना को मैप किया गया है।

## <a name="create-and-maintain-organizational-units-in-project-operations"></a>प्रोजेक्ट ऑपरेशंस में संगठनात्मक इकाइयां बनाएं और बनाए रखें

प्रोजेक्ट ऑपरेशंस में एक संगठनात्मक इकाई बनाने के लिए, इन चरणों का पालन करें।

1. के लिए जाओ **समायोजन \> संगठनात्मक इकाइयाँ**.
2. **नया** चुनें.
3. में **आम** क्षेत्र, में **नाम** फ़ील्ड, संगठनात्मक इकाई के लिए एक नाम दर्ज करें। फिर अन्य फ़ील्ड को आवश्यकतानुसार सेट करें।
4. चुनना**बचाना** रिकॉर्ड बनाने के लिए ताकि आप इसे संपादित करना जारी रख सकें।
5. नीचे **लागत मूल्य सूचियाँ**, प्लस चिह्न चुनें (**+**) मूल्य सूची जोड़ने के लिए। आप केवल वही मूल्य सूचियां जोड़ सकते हैं जिनमें **कीमत** संदर्भ यहाँ।
6. में **नाम** फ़ील्ड, चुनें **खोज** बटन पर क्लिक करें और उस मूल्य सूची का चयन करें जिसे आप संगठनात्मक इकाई को उपलब्ध कराना चाहते हैं। आवश्यकतानुसार मूल्य सूची जोड़ना जारी रखें।
7. जब आप मूल्य सूचियां जोड़ना समाप्त कर लें, तो चुनें **बचाना** पृष्ठ के निचले-दाएँ कोने में।

[!INCLUDE[footer-include](../includes/footer-banner.md)]