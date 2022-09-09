---
title: नया क्या है जुलाई 2022 - संसाधन/गैर-स्टॉक-आधारित परिदृश्यों के लिए Project Operations
description: यह आलेख Microsoft के जुलाई 2022 रिलीज़ में उपलब्ध गुणवत्ता अद्यतनों के बारे में जानकारी प्रदान करता है Dynamics 365 Project Operations संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए।
author: ramagadu
ms.date: 07/19/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: e63b29741dbaa400a2176ff8b4c35c6d64dfeab4
ms.sourcegitcommit: 7ed8e77a92917f2d242988ca02bd7de9571cce5e
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/02/2022
ms.locfileid: "9403953"
---
# <a name="whats-new-july-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>नया क्या है जुलाई 2022 - संसाधन/गैर-स्टॉक-आधारित परिदृश्यों के लिए Project Operations

_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए Project Operations_

यह आलेख Microsoft Dynamics 365 Project Operations के निम्न घटकों और संस्करणों पर लागू होता है:

- में परियोजना संचालन Dataverse पर्यावरण संस्करण 4.44.0.22
- Dynamics 365 Finance पर्यावरण संस्करण 10.0.28 . में परियोजना प्रबंधन और लेखांकन

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations ड्यूल-राइट मानचित्र अपडेट्स

इस रिलीज़ में Project Operations ड्यूल-राइट मैप के लिए कोई अद्यतन नहीं हैं. वर्तमान सूची और Project Operations डुअल-राइट मानचित्र के संस्करणों के लिए, [Project Operations डुअल-राइट मैप संस्करण](../environment/resource-dual-write-maps.md) देखें.

अपने परिवेश में हमेशा मानचित्र का नवीनतम संस्करण चलाएं, और अपने प्रोजेक्ट संचालन को अपडेट करते समय सभी संबंधित तालिका मानचित्रों को सक्षम करें Dataverse समाधान और वित्त समाधान संस्करण। यदि मानचित्र का नवीनतम संस्करण सक्रिय नहीं है, तो हो सकता है कि कुछ सुविधाएं और क्षमताएं ठीक से काम न करें। आप **ड्यूल-राइट** पेज पर **संस्करण** कॉलम में मानचित्र के सक्रिय संस्करण को देख सकते हैं. मैप के नए संस्करण को सक्रिय करने के लिए **तालिका मैप संस्करण** का चयन करें, नवीनतम संस्करण चुनें और फिर चुने गए संस्करण को सहेजें. यदि आपने आउट-ऑफ़-बॉक्स तालिका मानचित्र को अनुकूलित किया है, तो परिवर्तनों को पुन: लागू करें। अधिक जानकारी के लिए देखें [एप्लिकेशन जीवनचक्र प्रबंधन](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

यदि आप मानचित्र प्रारंभ करते समय किसी समस्या का सामना करते हैं, तो इसमें दिए गए निर्देशों का पालन करें [मानचित्र पर अनुपलब्ध तालिका स्तंभ समस्या](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) दोहरी-लेखन समस्या निवारण मार्गदर्शिका का अनुभाग।

## <a name="quality-updates"></a>गुणवत्ता अद्यतन

### <a name="project-operations-on-dataverse"></a>Dataverse पर Project Operations

| सुविधा क्षेत्र | संदर्भ संख्या | गुणवत्ता अद्यतन |
| --- | --- | --- |
| परिनियोजन और कॉन्फ़िगरेशन | 2761472 | एक प्रोजेक्ट ऑपरेशंस इंस्टॉलेशन त्रुटि को संभाला जाता है। |
| बिलिंग और मूल्य निर्धारण | 2746940 | उपसंविदा लाइन नाम की अधिकतम लंबाई 100 वर्ण होनी चाहिए। |
| बिलिंग और मूल्य निर्धारण | 2739162 | ग्राहकों को वास्तविक ग्रिड दृश्य में रिबन बटन देखने में सक्षम होना चाहिए। |
| परियोजना नियोजन और ट्रैकिंग | 2730318 | प्रोजेक्ट विषय में असमर्थित वर्णों के लिए अद्यतन सत्यापन। |
| बिलिंग और मूल्य निर्धारण | 2705361 | माइलस्टोन बिल की गई वास्तविक बिक्री को प्रोजेक्ट ट्रैकिंग फ़ील्ड में शामिल किया जाना चाहिए। |
| बिलिंग और मूल्य निर्धारण | 2675880 | किसी प्रोजेक्ट को उस अनुबंध लाइन से लिंक होने से रोकें जो कार्य-आधारित नहीं है। |
| बिलिंग और मूल्य निर्धारण | 2664396 | यदि कोई कोट मूल्य सूची बिना कोट के सहेजी जाती है, तो एक त्रुटि होनी चाहिए जो बताती है कि कोट खाली नहीं हो सकता। |
| बिलिंग और मूल्य निर्धारण | 2184019 | **कार्य आधारित बिलिंग** उन परियोजनाओं के लिए टैब नहीं दिखाया जाना चाहिए जिनके पास कोई समर्थन अनुबंध या उद्धरण नहीं है। |
| समय और व्यय | 2754459 | जब आवर्तक शेड्यूलिंग क्लाउड प्रवाह निष्क्रिय हो, तो बैनर दिखाएं और async प्रसंस्करण को बायपास करें। |
| बिलिंग और मूल्य निर्धारण | 2724391 | प्रोजेक्ट अनुबंध स्प्लिट बिलिंग नियम में ग्राहक मान अनुपलब्ध होने पर गलत अपवाद दिया जाता है। |
| बिलिंग और मूल्य निर्धारण | 2708638 | सामग्री उपयोग और सामग्री उपयोग के लिए अनुमोदन में ग्रिड खोज का उपयोग करते हुए खोज करते समय रिकॉर्ड नहीं मिला।|
| बिलिंग और मूल्य निर्धारण | 2686977 | इनवॉइस निर्माण के दौरान इनवॉइस लाइन के लिए सत्यापन रोकें। |
| बिलिंग और मूल्य निर्धारण | 2683032 | प्रभार्य भूमिकाओं और श्रेणियों की प्रतिलिपि 5000 रिकॉर्ड से अधिक नहीं होती है।|
| बिलिंग और मूल्य निर्धारण | 2673363 | किसी प्रोजेक्ट के लिए प्रयास और व्यय अनुमान और वास्तविक दोनों मौजूद होने पर परियोजना पर लागत खपत% दूषित हो जाता है। |

### <a name="project-management-and-accounting-in-finance"></a>वित्त में परियोजना प्रबंधन और लेखांकन

इस अद्यतन में शामिल बग फिक्स के बारे में जानकारी के लिए, लॉग इन करें Microsoft Dynamics जीवनचक्र सेवाएँ (LCS), और देखें [केबी लेख](https://fix.lcs.dynamics.com/Issue/Details?bugId=694438).

## <a name="features-turned-on-by-default-in-upcoming-release"></a>आगामी रिलीज़ में डिफ़ॉल्ट रूप से चालू की गई सुविधाएँ

निम्न तालिका 10.0.29 संस्करण में डिफ़ॉल्ट रूप से चालू सुविधाओं को सूचीबद्ध करती है। स्वचालित रूप से चालू की गई अधिकांश सुविधाओं को बंद किया जा सकता है [सुविधा प्रबंधन](/dynamics365/fin-ops-core/fin-ops/get-started/feature-management/feature-management-overview). भविष्य में, स्वचालित रूप से चालू की गई कुछ सुविधाएं फ़ीचर प्रबंधन से हटाई जा सकती हैं और अनिवार्य हो सकती हैं। यह परिवर्तन सुनिश्चित करता है कि ग्राहक वर्तमान कार्यक्षमता का उपयोग कर रहे हैं, ताकि एन्हांसमेंट वर्तमान कार्यक्षमता को जोड़े जाने पर बना सकें। सुविधाओं को एक वर्ष से कम समय में स्वचालित रूप से सक्षम नहीं किया जाएगा, जब तक कि वे आवश्यक होने के लिए निर्धारित न हों।

| फ़ीचर का नाम | दिनांक सक्षम करें | फीचर जोड़ा गया | फ़ीचर स्थिति | मॉड्यूल |
| --- | --- | --- |--- |--- |
| फंडिंग नियम आवंटन में बदलाव के आधार पर घंटे के लेन-देन का समायोजन सक्षम करें | 16 सितंबर 2022 | 7 अक्तूबर, 2020 | डिफ़ॉल्ट रूप से चालू | परियोजना प्रबंधन और लेखांकन |
| परियोजना खरीद आदेश पूर्व भुगतान चालान उलटने की सुविधा | 16 सितंबर 2022 | 6 अक्तूबर, 2021 | डिफ़ॉल्ट रूप से चालू | परियोजना प्रबंधन और लेखांकन |
| संसाधन आधारित/गैर-स्टॉक किए गए परिदृश्यों के लिए प्रोजेक्ट संचालन का उपयोग करते समय इनवॉइस प्रस्ताव पंक्तियों को हटा दें | 16 सितंबर 2022 | 6 अक्तूबर, 2021 | डिफ़ॉल्ट रूप से चालू | परियोजना प्रबंधन और लेखांकन |
| पोस्ट किए गए प्रोजेक्ट लेनदेन पर लेखांकन समायोजित करें | 16 सितंबर 2022 | 10 मई, 2020 | डिफ़ॉल्ट रूप से चालू | परियोजना प्रबंधन और लेखांकन |
| प्रोजेक्ट के लिए डिफ़ॉल्ट अकाउंटिंग सेटअप सक्षम करें | 16 सितंबर 2022 | 19 फ़रवरी, 2020 | डिफ़ॉल्ट रूप से चालू | परियोजना प्रबंधन और लेखांकन |
| प्रकल्प के लिये एकाधिक अनुबन्ध लाइन्स सक्रिय कीजिये | 16 सितंबर 2022 | 29 जून, 2020 | डिफ़ॉल्ट रूप से चालू | परियोजना प्रबंधन और लेखांकन |
| यदि वर्तमान स्वीकृति स्थिति संपादन की अनुमति नहीं देती है, तो प्रोजेक्ट आवर जर्नल्स को केवल पढ़ने के लिए बनाएं | 16 सितंबर 2022 | 6 अक्तूबर, 2021 | डिफ़ॉल्ट रूप से चालू | परियोजना प्रबंधन और लेखांकन |
| खरीद लाइनों के अद्यतन होने और खरीद आदेश परिवर्तन प्रबंधन पैरामीटर चालू होने पर खरीद लाइनों से बिक्री लाइनों को सिंक करें सक्षम करें | 16 सितंबर 2022 | 7 अक्तूबर, 2020 | डिफ़ॉल्ट रूप से चालू | परियोजना प्रबंधन और लेखांकन |
| Dynamics 365 Customer Engagement . पर परियोजना संचालन सक्षम करें | 16 सितंबर 2022 | 29 जून, 2020 | डिफ़ॉल्ट रूप से चालू | परियोजना प्रबंधन और लेखांकन |
| प्रोजेक्ट ट्रांजैक्शन रिवर्सल करेक्शन फीचर | 16 सितंबर 2022 | 13 जुलाई, 2020 | डिफ़ॉल्ट रूप से चालू | परियोजना प्रबंधन और लेखांकन |

## <a name="features-that-become-mandatory-in-the-upcoming-release"></a>आगामी रिलीज़ में अनिवार्य हो जाने वाली सुविधाएँ

निम्न तालिका उन सुविधाओं को सूचीबद्ध करती है जो संस्करण 10.0.29 से अनिवार्य हैं।

| फ़ीचर का नाम | दिनांक सक्षम करें | फीचर जोड़ा गया | फ़ीचर स्थिति | मॉड्यूल |
| --- | --- | --- | --- | --- |
| विनिमय दर को गोल किए बिना फंडिंग स्रोत पर प्रतिबद्ध मूल्य की गणना करें | 16 सितंबर 2022 | 14 जून, 2020 | अनिवार्य | परियोजना प्रबंधन और लेखांकन |
| मूल लेन-देन के समान लेज़र खाते के साथ प्रोजेक्ट समायोजन पोस्टिंग सक्षम करें | 16 सितंबर 2022 | 14 जून, 2020 | अनिवार्य | परियोजना प्रबंधन और लेखांकन |
| परियोजना अनुबंध प्रतिबद्ध राशि विवरण | 16 सितंबर 2022 | 31 अगस्त, 2019 | अनिवार्य | परियोजना प्रबंधन और लेखांकन |
| प्रोजेक्ट इनवॉइस प्रस्ताव निर्माण के दौरान संसाधन द्वारा छँटाई सक्षम करें | 16 सितंबर 2022 | 31 अगस्त, 2019 | अनिवार्य | परियोजना प्रबंधन और लेखांकन |