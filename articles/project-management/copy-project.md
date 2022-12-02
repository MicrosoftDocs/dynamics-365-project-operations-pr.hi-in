---
title: परियोजना की प्रतिलिपि बनाएँ
description: यह आलेख Dynamics 365 Project Operations में परियोजना कॉपी करने के बारे में जानकारी प्रदान करता है।
author: ruhercul
ms.date: 03/07/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: b358f9e45278d886f3e6e8e8cd747fc0ea30212b
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8925766"
---
# <a name="copy-a-project"></a>परियोजना की प्रतिलिपि बनाएँ

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

Dynamics 365 Project Operations के साथ, आप **परियोजना** प्रपत्र पर **परियोजना की प्रतिलिपि बनाएँ** चुनकर तेज़ी से नई परियोजनाएँ बना सकते हैं. किसी/एक परियोजना को कॉपी करने के लिए उस परियोजना को खोलें जिसे आप कॉपी करना चाहते हैं और फिर **परियोजना कॉपी करें** चुनें. कार्रवाई निम्नलिखित को कॉपी करेगी:

- परियोजना के गुण 
- कार्य विश्लेषण संरचना
- परियोजना टीम के सदस्य
- परियोजना अनुमान
- परियोजना व्यय का अनुमान
- परियोजना सामग्री अनुमान
- परियोजना चेकलिस्ट
- परियोजना बकेट

## <a name="project-properties"></a>परियोजना के गुण

जब परियोजना की कॉपी बनाई जाती है, तो निम्न फ़ील्ड के मान कॉपी किए जाते हैं।

| क्षेत्र | Project Operations गैर-स्टॉक सामग्रियाँ | Project Operations लाइट | Project for the Web |
|-------|------------------------------------------|-------------------------|---------------------|
| Name | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| विवरण | :heavy_check_mark: | :heavy_check_mark: | |
| ग्राहक | :heavy_check_mark: | :heavy_check_mark: | |
| कैलेंडर टेम्पलेट | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| मुद्रा | :heavy_check_mark: | :heavy_check_mark: | |
| अनुबंध इकाई | :heavy_check_mark: | :heavy_check_mark: | |
| स्वामी कंपनी | :heavy_check_mark: | | |
| परियोजना प्रबंधक | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| स्थिति | :heavy_check_mark: | :heavy_check_mark: | |
| संपूर्ण परियोजना स्थिति | :heavy_check_mark: | :heavy_check_mark: | |
| टिप्पणियां | :heavy_check_mark: | :heavy_check_mark: | |
| अनुमान | :heavy_check_mark: | :heavy_check_mark: | |
| <p>अनुमानित प्रारंभ दिनांक</p><p><strong>ध्यान दें:</strong> यह फ़ील्ड वह तिथि निर्दिष्ट करती है जब परियोजना कॉपी से बनाया जाता है. | :heavy_check_mark: | :heavy_check_mark: | |
| <p>अनुमानित समाप्ति दिनांक</p><p><strong>ध्यान दें:</strong> इस फ़ील्ड में तिथि उस आरंभ तिथि के आधार पर समायोजित की जाती है जब परियोजना को कॉपी से बनाया गया था.</p> | :heavy_check_mark: | :heavy_check_mark: | |
| प्रयास (घंटे) | :heavy_check_mark: | :heavy_check_mark: | |
| अनुमानित श्रम लागत | :heavy_check_mark: | :heavy_check_mark: | |
| अनुमानित व्यय लागत | :heavy_check_mark: | :heavy_check_mark: | |
| अनुमानित सामग्री लागत | | :heavy_check_mark: | |

> [!NOTE]
> परियोजना कॉपी करना लंबी अवधि तक चलने वाली कार्रवाई है. परियोजना रिकॉर्ड, उनकी प्रासंगिक विशेषताएं और कई संबंधित निकाय भी कॉपी किए जाते हैं. कार्रवाई की लंबी चलने वाली प्रकृति के कारण, कॉपी शुरू होने के बाद, कॉपी कार्रवाई पूरी होने तक लक्ष्य परियोजना पृष्ठ को संपादन के लिए लॉक कर दिया जाता है.

## <a name="work-breakdown-structure"></a>कार्य विश्लेषण संरचना

जब परियोजना की प्रतिलिपि बनाई जाती है, तो संपूर्ण संसाधन से युक्त कार्य विभाजन संरचना की कॉपी होती है. नाम युक्त संसाधनों को सामान्य संसाधनों से स्थानापन्न किया जाता है. यदि नामित संसाधनों में सामान्य संसाधन के समान कार्य समय नहीं है, तो शेड्यूल की गणना फिर से की जाएगी, और कार्य अवधि बदल सकती है.

## <a name="project-team-members"></a>परियोजना टीम के सदस्य

जब किसी परियोजना टीम को स्रोत परियोजना से कॉपी की जाती है, तो सामान्य संसाधनों की प्रतिलिपि बनाई जाती है. सामान्य संसाधन असाइनमेंट को भी स्रोत परियोजना की तरह रखा जाता है. नाम युक्त संसाधनों को सामान्य टीम के सदस्यों में परिवर्तित किया जाएगा.

> [!NOTE]
> Project for the Web में टीम के सदस्यों और असाइनमेंट की कॉपी नहीं बनाई जाती है।

## <a name="estimates"></a>अनुमान

जब परियोजना कॉपी किया जाता है, तो स्रोत परियोजना से संसाधन, व्यय और सामग्री अनुमान पंक्तियों की कॉपी बनाई जाती है. 

कॉपी की गई परियोजना तक प्रोग्राम के अनुसार पहुंचने की जानकारी पाने के लिए [Develop project templates with Copy Project](dev-copy-project.md) देखें.

## <a name="quotes-and-contracts"></a>उद्धरण और अनुबंध

कोट और अनुबंध गंतव्य परियोजना से लिंक नहीं हैं।

[!INCLUDE[footer-include](../includes/footer-banner.md)]
