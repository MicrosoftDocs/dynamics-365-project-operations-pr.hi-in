---
title: Project Service Automation के अपडेट रिलीज़ 13, V3 में नया क्या है
description: यह टॉपिक Project Service Automation अपडेट रिलीज़ 13, V3 में क्या नया है, इसके बारे में जानकारी प्रदान करता है.
author: ruhercul
manager: kfend
ms.service: business-applications
ms.custom: dyn365-projectservice
ms.date: 02/04/2020
ms.topic: article
ms.prod: ''
ms.technology: Microsoft Dynamics 365 Project Service Automation 3.x
ms.assetid: c6f6a5b6-b5bb-467c-b7c7-7fb962504c6d
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 5f1b6b3879c94a77ab62082aad1e470a3ba66552
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3752015"
---
# <a name="project-service-automation-v3-update-release-13"></a>Project Service Automation V3 अपडेट रिलीज़ 13
हमें Dynamics 365 Project Service Automation (PSA) अनुप्रयोग के लिए नवीनतम अपडेट की घोषणा करते हुए बेहद खुशी है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं. यह रिलीज़ Dynamics 365 9.x के साथ संगत में है. इस रिलीज़ पर अपडेट करने के लिए, Dynamics 365 online के लिए व्यवस्थापन केंद्र पर जाएँ, और अपडेट को स्थापित करने के लिए समाधान पृष्ठ पर जाएँ. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

यह टॉपिक Project Service Automation V3, अपडेट रिलीज़ 13 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है. इस वर्ज़न की बिल्ड संख्या V3.10.3.18 है और यह निम्नलिखित शेड्यूल पर उपलब्ध है:

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
     - फ़िक्स्ड: अवसरों, उद्धरणों, उत्पादों के ऑर्डर और परियोजना-आधारित पंक्ति सब-ग्रिड के लिए **नया मौका**, **उद्धरण**, **ऑर्डर पंक्ति** और **उत्पाद जोड़ें** के लिए अतिरिक्त बटन आदेश में दिखाई देते हैं.


