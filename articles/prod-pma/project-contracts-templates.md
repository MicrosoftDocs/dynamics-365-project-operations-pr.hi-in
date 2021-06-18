---
title: परियोजना अनुबंधों और परियोजनाओं को सीधे Project Service Automation से Finance तक सिंक्रनाइज़ करें
description: यह विषय टेम्पलेट और अंतर्निहित कार्यों का वर्णन करता है जिनका उपयोग परियोजना अनुबंधों और परियोजनाओं को सीधे Microsoft Dynamics 365 Project Service Automation से Dynamics 365 Finance तक सिन्क्रोनाइज करने के लिए किया जाता है.
author: Yowelle
ms.date: 12/17/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2017-12-13
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 2f5fa0143c903f08b3937426805cb43d5d6109e3
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5999808"
---
# <a name="synchronize-project-contracts-and-projects-directly-from-project-service-automation-to-finance"></a>परियोजना अनुबंधों और परियोजनाओं को सीधे Project Service Automation से Finance तक सिंक्रनाइज़ करें 

[!include[banner](../includes/banner.md)]

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

यह विषय टेम्पलेट और अंतर्निहित कार्यों का वर्णन करता है जिनका उपयोग परियोजना अनुबंधों और परियोजनाओं को सीधे Dynamics 365 Project Service Automation से Dynamics 365 Finance तक सिन्क्रोनाइज करने के लिए किया जाता है.

> [!NOTE] 
> यदि आप Enterprise Edition 7.3.0 का इस्तेमाल कर रहे हैं, तो आपको KB 4074835 इंस्टॉल करना चाहिए.

## <a name="data-flow-for-project-service-automation-to-finance"></a>Project Service Automation से Finance के लिए डेटा प्रवाह

> [!NOTE]
> इससे पहले कि आप Finance एकीकरण समाधान के लिए Project Service Automation का उपयोग कर सकें, आपको Dynamics 365 डेटा एकीकरण सुविधा से परिचित होना चाहिए.

Project Service Automation से Finance एकीकरण समाधान Project Service Automation और Finance के उदाहरणों में डेटा सिन्क्रोनाइज करने के लिए डेटा एकीकरण सुविधा का उपयोग करता है. एकीकरण टेम्पलेट जो डेटा एकीकरण सुविधा के साथ उपलब्ध है परियोजना अनुबंधों, परियोजनाओं, परियोजना अनुबंध लाइनों, और Project Service Automation से Finance तक परियोजना अनुबंध लाइन उपलब्धियों के बारे में डेटा के प्रवाह को सक्षम बनाता है.

निम्नलिखित दृष्टांत दर्शाता है कि Project Service Automation और Finance के बीच डेटा को सिन्क्रोनाइज कैसे किया जाता है.

[![वित्त के साथ Project Service Automation एकीकरण के लिए डेटा प्रवाह](./media/ProjectsAndContractsFlow_upd.JPG)](./media/ProjectsAndContractsFlow.JPG)

## <a name="templates-and-tasks"></a>टेम्पलेट और कार्य

उपलब्ध टेम्पलेटों तक पहुंचने के लिए, Microsoft Power Apps एडमिन सेंटर में, **परियोजनाएं** का चयन करें, और फिर, ऊपरी-दाएं कोने में, सार्वजनिक टेम्पलेटों का चयन करने के लिए **नई परियोजना** का चयन करें.

Project Service Automation से Finance तक परियोजना अनुबंधों और परियोजनाओं को सिन्क्रोनाइज करने के लिए निम्नलिखित टेम्पलेट्स और अंतर्निहित कार्यों का उपयोग किया जाता है:

### <a name="integrating-with-dynamics-365-project-service-automation-v2x"></a>Dynamics 365 Project Service Automation v2.x के साथ एकीकृत
- **डेटा एकीकरण में टेम्पलेट का नाम:** परियोजनाएं और अनुबंध (Project Service Automation से Finance)
- **परियोजना में कार्य का नाम:**

    - परियोजना अनुबंध Project Service Automation से Finance
    - परियोजना Project Service Automation से Finance
    - परियोजना अनुबंध पंक्तियाँ Project Service Automation से Finance
    - परियोजना अनुबंध पंक्ति माइलस्टोन Project Service Automation से Finance
  
### <a name="integrating-with-dynamics-365-project-service-automation-v3x"></a>Dynamics 365 Project Service Automation v3.x के साथ एकीकृत
Project Service Automation में एक रूपरेखा परिवर्तन है जो परियोजना अनुबंध लाइन उपलब्धि टेम्पलेट को और Dynamics 365 के साथ Project Service Automation v3.x को एकीकृत करने के लिए आवश्यक टेम्पलेट के संस्करण v2 के उपयोग को प्रभावित करता है.

- **डेटा एकीकरण में टेम्पलेट का नाम:** परियोजनाएं और अनुबंध (Project Service Automation 3.x से Finance) - v2
- **परियोजना में कार्य का नाम:**

    - परियोजना अनुबंध Project Service Automation से Finance
    - परियोजना Project Service Automation से Finance
    - परियोजना अनुबंध पंक्तियाँ Project Service Automation से Finance
    - परियोजना अनुबंध पंक्ति माइलस्टोन Project Service Automation से Finance

परियोजना अनुबंधों और परियोजनाओं के सिन्क्रोनाइजेशन से पहले, आपको खातों को सिन्क्रोनाइज करना होगा.

## <a name="entity-set"></a>निकाय सेट

| Project Service Automation       | वित्त                                                |
|----------------------------------|--------------------------------------------------------|
| ऑर्डर्स                           | परियोजना अनुबंध के लिए एकीकरण निकाय                |
| परियोजनाएँ                         | परियोजना के लिए एकीकरण निकाय                         |
| ऑर्डर पंक्तियाँ                      | परियोजना अनुबंध पंक्ति के लिए एकीकरण निकाय           |
| परियोजना अनुबंध पंक्ति माइलस्टोन | परियोजना अनुबंध लाइन उपलब्धि के लिए एकीकरण निकाय |

## <a name="entity-flow"></a>निकाय प्रवाह

परियोजना अनुबंध Project Service Automation में प्रबंधित किए जाते हैं, और वे परियोजना अनुबंधों के रूप में Finance से सिन्क्रोनाइज होते हैं. एकीकरण टेम्पलेट के हिस्से के रूप में, आप परियोजना अनुबंध के लिए Finance में एकीकरण स्रोत सेट कर सकते हैं.

समय और सामग्री और निश्चित मूल्य परियोजनाएं Project Service Automation में प्रबंधित की जाती हैं और परियोजनाओं के रूप में Finance के साथ सिंक्रनाइज़ की जाती हैं. टेम्पलेट एकीकरण के भाग के रूप में, आप Finance में परियोजना के लिए एकीकरण स्रोत सेट कर सकते हैं. वर्तमान में, केवल समय और सामग्री और निर्धारित मूल्य परियोजनाएँ समर्थित हैं.


परियोजना अनुबंध लाइनों को Project Service Automation में प्रबंधित किया जाता है, और वे परियोजना अनुबंध के बिलिंग के नियमों के रूप में Finance से सिन्क्रोनाइज होते हैं. यदि बिलिंग विधि डिफ़ॉल्ट परियोजना के प्रकार से अलग है, तो सिन्क्रोनाइजेशन अनुबंध लाइन परियोजना और परियोजना समूह के लिए परियोजना के प्रकार को अपडेट करता है.

परियोजना अनुबंध लाइन उपलब्धियों को Project Service Automation में प्रबंधित किया जाता है, और वे परियोजना अनुबंध के बिलिंग के नियम की उपलब्धियों के रूप में Finance से सिन्क्रोनाइज होते हैं.

## <a name="project-service-automation-to-finance-integration-solution"></a>Project Service Automation से Finance एकीकरण समाधान

**परियोजना अनुबंध ID** फ़ील्ड **परियोजना अनुबंध** पृष्ठ पर उपलब्ध है. एकीकरण का समर्थन करने के लिए इस फ़ील्ड को एक प्राकृतिक और अद्वितीय कुंजी बनाया गया है.

जब कोई नया परियोजना अनुबंध बनाया जाता है, तो यदि **परियोजना अनुबंध ID** मान पहले से मौजूद नहीं है, तो यह एक संख्या अनुक्रम का उपयोग करके स्वचालित रूप से उत्पन्न होता है. मान में **ORD** शामिल होते हैं जिसके बाद एक वृद्धि संख्या अनुक्रम और फिर छ: वर्णों का एक सफ़िक्स होता है. यहां एक उदाहरण दिया गया है: **ORD-01022-Z4M9Q0**.

**परियोजना संख्या** फ़ील्ड **परियोजना** पृष्ठ पर उपलब्ध है. एकीकरण का समर्थन करने के लिए इस फ़ील्ड को एक प्राकृतिक और अद्वितीय कुंजी बनाया गया है.

जब कोई नई परियोजना बनाई जाती है, तो यदि **परियोजना संख्या** मान पहले से मौजूद नहीं है, तो यह एक संख्या अनुक्रम का उपयोग करके स्वचालित रूप से उत्पन्न होता है. मान में **PRJ** शामिल होते हैं जिसके बाद एक वृद्धि संख्या अनुक्रम और फिर छ: वर्णों का एक सफ़िक्स होता है. यहां एक उदाहरण दिया गया है: **PRJ-01049-CCNID0**.

जब Project Service Automation से Finance एकीकरण समाधान लागू किया जाता है, तो एक अपग्रेड स्क्रिप्ट मौजूदा परियोजना अनुबंधों के लिए **परियोजना अनुबंध ID** फील्ड और Project Service Automation में मौजूदा परियोजनाओं के लिए **परियोजना संख्या** फील्ड सेट करती है.

## <a name="prerequisites-and-mapping-setup"></a>आवश्यकताएँ और मानचित्रण सेटअप

- परियोजना अनुबंधों और परियोजनाओं के सिन्क्रोनाइजेशन से पहले, आपको खातों को सिन्क्रोनाइज करना होगा.
- अपने कनेक्शन सेट में, **msdyn\_organizationalunits** से **msdyn\_name \[Name\]** के लिए एक एकीकरण कुंजी फ़ील्ड मानचित्रण जोड़ें. आपको सबसे पहले कनेक्शन सेट में एक परियोजना जोड़ने की आवश्यकता हो सकती है. अधिक जानकारी के लिए, [अनुप्रयोग के लिए Common Data Service में डेटा को एकीकृत करे](/powerapps/administrator/data-integrator) देखें.
- अपने कनेक्शन सेट में, **msdyn\_projects** से **msdynce\_projectnumber \[प्रोजेक्ट नंबर\]** के लिए एक एकीकरण कुंजी फ़ील्ड मानचित्रण जोड़ें. आपको सबसे पहले कनेक्शन सेट में एक परियोजना जोड़ने की आवश्यकता हो सकती है. अधिक जानकारी के लिए, [अनुप्रयोग के लिए Common Data Service में डेटा को एकीकृत करे](/powerapps/administrator/data-integrator) देखें.
- **SourceDataID** को परियोजना अनुबंधों और परियोजनाओं के लिए एक अलग मान पर अपडेट किया जा सकता है या मानचित्रण से हटाया जा सकता है. डिफ़ॉल्ट टेम्पलेट मान **Project Service Automation** है.
- **PaymentTerms** मानचित्रण को अपडेट किया जाना चाहिए ताकि यह Finance में भुगतान की वैध शर्तों को दर्शाता हो. आप परियोजना टास्क से मानचित्रण को हटा भी सकते हैं. डिफ़ॉल्ट मान मानचित्र में डेमो डेटा के लिए डिफॉल्ट मान हैं. निम्नलिखित तालिका Project Service Automation में मानों को प्रदर्शित करती है.

    | मान | विवरण   |
    |-------|---------------|
    | 1     | नेट 30        |
    | 2     | 2% 10, नेट 30 |
    | 3     | नेट 45        |
    | 4     | नेट 60        |

## <a name="power-query"></a>Power Query

यदि निम्न शर्तें पूरी की जाती हैं, तो डेटा को फ़िल्टर करने के लिए Excel के लिए Microsoft Power Query का उपयोग करें:

- आपके पास Dynamics 365 Sales में बिक्री आदेश हैं.
- Project Service Automation में आपके पास कई संगठनात्मक इकाईयाँ हैं, और इन संगठनात्मक इकाईयों का Finance में कई कानूनी निकायों में मानचित्रण किया जाएगा.

यदि आपको Power Query का उपयोग करना ही है, तो इन दिशानिर्देशों का पालन करें:

- परियोजना और अनुबंध (PSA से Fin और Ops) टेम्पलेटों में एक डिफ़ॉल्ट फ़िल्टर है जिसमें **कार्य आइटम (msdyn\_ordertype = 192350001)** प्रकार के केवल बिक्री आदेश शामिल हैं. यह फ़िल्टर यह गारंटी देने में मदद करता है कि Finance में बिक्री आदेशों के लिए परियोजना अनुबंध नहीं बनाए जाते हैं. यदि आप अपना टेम्पलेट बनाते हैं, तो आपको यह फिल्टर जोड़ना होगा.
- एक ऐसा Power Query फ़िल्टर बनाएँ, जिसमें केवल अनुबंध संगठन शामिल हों, जिन्हें एकीकरण कनेक्शन सेट के कानूनी निकाय के साथ सिंक्रनाइज़ किया जाना चाहिए. उदाहरण के लिए, आपके वे परियोजना अनुबंध जो Contoso यूएस की अनुबंध संगठनात्मक इकाई के साथ हैं, उन्हें यूएसएसआई कानूनी निकाय से सिंक्रनाइज़ किया जाना चाहिए, लेकिन आपके वे परियोजना अनुबंध जो Contoso ग्लोबल के अनुबंध संगठनात्मक इकाई के साथ हैं, उन्हें यूएसएमएफ कानूनी निकाय से सिंक्रनाइज़ किया जाना चाहिए. यदि आप इस फ़िल्टर को अपने कार्य मानचित्रण में नहीं जोड़ते हैं, तो सभी परियोजना अनुबंध अनुबंध संगठनात्मक इकाई की परवाह किए बिना, कनेक्शन सेट के लिए परिभाषित कानूनी निकाय से सिन्क्रोनाइज हो जाएगा.

## <a name="template-mapping-in-data-integration"></a>डेटा इंटीग्रेशन में टेम्पलेट मैपिंग

> [!NOTE] 
> **CustomerReference** **AddressCity**, **AddressCountryRegionID**, **AddressDescription**, **AddressLine1**, **AddressLine2**, **AddressState**, और **AddressZipCode** फ़ील्ड परियोजना अनुबंधों के लिए डिफॉल्ट मानचित्रण में शामिल नहीं हैं. यदि आपको आवश्यकता लगती है कि यह डेटा परियोजना अनुबंधों के लिए सिन्क्रोनाइज हो जाए तो आप मानचित्रण जोड़ सकते हैं.
>
> **विवरण**, **ParentID**, **ProjectGroup**, **ProjectManagerPersonnelNumber**, और **ProjectType** फ़ील्ड परियोजनाओं के लिए डिफ़ॉल्ट मानचित्रण में शामिल नहीं हैं. यदि आपको आवश्यकता लगती है कि यह डेटा परियोजना के लिए सिन्क्रोनाइज हो जाए तो आप मानचित्रण जोड़ सकते हैं.

निम्नलिखित चित्र डेटा एकीकरण में टेम्पलेट कार्य मानचित्रण का उदाहरण प्रदर्शित करते हैं. मानचित्रण फील्ड की जानकारी को प्रदर्शित करता है जिसे Project Service Automation से Finance तक सिन्क्रोनाइज्ड किया जाएगा.

[![परियोजना अनुबंध टेम्पलेट मैपिंग](./media/ProjectContractTemplateMapping.JPG)](./media/ProjectContractTemplateMapping.JPG)

[![परियोजना टेम्पलेट मैपिंग](./media/ProjectTemplateMapping.JPG)](./media/ProjectTemplateMapping.JPG)

[![परियोजना अनुबंध पंक्ति टेम्पलेट मैपिंग](./media/ProjectContractLinesMapping.JPG)](./media/ProjectContractLinesMapping.JPG)

[![परियोजना अनुबंध पंक्ति माइलस्टोन टेम्पलेट मैपिंग](./media/ProjectContractLineMilestonesMapping.JPG)](./media/ProjectContractLineMilestonesMapping.JPG)

#### <a name="project-contract-line-milestone-mapping-in-the-projects-and-contracts-psa-3x-to-dynamics---v2-template"></a>परियोजनाओं और अनुबंधों में परियोजना अनुबंध लाइन उपलब्धि मानचित्रण (PSA 3.x से Dynamics) - v2 टेम्पलेट:

[![परियोजना अनुबंध लाइन माइलस्टोन मैपिंग संस्करण दो टेम्पलेट के साथ](./media/ProjectContractLineMilestoneMapping_v2.jpg)](./media/ProjectContractLineMilestoneMapping_v2.jpg)


[!INCLUDE[footer-include](../includes/footer-banner.md)]