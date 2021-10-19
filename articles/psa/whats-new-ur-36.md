---
title: Project Service Automation के अपडेट रिलीज़ 36, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Microsoft Dynamics 365 Project Service Automation Update Release 36, V3 में उपलब्ध फ़ीचर और सुधारों को सूचीबद्ध करता है.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 10/06/2021
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
ms.openlocfilehash: 9b85aed79acb7e7784a23f54a2e9af1cc83f5f4d
ms.sourcegitcommit: 6d9fc4dc851814664bf71729904ab4bedd85fe70
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/06/2021
ms.locfileid: "7606767"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-36-v3"></a>Project Service Automation के अपडेट रिलीज़ 36, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है

[!include [banner](../includes/psa-now-project-operations.md)]

हमें Microsoft Dynamics 365 Project Service Automation अनुप्रयोग के लिए नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं. यह Dynamics 365 9.x से मेल के योग्य है. इस रिलीज़ में अद्यतन करने के लिए, Dynamics 365 ऑनलाइन समाधान के लिए व्यवस्थापन केंद्र पृष्ठ पर जाएं और अद्यतन इंस्टॉल करें. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).

यह विषय Project Service Automation अद्यतन रिलीज़ 36, V3 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है. इस वर्ज़न की बिल्ड संख्या V3.10.57.152 है और यह आमतौर पर अक्टूबर 2021 के सेल्फ-अपडेट के माध्यम से उपलब्ध है.

## <a name="update-release-36"></a>अपडेट रिलीज़ 36

### <a name="bug-fixes"></a>बग समाधान

निम्नलिखित मुद्दों को ठीक किया गया है.

**सामान्य**
- **प्रोजेक्ट पैरामीटर्स** पृष्ठ पर **डिफ़ॉल्ट कार्य समय टेम्प्लेट** फ़ील्ड नाम का गलत अनुवाद किया गया है.
- Async प्लग-इन **SharedVariableService** से संबंधित अपवादों को सही ढंग से हैंडल नहीं कर रहे हैं.

**समय और व्यय**
- जब जर्नल लाइनें गायब होती हैं या उपयोगकर्ता के पास जर्नल लाइन पढ़ने के लिए सही विशेषाधिकार नहीं होते हैं, तो प्रोजेक्ट अनुमोदन रद्द होने पर एक गलत त्रुटि उत्पन्न होती है.
- जब किसी व्यय या समय प्रविष्टि में एक से अधिक संबद्ध प्रोजेक्ट अनुमोदन हों, तो उपयोगकर्ता किसी अनुमोदन को रद्द नहीं कर सकते.
- **अनुपस्थिति** और **अवकाश** का चीनी भाषा के लिए **समय प्रविष्टि** त्वरित निर्माण पृष्ठ पर एक लुकअप में गलत अनुवाद किया गया है.

**संसाधन प्रबंधन**
- जब दृश्य मोड **दिन**, **सप्ताह**, या **माह** पर सेट हो, तो उपयोगकर्ता **शेड्यूल सहायक** में संसाधनों की खोज नहीं कर सकता.
- जेनेरिक संसाधनों को गलत स्थिति नाम रखने की अनुमति है. 
- एक अनुबंध को खो जाने के रूप में बंद करने से भविष्य की बुकिंग रद्द नहीं होती है.

**सेल्स**
- जब किसी परिवेश में प्रोडक्ट की बड़ी मात्रा होती है, तो **सामग्री अनुमान** ग्रिड में प्रदर्शन खराब हो जाता है.
- टेम्प्लेट से प्रोजेक्ट बनाते समय, प्रोजेक्ट मुद्रा संबंधित प्रोजेक्ट मैनेजर की अनुबंध इकाई के लिए डिफ़ॉल्ट नहीं होती है.
- वास्तविक राशियाँ हमेशा उस राशि से मेल नहीं खातीं जो देय प्रोजेक्ट पर दिखाई देती हैं, या विशिष्ट रिकॉल परिदृश्यों में राशियां निगेटिव हो जाती हैं.
- एक त्रुटि तब होती है जब आप प्रोजेक्ट टेम्पलेट से बनाए गए प्रोजेक्ट को अनुबंध लाइन से संबद्ध करते हैं.
- उपयोगकर्ता माइलस्टोन के साथ एक अनुबंध लाइन को हटाने में सक्षम हैं, **इनवॉइस के लिए तैयार** और **इनवॉइस बनाया गया**. इसकी अनुमति नहीं दी जानी चाहिए.
- जब किसी प्रोजेक्ट से अनुमान आयात किए जाते हैं, तो कोट लाइन के लिए टास्क-आधारित बिलिंग सक्षम होने पर कोट लाइन विवरण चार्जेबिलिटी गलत तरीके से सेट की जाती है.
- जब आप एक निश्चित मूल्य बिलिंग माइलस्टोन जोड़ते हैं, तब तक माइलस्टोन माइलस्टोन सबग्रिड में तब तक नहीं दिखता, जब तक कि पेज रीफ्रेश नहीं हो जाता.
- एक शून्य संदर्भ अपवाद उत्पन्न होता है जब आप एक कोट नाम के साथ एक प्रोजेक्ट अनुबंध बनाते हैं जो शून्य है.
- मैन्युअल मोड कार्य जहां प्रोजेक्ट मुद्रा संसाधन की मुद्रा से भिन्न होती है, जिसके परिणामस्वरूप गलत मूल्य अनुमान होते हैं.
- उपयोगकर्ता उस लेन-देन को याद नहीं कर सकते जिसे सुधारात्मक इनवॉयस द्वारा सफलतापूर्वक ठीक किया गया हो.
- निष्क्रिय लेनदेन श्रेणियां **व्यय अनुमान** ग्रिड में दिखाई देती हैं.


