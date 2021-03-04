---
title: परियोजना लागत और आय अनुमान निर्धारित करें
description: Project Service में परियोजना लागत और आय अनुमान निर्धारित करने का तरीका
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
ms.openlocfilehash: 66fa8f4374caa08b07663cc9d261bfff8ce30c87
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4133010"
---
# <a name="determine-project-cost-and-revenue-estimates"></a>परियोजना लागत और आय अनुमान निर्धारित करें 

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

परियोजना अनुमान, परियोजना की कार्य विश्लेषण संरचना में अनुमानित और शेड्यूल किए गए कार्य के लिए वित्तीय दृश्य प्रदान करते हैं. अनुमान दृश्य आपको नियोजित कार्य के लागत और आय प्रभाव के बारे में सूचित करता है. अनुमान दृश्य आपको परियोजना के वित्तीय प्रभाव की सर्वोत्तम जानकारी देने के लिए, कई पूर्व-निर्धारित आयामों के बारे में जानकारी देखने हेतु साधन प्रदान करता है.  
  
## <a name="cost-and-sales-value-of-the-project"></a>परियोजना की लागत और विक्रय मान  
[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] मूल्य सूचियाँ परियोजना द्वारा उपयोग की जाने वाली भूमिकाओं के लिए लागत और बिल की दरें निर्धारित करती हैं. परियोजना की कार्य विश्लेषण संरचना में कार्यों के साथ संबंधित भूमिकाओं के आधार पर, आप शामिल कार्य की लागत और आय के प्रभाव को निर्धारित कर सकते हैं.  
  
## <a name="cost-price-defaulting"></a>लागत मूल्य डिफ़ॉल्ट बनाना  
प्रत्येक परियोजना किसी संगठन से संबंधित होती है (परियोजना में **स्वामी इकाई**). स्वामी संगठनात्मक इकाई के साथ संबंधित मूल्य सूची इकाई लागत मूल्य निर्धारित करती है. [!INCLUDE[pn_dyn_365_project_service_auto](../includes/pn-dyn-365-project-service-auto.md)] अनुमान पंक्तियों पर प्रभावी दिनांक के लिए सही लागत मूल्य प्राप्त करने के लिए, लागत मूल्य सूची में भूमिका, इकाई और संगठनात्मक इकाई की खोज करके भूमिकाओं के लिए लागत मूल्य निर्धारित करती हैं.  
  
यदि भूमिका, इकाई, और संगठनात्मक इकाई के संयोजन का परिणाम स्वामी इकाई की मूल्य सूची से लागत मूल्य के रूप में नहीं मिलता है, तो भूमिका और संगठनात्मक इकाई के संयोजन के पक्ष में उस इकाई की उपेक्षा कर दी जाती है. यदि कोई लागत मूल्य है, तो इस मूल्य को उस इकाई में रूपांतरित कर दिया जाता है, जिसे आपने अनुमान पंक्ति में चुना था.  
  
यदि भूमिका और संगठनात्मक इकाई के संयोजन का परिणाम लागत मूल्य के रूप में नहीं मिलता है, तो भूमिका और इकाई के संयोजन के पक्ष में उस संगठनात्मक इकाई की उपेक्षा कर दी जाती है और आवश्यक होने पर, सभी रूपांतरण लागू करने के बाद मूल्य को डिफ़ॉल्ट बना दिया जाता है.  
  
 यदि भूमिका के लिए कोई मूल्य नहीं है, तो लागत मूल्य अनुमान पंक्ति पर डिफ़ॉल्ट रूप से 0.00 हो जाता है.  
  
 परियोजना लागत अनुमान पंक्तियों पर मौजूद सभी लागत राशियाँ स्वामी संगठनात्मक इकाई की मुद्रा में होती हैं.  
  
## <a name="sales-price-defaulting"></a>विक्रय मूल्य डिफ़ॉल्ट बनाना  
विक्रय मूल्य सूची उस विक्रय निकाय पर आधारित है, जिससे यह परियोजना अनुलग्न है. कोट या अनुबंध के साथ संबंधित विक्रय मूल्य सूची इकाई विक्रय मूल्य निर्धारित करती है. यदि कोट या अनुबंध में कस्टम मूल्य सूची है, तो यह परियोजना अनुमानों के लिए डिफ़ॉल्ट विक्रय मूल्य सूची होगी. यदि विक्रय निकायों से कोई संबंध नहीं है, तो पैरामीटर सेटिंग में कॉन्फ़िगर की गई डिफ़ॉल्ट विक्रय मूल्य सूची उस परियोजना के लिए डिफ़ॉल्ट विक्रय मूल्य सूची होगी. प्रत्येक अनुमान पंक्ति में कार्य पूरा करने के लिए बुक किए जाने वाले संसाधनों की संगठनात्मक इकाई को इंगित करने के लिए, संबंधित संसाधन संगठनात्मक इकाई है. अनुमान पंक्तियों पर प्रभावी दिनांक के लिए सही विक्रय मूल्य प्राप्त करने हेतु विक्रय मूल्य सूची में भूमिका, इकाई और संसाधन संगठनात्मक इकाई के संयोजन की खोज करके संबंधित भूमिकाओं के लिए विक्रय मूल्य निर्धारित किया जाता है.  
  
यदि भूमिका, इकाई और संसाधन संगठनात्मक इकाई के संयोजन का परिणाम विक्रय मूल्य सूची के विक्रय मूल्य के रूप में नहीं मिलता है, तो सिस्टम उस इकाई की उपेक्षा कर देगा और भूमिका एवं संसाधन संगठनात्मक इकाई के संयोजन की खोज करेगा. यदि कोई विक्रय मूल्य प्राप्त होता है, तो इसे उस इकाई में रूपांतरित कर दिया जाएगा, जिसे आपने विक्रय अनुमान पंक्ति में चुना था.  
  
यदि सिस्टम को भूमिका के लिए कोई मूल्य प्राप्त नहीं होता है, तो विक्रय मूल्य को अनुमान पंक्ति पर डिफ़ॉल्ट रूप से 0.00 कर दिया जाना चाहिए.  
  
अनुमान दृश्य में एक ग्रिड दृश्य होता है, जो इकाई और कुल लागत एवं विक्रय मूल्य के साथ अनुमान पंक्तियों का सपाट ग्रिड प्रदर्शित करता है.  
  
## <a name="time-phased-view-of-project-estimates"></a>परियोजना अनुमानों का समय-चरणबद्ध दृश्य  
परियोजना अनुमानों के लिए समय-चरणबद्ध दृश्य में, ग्रिड दृश्य से अनुमान डेटा को भूमिका के अनुसार डिफ़ॉल्ट रूप से पिवट में बदल दिया जाता है और वह दृश्य चुने गए टाइम-स्केल में समय-रेखा में अनुमान डेटा विस्तार को दिखाता है.  
  
## <a name="effort-estimate-allocation-based-on-task-mode"></a>कार्य मोड के आधार पर मेहनत अनुमान आबंटन  
समय-चरणबद्ध दृश्य में, कार्य के लिए कुल अनुमानित मेहनत को चुने गए समय-स्केल की प्रति इकाई समय अवधि, मेहनत के घंटों की निश्चित संख्या आबंटित करके वितरित किया जाता है. project service में, कार्य मोड यह निर्धारित करता है कि कार्य की अवधि के दौरान मेहनत का आबंटन कैसे किया जाता है. दो प्रकार के आबंटन हैं, समान आबंटन और कार्य घंटों पर आधारित आबंटन  
  
## <a name="work-hours-based-allocation"></a>कार्य घंटों पर आधारित आबंटन  
किसी कार्य के लिए स्वतः शेड्यूलिंग कार्य मोड उस कार्य पर अनुमानित कई संसाधनों के लिए उसका नियंत्रण करता है, जिनका अनुमान प्रति दिन पूरे कार्य घंटों के लिए उपयोग में लाए जाने के लिए किया जाता है. यह समय-चरणबद्ध दृश्य में भी कार्यों की अवधि में इसे विभाजित करके मेहनत के आबंटन के समय लागू होता है. उदाहरण के लिए, प्रति ‘दिन’ समय-स्केल पर, एक संसाधन द्वारा पूरा किए जाने वाले किसी अनुमानित कार्य के लिए, प्रति दिन आबंटित मेहनत की समय सीमा परियोजना कैलेंडर में निर्धारित प्रति दिन कार्य घंटों से अधिक नहीं होगी. इसलिए, मेहनत आबंटन हमेशा यह सुनिश्चित करता है कि संसाधनों का अनुमान पूरे दिन के लिए उन्हें उपयोग में लाने के लिए लगाया गया है.  
  
## <a name="even-distribution"></a>समान वितरण  
मैन्युअल तरीके से शेड्यूल किए गए कार्य मोड में कार्य घंटों, परियोजना कैलेंडर या कार्य के लिए निर्धारित संसाधनों की संख्या पर ध्यान नहीं दिया जाता. कार्य शेड्यूल उपयोगकर्ता सहयोग पर आधारित होता है. ऐसे कार्यों के लिए, चुने गए समय-स्केल की प्रति इकाई समय अवधि में मेहनत आबंटन की कोई सीमा नहीं होती. कार्य पर लगने वाली कुल मेहनत को बराबर विभाजित किया जाता है और चुने गए समय-स्केल पर प्रत्येक इकाई समय अवधि के लिए आबंटित कर दिया जाता है.  
  
इस प्रकार, कार्य पर निर्धारित कार्य मोड मेहनत वितरण या समय-चरणबद्ध अनुमानों में प्रति इकाई समय अवधि में मेहनत के आबंटन को निर्धारित करता है.  
  
## <a name="grouping-and-time-phasing-options"></a>समूहीकरण और समय-चरणबद्ध करने के विकल्प  
इस दृश्य से आपको प्रति दिन, सप्ताह, माह या वर्ष के आधार पर मेहनत, लागत और विक्रय अनुमानों को समझने में मदद मिलती है. 'इसके अनुसार समूहीकृत करें' विकल्प से पिवट कार्रवाई द्वारा दो अन्य आयामों पर डेटा का अनुमान लगाया जा सकता है: श्रेणी और संसाधन. ग्रिड दृश्य और समय-चरणबद्ध दृश्य, दोनों में आप प्रदर्शित की जाने वाली फ़ील्ड चुन सकते हैं. प्रत्येक समय ब्लॉक के लिए कुलयोग निचले भाग में प्रदर्शित किया जाता है, जो उस दिन, सप्ताह, माह या वर्ष के दौरान कुल अनुमानित मेहनत, लागत, और विक्रय को इंगित करता है.  
  
लागत और विक्रय मूल्य डिफ़ॉल्ट क्रिया दिनांक प्रभावी होती है—जब भूमिकाओं के लिए दरें बदलेंगी, तो सप्ताह के अनुसार ‘संसाधन’ और समय-चरणबद्ध पर अनुमानित डेटा को पिवट करने पर यह समय-चरणबद्ध दृश्य में अधिक पारदर्शी होगी.  
  
## <a name="expense-estimates"></a>व्यय अनुमान  
परियोजना में होने वाले सभी व्यय, जो व्यय किए जाने वाले श्रम से सीधे तौर पर संबंधित नहीं हैं, को ग्रिड दृश्य में परियोजना अनुमानों में रिकॉर्ड किया जा सकता है. ग्रिड दृश्य में **व्यय अनुमान जोड़ें** विकल्प का उपयोग करके, आप इसे पूरा कर सकते हैं. इन व्यय अनुमानों को किसी विशिष्ट कार्य या संपूर्ण परियोजना के लिए रिकॉर्ड किया जा सकता है; आप इन पंक्तियों में व्यय श्रेणियाँ चुन सकते हैं और कोई ऐसा संभावित दिनांक चुन सकते हैं, जब ऐसा व्यय होना अपेक्षित हो. यदि संबंधित लागत और विक्रय मूल्य सूची में डिफ़ॉल्ट मूल्य हों या विक्रय श्रेणियों के लिए मार्कअप प्रतिशत निर्धारित किए गए हों, तो संबद्धता की स्थिति में अनुमान पंक्ति पर उसे डिफ़ॉल्ट बना दिया जाएगा.  
  
### <a name="see-also"></a>यह भी देखें  
 [परियोजना प्रबंधक मार्गदर्शिका](../psa/project-manager-guide.md)