---
title: नया क्या है नवंबर 2022 - संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए Project Operations
description: यह आलेख उन गुणवत्ता अद्यतनों के बारे में जानकारी प्रदान करता है जो संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Microsoft Dynamics 365 Project Operations के नवंबर 2022 रिलीज़ में उपलब्ध हैं।
author: ryansandness
ms.date: 12/16/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ryansandness
ms.openlocfilehash: 509e303aeb0567627590fd89c6888b59a414c6f1
ms.sourcegitcommit: 952fcefe33de192ad48f4108c3adbe658fd7b94f
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 12/08/2022
ms.locfileid: "9831131"
---
# <a name="whats-new-november-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>नया क्या है नवंबर 2022 - संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए Project Operations

_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए Project Operations_

यह आलेख निम्न Microsoft Dynamics 365 Project Operations घटक और संस्करणों पर लागू होता है:

- Dataverse परिवेश संस्करण 4.58.0.119 में Project Operations
- Dynamics 365 Finance परिवेश संस्करण 10.0.30 में परियोजना प्रबंधन और लेखांकन

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations ड्यूल-राइट मैप अपडेट्स

इस रिलीज़ में Project Operations ड्यूल-राइट मैप के लिए कोई अद्यतन नहीं हैं. वर्तमान सूची और Project Operations डुअल-राइट मानचित्र के संस्करणों के लिए, [Project Operations डुअल-राइट मैप संस्करण](../environment/resource-dual-write-maps.md) देखें.

अपने परिवेश में मैप के नवीनतम संस्करण को हमेशा चलाएं और अपने Project Operations Dataverse समाधान और वित्त समाधान संस्करण को अद्यतित करते समय सभी संबंधित तालिका मैप सक्षम करें. यदि मानचित्र का नवीनतम संस्करण सक्रिय नहीं है तो कुछ सुविधाएं और क्षमताएं सही तरीके से काम नहीं कर सकती हैं. आप **ड्यूल-राइट** पेज पर **संस्करण** कॉलम में मानचित्र के सक्रिय संस्करण को देख सकते हैं. मैप के नए संस्करण को सक्रिय करने के लिए **तालिका मैप संस्करण** का चयन करें, नवीनतम संस्करण चुनें और फिर चुने गए संस्करण को सहेजें. यदि आपने एक आउट-ऑफ-द-बॉक्स तालिका मानचित्र को अनुकूलित किया है, तो परिवर्तनों को फिर से लागू करें. अधिक जानकारी के लिए देखें [एप्लिकेशन जीवनचक्र प्रबंधन](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

यदि आप मानचित्र शुरू करते समय किसी समस्या का सामना करते हैं, तो डुअल-राइट समस्या निवारण गाइड का [मानचित्र पर अनुपलब्ध तालिका कॉलम समस्या](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) अनुभाग पर दिए गए निर्देशों का पालन करें.

## <a name="quality-updates"></a>गुणवत्ता अद्यतन

### <a name="project-operations-on-dataverse"></a>Dataverse पर Project Operations

| सुविधा क्षेत्र | संदर्भ संख्या | गुणवत्ता अद्यतन |
| --- | --- | --- |
| बिलिंग और मूल्य निर्धारण | 2781818 | सामग्री उपयोग लॉग के लिए डिफ़ॉल्ट मूल्य के दौरान कुंजी को त्रुटि नहीं मिली। |
| बिलिंग और मूल्य निर्धारण | 2922373 | कोटेशन लाइन को उस प्रोजेक्ट से लिंक नहीं किया जा सकता जो खोई हुई कोटेशन के रूप में बंद हो गया है। |
| बिलिंग और मूल्य निर्धारण | 2943206 | **प्रोजेक्ट इकाई में अनुबंध पंक्ति** फ़ील्ड वैकल्पिक होना चाहिए। |
| बिलिंग और मूल्य निर्धारण | 2953182 | सुधार चालान के लिए त्रुटि संदेश में सुधार करें।|
| बिलिंग और मूल्य निर्धारण | 2959500 | कोटेशन लाइन को किसी ऐसे प्रोजेक्ट टास्क से लिंक नहीं किया जा सकता जो पहले से ही खोए हुए कोटेशन से जुड़ा है।|
| बिलिंग और मूल्य निर्धारण | 2959560 | "यह ग्राहक पहले से ही परियोजना अनुबंध पर है" संदेश प्राप्त हुआ जब बोली को कुछ स्थानों में जीत के रूप में बंद किया गया। |
| बिलिंग और मूल्य निर्धारण | 3031727 | आवश्यक फ़ील्ड के साथ संसाधन असाइनमेंट विफल 'msdyn_Company' में त्रुटि गुम है। |
| बिलिंग और मूल्य निर्धारण | 3036905 | स्वामित्व वाली कंपनी को कभी भी ProjectTeamMember पर इनिशियलाइज़ नहीं किया जाता है। |
| अवसर प्रबंधन | 2763519 | EnsureProjectContractAllowsUpdates में अशक्त संदर्भ त्रुटि। |
| अवसर प्रबंधन | 2783798 | कोट लाइन पर परियोजना अनुमानों को आयात करते समय, व्यय और भौतिक अनुमानों के लिए कार्य विवरण गायब हैं।|
| अवसर प्रबंधन | 2988635 | ग्राहक को कोट पर हटाते समय त्रुटि संदेश विवरण में सुधार करें। |
| अवसर प्रबंधन | 3001191 | अवसर से उद्धरण बनाने में असमर्थ जहां बिलिंग पद्धति को शून्य के रूप में निर्दिष्ट किया गया है। |
| अपग्रेड करें | 3012324 | प्रोजेक्ट कनवर्ज़न उसके नाम में टैब जैसे नियंत्रण वर्ण वाले किसी प्रोजेक्ट पर विफल रहा। || परियोजना नियोजन और ट्रैकिंग | 2790384 | लंबित OperationSet टाइम-आउट बहुत कम है। |
| परियोजना नियोजन और ट्रैकिंग | 3044275 | इसके लिए गुम स्थानीयकरण: अनुपलब्धप्रोजेक्ट शेड्यूलर त्रुटि संदेश। |
| परियोजना नियोजन और ट्रैकिंग | 3044277 | शेड्यूलर सेट न होने पर प्रोजेक्ट रिकॉन ग्रिड लोड नहीं होता है।|
| संसाधन प्रबंधन | 2943153 | अवधि के लिए दो दशमलव स्थान दिखाने के लिए ट्रैकिंग टैब अपडेट करें।|
| उपअनुबंध | 2932774 | विक्रेता इनवॉइस लाइन रीड ओनली थ्रोइंग एरर गलत है। |
| उपअनुबंध | 2939556 | वेंडर इनवॉयस हैडर की स्थिति को ड्राफ्ट ऑनलाइन डिलीट पर सेट नहीं किया जाना चाहिए यदि सक्रिय नहीं है। |
| समय और व्यय | 2939998 | ProjOps में नया TESA संस्करण लें। |


### <a name="project-management-and-accounting-in-finance"></a>फाइनेंस में परियोजना प्रबंधन और लेखांकन

इस अद्यतन में शामिल बग फ़िक्सेस के बारे में जानकारी के लिए, Microsoft Dynamics Lifecycle Services (LCS) पर साइन इन करें, और [KB आलेख](https://fix.lcs.dynamics.com/Issue/Details?bugId=745468) देखें.