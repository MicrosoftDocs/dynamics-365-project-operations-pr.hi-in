---
title: Project Service Automation के अपडेट रिलीज़ 25, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 25, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 10/26/2020
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
ms.openlocfilehash: 3aa10e1d4b23fbe6c2743d71497bdef840776008
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/27/2021
ms.locfileid: "5948873"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-25-v3"></a>Project Service Automation के अपडेट रिलीज़ 25, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है

[!include [banner](../includes/psa-now-project-operations.md)]

हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं. यह रिलीज़ Dynamics 365 9.x के साथ संगत में है. इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).

यह विषय उन सुविधाओं और सुधारों को सूचीबद्ध करता है, जो नए हैं या Project Service Automation V3, अद्यतन रिलीज़ 25 के लिए बदल गए हैं. इस संस्करण की बिल्ड संख्या V 3.10.43.76 है और आमतौर पर अक्टूबर 2020 में स्वयं-अद्यतन के माध्यम से उपलब्ध है.

## <a name="update-release-25"></a>अपडेट रिलीज़ 25

### <a name="bug-fixes"></a>बग समाधान

**समय और व्यय**

निम्न समस्या को ठीक किया गया है:

- पुनः प्राप्त किया जा रहे हैं बहुत बड़े अंतराल के आधार पर अतिरिक्त डेटा दिखा रहा समय प्रविष्टि चार्ट.

**संसाधन प्रबंधन**

निम्न समस्या को ठीक किया गया है:

- यदि उच्च संस्करण पैच पहले से मौजूद है, तो Universal Resource Scheduling पैच आयात को छोड़ने के लिए जोड़ा गया Package Deployer कोड.

**परियोजना प्रबंधन**

निम्नलिखित मुद्दों को ठीक किया गया है:

- सही राउंडिंग और विनिमय दर की विसंगतियों के परिणामस्वरूप परियोजना ट्रैकिंग ग्रिड में गलत नियोजित लागत.
- **परियोजना** प्रपत्र पर दो या अधिक प्रतिक्रिया ग्रिड को दिखाने की क्षमता का समर्थन.
- कैलेंडर समाप्ति दिनांक के बाद कार्य को असाइन करने की क्षमता, जिसके परिणामस्वरूप एक असफल संसाधन असाइनमेंट होता है, को हल करने के लिए प्रदान किया गया सत्यापन.
- निम्न से उत्पन्न नल संदर्भ अपवाद को हल करने के लिए बेहतर त्रुटि हैंडलिंग:

    - **PreValidateProjectTeamMemberCreate** प्लग-इन
    - **PreValidateProjectTaskCreate** जब बिना किसी संबद्ध परियोजना के परियोजना कार्य बनाया जाता है
    - **PreProjectTeamMemberCreate** प्लग-इन
    - **PostProjectTeamMemberDelete** प्लग-इन
    - **PreValidateProjectTaskDelete** प्लग-इन

**Sales**

निम्नलिखित मुद्दों को ठीक किया गया है:

- **परियोजना को कॉपी करें: HelperResource प्रबंधन का अनुमान लगाता है** से उत्पन्न नल संदर्भ अपवाद को हल करने के लिए बेहतर त्रुटि हैंडलिंग: 
- **समय और सामग्री बिलिंग बैकलॉग** पर **इनवॉइस के लिए तैयार नहीं** बिलिंग स्थिति को साफ़ नहीं करता.
- **भूमिका मूल्य** और **बैकलॉग आइटम** टैब पर सही किया गया गलत लेबल **मूल्य** बटन.


[!INCLUDE[footer-include](../includes/footer-banner.md)]