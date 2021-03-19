---
title: कार्य की विवरण संरचना के लिए अपग्रेड संबंधी विचार
description: इस टॉपिक में Project Service Automation 2.x से 3.x के मामले में कार्य की विवरण संरचना को अपग्रेड करने के बारे में जानकारी प्रदान की गई है।
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 10/18/2019
ms.topic: article
author: ruhercul
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: a067521410f0fe0d8f5d4c510a35f2a3b018dce3
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281750"
---
# <a name="upgrade-considerations-for-the-work-breakdown-structure"></a>कार्य की विवरण संरचना के लिए अपग्रेड संबंधी विचार

[!include [banner](../includes/psa-now-project-operations.md)]

इस टॉपिक में Project Service Automation 2.x से 3.x के मामले में कार्य की विवरण संरचना को अपग्रेड करने के बारे में जानकारी प्रदान की गई है। इस टॉपिक में Project Service Automation (PSA) में किसी परियोजना के स्वास्थ्य को परिभाषित किया गया है, जो सफल अपग्रेड के लिए आवश्यक है। आम पायी जाने वाली ब्लॉकिंग परिस्थितियों के बारे में भी जानकारी दी गई है, जो अपग्रेड को विफल बना सकती हैं। किसी परियोजना शेड्यूल में परियोजना टास्क और उनके कार्यों को परिभाषित करने के बारे में अधिक जानकारी के लिए [प्रोजेक्ट शेड्यूल](project-creating.md) देखें।

## <a name="key-entities"></a>प्रमुख इकाइयां
पहले से ही संसाधनों से लैस किसी सटीक कार्य विवरण संरचना को परिभाषित करने हेतु आपको निम्न इकाइयों की आवश्यकता होगी:

- [परियोजना](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project)
- [परियोजना टीम](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam)
- [परियोजना कार्य](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask)
- [संसाधन असाइनमेंट](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment)
- [परियोजना कार्य निर्भरता](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency)
- [बुक करने योग्य संसाधन](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/bookableresource)

संसाधनों से लैस किसी कार्य विवरण संरचना को परिभाषित करने हेतु आपको निम्न चरण पूरे करने होंगे:

1. कोई नई परियोजना बनाएं। नई परियोजना बनाने के बारे में अधिक जानकारी के लिए [msdyn_project](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_project) देखें।
2. एक या एक से अधिक टास्क बनाएं। टास्क बनाने के तरीके के बारे में अधिक जानकारी के लिए [msdyn_projecttask](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttask).
3. टास्क की डिपेंडेंसी को परिभाषित करें। अधिक जानकारी के लिए, देखें [परियोजना कार्य निर्भरता](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projecttaskdependency) ।
4. परियोजना टीम के सदस्यों को परियोजना एसाइन करें। अधिक जानकारी के लिए [msdyn_projectteam](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_projectteam) देखें।
5. परियोजना टीम के सदस्यों को कार्य एसाइन करें। अधिक जानकारी के लिए [msdyn_resourceassignment](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/developer/entities/msdyn_resourceassignment) देखें।

## <a name="project-team-relationships"></a>परियोजना टीम के संबंध

सफल अपग्रेड पाने के लिए निम्न संबंधों को सही ढंग से बनाए रखा जाना चाहिए:
- परियोजना टीम के सभी सदस्य किसी बुक करने-योग्य संसाधन से जुड़े होने चाहिए।
- परियोजना टीम के सभी सदस्य उसी परियोजना से जुड़े होने चाहिए। 

## <a name="project-task-relationships"></a>परियोजना टास्क से जुड़े संबंध
सफल अपग्रेड पाने के लिए निम्न संबंधों को सही ढंग से बनाए रखा जाना चाहिए:

- कोई भी संबंधित टास्क उसी परियोजना से ही जुड़े होने चाहिए।
- हर लाइन टास्क में एक पैरेंट टास्क होना चाहिए।
- प्रत्येक टास्क के लिए एक पैरेंट परियोजना होनी चाहिए।

### <a name="valid-conditions"></a>मान्य स्थितियां

- सभी टास्क की अवधि एक घंटे के बराबर या उससे अधिक (> =) और 1,800,000 मिनट (1,250 दिन) से कम होनी चाहिए.*
- किसी भी टास्क की प्रारंभ तिथि 2000/01/01 से पहले की नहीं होनी चाहिए.*
- किसी भी टास्क की प्रारंभ तिथि आज से 17 साल के बाद वाली नहीं होनी चाहिए.*
- सभी टास्क की प्रारम्भ तिथि उनकी समाप्ति तिथि के बराबर या उससे पहले होनी चाहिए.
- क्लासिफिकेशन से जुड़े सभी लेनदेन के मामलों (व्यय, सामग्री, टैक्स और समय) में **डिफ़ॉल्ट यूनिट** और **यूनिट समूह** के लिए मान होना चाहिए।
- तिथि के अक्षरों वाले फॉर्मेट से परेहज करें।

### <a name="potential-mitigation-steps"></a>संभावित मिटीगेशन चरण
- उन परियोजना कार्यों की पहचान करने के लिए उन्नत खोज का उपयोग करें, जिनकी कोई परियोजना आईडी नहीं है.
- उन परियोजना कार्यों की पहचानने के लिए उन्नत खोज का उपयोग करें, जहां शेड्यूल की गई अवधि > 1,800,000 से अधिक है.
- कोई भी डेटा परिवर्तन करने से पहले, आपको उस इकाई से जुड़े किसी भी अनुकूलन की जांच करनी चाहिए जिसके कारण डेटा खराब स्थिति में आ सकता है. किसी भी डेटा-संबंधित अपडेट के साथ आगे बढ़ने से पहले इन अनुकूलन को संबोधित किया जाना चाहिए.
- ओरफनड के रूप में पहचाने गए कार्यों के लिए, यदि इन कार्यों की आवश्यकता नहीं है या यदि वे सही पैरेंट परियोजना से जुड़े होने चाहिए, तो इन्हें हटाने पर विचार करें.
- ऐसे किसी भी कार्य के लिए, जहां अवधि 1,250 दिनों से अधिक है, यदि संभव हो, तो कुल अवधि दर्शाने के लिए कई कार्यों को जोड़ने पर विचार करें.

> [!NOTE]
> तारे के चिह्न (\*) वाली आइटमों की सीमाएं हैं, जो इस तथ्य के कारण हैं कि कस्टमर रिलेशनशिप मैनेजमेंट (CRM) केवल 7,320 रेकरेन्स एक्सपेंशन को समर्थित करता है. आपको इस सीमा के अंदर ही रहना है।

## <a name="resource-assignment-relationships"></a>संसाधनों की एसाइनमेंट से जुड़े संबंध
सफल अपग्रेड पाने के लिए निम्न संबंधों को सही ढंग से बनाए रखा जाना चाहिए:

- कार्य विश्लेषण संरचना में एसाइन किए गए सभी संसाधन एक ही परियोजना से संबंधित होने चाहिए.
- कार्य विश्लेषण संरचना में एसाइन किए गए सभी संसाधन एक ही परियोजना के परियोजना टीम सदस्यों से संबंधित होने चाहिए.

### <a name="potential-mitigation-steps"></a>संभावित मिटीगेशन चरण
- उन सभी कार्यों की पहचान करें, जो उपरोक्त वर्णित शर्तों के बाहर हैं.  
- कोई भी संसाधन असाइनमेंट, जो अब मान्य नहीं हैं, उन्हें हटा दिया जाना चाहिए.

## <a name="project-task-dependency-relationships"></a>परियोजना टास्क डिपेंडेंसी संबंध
सफल अपग्रेड पाने के लिए निम्न संबंधों को सही ढंग से बनाए रखा जाना चाहिए:

- सभी परियोजना टास्क डिपेंडेंसी संबंध एक ही परियोजना से संबंधित होनी चाहिए।
- किसी टास्क की डिपेंडेंसी को एक से अधिक बार संदर्भित नहीं किया जा सकता है।


[!INCLUDE[footer-include](../includes/footer-banner.md)]