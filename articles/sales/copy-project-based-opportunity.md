---
title: एक परियोजना-आधारित अवसर प्रतिलिपि करें
description: यह विषय परियोजना संचालन में परियोजना-आधारित अवसरों को कॉपी करने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 26ae5cc267bb06f958bbf9cdce2d80ccde9d3d24
ms.sourcegitcommit: f6f86e80dfef15a7b5f9174b55dddf410522f7c8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/31/2020
ms.locfileid: "4181652"
---
# <a name="copy-project-based-opportunities"></a>एक परियोजना-आधारित अवसर प्रतिलिपि करें

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_


परियोजना अवसरों को आसानी से कॉपी करके नई परियोजना अवसरों को तैयार किया जा सकता है. 

1. **परियोजना अवसर** सूची पृष्ठ पर जाएं और सूची से एक अवसर चुनें. या, किसी विशेष अवसर के विवरण पृष्ठ को खोलें. 
2. किसी भी पृष्ठ के लिए **कॉपी करें** को चुनें. एक संवाद पृष्ठ खुलेगा जिसमें निम्न क्षेत्र जानकारी होगी।. इस संवाद में चयनित मूल्यों के आधार पर, कॉपी करने की प्रक्रिया बदल सकती है.

    | **फ़ील्ड** | **वर्णन** | **डाउनस्ट्रीम प्रभाव** |
    | --- | --- | --- |
    | विषय | लक्ष्य अवसर के लिए संबंधित विषय को दर्ज़ करें. जब संवाद खुलेगा तो, सिस्टम इसे संलग्न **कॉपी** के साथ स्रोत अवसर के विषय पर सेट कर देगा. | इस फील्ड का प्रवाह की दिशा में कोई प्रभाव नहीं होता है. |
    | अकाउंट | ग्राहक की कंपनी या खाता रिकॉर्ड का संदर्भ. जब संवाद खुलता है, तो सिस्टम इसे स्रोत अवसर पर खाते में सेट करेगा. | यह फ़ील्ड अवसर पर प्राथमिक ग्राहक है. |
    | अनुबंध इकाई | संगठन इकाई जो इस समझौते से जुड़ी परियोजना(ओं) की डिलीवरी के लिए जिम्मेदार है. जब संवाद खुलता है, तो सिस्टम इसे स्रोत अवसर की अनुबंध इकाई में सेट करेगा. | अनुबंध इकाई उस कंपनी का हिस्सा है जो सौदे के बंद होने के बाद परियोजनाओं का निष्पादन करती है. हर अनुबंधकारी इकाई के पास एक मुद्रा है, और इस मुद्रा का उपयोग परियोजना के दौरान किए गए अनुमानित और वास्तविक लागत की रिपोर्ट करने के लिए किया जाता है. |
    | मुद्रा | इस सौदे में जिस मुद्रा का लेन-देन होता है. जब संवाद पृष्ठ खुलता है, तो सिस्टम इसे स्रोत अवसर की मुद्रा में सेट कर देगा. | मुद्रा को मूल्य सूची के डिफ़ॉल्ट के लिए उपयोग में लाया जाता है और बोली पर वित्तीय अनुमान बनाए जाते हैं. अंततः, जब सौदे को जीत लिया जाता है तो मुद्रा का उपयोग ग्राहक को इनवॉइस करने के लिए किया जाता है. |
    | मूल्य-निर्धारण की प्रतिलिपि बनाएँ | एक हां/नहीं मूल्य जो यह इंगित करती है कि अवसर पर मूल्य को स्रोत अवसर से कॉपी करना चाहिए. | यदि **हां** को चुना जाता है, तो स्रोत से मूल्य सूचियों को लक्ष्य अवसर पर कॉपी किया जाता है. यदि **नहीं** को चुना जाता है, तो मूल्य सूचियों को सेट किए गए नवीनतम मूल्य सूचियों के आधार पर डिफ़ॉल्ट कर दिया जाता है. |

3. **ठीक** चुनें। सिस्टम चुने हुए मापदंडों के आधार पर परियोजना अवसर की एक कॉपी बनाता है और नया परियोजना अवसर खुल जाता है.