---
title: Project Service Automation से सीधे Finance and Operations में परियोजना कार्यों को सिंक्रनाइज़ करें
description: यह विषय टेम्प्लेट और अंतर्निहित कार्य का वर्णन करता है जिसका इस्तेमाल परियोजना कार्यों को सीधे Microsoft Dynamics 365 Project Service Automation से Dynamics 365 Finance में सिंक्रनाइज़ करने के लिए किया जाता है.
author: KimANelson
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: d7f32327-33c4-43ab-b799-786210e93277
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 66a255346727c7ee4fbbf2920d2ef437ded03308
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3752080"
---
# <a name="synchronize-project-tasks-directly-from-project-service-automation-to-finance-and-operations"></a>Project Service Automation से सीधे Finance and Operations में परियोजना कार्यों को सिंक्रनाइज़ करें

[!include[banner](../includes/banner.md)]

यह विषय टेम्प्लेट और अंतर्निहित कार्य का वर्णन करता है जिसका इस्तेमाल परियोजना कार्यों को सीधे Dynamics 365 Project Service Automation से Dynamics 365 Finance में सिंक्रनाइज़ करने के लिए किया जाता है.

> [!NOTE]
> - परियोजना कार्य एकीककरण, व्यय लेनदेन श्रेणियां, घंटा अनुमान, व्यय अनुमान, और कार्यात्मकता लॉकिंग वर्शन 8.0 में उपलब्ध है.
> - अगर आप KB 4132657 और KB 4132660 इंस्टॉल करने के बाद, Enterprise Edition 7.3.0 इस्तेमाल कर रहे हैं तो आप परियोजना कार्यों, व्यय लेनदेन श्रेणियों, घंटे के अनुमानों, व्यय के अनुमानों और वास्तविक आकड़ों को एकीकृत करने के लिए टेम्पलेट्स का इस्तेमाल करने और कार्यात्मकता को कॉन्फ़िगर करने में सक्षम होंगे. यदि आपको लेखांकन वितरणों को रीसेट करना ही है, तो हम अनुशंसित करते हैं कि आप KB 4131710 को भी इंस्टॉल करें.
> - वास्तविक आंकड़ों का एकीकरण वर्शन 8.0.1 और आगे के वर्शन में उपलब्ध है.

## <a name="data-flow-for-project-service-automation-to-finance"></a>Project Service Automation से Finance के लिए डेटा प्रवाह

Project Service Automation से Finance एकीकरण समाधान Project Service Automation और Finance के उदाहरणों में डेटा सिन्क्रोनाइज करने के लिए डेटा एकीकरण सुविधा का उपयोग करता है. डेटा एकीकरण सुविधा के साथ उपलब्ध एकीकरण टेम्पलेट Project Service Automation से वित्त तक परियोजना कार्य के बारे में डेटा के प्रवाह को सक्षम करता है.

निम्नलिखित दृष्टांत दर्शाता है कि Project Service Automation और Finance के बीच डेटा को सिन्क्रोनाइज कैसे किया जाता है.

[![वित्त के साथ Project Service Automation एकीकरण के लिए डेटा प्रवाह](./media/ProjectTasksFlow.png)](./media/ProjectTasksFlow.png)

## <a name="template-and-task"></a>टेम्पलेट और कार्य

टेम्पलेट तक पहुंचने के लिए, Microsoft Power Apps एडमिन सेंटर में, **परियोजना** का चयन करें, और फिर, ऊपरी-दाएं कोने में, सार्वजनिक टेम्पलेट्स का चयन करने के लिए **नई परियोजना** का चयन करें.

यह विषय टेम्प्लेट और अंतर्निहित कार्य का वर्णन करता है जिसका इस्तेमाल परियोजना कार्यों को सीधे Project Service Automation से Finance में सिंक्रनाइज़ करने के लिए किया जाता है.

- **डेटा एकीकरण में टेम्पलेट का नाम:** परियोजना कार्य (PSA से Fin और Ops)
- **परियोजना में कार्य का नाम:** परियोजना के कार्य

परियोजना कार्यों का सिंक्रनाइज़ेशन होने से पहले, आपको परियोजना अनुबंधों और परियोजनाओं को सिंक्रनाइज़ करना होगा.

## <a name="entity-set"></a>निकाय सेट

| Project Service Automation | वित्त                             |
|----------------------------|-------------------------------------|
| परियोजना कार्य              | परियोजना कार्य के लिए एकीकरण निकाय |

## <a name="entity-flow"></a>निकाय प्रवाह

परियोजना कार्यों को Project Service Automation में प्रबंधित किया जाता है, और उन्हें परियोजना गतिविधियों के रूप में Finance में सिंक्रनाइज़ किया जाता है.

## <a name="prerequisites-and-mapping-setup"></a>आवश्यकताएँ और मानचित्रण सेटअप

परियोजना कार्यों का सिंक्रनाइज़ेशन होने से पहले, आपको परियोजना अनुबंधों और परियोजनाओं को सिंक्रनाइज़ करना होगा.

## <a name="power-query"></a>Power Query

अगर यह शर्त पूरी होती है तो आपको डेटा फ़िल्टर करने के लिए Excel के लिए Microsoft Power Query का उपयोग करना चाहिए:

- आपके पास परियोजना कार्य में संसाधन-विशिष्ट रिकॉर्ड होते हैं.

यदि आपको Power Query का उपयोग करना ही है, इस दिशानिर्देश का पालन करें:

- परियोजना कार्यों (PSA से Fin and Ops में) टेम्पलेट में डिफ़ॉल्ट फ़िल्टर होता है, जो **IsLineTask** से **गलत** पर फ़िल्टर सेट करके किसी परियोजना कार्य से संसाधन-विशिष्ट रिकॉर्ड को अलग करता है. यदि आप अपना टेम्पलेट बनाते हैं, तो आपको यह फिल्टर जोड़ना होगा.

## <a name="template-mapping-in-data-integration"></a>डेटा इंटीग्रेशन में टेम्पलेट मैपिंग

निम्नलिखित चित्रण डेटा इंटीग्रेशन में टेम्पलेट टास्क मैपिंग का उदाहरण दिखाता है. मानचित्रण फील्ड की जानकारी को प्रदर्शित करता है जिसे Project Service Automation से Finance तक सिन्क्रोनाइज्ड किया जाएगा.

-[![टेम्पलेट मैपिंग](./media/ProjectTasksMapping.png)](./media/ProjectTasksMapping.png)
