---
title: Finance and Operations और Project Service Automation के बीच परियोजना व्यय श्रेणियों को सिन्क्रोनाइज करें
description: यह विषय टेम्पलेट्स और अंतर्निहित कार्यों का वर्णन करता है जिनका उपयोग Microsoft Dynamics 365 Finance और Dynamics 365 Project Service Automation के बीच परियोजना व्यय श्रेणियों को सिन्क्रोनाइज करने के लिए किया जाता है.
author: Yowelle
ms.date: 07/20/2018
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
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: 52c79f8b641d4b2df3b30964331633f2487402f8f8d229b540f9544c0f848557
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 08/06/2021
ms.locfileid: "7001118"
---
# <a name="synchronize-project-expense-categories-between-finance-and-operations-and-project-service-automation"></a>Finance and Operations और Project Service Automation के बीच परियोजना व्यय श्रेणियों को सिन्क्रोनाइज करें

[!include[banner](../includes/banner.md)]

यह विषय टेम्पलेट्स और अंतर्निहित कार्यों का वर्णन करता है जिनका उपयोग Dynamics 365 Finance और Dynamics 365 Project Service Automation के बीच परियोजना व्यय श्रेणियों को सिन्क्रोनाइज करने के लिए किया जाता है.

> [!NOTE]
> - परियोजना कार्य एकीककरण, व्यय लेनदेन श्रेणियां, घंटा अनुमान, व्यय अनुमान, और कार्यात्मकता लॉकिंग वर्शन 8.0 में उपलब्ध है.
> - वास्तविक आंकड़ों का एकीकरण वर्शन 8.0.1 और आगे के वर्शन में उपलब्ध है.
> - अगर आप KB 4132657 और KB 4132660 इंस्टॉल करने के बाद, Enterprise Edition 7.3.0 इस्तेमाल कर रहे हैं तो आप परियोजना कार्यों, व्यय लेनदेन श्रेणियों, घंटे के अनुमानों, व्यय के अनुमानों और वास्तविक आकड़ों को एकीकृत करने के लिए टेम्पलेट्स का इस्तेमाल करने और कार्यात्मकता को कॉन्फ़िगर करने में सक्षम होंगे. यदि आपको लेखांकन वितरणों को रीसेट करना ही है, तो हम अनुशंसित करते हैं कि आप KB 4131710 को भी इंस्टॉल करें.

## <a name="data-flow-for-project-service-automation-and-finance"></a>Project Service Automation और Finance के लिए डेटा प्रवाह

Project Service Automation और Finance एकीकरण समाधान Project Service Automation और Finance के उदाहरणों में डेटा सिन्क्रोनाइज करने के लिए डेटा एकीकरण सुविधा का उपयोग करता है. एकीकरण टेम्पलेट्स जो डेटा एकीकरण सुविधा के साथ उपलब्ध हैं Finance और Project Service Automation के बीच परियोजना व्यय लेनदेन की श्रेणियों के बारे में डेटा के प्रवाह को सक्षम करते हैं.

यदि परियोजना व्यय श्रेणियों को Finance में महारत हासिल है, तो एकीकरण प्रवाह Finance से Project Service Automation तक प्रथम है. परियोजना व्यय श्रेणियों की एकीकरण IDs, Project Service Automation से Finance तक सिन्क्रोनाइजेशन के माध्यम से अपडेट होती हैं.

यदि परियोजना व्यय श्रेणियों को Project Service Automation में महारत हासिल है, तो एकीकरण प्रवाह Project Service Automation से Finance तक प्रथम है. Project Service Automation से सिन्क्रोनाइजेशन से पहले परियोजना श्रेणियों को पहले से ही Finance में कॉन्फ़िगर किया जाना चाहिए. फिर Finance से Project Service Automation के लिए वापस सिन्क्रोनाइज करें, और फिर Project Service Automation से Finance के लिए फिर से करें. इस तरह से, आप यह गारंटी देने में मदद करते हैं कि श्रेणियां जुड़ी हुई हैं, और कोई डुप्लिकेट नहीं बनाई जाती हैं.

> [!NOTE]
> आमतौर पर, परियोजना व्यय श्रेणियों को Finance में महारत हासिल है. हालांकि, यदि वे नहीं हैं, या यदि Project Service Automation में व्यय श्रेणियां पहले ही बनाई जा चुकी हैं, तो आपको पहले परियोजना व्यय लेनदेन की श्रेणियों (PSA से Fin और Ops) की टेम्पलेट का उपयोग करके सिन्क्रोनाइज करना होगा. फिर परियोजना व्यय लेनदेन की श्रेणियों (Fin और Ops से PSA) की टेम्पलेट का उपयोग करके सिन्क्रोनाइज करें. इसके बाद आपको Project Service Automation से Finance तक एक और बार सिन्क्रोनाइजेशन को चलाना चाहिए.
>
> यदि आप Project Service Automation से सिन्क्रोनाइज पहले करते हैं, तो सिन्क्रोनाइजेशन चलाने से पहले Finance में निम्नलिखित आवश्यकताओं को पूरा किया जाना चाहिए:
>
> - Project Service Automation में स्थापित परियोजना श्रेणी से मेल खाती साझा श्रेणी जरूर मौजूद होनी चाहिए, और इसे **परियोजना** और **व्यय** दोनों के लिए सक्षम होना जाना चाहिए.
> - प्रत्येक Finance legal निकाय के लिए जिसे एकीकृत किया जाना चाहिए, निम्नलिखित परियोजना श्रेणियां जरूर मौजूद होनी चाहिए:
>
>     - **प्रोजेक्ट श्रेणी** मौजूद है. 
>     - **व्यय में उपयोग** सक्षम है.
>     - **जर्नल में सक्रिय** सक्षम है.
>     - **लेनदेन के प्रकार** **खर्च** के लिए सेट है.

निम्नलिखित दृष्टांत दर्शाता है कि Project Service Automation और Finance के बीच डेटा को सिन्क्रोनाइज कैसे किया जाता है.

[![वित्त के साथ Project Service Automation एकीकरण के लिए डेटा प्रवाह.](./media/ProjectExpenseCategoriesFlow.png)](./media/ProjectExpenseCategoriesFlow.png)

## <a name="project-expense-category-synchronization-from-finance-to-project-service-automation"></a>Finance से Project Service Automation के लिए परियोजना व्यय श्रेणी सिन्क्रोनाइजेशन

### <a name="template-and-task"></a>टेम्पलेट और कार्य

टेम्पलेट तक पहुंचने के लिए, Microsoft Power Apps एडमिन सेंटर में, **परियोजना** का चयन करें, और फिर, ऊपरी-दाएं कोने में, सार्वजनिक टेम्पलेट्स का चयन करने के लिए **नई परियोजना** का चयन करें.

निम्नलिखित टेम्पलेट और अंतर्निहित कार्य का उपयोग Finance से Project Service Automation तक परियोजना व्यय श्रेणियों को सिन्क्रोनाइज करने के लिए किया जाता है:

- **डेटा एकीकरण में टेम्पलेट का नाम:** परियोजना व्यय लेनदेन की श्रेणियां (Fin और Ops से PSA)
- **परियोजना में कार्य का नाम:** PSA से श्रेणियों को सिंक करें

### <a name="entity-set"></a>निकाय सेट

| वित्त                           | Project Service Automation |
|-----------------------------------|----------------------------|
| श्रेणियों के लिए एकीकरण निकाय | लेन-देन श्रेणियाँ     |

### <a name="entity-flow"></a>निकाय प्रवाह

परियोजना व्यय श्रेणियों को Finance में प्रबंधित किया जाता है, और उन्हें लेनदेन श्रेणियों के रूप में Project Service Automation के लिए सिन्क्रोनाइज किया जाता है.

### <a name="power-query"></a>Power Query

जब आप Project Service Automation से सिन्क्रोनाइज कर रहे हैं, तो आपको लेनदेन श्रेणी पर बिलिंग प्रकार सेट करने के लिए Excel के लिए Microsoft Power Query का उपयोग करना होगा. परियोजना व्यय लेनदेन की श्रेणियों (Fin और Ops से PSA) का टेम्पलेट एक डिफ़ॉल्ट कॉलम और मानचित्रण प्रदान करता है. यदि आप अपना खुद का टेम्पलेट बनाते हैं, तो आपको Power Query में एक सशर्त कॉलम जोड़ना होगा. इन चरणों का अनुसरण करें.

1. परियोजना व्यय लेनदेन की श्रेणियों (Fin और Ops से PSA) के टेम्पलेट में परियोजना व्यय श्रेणियों के कार्य का मानचित्रण खोलने के लिए तीर पर क्लिक करें.
2. Power Query खोलने के लिए **उन्नत क्वेरी और फ़िल्टरिंग** लिंक पर क्लिक करें.
2. **सशर्त कॉलम जोड़ें** का चयन करें.
3. नए स्तंभ के लिए एक नाम दर्ज करें, जैसे **बिलिंग प्रकार**.
4. निम्नलिखित शर्त दर्ज करें: **यदि CATEGORYID शून्य के बराबर नहीं है तो 19235001, अन्यथा शून्य**.
5. कॉलम पर **ठीक है** पर क्लिक करें.
6. मानचित्रण पृष्ठ पर इस नए कॉलम का मानचित्र बनाना सुनिश्चित करें.

निम्नलिखित चित्रण डेटा इंटीग्रेशन में टेम्पलेट टास्क मैपिंग का उदाहरण दिखाता है. मानचित्रण फील्ड की जानकारी को प्रदर्शित करता है जिसे Finance से Project Service Automation तक सिन्क्रोनाइज्ड किया जाएगा.

[![परियोजना व्यय श्रेणी से Project Service Automation टेम्पलेट मैपिंग.](./media/ProjectExpenseCategoriesToPSAMapping.jpg)](./media/ProjectExpenseCategoriesToPSAMapping.jpg)

## <a name="project-expense-category-synchronization-from-project-service-automation-to-finance"></a>Project Service Automation to Finance के लिए परियोजना व्यय श्रेणी सिन्क्रोनाइजेशन

### <a name="template-and-task"></a>टेम्पलेट और कार्य

निम्नलिखित टेम्पलेट और अंतर्निहित कार्य का उपयोग Project Service Automation to Finance तक परियोजना व्यय श्रेणियों को सिन्क्रोनाइज करने के लिए किया जाता है:

- **डेटा एकीकरण में टेम्पलेट का नाम:** परियोजना व्यय लेनदेन की श्रेणियां (PSA से Fin और Ops)
- **परियोजना में कार्य का नाम:** Fin Ops से श्रेणियों को सिंक करें

### <a name="entity-set"></a>निकाय सेट

| Project Service Automation | वित्त                           |
|----------------------------|-----------------------------------|
| लेन-देन श्रेणियाँ     | श्रेणियों के लिए एकीकरण निकाय |

### <a name="entity-flow"></a>निकाय प्रवाह

परियोजना व्यय श्रेणियों को Finance में प्रबंधित किया जाता है, और उन्हें लेनदेन श्रेणियों के रूप में Project Service Automation के लिए सिन्क्रोनाइज किया जाता है. Finance के लिए वापस सिन्क्रोनाइजेशन Project Service Automation से एकीकरण ID के साथ Finance में परियोजना श्रेणी को अपडेट करता है.

### <a name="template-mapping-in-data-integration"></a>डेटा इंटीग्रेशन में टेम्पलेट मैपिंग

निम्नलिखित चित्रण डेटा इंटीग्रेशन में टेम्पलेट टास्क मैपिंग का उदाहरण दिखाता है.

> [!NOTE]
> मानचित्रण फील्ड की जानकारी को प्रदर्शित करता है जिसे Project Service Automation से Finance तक सिन्क्रोनाइज्ड किया जाएगा.

[![Project Service Automation से Finance टेम्पलेट मैपिंग.](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)](./media/ProjectExpenseCategoriesToFinOpsMapping.jpg)


[!INCLUDE[footer-include](../includes/footer-banner.md)]