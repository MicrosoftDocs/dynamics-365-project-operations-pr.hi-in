---
title: क्या नया है मई 2022 - संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations
description: यह आलेख संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Microsoft Dynamics 365 Project Operations की मई 2022 रिलीज़ में उपलब्ध गुणवत्ता अपडेट के बारे में जानकारी प्रदान करता है.
author: sigitac
ms.date: 05/02/2022
ms.topic: article
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: beb75fc4b721d52cddbdaf2d20194218cefced5e
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8921396"
---
# <a name="whats-new-may-2022---project-operations-for-resourcenon-stocked-based-scenarios"></a>क्या नया है मई 2022 - संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations

_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए Project Operations_

यह आलेख निम्न Microsoft Dynamics 365 Project Operations घटक और संस्करणों पर लागू होता है:

- Dataverse परिवेश संस्करण 4.42.0.70 में Project Operations
- Dynamics 365 Finance परिवेश संस्करण 10.0.26 में परियोजना प्रबंधन और लेखांकन

## <a name="project-operations-dual-write-maps-updates"></a>Project Operations ड्यूल-राइट मानचित्र अपडेट्स

इस रिलीज़ में Project Operations ड्यूल-राइट मैप के लिए कोई अद्यतन नहीं हैं. वर्तमान सूची और Project Operations डुअल-राइट मैप के संस्करणों के लिए, [Project Operations डुअल-राइट मैप संस्करण](../environment/resource-dual-write-maps.md) देखें.

अपने परिवेश में मैप के नवीनतम संस्करण को हमेशा चलाएं और अपने Project Operations Dataverse समाधान और वित्त समाधान संस्करण को अद्यतित करते समय सभी संबंधित तालिका मैप सक्षम करें. यदि मानचित्र का नवीनतम संस्करण सक्रिय नहीं है तो कुछ सुविधाएं और क्षमताएं सही तरीके से काम नहीं कर सकती हैं. आप **ड्यूल-राइट** पेज पर **संस्करण** कॉलम में मानचित्र के सक्रिय संस्करण को देख सकते हैं. मैप के नए संस्करण को सक्रिय करने के लिए **तालिका मैप संस्करण** का चयन करें, नवीनतम संस्करण चुनें और फिर चुने गए संस्करण को सहेजें. यदि आपने एक आउट-ऑफ-द-बॉक्स तालिका मानचित्र को अनुकूलित किया है, तो परिवर्तनों को फिर से लागू करें. अधिक जानकारी के लिए देखें [एप्लिकेशन जीवनचक्र प्रबंधन](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/app-lifecycle-management).

यदि आप मानचित्र शुरू करते समय किसी समस्या का सामना करते हैं, तो डुअल-राइट समस्या निवारण गाइड का [मानचित्र पर अनुपलब्ध तालिका कॉलम समस्या](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-troubleshooting-finops-upgrades#missing-table-columns-issue-on-maps) अनुभाग पर दिए गए निर्देशों का पालन करें.

## <a name="quality-updates"></a>गुणवत्ता अद्यतन
### <a name="project-operations-on-dataverse"></a>Dataverse पर Project Operations

| सुविधा क्षेत्र | संदर्भ संख्या | गुणवत्ता अद्यतन |
| --- | --- | --- |
| संसाधन प्रबंधन | 2634019 | जेनेरिक टीम के सदस्यों को संसाधनों के रूप में जोड़ते समय व्यावसायिक सत्यापन के लिए बेहतर त्रुटि संदेश। |
| प्रोजेक्ट नियोजन और ट्रैकिंग | 2648515 | शेड्यूलिंग संस्थाओं में **ownerid**, **राज्य**, तथा **दर्जा** के प्रतिबंधित अद्यतन। |
| बिलिंग और मूल्य निर्धारण | 2653167 | **व्यक्तिगत विकल्प** में **अनुमान** ग्रिड दशमलव विभाजक को प्रारूप सेटिंग्स का पालन करना चाहिए. |
| बिलिंग और मूल्य निर्धारण| 2662251 | **सही इकाई** और **इकाई समूह** फील्ड के मान जब सामग्री अनुमान में रिकॉर्ड बनाते हैं. |
| बिलिंग और मूल्य निर्धारण| 2571408 | ड्राफ्ट इनवॉइस बनाते समय बिल न किए गए वास्तविक विक्रय प्रोफार्मा इनवॉइस आईडी के साथ स्टाम्पित होते हैं। |

### <a name="project-management-and-accounting-in-dynamics-365-finance"></a>Dynamics 365 Finance में परियोजना प्रबंधन और लेखांकन

इस अद्यतन में शामिल बग फ़िक्सेस के बारे में जानकारी के लिए,  Microsoft Dynamics Lifecycle Services (LCS) पर साइन इन करें और [KB आलेख](https://fix.lcs.dynamics.com/Issue/Details?bugId=662864) देखें.
