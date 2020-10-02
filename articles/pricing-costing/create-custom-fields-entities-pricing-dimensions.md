---
title: मूल्य निर्धारण आयामों के रूप में कस्टम फ़ील्ड और निकाय बनाएँ
description: यह विषय कस्टम विकल्प सेट या निकाय बनाने के बारे में जानकारी देता है.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 2000f7e710267560fe2bd52b0e33024617d108ea
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898263"
---
# <a name="create-custom-fields-and-entities-as-pricing-dimensions"></a>मूल्य निर्धारण आयामों के रूप में कस्टम फ़ील्ड और निकाय बनाएँ

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

निम्नलिखित चरणों को किसी भी समय पूरा करें, जिनको आप कस्टम विकल्प सेट या निकाय बनाना चाहते हैं.

> [!IMPORTANT]
> हम सिफारिश करते हैं कि आप एक अलग समाधान में सभी कस्टम मूल्य निर्धारण आयाम परिवर्तन करें। यह महत्वपूर्ण सर्वोत्तम अभ्यास भविष्य में आवश्यकतानुसार परिवर्तन या अपडेट करने के लिए लचीलापन प्रदान करता है, आपके काम के पुन: उपयोग में मदद करेगा, और इन परिवर्तनों को दूसरे उदाहरण में पोर्ट करना आसान बनाता है। आपके द्वारा सभी आवश्यक परिवर्तन किए जाने के बाद, इस समाधान को **प्रबंधित समाधान** के रूप में निर्यात करें और अपने मूल्य निर्धारण सेटअप का पुन: उपयोग करने के लिए इसे अन्य उदाहरणों में आयात करें।


## <a name="create-a-custom-solution-for-pricing-dimensions"></a>मूल्य निर्धारण आयामों के लिए एक कस्टम समाधान बनाएं
1. **सेटिंग्स** > **समाधान** पर जाएँ, और फिर नया समाधान बनाने के लिए **नया** चुनें. 
2. समाधान का नाम दें, **\<your organization name> मूल्य निर्धारण के आयामों**, शेष आवश्यक जानकारी दर्ज करें और फिर **सहेजें** चुनें.
  
## <a name="create-custom-fields-and-option-sets-in-the-pricing-dimension-solution"></a>मूल्य निर्धारण आयाम समाधान में कस्टम फ़ील्ड और विकल्प सेट बनाएं

एक मूल्य निर्धारण आयाम विकल्प सेट या इकाई हो सकता है। दोनों को आपके मूल्य निर्धारण समाधान में बनाया जाना चाहिए। इस प्रक्रिया के चरण बताते हैं कि इकाई-आधारित आयाम और विकल्प सेट-आधारित आयाम कैसे बनाएं।

### <a name="entity-based-dimensions"></a>इकाई-आधारित आयाम

1. **समायोजन** > **समाधान** पर जाएँ, और तब डबल-क्लिक करें **\<your organization name> मूल्य निर्धारण के आयाम**.
2. Solution Explorer में, बाएं नेविगेशन पैन पर, **इकाइयां** चुनें।
3. मानक लीड सत्व **मानक शीर्षक** नामक एक नई निकाय बनाने के लिए **नया** चुनें. 
4. शेष आवश्यक जानकारी दर्ज करें और फिर **सहेजें** चुनें.


### <a name="option-set-based-dimensions"></a>विकल्प सेट-आधारित आयाम 
आप दो विकल्प सेट-आधारित आयाम बना सकते हैं। **घर** कार्य स्थान और **ऑनसाइट** काम की कीमत को ट्रैक करने के लिए **संसाधन कार्य स्थान** का उपयोग करें और काम पूरा होने पर मार्कअप लागू करने के लिए **संसाधन कार्य के घंटे** को मूल्य **नियमित** और **ओवरटाइम** के साथ उपयोग करें।


1. **समायोजन** > **समाधान** पर जाएँ, और डबल-क्लिक करें  **\<your organization name> मूल्य निर्धारण के आयाम**. 
2. समाधान एक्स्प्लोरर में, बाएं नेविगेशन पैन पर, **विकल्प सेट** का चयन करें। 
3. नया विकल्प सेट करने के लिए **नया** चुनें, बाकी आवश्यक जानकारी दर्ज करें और फिर **सहेजें** चुनें.

## <a name="create-data-for-entity-based-dimensions"></a>इकाई-आधारित आयामों के लिए डेटा बनाएं

आप इकाई-आधारित आयामों के लिए मैनुअल रूप से या Microsoft Excel आयात या सेवा कॉल का उपयोग करके डेटा बना सकते हैं। दो मानक शीर्षक बनाने के लिए इस प्रक्रिया में चरणों का उपयोग करें, इकाई-आधारित आयाम, **मानक शीर्षक** से **सिस्टम इंजीनियर** और **वरिष्ठ सिस्टम इंजीनियर**। यदि आप जो डेटा बनाना चाहते हैं वह छोटा है, तो निम्न उदाहरण में, आप एक मानक फॉर्म का उपयोग कर सकते हैं।

1. **उन्नत खोज** चुनें, निकाय **मानक शीर्षक** चुनें और फिर **परिणाम** चुनें. **मानक शीर्षक** इकाई में सभी पंक्तियों को दिखाया जाएगा।
2. **नया** चुनें, और **नाम** फ़ील्ड में, "सिस्टम इंजीनियर" दर्ज करें और फिर **सहेजें** चुनें.
3. प्रपत्र बंद करें. 
4. "सीनियर सिस्टम्स इंजीनियर" के लिए एक और मानक शीर्षक बनाने के लिए चरण 1 - 3 को दोहराएं।

## <a name="add-all-required-entities-and-related-components-to-the-pricing-dimension-solution"></a>मूल्य निर्धारण आयाम समाधान के लिए सभी आवश्यक संस्थाओं और संबंधित हिस्सों को जोड़ें
आपको अपने मूल्य निर्धारण समाधान में निम्नलिखित इकाइयों को जोड़ना होगा. मूल्य निर्धारण समाधान में कुछ महत्वपूर्ण स्कीमा परिवर्तन करने के लिए इस प्रक्रिया में चरणों का उपयोग करें ताकि इकाइयां नए मूल्य निर्धारण आयामों से अवगत हो सकें।

1. **समायोजन** > **समाधान** चुनें, और डबल-क्लिक करें **\<your organization name> मूल्य निर्धारण के आयाम**. 
2. समाधान एक्सप्लोरर में, बाएं नेविगेशन पैन पर, **मौजूदा जोड़ें** > **इकाइयां** चुनें।
3. **समाधान हिस्से** संवाद बॉक्स में, निम्नलिखित इकाइयों का चयन करें:

  - वास्तविक
  - बुक करने योग्य संसाधन
  - अनुमान पंक्ति
  - इनवॉइस पंक्ति विवरण
  - जर्नल पंक्ति
  - प्रोजेक्ट अनुबंध लाइन विवरण
  - परियोजना टीम सदस्य
  - कोट पंक्ति विवरण
  - भूमिका मू्ल्य मार्कअप
  - भूमिका मू्ल्य 
  - समय प्रविष्टि 


> [!NOTE]
> चयनित सभी संस्थाओं के लिए सभी फॉर्मों और दृश्य को शामिल करना सुनिश्चित करें।

4. जब ऊपर चयनित संस्थाओं के लिए किसी भी निर्भर संस्थाओं को शामिल करने के लिए कहा जाए, तो **नहीं** चुनें.
