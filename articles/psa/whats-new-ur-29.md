---
title: Project Service Automation के अपडेट रिलीज़ 29, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 29, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 02/22/2021
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
ms.openlocfilehash: 0e1ff0db42adb8b991b26dca1585bd603b2e2276
ms.sourcegitcommit: f57408d6637f670b920d7ce95f8ace8eb1963093
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/17/2021
ms.locfileid: "5664645"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-29-v3"></a>Project Service Automation के अपडेट रिलीज़ 29, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है

[!include [banner](../includes/psa-now-project-operations.md)]

हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं. यह रिलीज़ Dynamics 365 9.x के साथ संगत में है. इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 29 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है. इस संस्करण की बिल्ड संख्या V3.10.47.7 है और आमतौर से फरवरी 2021 में स्वयं-अद्यतन के माध्यम से उपलब्ध है.

## <a name="update-release-29"></a>अपडेट रिलीज़ 29

### <a name="bug-fixes"></a>बग समाधान

**समय और व्यय**

निम्नलिखित मुद्दों को ठीक किया गया है:

- उपयोगकर्ता समय प्रविष्टि ग्रिड में गैर-कार्य दिवसों में लॉग किए गए कार्य समय को नहीं देख सकते हैं.
- स्वीकृत व्यय प्रविष्टियों को ग्रिड पर संपादित किया जा सकता है.

**परियोजना प्रबंधन**

निम्नलिखित मुद्दों को ठीक किया गया है:

- संसाधन असाइनमेंट के प्रयास ऋणात्मक नहीं हो सकते सुनिश्चित करने के लिए सत्यापन तर्क उपलब्ध नहीं है.
- कस्टम क्रिया, **AssignResourcesForTask** केवल बदले गए फ़ील्ड के बजाय सभी फ़ील्ड अपडेट करता है.
- उन प्लग-इन या कार्यप्रवाह वाले परिवेश में किसी परियोजना की प्रतिलिपि बनाते समय, जो **CreateProject** इवेंट पर पंजीकृत हैं, अब अगर **CopyWBSToProject** विफल हो जाता है, तो **msdyn_bulkgenerationstatus** एट्रिब्यूट अद्यतन नहीं होता है.
- जब आप परियोजना कैलेंडर का विस्तार करते हैं, तो कार्य दिवस आरोही क्रम में सॉर्ट नहीं किए जाते हैं, जिससे कुछ परियोजना कार्य अपडेट विफल हो जाते हैं.
- किसी मौजूदा परियोजना पर परियोजना प्रबंधन को बदलने से संगठनात्मक इकाई डिफ़ॉल्ट तर्क ट्रिगर हो जाता है.

**सेल्स**

निम्नलिखित मुद्दों को ठीक किया गया है:

- **अनुबंध** पृष्ठ पर **अनुबंध प्रदर्शन** टैब प्रारंभ के दौरान चुपचाप से विफल रहता है, जब कोई अनुबंध पंक्ति मौजूद नहीं होती है.
