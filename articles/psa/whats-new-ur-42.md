---
title: Project Service Automation के अपडेट रिलीज़ 42, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह आलेख Microsoft Dynamics 365 Project Service Automation अपडेट रिलीज़ 42, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 04/05/2022
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
ms.openlocfilehash: e9911531e4acbd78db416f554c8d85c4f1fee1cf
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912717"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-42-v3"></a>Project Service Automation के अपडेट रिलीज़ 42, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है

[!include [banner](../includes/psa-now-project-operations.md)]

हमें Microsoft Dynamics 365 Project Service Automation अनुप्रयोग के लिए नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं. यह Dynamics 365 9.x से मेल के योग्य है. इस रिलीज़ में अद्यतन करने के लिए, Dynamics 365 ऑनलाइन समाधान के लिए व्यवस्थापन केंद्र पृष्ठ पर जाएं और अद्यतन इंस्टॉल करें. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).

यह आलेख Project Service Automation अपडेट रिलीज़ 42, V3 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है. इस संस्करण की बिल्ड संख्या V3.10.73.61 है और यह आमतौर पर अप्रैल 2022 में एक स्व-अद्यतन के माध्यम से उपलब्ध है.

## <a name="update-release-42"></a>अपडेट रिलीज़ 42

### <a name="bug-fixes"></a>बग समाधान

निम्नलिखित मुद्दों को ठीक किया गया है.

**समय और व्यय**

- जब एक टाइम शीट को अस्वीकार कर दिया जाता है, तो इसे अस्वीकार करने वाले उपयोगकर्ता को ऐसे **सिस्टम** गलत तरीके से पहचाना जाता है.
- जब समय प्रविष्टियाँ आयात की जाती हैं, तो **संसाधन श्रेणी** मूल्य गायब है.
- प्रोजेक्ट अनुमोदक सबमिट किए गए प्रोजेक्ट को तब मंज़ूरी दे सकते हैं, जब उनकी अनुमतियां खास तौर पर इस पर सेट न हों **स्वीकृत कर सकते हैं**.

**सेल्स**

- जब वास्तविक गैर-रूट स्तर के कार्यों पर लॉग होते हैं, तो वास्तविक लागत गलत तरीके से एकत्रित की जाती है.
