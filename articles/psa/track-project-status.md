---
title: परियोजना की स्थिति ट्रैक करें
description: Project Service में परियोजना की स्थिति को ट्रैक करने का तरीका
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: 00b6d874b42a415fe567d17e49c0ea319d8952a0
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4127835"
---
# <a name="track-a-projects-status-project-service"></a>परियोजना की स्थिति ट्रैक करना (Project Service)

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

किसी क्लाइंट की परियोजना की प्रगति को ट्रैक करने के लिए [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] का उपयोग करें.  

व्‍यस्‍तता बढ़ने के साथ-साथ, परियोजना अवस्‍थाएँ अद्यतन होती हैं ताकि व्‍यस्‍तता की अवस्‍था दर्शाई जा सके:  


|              |                                                                                                                                                                                                                                                                                                  |
|--------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|   **नया**    | जब आप एक परियोजना बनाते हैं, तो अवस्‍था को **नया** पर सेट किया जाता है. यदि आपने परियोजना एक टेम्‍पलेट से बनाई है, तो इस अवस्‍था पर परियोजना के पास एक शेड्यूल, अनुमान और टीम डेटा हो सकता है. अन्यथा, परियोजना की रूपरेखा मौजूद होगी और आपको शेष परियोजना घटक मैन्युअल रूप से दर्ज करना पड़ेगा. |
|  **कोट**   |      जब आप किसी परियोजना को एक कोट से संबद्ध करते हैं, या इसे कोट से बनाते हैं, तो परियोजना अवस्‍था **कोट** पर सेट की जाती है, और अनुमानित प्रारंभ और समाप्ति दिनांक का अद्यतन भी किया जाता है. जब परियोजना एक कोट अवस्‍था में है, तो कोट पर विवरण **परियोजना** पृष्ठ पर **विक्रय** टैब पर प्रदर्शित होता है.      |
|   **योजना**   |                                     जब आप किसी परियोजना के साथ संबद्ध कोट जीतते हैं, और जब व्‍यस्‍तताएँ अनुबंध अवस्‍था पर बढ़ती हैं, तो परियोजना अवस्‍था **योजना** पर अद्यतन करती है. **परियोजना** पृष्ठ पर, अनुबंध विवरण **विक्रय** टैब पर प्रदर्शित होते हैं.                                      |
| **पूर्ण** |                    जब परियोजना पूर्ण होती है, तो आप अवस्था को **पूर्ण** पर फ़्लिप कर सकते हैं. जब परियोजना चरण पर सेट होता है, तो यह समझा जाता है कि कार्य 100% पूर्ण हो गया है, परंतु परियोजना किसी भी लंबित समय या व्‍यय प्रविष्टि रिकार्ड किए जाने के लिए खुली रखी जाती है.                     |
|  **बंद करें**   |           जब परियोजना में सभी लेन-देन को रिकॉर्ड कर लिया जाता है, और आप इसके बाद और लॉग ऑन करने की अपेक्षा नहीं करते, तो आप अवस्‍था को मैन्‍युअल रूप से **बंद** पर सेट कर सकते हैं. जब परियोजना **बंद** पर सेट कर दिया जाता है, किसी परियोजना पर कोई और लेन-देन लॉग नहीं कर सकते और परियोजना केवल पढ़ने के लिए हो जाएगी.           |

## <a name="to-track-a-projects-status"></a>एक परियोजना स्थिति ट्रैक करना  

1.  **Project Service > परियोजना** पर जाएँ.  

2.  जिस परियोजना पर आप काम करना चाहते हैं, उस पर क्लिक करें.  

3.  स्क्रीन के ऊपर पट्टी में, परियोजना नाम के आगे स्थित नीचे तीर का चयन करें, और उसके बाद **परियोजना ट्रैकिंग** पर क्लिक करें.  

4.  कार्य सूची के ऊपर ड्रॉप डाउन सूची में **प्रयास ट्रैकिंग** या **लागत ट्रैकिंग** का चयन करें.  

5.  किसी भी कार्य को संपादित करने के लिए उसे डबल-क्लिक करें. आप कार्य के समय और प्रगति में परिवर्तन करने के लिए गैंट चार्ट पर स्‍तंभों को स्‍थानांतरित कर सकते हैं या उनका आकार बदल सकते हैं.  

### <a name="see-also"></a>यह भी देखें  
 [परियोजना प्रबंधक मार्गदर्शिका](../psa/project-manager-guide.md)