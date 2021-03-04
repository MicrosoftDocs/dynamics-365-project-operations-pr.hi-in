---
title: समय लागत वास्तविक पर मूल्य को शून्य पर डिफ़ॉल्ट क्यों बनाया जा रहा है?
description: इस समस्या का निवारण करना कि समय लागत वास्तविक पर मूल्य को 0 पर डिफ़ॉल्ट क्यों बनाया जा रहा है.
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/21/2018
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 635fe6dfb547e8b9f96ca1786912309a770e24c2
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/10/2021
ms.locfileid: "5146260"
---
# <a name="why-is-the-price-defaulting-to-zero-on-time-cost-actuals"></a>समय लागत वास्तविक पर मूल्य को शून्य पर डिफ़ॉल्ट क्यों बनाया जा रहा है?

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

यह सामान्य प्रश्न उस वास्तविक के लिए लागू होता है जहाँ लेनदेन श्रेणी समय पर और लेनदेन प्रकार लागत पर सेट है. निम्न तीन जाँचें इस समस्या का निवारण करने में आपकी मदद करेंगी कि समय लागत वास्तविक पर मूल्य को 0 पर डिफ़ॉल्ट क्यों बनाया जा रहा है.
 
## <a name="check-1-identify-the-cost-price-list-for-the-project"></a>जाँच 1: प्रोजेक्ट की लागत मूल्य सूची की पहचान करें

वास्तविक के प्रोजेक्ट फ़ील्ड से प्रोजेक्ट ढूँढें और फिर प्रोजेक्ट पृष्ठ पर जाएँ. फ़ील्ड में अनुबंध इकाई लिंक पर क्लिक करें. अनुबंध इकाई पृष्ठ पर, यह जाँचें कि लागत मूल्य सूचियाँ ग्रिड में अनुबंध इकाई में एक मूल्य सूची है या नहीं.

यदि एक से अधिक मूल्य सूचियाँ हैं, तो आपने समस्या को अलग कर दिया है. Project Service केवल एक मूल्य सूची प्रति संगठनात्मक इकाई का समर्थन करती है. इस निकाय से तब तक सभी मूल्य सूचियाँ निकालें जब तक संगठनात्मक इकाई की लागत मूल्य सूचियाँ ग्रिड में केवल एक मूल्य सूची संलग्न न रह जाए.

यदि संगठनात्मक इकाई से कोई मूल्य सूची संलग्न नहीं है, तो संगठनात्मक इकाई की मुद्रा नोट करें. Project Service पर जाएँ और मूल्य सूचियाँ टैब खोलें. यह जाँचें कि क्या ऐसी कोई मूल्य सूची है जिसके संदर्भ को लागत और ऐसी मुद्रा पर सेट किया गया है जो संगठनात्मक इकाई की मुद्रा से मेल खाती है.
 
यदि ऐसी कोई मूल्य सूची नहीं है जो आपके मापदंड से मेल खाती है, तो आपने समस्या को अलग कर दिया है. यह सुनिश्चित करें कि आपके पास कम से कम ऐसी एक मूल्य सूची है जिसके संदर्भ को लागत पर सेट किया गया है और जिसकी मुद्रा संगठनात्मक इकाई की मुद्रा से मेल खाती है.

यदि एक से अधिक मूल्य सूची है जो उस मापदंड से मेल खाती है, तो अधिक जाँच करने के लिए इस दस्तावेज़ को पढ़ना जारी रखें.

## <a name="check-2-are-any-of-the-price-lists-identified-above-valid-for-the-specific-date-of-the-time-cost-actual"></a>जाँच 2: क्या ऊपर पहचानी गई कोई भी मूल्य सूची समय लागत वास्तविक के विशिष्ट दिनांक के लिए मान्य है?

मूल्य को डिफ़ॉल्ट बनाने हेतु Project Service द्वारा किसी मूल्य सूची पर विचार करने के लिए, वह मूल्य सूची समय लागत वास्तविक पर दिनांक के लिए लागू होनी चाहिए. यह देखने के लिए निम्न की जाँच करें कि ऊपर पहचानी गई सूची(सूचियाँ) लागू होती हैं या नहीं.

- यह जाँचें कि संलग्न मूल्य सूचियों के लिए सामान्य टैब पर प्रारंभ और समाप्ति दिनांक रिक्त नहीं हैं. यदि ऊपर पहचानी गए मूल्य सूचियों में प्रारंभ और समाप्ति दिनांक रिक्त हैं, तो आपने समस्या को अलग कर दिया है. 
- अपने समय लागत वास्तविक पर प्रारंभ दिनांक फ़ील्ड नोट करें और यह जाँचें कि पहचानी गई कोई भी मूल्य सूची उस दिनांक पर लागू होती है या नहीं. उदाहरण के लिए, समय लागत वास्तविक का दिनांक मूल्य सूची में प्रारंभ दिनांक और समाप्ति दिनांक के भीतर होना चाहिए. 
    - यदि ऐसी कोई मूल्य सूची नहीं है जिसमें समय लागत वास्तविक का वह दिनांक शामिल है, तो आपने समस्या को अलग कर दिया है. यह सुनिश्चित करने के लिए मूल्य सूची के प्रारंभ और समाप्ति दिनांक संशोधित करें कि मूल्य सूची में समय लागत वास्तविक का दिनांक शामिल है. 
    - यदि एक से अधिक मूल्य सूची है जिसमें समय लागत वास्तविक का दिनांक शामिल है, तो आपने समस्या को अलग कर दिया है. आप मूल्य सूची(सूचियों) के प्रारंभ और समाप्ति दिनांक संपादित करके इसका समाधान कर सकते हैं ताकि ऐसी केवल एक मूल्य सूची हो जिसमें समय लागत वास्तविक का दिनांक शामिल हो. 
    - यदि ऐसी केवल एक मूल्य सूची है जिसमें समय लागत वास्तविक का दिनांक शामिल है, तो दस्तावेज़ में अगली जाँच पर जाएँ.
आवश्यक समाधान करने के बाद, एक समय प्रविष्टि पुन: बनाएँ, उसे अनुमोदित करें और यह सत्यापित करें कि समय लागत वास्तविक एक वैध मूल्य दिखाता है.

## <a name="check-3-is-there-a-price-in-the-price-list-for-the-pricing-dimensions-on-the-time-cost-actual"></a>जाँच 3: क्या समय लागत वास्तविक पर मूल्य निर्धारण आयामों के लिए मूल्य सूची में कोई मूल्य है?

यदि आपने जाँच 1 और जाँच 2 को सफलतापूर्वक पूरा कर लिया है, तो अब आपके पास केवल एक मूल्य सूची होनी चाहिए जो समय लागत वास्तविक के दिनांक के लिए लागू होती है. इस मूल्य सूची को खोलें और भूमिका मू्ल्य टैब पर जाएँ. यह सुनिश्चित करें कि समय लागत वास्तविक पर मूल्य निर्धारण आयामों के लिए ग्रिड में एक पंक्ति मौजूद है.

यदि समय लागत वास्तविक पर मूल्य निर्धारण आयामों के लिए भूमिका मू्ल्य ग्रिड में कोई पंक्ति मौजूद नहीं है, तो आपने समस्या को अलग कर दिया है. आपके समय लागत वास्तविक पर मूल्य निर्धारण आयामों के लिए भूमिका मू्ल्य ग्रिड में एक पंक्ति बनाएँ. इसे करने के बाद, एक समय प्रविष्टि पुन: बनाएँ, उसे अनुमोदित करें और यह सत्यापित करें कि समय लागत वास्तविक एक वैध मूल्य दिखाता है.
 
यदि उपरोक्त तीनों जाँचें करने के बाद आपको अभी भी अपने समय लागत वास्तविक पर एक वैध मूल्य दिखाई नहीं देता, तो कृपया एक समर्थन टिकट लॉग करें.


