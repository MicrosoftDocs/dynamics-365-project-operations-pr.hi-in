---
title: Project Service Automation के अपडेट रिलीज़ 13, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह आलेख Project Service Automation अपडेट रिलीज़ 13, V3 में क्या नया है, इसके बारे में जानकारी प्रदान करता है.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
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
ms.openlocfilehash: f4898391922f5ecbc99d78e49358ea749fe27b3f
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8930688"
---
# <a name="project-service-automation-update-release-13-v3"></a>Project Service Automation V3 अद्यतन रिलीज़ 13, V3

[!include [banner](../includes/psa-now-project-operations.md)]

हमें Dynamics 365 Project Service Automation (PSA) अनुप्रयोग के लिए नवीनतम अपडेट की घोषणा करते हुए बेहद खुशी है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं. यह रिलीज़ Dynamics 365 9.x के साथ संगत में है. इस रिलीज़ पर अपडेट करने के लिए, Dynamics 365 online के लिए व्यवस्थापन केंद्र पर जाएँ, और अपडेट को स्थापित करने के लिए समाधान पृष्ठ पर जाएँ. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).

यह आलेख Project Service Automation V3, अपडेट रिलीज़ 13 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है. इस वर्ज़न की बिल्ड संख्या V3.10.3.18 है और यह निम्नलिखित शेड्यूल पर उपलब्ध है:

- **सामान्य उपलब्धता (सेल्फ-अपडेट):** नवंबर 2019
- **ऑटो-अपडेट:** दिसंबर 2019


## <a name="update-release-13"></a>अपडेट रिलीज़ 13 

### <a name="bug-fixes"></a>बग समाधान

- समय और व्यय

     - फ़िक्स्ड: व्यय उद्देश्य से खोज करने पर **व्यय अनुमोदन** पृष्ठ पर खोज कार्यक्षमता काम नहीं करती है.

- संसाधन प्रबंधन

     - फ़िक्स्ड: समायोजन में संख्याओ को दाहिनी ओर जस्टिफ़ाई पर अपडेट किया गया है.
     - फ़िक्स्ड: नामित संसाधनों को **शेड्यूल** टैब के माध्यम से कार्यों को असाइन नहीं किया जा सकता.

- परियोजना प्रबंधन

     - फ़िक्स्ड: टीम सदस्य को असाइन करते समय नल संदर्भ अपवाद, जब **TransactionType**, **इकाई** और **DefaultGroup** के लिए सेटअप जानकारी उपलब्ध न हो.

- Sales

     - फ़िक्स्ड: डुप्लिकेट ट्रांजेक्शन टाइप रिकॉर्ड एक त्रुटि लौटाते हैं जब भूमिका मूल्य रिकॉर्ड बनाया जाता है.
     - ठीक किया गया: **नया अवसर**, **कोट**, **ऑर्डर पंक्ति**, और **उत्पाद जोड़ें** के लिए अतिरिक्त बटन, अवसर, कोट, उत्पाद ऑर्डर और परियोजना-आधारित पंक्ति सबग्रिड के आदेशों में दिखाई देते हैं.




[!INCLUDE[footer-include](../includes/footer-banner.md)]
