---
title: नया क्या है अगस्त 2022 - संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations
description: यह आलेख संसाधन/गैर-स्टॉक किए गए आधारित परिदृश्यों के लिए Microsoft Dynamics 365 Project Operations के अगस्त 2022 रिलीज़ में उपलब्ध गुणवत्ता अद्यतनों के बारे में जानकारी प्रदान करता है।
author: ramagadu
ms.date: 07/19/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: 4042dca72a33f48e04e51af2a3cfd2da83146afd
ms.sourcegitcommit: 7ed8e77a92917f2d242988ca02bd7de9571cce5e
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/02/2022
ms.locfileid: "9403858"
---
# <a name="whats-new-august-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>नया क्या है अगस्त 2022 - संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations

_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए Project Operations_

यह आलेख Microsoft Dynamics 365 Project Operations के निम्न घटकों और संस्करणों पर लागू होता है:

- किसी Dataverse परिवेश संस्करण में प्रोजेक्ट ऑपरेशन 4.45.0.53
- Dynamics 365 Finance पर्यावरण संस्करण 10.0.28 . में परियोजना प्रबंधन और लेखांकन

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations ड्यूल-राइट मानचित्र अपडेट्स

इस रिलीज़ में Project Operations ड्यूल-राइट मैप के लिए कोई अद्यतन नहीं हैं. वर्तमान सूची और Project Operations डुअल-राइट मानचित्र के संस्करणों के लिए, [Project Operations डुअल-राइट मैप संस्करण](../environment/resource-dual-write-maps.md) देखें.

अपने परिवेश में हमेशा मानचित्र का नवीनतम संस्करण चलाएं, और अपने प्रोजेक्ट संचालन को अपडेट करते समय सभी संबंधित तालिका मानचित्रों को सक्षम करें Dataverse समाधान और वित्त समाधान संस्करण। यदि मानचित्र का नवीनतम संस्करण सक्रिय नहीं है, तो हो सकता है कि कुछ सुविधाएं और क्षमताएं ठीक से काम न करें। आप **ड्यूल-राइट** पेज पर **संस्करण** कॉलम में मानचित्र के सक्रिय संस्करण को देख सकते हैं. मैप के नए संस्करण को सक्रिय करने के लिए **तालिका मैप संस्करण** का चयन करें, नवीनतम संस्करण चुनें और फिर चुने गए संस्करण को सहेजें. यदि आपने आउट-ऑफ़-बॉक्स तालिका मानचित्र को अनुकूलित किया है, तो परिवर्तनों को पुन: लागू करें। अधिक जानकारी के लिए देखें [एप्लिकेशन जीवनचक्र प्रबंधन](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

यदि आप मानचित्र प्रारंभ करते समय किसी समस्या का सामना करते हैं, तो इसमें दिए गए निर्देशों का पालन करें [मानचित्र पर अनुपलब्ध तालिका स्तंभ समस्या](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) दोहरी-लेखन समस्या निवारण मार्गदर्शिका का अनुभाग।

## <a name="quality-updates"></a>गुणवत्ता अद्यतन

### <a name="project-operations-on-dataverse"></a>Dataverse पर Project Operations

| सुविधा क्षेत्र | संदर्भ संख्या | गुणवत्ता अद्यतन |
| --- | --- | --- |
|  अवसर प्रबंधक | 2762089 | यदि संगठन में स्वतः-सहेजना अक्षम है, तो अनुबंध को बंद करते समय त्रुटि हैंडलिंग खो गई है.|
|परियोजना नियोजन और ट्रैकिंग | 2767841 | टेलीमेट्री अद्यतन प्रोजेक्ट एंटिटी बनाएँ या परिदृश्य अद्यतन करें।|
|बिलिंग और मूल्य निर्धारण | 2771072 | उद्धरण जीतते समय शून्य संदर्भ अपवाद हैंडलिंग।|
|बिलिंग और मूल्य निर्धारण | 2844181 |सहसंबंध आईडी प्राप्त करने और चालान निर्माण को अवरुद्ध करने में विफलता।|
|बिलिंग और मूल्य निर्धारण | 2852836 | सीई में बनाए गए और अनुमोदित इंटरकंपनी व्यय के लिए इंटरकंपनी वास्तविक गायब हैं।|


### <a name="project-management-and-accounting-in-finance"></a>वित्त में परियोजना प्रबंधन और लेखांकन

इस अद्यतन में शामिल बग फिक्स के बारे में जानकारी के लिए, लॉग इन करें Microsoft Dynamics जीवनचक्र सेवाएँ (LCS), और देखें [केबी लेख](https://fix.lcs.dynamics.com/Issue/Details?bugId=694438).
