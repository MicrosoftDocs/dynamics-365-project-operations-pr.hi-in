---
title: Project Service Automation के अपडेट रिलीज़ 28, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह आलेख Project Service Automation अपडेट रिलीज़ 28, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/26/2021
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
ms.openlocfilehash: 56a87bce55c560e541e20709b10d38b9512ffcee
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8930596"
---
# <a name="whats-new-or-changed-in-project-service-automation-update-release-28-v3"></a>Project Service Automation के अपडेट रिलीज़ 28, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है

[!include [banner](../includes/psa-now-project-operations.md)]

हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं. यह रिलीज़ Dynamics 365 9.x के साथ संगत में है. इस रिलीज़ का अद्यतन करने के लिए, अपडेट को स्थापित करने हेतु Dynamics 365 online समाधन पृष्ठ के लिए व्यवस्थापन केंद्र पर जाएँ. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](/power-platform/admin/install-remove-preferred-solution).

इस आलेख में Project Service Automation V3, अद्यतन रिलीज़ 28 में उपलब्ध सुविधाएँ और सुधार सूचीबद्ध किए गए हैं. इस संस्करण की बिल्ड संख्या V3.10.46.32 है और आमतौर से जनवरी 2021 में स्वयं-अद्यतन के माध्यम से उपलब्ध है.

## <a name="update-release-28"></a>अपडेट रिलीज़ 28

### <a name="bug-fixes"></a>बग समाधान

**समय और व्यय**

निम्नलिखित मुद्दों को ठीक किया गया है:

- उपयोगकर्ता, अनुमोदित और सबमिट की गई समय प्रविष्टियों को अद्यतन करने के लिए **सामूहिक संपादन** का उपयोग कर सकते हैं.

**परियोजना प्रबंधन**

निम्नलिखित मुद्दों को ठीक किया गया है:

- ऐसे मामलों में जहां कार्य GUID को एक संख्या के रूप में व्याख्यायित किया जाता है, कार्यों को **कार्य विश्लेषण संरचना** पृष्ठ पर रिबन में **कार्य संपादित करें** का उपयोग करके संपादन के लिए खोला नहीं जा सकता है.

**Sales**

निम्नलिखित मुद्दों को ठीक किया गया है:

- जब **GetEstimatesForProject** प्लग-इन इनवोक किया जाता है, तो नल संदर्भ अपवाद जनरेट होता है.
- माइलस्टोन ग्रिड पर **इनवॉइस के लिए तैयार के रूप में चिह्नित करें** **InvoiceStatus** एट्रिब्यूट को छोड़कर, जो कि अद्यतन है, केवल आंशिक रूप से एट्रिब्यूट को अद्यतन करता है.



[!INCLUDE[footer-include](../includes/footer-banner.md)]
