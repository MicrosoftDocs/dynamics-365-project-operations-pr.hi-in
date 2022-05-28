---
title: Project Service Automation अवलोकन
description: यह विषय इसके बारे में जानकारी प्रदान करता है Dynamics 365 Project Service Automation Dynamics 365 Finance एकीकरण समाधान के लिए।
author: ruhercul
ms.date: 07/25/2019
ms.topic: overview
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: johnmichalak
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: ruhercul
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 1b8588e664f140ca1b0dd740d27fe6a5137da595
ms.sourcegitcommit: 2c2a5a11d446adec2f21030ab77a053d7e2da28e
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/04/2022
ms.locfileid: "8685518"
---
# <a name="project-service-automation-overview"></a>Project Service Automation अवलोकन

[!include[banner](../includes/banner.md)]


प्रोजेक्ट सर्विस ऑटोमेशन टू फाइनेंस इंटीग्रेशन सॉल्यूशन Dynamics 365 Finance के उदाहरणों में डेटा को सिंक्रोनाइज़ करने के लिए डेटा इंटीग्रेशन फीचर का उपयोग करता है और Dynamics 365 Project Service Automation के जरिए ।Common Data Service डेटा एकीकरण फ़ीचर के साथ उपलब्ध एकीकरण टेम्पलेट Project Service Automation से Finance में परियोजनाओं, परियोजना अनुबंधों, परियोजना अनुबंध लाइनों, परियोजना अनुबंध लाइन उपलब्धि, परियोजना कार्य, व्यय लेनदेन श्रेणियों और व्यय अनुमान के प्रवाह को सक्षम करते हैं.

> [!NOTE]
> - यदि आप वर्जन 7.3.0 का इस्तेमाल कर रहे हैं तो आपको KB 4074835 इंस्टॉल करना चाहिए. इसके बाद आप निर्धारित मूल्य परियोजनाओं को एकीकृत कर पाएंगे.
> - अगर आप 7.3.0 वर्शन का उपयोग कर रहे हैं, और आप Project Service Automation से शुल्क लेनदेन ला रहे हैं, तो आपको परियोजना इनवॉइस में उन शुक्लों को शामिल करने के लिए KB 4345320 इंस्टॉल करना होगा.
> - अगर आप वर्शन 8.0 का उपयोग कर रहे हैं, तो आप परियोजना कार्य एकीकरण, व्यय लेनदेन श्रणियों, घंटा अनुमानों, व्यय अनुमानों, तथा कार्यात्मकता लॉकिंग का उपयोग कर पाएंगे.
> - अगर आप वर्शन 8.0.1 का उपयोग कर रहे हैं, तो आप वास्तविक आंकड़ों को संकालित कर पाएंगे.

इससे पहले कि आप Project Service Automation फाइनेंस को एकीकृत करें, आपको Project Service Automation एकीकरण मानक को कन्फीगर करना होगा. और जानकारी: [Project Service Automation एकीकरण मानक](PSA-parameters.md) देखें.

एकीकरण का यह समाधान निम्न परिदृश्यों में सीधे संकालन को सक्रिय करता है:

- Project Service Automation में परियोजना अनुबंध को बरकरार रखता है, और उन्हें Project Service Automation से फाइनेंस में सीधे संकालित करता है.
- Project Service Automation में परियोजना तैयार करता है, तथा उन्हें Project Service Automation से फाइनेंस में सीधे संकालित करता है.
- Project Service Automation में परियोजना अनुबंध पंक्ति को बरकरार रखता है, और उन्हें Project Service Automation से फाइनेंस में सीधे संकालित करता है.
- Project Service Automation में परियोजना अनुबंध पंक्ति माइलस्टोन को बरकरार रखता है, और उन्हें Project Service Automation से फाइनेंस में सीधे संकालित करता है.
- Project Service Automation में परियोजना कार्यों को बरकरार रखता है, और उन्हें Project Service Automation से फाइनेंस में सीधे संकालित करता है.
- फाइनेंस में व्यय लेनदेन श्रेणियों को बरकरार रखता है और उन्हें फाइनेंस से सीधे Project Service Automation में संकालित करता है.
- Project Service Automation में परियोजना घंटा अनुमान को तैयार करता है, और उन्हें Project Service Automation से फाइनेंस में सीधे संकालित करता है.
- Project Service Automation में परियोजना व्यय अनुमान को तैयार करता है, और उन्हें Project Service Automation से फाइनेंस में सीधे संकालित करता है.
- Project Service Automation में परियोजना समय, व्यय और शुल्क के वास्तविक आंकड़े को तैयार करता है, और Project Service Automation एकीकरण जर्नल में परियोजना लेनदेन तैयार करता है ताकि उन्हें फाइनेंस में पोस्ट किया जा सके.

## <a name="data-synchronization"></a>डेटा सिंक्रोनाइज़ेशन

निम्न चित्रण दिखाता है कि आंकड़े Project Service Automation और फाइनेंस के बीच एकीकरण के रूप में किस तरह से संकालित होते हैं.

> [!NOTE]
> सभी टेम्प्लेट अभी उपलब्ध नहीं हैं. पूरा होते हैं टेम्प्लेट जारी किया जाएगा.

[![फाइनेंस के साथ Project Service Automation का एकीकरण.](./media/PSA-integration.png)](./media/PSA-integration.png)

## <a name="system-requirements-for-finance"></a>वित्त के लिए सिस्टम आवश्यकताएँ

फाइनेंस एकीकरण समाधान में Project Service Automation के उपयोग के लिए, आपको प्लेटफॉर्म अपडेट 12 या बाद वाले अपडेट के साथ Enterprise Edition 7.3 इंस्टॉल करना होगा.

## <a name="system-requirements-for-project-service-automation"></a>सिस्टम को Project Service Automation की जरूरत है

फाइनेंस एकीकरण समाधान में Project Service Automation के उपयोग के लिए, आपको निम्नलिखित घटक इंस्टॉल करने होंगे.

- Dynamics 365 Project Service Automation संस्करण 9.0.0.0 या बाद का संस्करण
- Dynamics 365 Sales, वर्शन 1.14.0.0 (v14) या आगे के वर्शन के लिए नकदी समाधान की संभावना
- Dynamics 365 Project Service Automation वर्शन1.0.0.0 या आगे के वर्शन के लिए Project Service Automation टू फाइनेंस समाधान

## <a name="install-the-project-service-automation-to-finance-integration-solution-in-your-project-service-automation-instance"></a>Project Service Automation टू फाइनेंस एकीकरण समाधान को अपने Project Service Automation आवृत्ति में इंस्टॉल करें

Project Service Automation टू फाइनेंस एकीकरण समाधान को [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=57016) से डाउनलोड करें, और समाधान के साथ शामिल निर्देशों का पालन करें.


[!INCLUDE[footer-include](../includes/footer-banner.md)]