---
title: व्यय प्रबंधन में वैट की वसूली
description: यह विषय बताता है कि योग्य मूल्य वर्धित कर (वैट) लेन-देन पर धनवापसी कैसे प्राप्त करें.
author: suvaidya
manager: AnnBe
ms.date: 10/10/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: 2c20e4a7fa9748e03bf1729fc2f7bdbfc2f292d1
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/01/2020
ms.locfileid: "3908210"
---
# <a name="vat-recovery-in-expense-management"></a>व्यय प्रबंधन में वैट की वसूली

_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_

योग्य मूल्य वर्धित कर (वैट) लेन-देन पर धनवापसी पाने के लिए, कंपनी या संगठन को सटीक जानकारी को पहचानना, संग्रह, सत्यापन और सबमिट करना होगा. इस प्रक्रिया में कई कार्य शामिल हैं और आपकी कंपनी के आकार के आधार पर, इसमें कई कर्मचारी या भूमिकाएं शामिल हो सकती हैं।

**व्यय प्रबंधन** मॉड्यूल में वैट की धनवापसी के लिए, निम्नलिखित पूर्वापेक्षाएं पूरी की जानी चाहिएं:

- टैक्स कोड उन देशों/क्षेत्रों के लिए बनाए जाने चाहिए जिन्हें व्यय श्रेणियों को आवंटित किया गया है।
- प्रत्येक टैक्स कोड के लिए एक बिक्री कर समूह बनाया जाना चाहिए।
- प्रत्येक बिक्री कर समूह के लिए एक आइटम बिक्री टैक्स कोड बनाया जाना चाहिए।

पूर्वापेक्षाएं पूरी होने के बाद, वैट लेन-देन के लिए धनवापसी का अनुरोध करने के लिए निम्न चरणों को पूरा किया जाना चाहिए।

1. व्यय रिपोर्ट पर, योग्य VAT धनवापसी की पहचान करने के लिए क्रेडिट कार्ड लेन-देन के बारे में कर जानकारी दर्ज करें।
2. सत्यापित करें कि सभी कर जानकारी पूर्ण हैं, और फिर व्यय रिपोर्ट पोस्ट करें।
3. प्रोसेस व्यय, जो अंतरराष्ट्रीय VAT वसूली के योग्य हैं.
4. अंतरराष्ट्रीय वसूली रिर्टन दाखिल करने के लिए तीसरे पक्ष के विक्रेता को वैट वसूली डेटा भेजें.
5. घरेलू VAT वसूली के लिए प्रोसेस के व्यय.

निम्नलिखित अनुभाग ऐसे उदाहरण प्रदान करते हैं, जो दिखाते हैं कि Contoso कर्मचारी प्रत्येक चरण को कैसे पूरा करते हैं।

## <a name="enter-tax-information-about-credit-card-transactions-to-identify-eligible-vat-refunds"></a>योग्य वैट धनवापसी की पहचान करने के लिए क्रेडिट कार्ड लेन-देन के बारे में कर जानकारी दर्ज करें

Contoso की बिक्री प्रतिनिधि नैन्सी संयुक्त राज्य अमेरिका में रहती है, हाल ही में यूनाइटेड किंगडम की बिक्री यात्रा से लौटी है. यात्रा के दौरान, नैन्सी ने भोजन के लिए व्यक्तिगत क्रेडिट कार्ड से कुछ खर्चे किए। खर्चों को मिलाने के लिए नैन्सी को अब एक व्यय रिपोर्ट बनानी होगी।

जब नैन्सी व्यय रिपोर्ट पर जानकारी दर्ज करती है, तो वह **व्यय रिपोर्ट संपादित करें** पृष्ठ पर **देश/क्षेत्र** फ़ील्ड में **यूनाइटेड किंगडम** चुनती है. तब बिक्री कर समूहों की सूची को फ़िल्टर किया जाता है, ताकि यह केवल उन समूहों को दिखाए जो यूनाइटेड किंगडम पर लागू होते हैं. नैन्सी **यूनाइटेड किंगडम 001** बिक्री कर समूह चुनती है और फिर **भोजन** आइटम बिक्री कर समूह चुनती है. इसके बाद, नैन्सी ने ठहरने के लिए एक नया लेन-देन जोड़ा। क्योंकि यूनाइटेड किंगडम में ठहरने के लिए केवल एक बिक्री कर समूह और एक आइटम बिक्री कर समूह है, यह जानकारी नैन्सी की व्यय रिपोर्ट में अपने आप भर जाती है.

Contoso की नीति के अनुसार, सभी खर्चों की एक मिलान रसीद होनी चाहिए। इसलिए, जब नैन्सी व्यय रिपोर्ट को सहेजती है, तो उसे एक संदेश मिलता है जिसमें कहा गया है कि उसे प्रत्येक उस लेन-देन के लिए एक रसीद संलग्न करनी होगी, जिसे उसने अपनी व्यय रिपोर्ट में सूचीबद्ध किया है. नैन्सी पुष्टि करती है कि उसने प्रत्येक लेन-देन रसीद की एक डिजिटल तस्वीर अपनी व्यय रिपोर्ट में संलग्न की है और फिर स्वीकृति के लिए अपनी रिपोर्ट सबमिट करती है। इसके बाद वह कागजी रसीदों को बैक-ऑफिस प्रोसेसिंग टीम को भेजती है। यह टीम वैट वसूली डेटा को तीसरे- पक्ष के विक्रेता को भेज देगी जो Contoso के लिए अंतरराष्ट्रीय वैट वसूली रिर्टन को फ़ाइल करता है.

## <a name="verify-tax-information-and-post-an-expense-report"></a>कर जानकारी सत्यापित करें और व्यय रिपोर्ट पोस्ट करें

Contoso के लिए देय खातों की समन्वयक अप्रैल द्वारा व्यय रिपोर्ट को पोस्ट करने से पहले उसे किसी भी कर जानकारी को दर्ज करना होगा जो उसमें नहीं है. वह **व्यय रिपोर्ट विवरण** पृष्ठ खोलती है और नैंसी की स्वीकृत व्यय रिपोर्ट देखती है। अप्रैल तब लेन-देन का विवरण देखने के लिए व्यय रिपोर्ट खोलती है। वह देखती है कि नैन्सी ने लेन-देन में से एक के लिए एक आइटम बिक्री कर समूह को दर्ज नहीं किया है. क्योंकि यह जानकारी प्रदान नहीं की गई है, अप्रैल व्यय रिपोर्ट पोस्ट नहीं कर सकती है। इसलिए, वह व्यय प्रबंधन में **कर कॉन्फ़िगरेशन** पृष्ठ पर देखती है, और देश/क्षेत्र और लेन-देन प्रकार के लिए उपयुक्त आइटम बिक्री कर समूह पाती है। अप्रैल अब व्यय रिपोर्ट को सामान्य खाता बही में पोस्ट कर सकती है।

जब अप्रैल व्यय रिपोर्ट पोस्ट करती है, तो वैट धनवापसी योग्य कार्य आइटम बनाया जाता है। यह कार्य आइटम बैक-ऑफ़िस प्रोसेसिंग टीम के एक सदस्य को सौंपा जाता है। अप्रैल एक संदेश प्राप्त करती है जो पुष्टि करता है कि पोस्ट करना सफल रहा। यह संदेश वैट लेन-देन की संख्या को भी सूचीबद्ध करता है जो वसूली के लिए पहचाने गए थे.

## <a name="process-expenses-that-are-eligible-for-international-vat-recovery"></a>प्रोसेस व्यय, जो अंतरराष्ट्रीय VAT वसूली के योग्य हैं

Contoso की बैक-ऑफ़िस प्रोसेसिंग टीम का सदस्य आर्नी यह सत्यापित करने के लिए जिम्मेदार है कि वैट वसूली के लिए सभी आवश्यक जानकारी व्यय रिपोर्ट में शामिल हैं. वह **व्यय कर धनवापसी** पृष्ठ खोलता है और नैन्सी द्वारा सबमिट व्यय रिपोर्ट को चुनता है। आर्नी तब पुष्टि करता है कि सभी आवश्यक रसीदें संलग्न हैं, और यह कि सही बिक्री कर समूह और आइटम बिक्री टैक्स कोड दर्ज किए गए थे।

जब आर्नी को नैन्सी से कागजी रसीदें मिलती हैं, तो वह उन्हें डिजिटल रसीदों से सत्यापित करता है और फिर व्यय रिपोर्ट की स्थिति को **धनवापसी के लिए तैयार**में बदल देता है।

## <a name="send-vat-recovery-data-to-the-third-party-vendor"></a>तीसरे-पक्ष विक्रेता को वैट वसूली डेटा भेजें

जब आर्नी तृतीय-पक्ष विक्रेता को व्यय रिपोर्ट डेटा भेजने के लिए तैयार होता है, जो वैट धनवापसी रिर्टन दाखिल करेगा, तो वह **व्यय कर धनवापसी** पृष्ठ खोलता है। वह पृष्ठ को फ़िल्टर करता है ताकि यह केवल वह व्यय रिपोर्ट दिखाता है जो **धनवापसी के लिए तैयार** के रूप में चिह्नित हैं। तब आर्नी **फ़ाइल** &gt; **Excel में निर्यात करें**को चुनता है। व्यय रिपोर्ट की वैट जानकारी Microsoft Excel वर्कशीट में निर्यात की जाती है। आर्नी इस वर्कशीट को तृतीय पक्ष के विक्रेता के पास सबमिट करता है और इसमें एक संदेश शामिल होता है, जिसमें लिखा होता है कि कागजी रसीदें कूरियर द्वारा भेजी गई हैं।

## <a name="process-expenses-for-domestic-vat-recovery"></a>घरेलू VAT वसूली के लिए प्रोसेस के व्यय

आर्नी को सत्यापित करना चाहिए कि व्यय रिपोर्ट लेन-देन वैट धनवापसी के लिए योग्य हैं, और रिपोर्ट में डिजिटल रसीदें संलग्न हैं। घरेलू धनवापसी के लिए योग्य खर्चों की प्रोसेस शुरू करने के लिए, आर्नी **व्यय कर धनवापसी** पृष्ठ खोलता है और सत्यापन के लिए आवश्यक व्यय रिपोर्ट चुनता है। वह सत्यापित करता है कि रसीदें कर्मचारी के बजाय कंपनी के नाम पर हैं। (वैट धनवापसी के लिए, रसीदें कंपनी के नाम पर होनी चाहिए।) आर्नी ने फिर पुष्टि की कि सही बिक्री कर समूह और आइटम बिक्री टैक्स कोड दर्ज किए गए थे।

जब आर्नी कागजी र‍सीदें प्राप्त करता है, तो वह व्यय रिपोर्ट की स्थिति को **धनवापसी के लिए तैयार**में बदल देता है। वह तब उचित कर प्राधिकरण के साथ रिर्टन दाखिल कर सकता है। इस मामले में, संयुक्त राज्य में उपयुक्त कर प्राधिकरण आंतरिक राजस्व सेवा (IRS) है।
