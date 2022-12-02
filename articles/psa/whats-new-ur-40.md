---
title: Project Service Automation के अपडेट रिलीज़ 40, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह आलेख Microsoft Dynamics 365 Project Service Automation अपडेट रिलीज़ 40, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/31/2022
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
ms.openlocfilehash: dca7f340b8d544b183aa0390ac3c11a38f536ed0
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8912794"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-40-v3"></a>Project Service Automation के अपडेट रिलीज़ 40, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है

[!include [banner](../includes/psa-now-project-operations.md)]

हमें Microsoft Dynamics 365 Project Service Automation अनुप्रयोग के लिए नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं. यह Dynamics 365 9.x से मेल के योग्य है. इस रिलीज़ में अद्यतन करने के लिए, Dynamics 365 ऑनलाइन समाधान के लिए व्यवस्थापन केंद्र पृष्ठ पर जाएं और अद्यतन इंस्टॉल करें. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).

यह आलेख Project Service Automation अपडेट रिलीज़ 40, V3 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है. इस संस्करण की बिल्ड संख्या V3.10.61.61 है और आमतौर से फरवरी 2022 में स्वयं-अद्यतन के माध्यम से उपलब्ध है.

## <a name="update-release-40"></a>अपडेट रिलीज़ 40

### <a name="features"></a>सुविधाएँ
Project Service Automation से Project Operations - Lite में अपग्रेड का पहला चरण 1 फरवरी 2022 में सभी ग्राहकों के लिए रिलीज़ किया जाएगा. योग्यता जाँचने के लिए, [Project Service Automation से Project Operations में अपग्रेड](upgrade-project-operations-non-stocked.md) देखें. यदि एप्लिकेशन Power Platform व्यवस्थापन केंद्र में आपकी आवृत्ति में प्रकट नहीं होता है, तो सहायता से संपर्क करें और अनुरोध करें कि आपके परिवेश के लिए फ़्लाइट सक्षम की जाए. आपके अनुरोध में उन परिवेश आईडी की एक सूची शामिल होनी चाहिए, जहां फ़्लाइट को सक्षम करने की आवश्यकता है.

### <a name="bug-fixes"></a>बग समाधान

निम्नलिखित मुद्दों को ठीक किया गया है.

**समय और व्यय**
- जब समय प्रविष्टि को अस्वीकार या रद्द किया जाता है तो एक नोट प्रविष्टि गुम होती है. 

**सेल्स**

- जब आप आउट-ऑफ़-द-बॉक्स प्लग-इन का उपयोग करके लागत या बिक्री अनुमान अपडेट करते हैं, तो आपको गलत तरीके से JSON पेलोड भेजने की अनुमति दी जाती है जो उपयोगकर्ता इंटरफ़ेस के बाहर मान्य नहीं हैं.
- जब आप त्वरित दृश्य का उपयोग करके कोट लाइनों को अपडेट करते हैं, तो आपको कोट सक्रिय करने की अनुमति होती है.
