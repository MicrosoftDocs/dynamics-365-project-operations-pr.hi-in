---
title: Project Operations ड्यूल-राइट एकीकरण
description: Project Operations ड्यूल-राइट एकीकरण अवलोकन.
author: sigitac
ms.date: 04/28/2021
ms.topic: overview
ms.prod: ''
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 9b57b8bab9a6821e71a16b191804af21ae5d0b5a
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/14/2022
ms.locfileid: "8582758"
---
# <a name="project-operations-dual-write-integration-overview"></a>Project Operations ड्यूल-राइट एकीकरण अवलोकन

_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations_

परियोजना संचालन का उपयोग करता है [दोहरी-लिखने की क्षमता](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-home-page) डेटा को सिंक्रनाइज़ करने के लिए Microsoft Dataverse और Dynamics 365 Finance.

निम्नलिखित चित्रण बताता है कि डेटा को Dataverse और फाइनेंस के बीच इस एकीकरण के हिस्से के रूप में कैसे सिंक्रनाइज़ किया गया है.

![Project Operations डेटा प्रवाह अवलोकन.](./media/ProjectOperationsFlows.jpg)

Dataverse पर Project Operations Power Platform क्षमताओं का उपयोग करके एक आधुनिक उपयोगकर्ता इंटरफ़ेस (UI) और आसान नो-कोड/कम-कोड विस्तारणीयता प्रदान करता है. प्रोजेक्ट मैनेजर, रिसोर्स मैनेजर, प्रोजेक्ट टीम के सदस्य और अन्य फ्रंट-ऑफिस व्यक्ति, Dataverse पर Project Operations में अपनी गतिविधियां प्रदर्शित करते हैं.

फाइनैंस में Project Operations प्रोजेक्ट लेखांकन और राजस्व मान्यता सहायता प्रदान करता है. Project Operations बिक्री कर गणना, मुद्रा विनिमय दरों, वित्तीय आयाम रिपोर्टिंग इत्यादि के लिए फाइनेंस में फाइनेंशियल फ्रेमवर्क के लिए प्लग करता है. प्रोजेक्ट अकाउंटेंट के अनुभव ज्यादातर फाइऩेंस आधारित होते हैं.

Project Operations एकीकरण में निम्नलिखित घटक एकीकरण शामिल हैं:


- [Project Operations सेटअप और कॉन्फ़िगरेशन डेटा एकीकरण](resource-dual-write-setup-integration.md) 
- [परियोजना अनुमान और वास्तविक आकड़ें](resource-dual-write-estimates-actuals.md)
- [परियोजना इनवॉइस](resource-dual-write-project-invoice.md)
- [व्यय प्रबंधन](resource-dual-write-expense.md)
- [विक्रेता इनवॉइस](resource-dual-write-vendor-invoice.md)
