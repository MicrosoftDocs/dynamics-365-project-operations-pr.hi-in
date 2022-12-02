---
title: Project Service Automation के अपडेट रिलीज़ 37, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह आलेख Microsoft Dynamics 365 Project Service Automation अपडेट रिलीज़ 37, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 11/01/2021
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
ms.openlocfilehash: bdbb125b4f41bb9970f5bd8a01cf0bb863c34738
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922500"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-37-v3"></a>Project Service Automation के अपडेट रिलीज़ 37, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है

[!include [banner](../includes/psa-now-project-operations.md)]

हमें Microsoft Dynamics 365 Project Service Automation अनुप्रयोग के लिए नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं. यह Dynamics 365 9.x से मेल के योग्य है. इस रिलीज़ में अद्यतन करने के लिए, Dynamics 365 ऑनलाइन समाधान के लिए व्यवस्थापन केंद्र पृष्ठ पर जाएं और अद्यतन इंस्टॉल करें. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).

यह आलेख Project Service Automation अपडेट रिलीज़ 37, V3 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है. इस संस्करण की निर्माण संख्या V3.10.58.120 है और आम तौर पर नवंबर 2021 में स्वयं-अपडेट के माध्यम से उपलब्ध है.

## <a name="update-release-37"></a>अपडेट रिलीज़ 37

### <a name="bug-fixes"></a>बग समाधान

निम्नलिखित मुद्दों को ठीक किया गया है.

**समय और व्यय**
- उपयोगकर्ता सेल को साफ़ करके समय प्रविष्टि को हटाने में असमर्थ.
- **मेरी असफल स्वीकृति** दृश्य में केवल **सबमिट** की स्थिति वाले परियोजना अनुमोदन शामिल हैं.

**परियोजना प्रबंधन**
- यदि परियोजना टीम के सदस्य की स्थिति का नाम खाली है तो Microsoft डेस्कटॉप ऐड-इन में परियोजना खोलने के दौरान उपयोगकर्ताओं को शून्य संदर्भ अपवाद त्रुटि प्राप्त होती है.
- **परियोजना कार्य** पृष्ठ पर **सहेजें** बटन नहीं है, जिससे उपयोगकर्ता कार्य रिकॉर्ड में परिवर्तनों को सहेज नहीं सकते.
- उपयोगकर्ता किसी ऐसी परियोजना को हटा नहीं सकते जिसमें **जीते** की स्थिति वाले कोट से संबद्ध कार्य है.

**सेल्स**
- लागू किए गए टेम्प्लेट की मुद्रा से मिलान करने के लिए **परियोजना** पृष्ठ पर **मुद्रा** फ़ील्ड को अपडेट किया जाता है.
- एक से अधिक मुद्राएं वाले कार्यों पर लागत की गणना गलत तरीके से की जाती है.
