---
title: Project Service Automation के अपडेट रिलीज़ 39, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह आलेख Microsoft Dynamics 365 Project Service Automation अपडेट रिलीज़ 39, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/20/2022
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
ms.reviewer: johnmichalak
ms.openlocfilehash: d5b5938762d98acaead9e26c47bce07e0059faf6
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922454"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-39-v3"></a>Project Service Automation के अपडेट रिलीज़ 39, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है

[!include [banner](../includes/psa-now-project-operations.md)]

हमें Microsoft Dynamics 365 Project Service Automation अनुप्रयोग के लिए नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं. यह Dynamics 365 9.x से मेल के योग्य है. इस रिलीज़ में अद्यतन करने के लिए, Dynamics 365 ऑनलाइन समाधान के लिए व्यवस्थापन केंद्र पृष्ठ पर जाएं और अद्यतन इंस्टॉल करें. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).

यह आलेख Project Service Automation अपडेट रिलीज़ 39, V3 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है. इस वर्ज़न की बिल्ड संख्या V3.10.60.170 है और यह आमतौर पर जनवरी 2022 के सेल्फ-अपडेट के माध्यम से उपलब्ध है.

## <a name="update-release-39"></a>अपडेट रिलीज़ 39

### <a name="bug-fixes"></a>बग समाधान

निम्नलिखित मुद्दों को ठीक किया गया है.

**सामान्य**

- अरबी अनुवाद के लिए साइट मानचित्र में कई सुधार किए गए हैं.

**परियोजना प्रबंधन**

- एक त्रुटि तब होती है जब आप किसी प्रोजेक्ट पर प्रोजेक्ट मैनेजर को किसी ऐसे उपयोगकर्ता में बदलते हैं, जो पहले से ही प्रोजेक्ट पर टीम का सदस्य है.

**सेल्स**

- जब मूल्य सूची स्वचालित रूप से बनाई जाती है, तब **प्रोजेक्ट अनुबंध मूल्य सूची** का स्वामी गलत होता है. 
- जब मूल्य सूची को प्रोजेक्ट पैरामीटर पर लागू किया जाता है, तो मूल्य सूची की दिनांक प्रभावशीलता पर ध्यान नहीं दिया जाता.
- दो अलग-अलग कोट को संपादित करते समय हो सकता है कि अनुबंधित इकाई में सही डिफ़ॉल्ट मान न हो.
