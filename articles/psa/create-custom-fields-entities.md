---
title: कस्टम फ़ील्ड और एंटिटी बनाएँ
description: यह विषय बताता है कि Power Apps प्लेटफ़ॉर्म में अपने स्वयं के समाधान में विकल्प सेट और इकाईयाँ कैसे बनाएं.
author: Rumant
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 10/01/2020
ms.topic: article
ms.service: business-applications
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: b9e32c8871a8986ba827f742baf4e4d5cd9dd235
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/10/2021
ms.locfileid: "5144865"
---
# <a name="create-custom-fields-and-entities"></a>कस्टम फ़ील्ड और एंटिटी बनाएँ 

[!include [banner](../includes/psa-now-project-operations.md)]

निम्नलिखित चरणों को किसी भी समय पूरा करें, जिनको आप Power Apps प्लेटफ़ॉर्म पर कस्टम विकल्प सेट या इकाई बनाना चाहते हैं।  
Project Service Automation (PSA) के वेब इंटरफेस का उपयोग करके इस विषय की प्रक्रियाओं को पूरा किया जाना चाहिए।

> [!IMPORTANT]
> हम सिफारिश करते हैं कि आप एक अलग समाधान में सभी कस्टम मूल्य निर्धारण आयाम परिवर्तन करें। यह महत्वपूर्ण सर्वोत्तम अभ्यास भविष्य में आवश्यकतानुसार परिवर्तन या अपडेट करने के लिए लचीलापन प्रदान करता है, आपके काम के पुन: उपयोग में मदद करेगा, और इन परिवर्तनों को दूसरे उदाहरण में पोर्ट करना आसान बनाता है। आपके द्वारा सभी आवश्यक परिवर्तन किए जाने के बाद, इस समाधान को **प्रबंधित समाधान** के रूप में निर्यात करें और अपने मूल्य निर्धारण सेटअप का पुन: उपयोग करने के लिए इसे अन्य उदाहरणों में आयात करें।

  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a>मूल्य निर्धारण आयाम समाधान में कस्टम फ़ील्ड और विकल्प सेट बनाएं

एक मूल्य निर्धारण आयाम विकल्प सेट या इकाई हो सकता है। दोनों को आपके मूल्य निर्धारण समाधान में बनाया जाना चाहिए। इस प्रक्रिया के चरण बताते हैं कि इकाई-आधारित आयाम और विकल्प सेट-आधारित आयाम कैसे बनाएं।

### <a name="entity-based-dimensions"></a>इकाई-आधारित आयाम

1. PSA में, **सेटिंग** > **समाधान** पर क्लिक करें, और उसके बाद **\<your organization name> के मूल्य निर्धारण आयाम पर डबल-क्लिक करें**.
2. Solution Explorer में, बाएं नेविगेशन पैन पर, **इकाइयां** चुनें।
3. **मानक शीर्षक** नामक एक नई इकाई बनाने के लिए **नया** पर क्लिक करें। शेष आवश्यक जानकारी दर्ज करें और फिर **सहेजें** पर क्लिक करें।

> ![मानक शीर्षक इकाई परिभाषा](media/Standard-Title-entity-definition.png)


### <a name="option-set-based-dimensions"></a>विकल्प सेट-आधारित आयाम 
आप दो विकल्प सेट-आधारित आयाम बना सकते हैं। **घर** कार्य स्थान और **ऑनसाइट** काम की कीमत को ट्रैक करने के लिए **संसाधन कार्य स्थान** का उपयोग करें और काम पूरा होने पर मार्कअप लागू करने के लिए **संसाधन कार्य के घंटे** को मूल्य **नियमित** और **ओवरटाइम** के साथ उपयोग करें।


1. PSA में, **सेटिंग** > **समाधान** पर क्लिक करें, और उसके बाद **\<your organization name> के मूल्य निर्धारण आयाम पर डबल-क्लिक करें**. 
2. समाधान एक्स्प्लोरर में, बाएं नेविगेशन पैन पर, **विकल्प सेट** का चयन करें। 
3. नया विकल्प सेट करने के लिए **नया** पर क्लिक करें, बाकी आवश्यक जानकारी दर्ज करें और फिर **सहेजें** पर क्लिक करें।

> ![विकल्प सेट आधारित मूल्य निर्धारण आयाम जिसे संसाधन कार्य स्थान कहा जाता है ](media/Option-set-PD-called-Resource-Work-Location.png)

> ![विकल्प सेट आधारित मूल्य निर्धारण आयाम जिसे संसाधन कार्य घंटे कहा जाता है ](media/Option-set-PD-called-Resource-Work-Hours.PNG)


## <a name="create-data-for-entity-based-dimensions"></a>इकाई-आधारित आयामों के लिए डेटा बनाएं

आप इकाई-आधारित आयामों के लिए मैनुअल रूप से या Microsoft Excel आयात या सेवा कॉल का उपयोग करके डेटा बना सकते हैं। दो मानक शीर्षक बनाने के लिए इस प्रक्रिया में चरणों का उपयोग करें, इकाई-आधारित आयाम, **मानक शीर्षक** से **सिस्टम इंजीनियर** और **वरिष्ठ सिस्टम इंजीनियर**। यदि आप जो डेटा बनाना चाहते हैं वह छोटा है, तो निम्न उदाहरण में, आप एक मानक फॉर्म का उपयोग कर सकते हैं।

1. PSA में, **उन्नत खोज** पर क्लिक करें। इकाई **मानक शीर्षक** का चयन करें और फिर **नतीजे** पर क्लिक करें। **मानक शीर्षक** इकाई में सभी पंक्तियों को दिखाया जाएगा।
2. **नया** पर क्लिक करें. **नाम** फ़ील्ड में, "सिस्टम इंजीनियर" दर्ज करें और फिर **सहेजें** पर क्लिक करें।
3. प्रपत्र बंद करें. 
4. "सीनियर सिस्टम्स इंजीनियर" के लिए एक और मानक शीर्षक बनाने के लिए चरण 1 - 3 को दोहराएं।

> ![मानक शीर्षक इकाई के लिए नमूना डेटा ](media/ST-data.png)

