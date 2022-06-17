---
title: Project Service Automation के अपडेट रिलीज़ 43, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह आलेख उन सुविधाओं और सुधारों को सूचीबद्ध करता है जो इसमें उपलब्ध हैं Microsoft Dynamics 365 Project Service Automation अद्यतन रिलीज़ 43, V3.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 05/04/2022
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
ms.openlocfilehash: b12cfda08f1ea1fc441782003130be445a437f7c
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8915323"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-43-v3"></a>Project Service Automation के अपडेट रिलीज़ 43, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है

[!include [banner](../includes/psa-now-project-operations.md)]

हमें Microsoft Dynamics 365 Project Service Automation अनुप्रयोग के लिए नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं. यह Dynamics 365 9.x के साथ संगत है। इस रिलीज़ में अद्यतन करने के लिए, Dynamics 365 ऑनलाइन समाधान के लिए व्यवस्थापन केंद्र पृष्ठ पर जाएं और अद्यतन इंस्टॉल करें. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).

यह आलेख उन सुविधाओं और सुधारों को सूचीबद्ध करता है जो Project Service Automation Update Release 43, V3 के लिए नए हैं या बदले गए हैं। इस संस्करण की बिल्ड संख्या V3.10.74.200 है और यह आमतौर पर मई 2022 में एक स्व-अद्यतन के माध्यम से उपलब्ध है.

## <a name="update-release-43"></a>अपडेट रिलीज़ 43

### <a name="bug-fixes"></a>बग समाधान

निम्नलिखित मुद्दों को ठीक किया गया है.


**समय और व्यय**

- बुकिंग या संसाधन असाइनमेंट से समय प्रविष्टियाँ आयात करते समय, संबंधित बुक करने योग्य संसाधन का संदर्भ नहीं रखा जाता है।
- जब टाइम एंट्री ग्रिड को पूर्ण स्क्रीन पर विस्तारित किया जाता है, तो टैब कुंजी के साथ ग्रिड को नेविगेट करना कार्य नहीं करता है।
- किसी अन्य उपयोगकर्ता द्वारा बनाई गई समय प्रविष्टि सबमिट करते समय, **द्वारा प्रस्तुत** समय पत्रक बनाने वाले उपयोगकर्ता के साथ फ़ील्ड गलत तरीके से भरा गया है।
