---
title: Project Service Automation के अपडेट रिलीज़ 19, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 19, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 05/05/2020
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
ms.openlocfilehash: 8a73a6acd4ce4c9559cdf4591ede735a613f4d52
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/10/2021
ms.locfileid: "5143608"
---
# <a name="project-service-automation-update-release-19-v3"></a>Project Service Automation V3 अद्यतन रिलीज़ 19, V3

[!include [banner](../includes/psa-now-project-operations.md)]

हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं. यह रिलीज़ Dynamics 365 9.x के साथ संगत में है. इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

यह टॉपिक PSA V3, अपडेट रिलीज़ 19 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है. इस संस्करण की बिल्ड संख्या V3.10.30.41 है और यह आमतौर पर मई 2020 में एक स्व-अद्यतन के माध्यम से उपलब्ध है.

## <a name="update-release-19"></a>अपडेट रिलीज़ 19

### <a name="bug-fixes"></a>बग समाधान

**समय और व्यय**

निम्नलिखित मुद्दों को ठीक किया गया है: 

- समय प्रविष्टि आयात से प्राप्त त्रुटियाँ सही ढंग से सामने नहीं आई हैं.
- समय प्रविष्टि ग्रिड **केवल दिनांक** फ़ील्ड व्यवहार का समर्थन नहीं करती है.
- परियोजना संसाधन किसी परियोजना के साथ एक व्यय बनाने में असमर्थ हैं.

**परियोजना प्रबंधन**

निम्नलिखित मुद्दों को ठीक किया गया है: 

-  ग्रैंडचाइल्ड कार्य पूर्णता (EAC) गणना के दौरान एक गलत प्रयास का अनुमान लगाता है.

**Sales**

निम्नलिखित मुद्दों को ठीक किया गया है: 

- **पुनर्गणना** कार्रवाई व्यय अनुबंध पंक्ति विवरण या कोट पंक्ति विवरण के साथ काम नहीं करती है.
- **अद्यतन मूल्य** व्यय अनुमानों के लिए गायब है.
-  ग्राहक **परियोजना अनुबंध** पृष्ठ से कस्टम अनुबंध स्थिति कारणों को चयन करने में असमर्थ हैं.
- किसी कोट से कस्टम मूल्य सूची बनाते समय ग्राहकों को अपमानजनक प्रदर्शन का अनुभव होता है.
- ग्राहकों को **कोट पंक्ति विवरण** और **अनुबंध पंक्ति विवरण** पृष्ठों पर डिफ़ॉल्ट **इकाई** के साथ असंगतता का अनुभव होता है.
- किसी प्रभार्य अनुबंध पंक्ति में गैर-प्रभार्य लेन-देन श्रेणी आइटम जोड़ने से यह लेन-देन श्रेणी के **गैर प्रभार्य** बिलिंग प्रकार का सम्मान नहीं होगा.
- ग्राहक पहले बनाए गए अनुबंधों पर नए रूप से जोड़ी गई भूमिकाओं और श्रेणी का उपयोग नहीं कर सकते हैं.
- ग्राहकों को अनावश्यक रूप से PreValidateProjectTeamMemberUpdate.cs में अपमानित प्रदर्शन का अनुभव प्राप्त होता है
- **संसाधन श्रेणियाँ** सूची में गैर-प्रभार्य के रूप में सेट अप की गई भूमिकाओं को परियोजना के लिए अनुबंध पंक्ति पर **प्रभार्य भूमिकाएँ** टैब में **गैर-प्रभार्य** के रूप में जोड़ा जाना चाहिए.
- ग्राहक एक परियोजना बनाते समय अपमानित प्रदर्शन का अनुभव कर सकते हैं क्योंकि **GetBookableResourceIdFromUser** केवल प्राथमिक आईडी के बजाय बुक करने योग्य संसाधनों के सभी स्तंभों को पुनर्प्राप्त करता है.
- **लेनदेन प्रकार** निकाय में उपयोगकर्ताओं को **इकाइयों** और **UnitGroups** से प्रवेश करने से रोकने के लिए पूर्व-सत्यापन अद्यतन प्लग-इन गुम होता है, जो लेनदेन प्रकारों के लिए मान्य नहीं होता.
- **हटाना** चरण समय प्रविष्टि आयात के लिए कार्य नहीं करता है.