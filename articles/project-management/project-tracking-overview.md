---
title: परियोजना ट्रैकिंग अवलोकन
description: इस विषय में प्रोजेक्ट की प्रगति और लागत की खपत का पता लगाने के बारे में जानकारी दी गई है।
author: ruhercul
manager: AnnBe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: c998addbbdbbea8fe69c95f65e58a24146f394c8
ms.sourcegitcommit: 56c42d7f5995a674426a1c2a81bae897dceb391c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/01/2020
ms.locfileid: "3907365"
---
# <a name="project-tracking-overview"></a>परियोजना ट्रैकिंग अवलोकन

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

शेड्यूल के समक्ष प्रगति का पता लगाने की ज़रूरत हर उद्योग की अलग-अलग होती है। कुछ उद्योग बुनियादी स्तर पर ट्रैक करते हैं, जहां अन्य उद्योग उच्च स्तर पर ट्रैक करते हैं. इस विषय में बताया गया है कि अपने संगठन की ज़रूरतों को पूरा करने के लिए शेड्यूल कैसे किया जाता है।

## <a name="effort-tracking-view"></a>प्रयास ट्रैकिंग दृश्य

**प्रयास की ट्रैकिंग** दृश्य कार्य के नियोजित प्रयास घंटों के लिए किसी कार्य पर बिताए गए वास्तविक प्रयास घंटों की तुलना करके शेड्यूल में कार्यों की प्रगति को ट्रैक करता है. Dynamics 365 Project Operations ट्रैकिंग मेट्रिक्स की गणना करने के लिए निम्नलिखित सूत्रों का उपयोग करता है:

- **प्रगति प्रतिशत**: आज तक किया गया वास्तविक प्रयास ÷ परियोजना की पूर्वानुमानित लागत (EAC) 
- **पूरा करने की अनुमानित लागत (ETC)**: नियोजित प्रयास - आज तक किया गया वास्तविक प्रयास 
- **EAC**: शेष प्रयास + आज तक किया गया वास्तविक प्रयास 
- **प्रस्तावित प्रयास विचरण**: नियोजित प्रयास - EAC

Project Operations कार्य पर प्रयास विचरण का अनुमान दिखाता है. यदि EAC नियोजित प्रयास से अधिक है, तो कार्य को मूल रूप से नियोजित होने की तुलना में अधिक समय लेने का अनुमान है और यह निर्धारित समय से पीछे है. यदि EAC नियोजित प्रयास से कम है, तो कार्य को मूल रूप से नियोजित की तुलना में कम समय लेने का अनुमान है और यह निर्धारित समय से आगे है.

## <a name="reprojecting-effort"></a>दोबारा अनुमान लगाने के प्रयास

परियोजना प्रबंधक अक्सर किसी कार्य पर मूल अनुमानों को संशोधित करते हैं. परियोजना की चालू अवस्था के बारे में, परियोजना का दोबारा अनुमान लगाना, दृष्टिकोण को लेकर परियोजना प्रबंधक के विचार होते हैं. हालांकि, हम यह सुझाव नहीं देते हैं कि परियोजना प्रबंधक बेसलाइन नंबर बदलें. इसका कारण यह है कि परियोजना बेसलाइन परियोजना शेड्यूल और लागत अनुमान के लिए सच्चाई के स्थापित स्रोत का प्रतिनिधित्व करता है, और सभी परियोजना हितधारकों ने इस पर सहमति व्यक्त की है.

ऐसे दो तरीके हैं जिससे परियोजना प्रबंधक कार्यों के प्रयासों का दोबारा अनुमान लगा सकता है:

- टास्क पर वास्तविक शेष प्रयास के एक नए अनुमान के साथ डिफ़ॉल्ट ETC को ओवरराइड करें। 
- टास्क पर सही प्रगति के एक नए अनुमान के साथ डिफ़ॉल्ट प्रगति प्रतिशत को ओवरराइड करें।

प्रत्येक दृष्टिकोण कार्य के ETC, EAC, प्रगति प्रतिशत और किसी कार्य पर प्रस्तावित प्रयास विचरण की पुनर्गणना का कारण बनता है. EAC, ETC और सारांश कार्यों पर प्रगति प्रतिशत की भी पुनर्गणना होती है और प्रयास विचरण के एक नए प्रक्षेपण का उत्पादन करता है.

## <a name="reprojection-of-effort-on-summary-tasks"></a>सारांश कार्य पर प्रयास का दोबारा अनुमान

सारांश कार्यों या कंटेनर कार्यों के प्रयास का दोबारा अनुमान लगाया जा सकता है. इस बात से संबंध न रखते हुए कि उपयोगकर्ता शेष प्रयास या सारांशित कार्यों पर प्रगति के प्रतिशत का इस्तेमाल करते हुए दोबारा अनुमान लगाता है या नहीं, परिकलन का निम्न सेट प्रारंभ होता है:

- EAC, ETC और टास्क पर प्रगति के प्रतिशत का परिकलन किया जाता है।
- नए EAC को छोटे टास्क में उसी अनुपात में नीचे वितरित किया जाता है जिस अनुपात में टास्क में मूल EAC था।
- प्रत्येक वैयक्तिक कार्यों के नए EAC से लेकर लीफ नोड कार्यों तक का परिकलन किया जाता है. 
- लीफ नोड के नीचे प्रभावित छोटे टास्क में उनका ETC होते हैं और EAC के मूल्य के आधार पर प्रगति के प्रतिशत का दोबारा परिकलन किया जाता है। इसके कारण टास्क के प्रयास भिन्नता का नया अनुमान करना होता है। 
- समरी टास्क के EAC का रूट नोड तक दोबारा परिकलन किया जाता है।

### <a name="cost-tracking-view"></a>लागत ट्रैकिंग दृश्य 

**लागत ट्रैकिंग** व्यू टास्क पर खर्च की गई वास्तविक लागत और टास्क पर योजित लागत की तुलना करता है। 

> [!NOTE]
> यह दृश्य केवल श्रम लागत दर्शाता है और इसमें खर्च के अनुमानों की लागतें शामिल नहीं होती। Project Operations ट्रैकिंग मीट्रिक की गणना करने के लिए निम्नलिखित सूत्रों का उपयोग करता है:

- **उपभोग की गई लागत का प्रतिशत**: आज तक ख़र्च की गई वास्तविक लागत ÷ समाप्ति पर अनुमानित लागत
- **पूरा करने की लागत (CTC)**: नियोजित लागत - आज तक ख़र्च की गई वास्तविक लागत
- **EAC**: शेष लागत + आज तक ख़र्च की गई वास्तविक लागत
- **प्रस्तावित लागत विचरण**: नियोजित लागत - EAC

लागत भिन्नता का अनुमान टास्क पर दिखाया जाता है। यदि EAC योजित लागत से अधिक होता है तो टास्क के बारे में यह अनुमान लगाया जाता है कि उसकी लागत मूल रूप से योजित लागत से अधिक होगी। इसलिए, यह बजट से अधिक होगा। यदि EAC योजित लागत से कम है तो टास्क के बारे में यह अनुमान लगाया जाता है कि उसकी लागत मूल रूप से योजित लागत से कम होगी। इसलिए, यह बजट से कम होगा।

## <a name="project-managers-reprojection-of-cost"></a>परियोजना प्रबंधक द्वारा लागत का दोबारा अनुमान लगाना

जब प्रयास का दोबारा अनुमान लगाया जाता है, तो CTC, EAC, उपभोग की गई लागत के प्रतिशत और अनुमानित लागत भिन्नता सभी का **लागत ट्रैकिंग** दृश्य में दोबारा परिकलन किया जाता है.

## <a name="project-status-summary"></a>प्रोजेक्ट स्थिति सारांश

**प्रयास ट्रैकिंग** और **लागत ट्रैकिंग** दृश्य में ट्रैकिंग डेटा प्रोजेक्ट रूट नोड में प्रगति और आई लागत, समरी टास्क और लीफ नोड टास्क स्तर दिखाता है। **प्रोजेक्ट एंटिटी** पेज पर **स्थिति** खंड प्रोजेक्ट-स्तर के स्टेटस का समरी दिखाता है।

## <a name="status-summary-fields"></a>स्थिति सारांश फ़ील्ड

**संपूर्ण परियोजना स्थिति** फील्ड एक एडिट करने योग्य फील्ड होता है जो प्रोजेक्ट का संपूर्ण स्टेटस दिखाता है। इसमें बढ़ते जोखिम को दर्शाने के लिए हरे, पीले और लाल जैसे कलर-कोडिंग का इस्तेमाल किया जाता है। **टिप्पणियां**फ़ील्ड परियोजना प्रबंधक को स्थिति के बारे में विशिष्ट टिप्पणी दर्ज करने देता है. फील्ड **पर स्थिति अद्यतन** एडिट नहीं किया जा सकता और इसका वैल्यू टाइमस्टैम्प होता है जो स्टेटस के अंतिम बार अपडेट करने को बताता है।

**शेड्यूल प्रदर्शन** और **लागत प्रदर्शन** फील्ड ट्रैकिंग की तारीख से सेट किए जाते हैं। जब **प्रयास ट्रैकिंग** व्यू में रूट नोड के लिए शेड्यूल और लागत भिन्नता पोज़िटिव होते हैं तो आप इन फील्ड को **Ahead** में सेट कर सकते हैं। जब रूट नोड के लिए शेड्यूल और लागत भिन्नता निगेटिव होते हैं तो आप इन फील्ड को **पीछे** में सेट कर सकते हैं।
