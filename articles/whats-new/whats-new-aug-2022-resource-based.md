---
title: नया क्या है अगस्त 2022 - संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations
description: यह आलेख उन गुणवत्ता अद्यतनों के बारे में जानकारी प्रदान करता है जो Microsoft के अगस्त 2022 रिलीज़ में उपलब्ध हैं Dynamics 365 Project Operations संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए।
author: ramagadu
ms.date: 07/19/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: ramagadu
ms.openlocfilehash: 112dbb98de09ef342c03d122a29cb8025058e47f
ms.sourcegitcommit: 6b6c2bfd04e3e613ed1f38355c7cd47c3a56748d
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 08/24/2022
ms.locfileid: "9348101"
---
# <a name="whats-new-august-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>नया क्या है अगस्त 2022 - संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations

_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए Project Operations_

यह आलेख Microsoft के निम्नलिखित घटकों और संस्करणों पर लागू होता है Dynamics 365 Project Operations:

- में परियोजना संचालन Dataverse पर्यावरण संस्करण 4.45.0.53
- Dynamics 365 Finance पर्यावरण संस्करण 10.0.28 . में परियोजना प्रबंधन और लेखांकन

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations ड्यूल-राइट मानचित्र अपडेट्स

इस रिलीज़ में Project Operations ड्यूल-राइट मैप के लिए कोई अद्यतन नहीं हैं. वर्तमान सूची और Project Operations डुअल-राइट मानचित्र के संस्करणों के लिए, [Project Operations डुअल-राइट मैप संस्करण](../environment/resource-dual-write-maps.md) देखें.

अपने परिवेश में हमेशा मानचित्र का नवीनतम संस्करण चलाएँ, और अपने प्रोजेक्ट संचालन को अद्यतन करते समय सभी संबंधित तालिका मानचित्रों को सक्षम करें Dataverse समाधान और वित्त समाधान संस्करण। यदि मानचित्र का नवीनतम संस्करण सक्रिय नहीं है, तो हो सकता है कि कुछ सुविधाएं और क्षमताएं ठीक से काम न करें। आप **ड्यूल-राइट** पेज पर **संस्करण** कॉलम में मानचित्र के सक्रिय संस्करण को देख सकते हैं. मैप के नए संस्करण को सक्रिय करने के लिए **तालिका मैप संस्करण** का चयन करें, नवीनतम संस्करण चुनें और फिर चुने गए संस्करण को सहेजें. यदि आपने आउट-ऑफ़-बॉक्स तालिका मानचित्र को अनुकूलित किया है, तो परिवर्तनों को पुन: लागू करें। अधिक जानकारी के लिए देखें [एप्लिकेशन जीवनचक्र प्रबंधन](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

यदि आप मानचित्र प्रारंभ करते समय किसी समस्या का सामना करते हैं, तो इसमें दिए गए निर्देशों का पालन करें [मानचित्र पर अनुपलब्ध तालिका स्तंभ समस्या](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) दोहरी-लेखन समस्या निवारण मार्गदर्शिका का अनुभाग।

## <a name="quality-updates"></a>गुणवत्ता अद्यतन

### <a name="project-operations-on-dataverse"></a>Dataverse पर Project Operations

| सुविधा क्षेत्र | संदर्भ संख्या | गुणवत्ता अद्यतन |
| --- | --- | --- |
|  अवसर प्रबंधक | 2762089 | org.org में ऑटो-सेव अक्षम होने पर अनुबंध को बंद करते समय त्रुटि प्रबंधन खो गया है।|

### <a name="project-management-and-accounting-in-finance"></a>वित्त में परियोजना प्रबंधन और लेखांकन

इस अद्यतन में शामिल बग फिक्स के बारे में जानकारी के लिए, लॉग इन करें Microsoft Dynamics जीवनचक्र सेवाएँ (LCS), और देखें [केबी लेख।](https://fix.lcs.dynamics.com/Issue/Details?bugId=694438)
