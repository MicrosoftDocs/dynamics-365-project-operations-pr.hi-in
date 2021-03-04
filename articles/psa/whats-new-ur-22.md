---
title: Project Service Automation के अपडेट रिलीज़ 22, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 22, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 07/28/2020
ms.topic: article
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
ms.openlocfilehash: 456ed68bc1d74c2c8e5d2420a3f5d1fb8e0465d6
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4126620"
---
# <a name="project-service-automation-update-release-22-v3"></a>Project Service Automation V3 अद्यतन रिलीज़ 22, V3

हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं. यह रिलीज़ Dynamics 365 9.x के साथ संगत में है. इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 22 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है. इस संस्करण की बिल्ड संख्या V 3.10.33.48 है और यह आमतौर पर जून 2020 में एक स्व-अद्यतन के माध्यम से उपलब्ध है.

## <a name="update-release-22"></a>अपडेट रिलीज़ 22

### <a name="bug-fixes"></a>बग समाधान



**समय और व्यय**

निम्नलिखित मुद्दों को ठीक किया गया है:

- **समय प्रविष्टियाँ** आयात के बाद समय प्रविष्टि शेड्यूल में स्वचालित रूप से नहीं जोड़ी जाती हैं.
- **समय प्रविष्टि** ग्रिड दिनांक पिकर उपयोगकर्ता की क्षेत्रीय सेटिंग को नहीं पहचानता है.

**संसाधन प्रबंधन**

निम्नलिखित मुद्दों को ठीक किया गया है:

- मैनुअल मोड में, **संसाधन असाइनमेंट** रूपरेखा में परिवर्तन, **संसाधन आवश्यकताएं** जनरेट करते समय पहचाने नहीं जाते.
- **संसाधन अनुरोध** कस्टम अनुरोध स्थितियों का समर्थन नहीं करते.

**परियोजना प्रबंधन**

निम्नलिखित मुद्दों को ठीक किया गया है:

- EstimateGridControl पर डबल-क्लिक का उपयोग डच स्वरूप संख्याओं को सही ढंग से पार्स नहीं करेगा.
- Microsoft परियोजना डेस्कटॉप क्लाइंट ऐड-इन का उपयोग करके असाइनमेंट बदले जाने पर असाइन किए गए घंटे सही ढंग से अद्यतन नहीं होते हैं.
- जब अनुबंध मुद्रा, ग्राहक मुद्रा से भिन्न होती है और संगठन मुद्रा चिह्नों के बजाय मुद्रा कोड प्रदर्शित करने के लिए कॉन्फ़िगर की गई होती है, तो परियोजना ट्रैकिंग और अनुमान ग्रिड गलत विक्रय मुद्रा कोड प्रदर्शित करते हैं.
- यदि कार्य समय शेड्यूल 24 घंटे प्रति दिन है, तो टीम सदस्य का समाप्ति दिनांक एक दिन जोड़ देगा.
- परियोजना शेड्यूल पर, किसी कार्य के लिए लेन-देन श्रेणी को जोड़ना, स्वतः सहेजें को ट्रिगर नहीं करता है.
- परियोजना टेम्पलेट में टीम के सदस्य को जोड़ते समय निम्न त्रुटि प्रदर्शित होती है: "संसाधन आवश्यकताओं को परियोजना टेम्पलेट से संबद्ध नहीं किया जा सकता". 
- रिबन नियम स्क्रिप्ट "msdyn.Approval.CanApproveOrReject" एक टाइमआउट त्रुटि प्रदर्शित करती है.

**Sales**

निम्नलिखित मुद्दों को ठीक किया गया है:

- 'नई कोट परियोजना मूल्य सूची' प्रपत्र/निकाय पर मूल्य सूची लुकअप में लागत मूल्य सूची के चुने जाने पर प्रमाणीकरण त्रुटि संदेश प्रदर्शित नहीं होता है.
- यदि कोट से संलग्न BPF अंतिम चरण में है, तो कोट को जीते गए के रूप में बंद करना, बनाए गए अनुबंध पर नेविगेट नहीं करता है.
- समय प्रविष्टि को रीकॉल किए जाने पर रीवर्सिंग **बिल न की गई विक्रय** मूल लागत से लिंक की जाती है.
- **पुष्टि करें** बटन चुने जाने के बाद, इनवॉइस स्थिति तब तक **पुष्टि हुई** में नहीं बदलती है, जब तक इनवॉइस को रीफ़्रेश न किए जाए.