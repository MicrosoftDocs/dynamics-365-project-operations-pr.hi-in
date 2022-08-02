---
title: Project Service Automation के अपडेट रिलीज़ 45, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह आलेख उन सुविधाओं और सुधारों को सूचीबद्ध करता है जो इसमें उपलब्ध हैं Microsoft Dynamics 365 Project Service Automation अद्यतन रिलीज़ 45, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 07/14/2022
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
ms.openlocfilehash: 98f7c973917d7d6334e6e0aeb15214c538b33143
ms.sourcegitcommit: 36fda4f45ddeb0f81d30bd1e22852727df644754
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 07/16/2022
ms.locfileid: "9169178"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-45-v3"></a>Project Service Automation के अपडेट रिलीज़ 45, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है

[!include [banner](../includes/psa-now-project-operations.md)]

हमें Microsoft Dynamics 365 Project Service Automation अनुप्रयोग के लिए नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं. यह Dynamics 365 9.x से मेल के योग्य है. इस रिलीज़ में अद्यतन करने के लिए, Dynamics 365 ऑनलाइन समाधान के लिए व्यवस्थापन केंद्र पृष्ठ पर जाएं और अद्यतन इंस्टॉल करें. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).

यह आलेख उन सुविधाओं और सुधारों को सूचीबद्ध करता है जो Project Service Automation Update Release 45, V3 के लिए नई या परिवर्तित हैं। इस संस्करण में V3.10.76.168 का बिल्ड नंबर है और यह आम तौर पर जुलाई 2022 में स्व-अद्यतन के माध्यम से उपलब्ध है.

## <a name="update-release-45"></a>अपडेट रिलीज़ 45

### <a name="bug-fixes"></a>बग समाधान

निम्नलिखित मुद्दों को ठीक किया गया है.

**सेल्स**

- बिना बिल न की गई बिक्री के बिना इनवॉइस बनाने का प्रयास करने के बाद उपयोगकर्ता सफलतापूर्वक इनवॉइस नहीं बना सकते हैं, यदि वे पृष्ठ का एक ही उदाहरण देख रहे हैं और इसे रीफ़्रेश नहीं करते हैं।

**समय और व्यय**

- जब आधुनिक स्वीकृतियां सक्षम की जाती हैं और वापस बुलाए गए प्रोजेक्ट अनुमोदन को स्वीकृत किया जाता है, तो रिकॉर्ड चरण को गलत तरीके से अद्यतन किया जाता है **रिकॉल अनुरोध स्वीकृत।**
- जब आधुनिक स्वीकृति सक्षम होती है और क्लाउड फ़्लो निष्क्रिय होता है, तो स्वीकृति प्रक्रिया सफल नहीं होती है, और सबमिट करने या स्वीकृत करने वाले उपयोगकर्ताओं को सूचित नहीं किया जाता है।
