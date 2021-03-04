---
title: अपना परिनियोजन प्रकार निर्धारित करें
description: यह विषय आपकी कंपनी के लिए Project operations के उचित नियोजन के प्रकार को निर्धारित करने में आपकी मदद करने हेतु जानकारी प्रदान करता है.
author: stsporen
manager: Annbe
ms.date: 11/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: e9d3a5d8e6e1daafac72a3b4c0380b679d1869bd
ms.sourcegitcommit: 14aa380759214713d9bf560f5a7f619b7f4bd5b8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/05/2020
ms.locfileid: "4401220"
---
# <a name="determine-your-deployment-type"></a>अपना परिनियोजन प्रकार निर्धारित करें

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

> [!IMPORTANT]
> लाइसेंस खरीदने के बाद, [निर्देशित इंस्टॉलेशन प्रवाह](https://aka.ms/provisionprojectoperations) का उपयोग करके Dynamics 365 Project Operations के सर्वश्रेष्ठ नियोजन मॉडल का निर्धारण करने के लिए यहां शुरू करें.
> निर्देशित इंस्टॉलेशन प्रवाह को पूरा करने के बाद, आपको अपनी इंस्टॉलेशन को पूरा करने के लिए उचित प्रबंधन पोर्टल पर निर्देशित किया जाएगा. इंस्टॉलेशन को पूरा करने के लिए नियोजन विवरण देखें.


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a>Dynamics 365 Project Service Automation उपयोग से Dynamics के मौजूदा ग्राहक
Project Operations में Project Service Automation के साथ भेजी गई क्षमताएं शामिल हैं. इन ग्राहकों के लिए 2021 रिलीज़ वेव 1 में एक अपग्रेड पथ जारी किया जाएगा.

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a>परियोजना प्रबंधन और लेखांकन के उपयोग से Dynamics 365 Finance के मौजूदा ग्राहक 

Finance के मौजूदा ग्राहक जो परियोजना प्रबंधन और लेखा कार्यक्षमता का उपयोग करते हैं, वे इसका, इसी तरह से उपयोग करना जारी रख सकते हैं. देखें [स्टॉक/उत्पादन आदेश परिदृश्यों के लिए Project Operations](#pma).


## <a name="deployment-types"></a>परिनियोजन प्रकार
Project Operations आपकी आवश्यकताओं से मेल खाने के लिए कई नियोजन विकल्पों का समर्थन करता है. चाहे आप एक नए या मौजूदा Dynamics 365 ग्राहक हों, Project Operations आपकी आवश्यकताओं का समर्थन कर सकता है.

हमारी [नियोजन प्रश्नावली](https://aka.ms/provisionprojectoperations) आपको सही नियोजन निर्धारित करने में मदद करेगी. परिणाम आपको निम्नलिखित प्रतिनियुक्ति प्रकारों में से एक की ओर निर्देशित करेंगे:

- [लाइट परिनियोजन – प्रोफ़ॉर्मा इनवॉइस करने के लिए डील](#lite)
- [संसाधन/गैर-स्टॉक परिदृश्यों के लिए Project Operations](#integrated)
- [स्टॉक/उत्पादन ऑर्डर परिदृश्यों के लिए Project Operations](#pma)

Project Operations कानूनी निकाय-स्तर के कॉन्फ़िगरेशन के माध्यम से एक ही परिवेश पर स्टॉक/उत्पादन आदेश परिदृश्यों और गैर-स्टॉक/संसाधन-आधारित परिदृश्यों का समर्थन करते हैं. उदाहरण के लिए, Contoso अपनी अमेरिकी विनिर्माण सुविधा (कानूनी निकाय = Contoso विनिर्माण संयुक्त राज्य अमेरिका) में स्टॉक/उत्पादन आदेश क्षमताओं का उपयोग कर सकता है. Contoso यूनाइटेड किंगडम में अपने Contoso रोबोटिक्स आर्म्स सर्विसिंग सुविधा में गैर-स्टॉक/संसाधन-आधारित क्षमताओं का उपयोग कर सकता है (कानूनी निकाय = Contoso रोबोटिक्स यूनाइटेड किंगडम).

### <a name="lite-deployment---deal-to-proforma-invoicing"></a><a  name="lite"></a>लाइट परिनियोजन - प्रोफ़ॉर्मा इनवॉइस करने के लिए डील

मामूली प्रतिनियुक्ति में निम्नलिखित क्षमताएं शामिल हैं:

- Dynamics 365 Sales एप्लिकेशन अनुभवों का विस्तार करने वाली परियोजनाओं के लिए विक्रय प्रक्रिया
- वेब के लिए Microsoft Project का उपयोग करके परियोजना की योजना
- बहु-आयामी मूल्य निर्धारण
- एकीकृत संसाधन प्रबंधन
- समय ट्रैकिंग
- मूल व्यय
- प्रोफ़ॉर्मा और ग्राहक-फोसिंग इनवॉयसिंग 

#### <a name="deployment-steps"></a>परिनियोजन चरण
[प्रतिनियुक्ति प्रश्नावली](https://aka.ms/provisionprojectoperations) का उपयोग करके Project Operations का सबसे अच्छा नियोजन मॉडल निर्धारित करें.

इस नियोजन के लिए, देखें [पूर्वावलोकन सदस्यता के लिए साइन-अप करें](lite-preview-subscription-sign-up.md) और [नए परिवेश का प्रावधान](lite-deployment.md). 


### <a name="project-operations-for-resourcenon-stocked-scenarios"></a><a name="integrated"></a>संसाधन/गैर-स्टॉक परिदृश्यों के लिए Project Operations
संसाधन/गैर-स्टॉक किए गए परिदृश्यों के लिए Project Operations में निम्नलिखित क्षमताएं शामिल हैं:
 
- Dynamics 365 Sales एप्लिकेशन का विस्तार करने वाली परियोजनाओं के लिए विक्रय प्रक्रिया
- वेब के लिए Microsoft Project का उपयोग करके परियोजना की योजना
- बहु-आयामी मूल्य निर्धारण
- एकीकृत संसाधन प्रबंधन
- समय ट्रैकिंग
- मूल व्यय
- पूरा व्यय
- OCR रसीद
- प्रोफ़ॉर्मा और ग्राहक-फोसिंग इनवॉयसिंग 
- परियोजनाओं के लिए राजस्व मान्यता

#### <a name="deployment-steps"></a>परिनियोजन चरण
[प्रतिनियुक्ति प्रश्नावली](https://aka.ms/provisionprojectoperations) का उपयोग करके Project Operations का सबसे अच्छा नियोजन मॉडल निर्धारित करें.

इस नियोजन के लिए, देखें [पूर्वावलोकन सदस्यता के लिए साइन-अप करें](resource-sign-up-preview-subscription.md) और [नए परिवेश का प्रावधान](resource-provision-new-environment.md). 


### <a name="project-operations-for-stockedproduction-order-scenarios"></a><a name="pma"></a>स्टॉक/उत्पादन ऑर्डर परिदृश्यों के लिए Project Operations

- WBS का उपयोग कर परियोजना की योजना बनाना
- संसाधन प्रबंधन
- समय ट्रैकिंग
- पूरा व्यय
- OCR रसीद
- पूर्ण इनवॉइस करना
- आमदनी मान्यता
- उत्पादन आदेश
- सामग्री समर्थन

#### <a name="deployment-steps"></a>परिनियोजन चरण
[प्रतिनियुक्ति प्रश्नावली](https://aka.ms/provisionprojectoperations) का उपयोग करके Project Operations का सबसे अच्छा नियोजन मॉडल निर्धारित करें.

इस नियोजन के लिए, देखें [पूर्वावलोकन सदस्यता के लिए साइन-अप करें](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) और [नए परिवेश का प्रावधान](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json). 



[!INCLUDE[footer-include](../includes/footer-banner.md)]