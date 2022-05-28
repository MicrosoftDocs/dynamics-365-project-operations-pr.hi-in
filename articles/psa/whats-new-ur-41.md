---
title: Project Service Automation के अपडेट रिलीज़ 41, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Microsoft Dynamics 365 Project Service Automation Update Release 41, V3 में उपलब्ध फ़ीचर और सुधारों को सूचीबद्ध करता है.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 03/07/2022
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
ms.openlocfilehash: 649d8bca36fda0a09dc7230ee4d742cadb32f3b3
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/14/2022
ms.locfileid: "8580918"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-41-v3"></a>Project Service Automation के अपडेट रिलीज़ 41, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है

[!include [banner](../includes/psa-now-project-operations.md)]

हमें Microsoft Dynamics 365 Project Service Automation अनुप्रयोग के लिए नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं. यह Dynamics 365 9.x से मेल के योग्य है. इस रिलीज़ में अद्यतन करने के लिए, Dynamics 365 ऑनलाइन समाधान के लिए व्यवस्थापन केंद्र पृष्ठ पर जाएं और अद्यतन इंस्टॉल करें. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).

यह विषय Project Service Automation अद्यतन रिलीज़ 41, V3 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है. इस संस्करण की बिल्ड संख्या V3.10.62.162 है और यह आमतौर पर मार्च 2022 के स्वयं-अपडेट के माध्यम से उपलब्ध है.

## <a name="update-release-41"></a>अपडेट रिलीज़ 41

### <a name="bug-fixes"></a>बग समाधान

निम्नलिखित मुद्दों को ठीक किया गया है.

**परियोजना प्रबंधन**
- जब आप डेस्कटॉप ऐड-इन से बनाए गए प्रोजेक्ट पर आधारित टेम्पलेट से कोई प्रोजेक्ट बनाने का प्रयास करते हैं, तो निम्न त्रुटि प्रदर्शित होती है, "संसाधन असाइनमेंट का नियोजित कार्य फ़ील्ड सत्यापन: प्रत्येक संसाधन असाइनमेंट समय स्लाइस की समाप्ति तिथि इसके प्रारंभ से पहले नहीं होनी चाहिए। दिनांक"।

**समय और व्यय**
- जब आप किसी समय प्रविष्टि को हटाने का प्रयास करते हैं, तो निम्न त्रुटि संदेश प्रदर्शित होता है, "आईएसवी कोड से एक अनपेक्षित त्रुटि उत्पन्न होती है"।

**सेल्स**
- जब आप एक निश्चित मूल्य मील के पत्थर के लिए एक चालान बनाते हैं, तो**विवरण** और **बाहरी विवरण** फ़ील्ड आबाद नहीं हैं। 