---
title: परियोजना अनुबंधों पर परियोजना मूल्य सूचियाँ प्रबंधित करें
description: यह विषय परियोजना अनुबंधों पर परियोजना मूल्य सूचियाँ प्रबंधित करने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/27/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 030684576e1f53d27921907b07c9e5e0c5efe612
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4133355"
---
# <a name="manage-project-price-lists-on-project-contracts"></a>परियोजना अनुबंधों पर परियोजना मूल्य सूचियाँ प्रबंधित करें

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

Dynamics 365 Project Operations में परियोजना अनुबंध किसी अनुबंध पर कई दिनांक प्रभावी विक्रय मूल्य सूचियों का समर्थन करने के लिए डिज़ाइन किया गया है. Project Operations में, **परियोजना मूल्य सूचियाँ** नामक एक नया संबद्ध निकाय मौजूद है. इस निकाय का परियोजना अनुबंध के साथ वन-टू-मैनी संबंध है.

परियोजना मूल्य सूचियों का उपयोग किसी परियोजना पर समय और ख़र्च की लेनदेन की कीमत लगाने के लिए किया जाता है. जब किसी अनुबंध में एक या अधिक परियोजना मूल्य सूचियाँ होती हैं, तो इन मूल्य सूचियों का उपयोग समय और व्यय अनुमानों और उन परियोजनाओं पर वास्तविक का मूल्यांकन करने के लिए किया जाता है, जो अनुबंध पंक्ति के माध्यम से अनुबंध से संबद्ध हैं.

जब किसी परियोजना अनुबंध पर कोई परियोजना मूल्य सूची नहीं होती है, तो आपको एक चेतावनी संदेश दिखाई देगा कि परियोजना मूल्य सूचियाँ नहीं है और आपके अनुमानों, वास्तविक परियोजना कार्य और व्ययों का मूल्यांकन नहीं किया जाएगा. विक्रय मानों के लिए कोई मूल्य नहीं होगा.

## <a name="associate-or-unassociate-a-project-price-list-on-a-project-contract"></a>परियोजना अनुबंध से परियोजना मूल्य सूची संबद्ध करें या असंबद्ध करें

### <a name="create-or-associate-a-specific-price-list-for-estimating-project-based-work-and-expenses"></a>परियोजना-आधारित कार्य और व्ययों के आकलन के लिए एक विशिष्ट मूल्य सूची बनाएं या संबद्ध करें

1. परियोजना अनुबंध पर, **परियोजना मूल्य सूचियाँ** टैब चुनें.
2. सबग्रिड में, **+ नई परियोजना मूल्य सूची जोड़ें** चुनें.
3. **त्वरित बनाएँ** स्लाइडर पर, एक मूल्य सूची चुनें. 

  ड्रॉप-डाउन सूची उन सभी मूल्य सूचियों को दिखाती है, जिनका संदर्भ **विक्रय** पर सेट है, जहां मूल्य सूची की मुद्रा अनुबंध की मुद्रा से मेल खाती है.
  
4. परियोजना मूल्य सूची संबद्धता के लिए एक विवरण दर्ज करें, **सहेजें** चुनें और उसके बाद **त्वरित बनाएँ** स्लाइडर बंद करें.

   एक परियोजना मूल्य सूची संबंद्ध बनाया जाता है.
   
5. परियोजना अनुबंध से एक से अधिक परियोजना मूल्य सूची संबद्ध करने के लिए चरण 1-4 दोहराएँ. यदि प्रत्येक संबद्ध परियोजना मूल्य सूची पर आपके पास भिन्न दिनांक प्रभाविकता है, तो केवल एकाधिक परियोजना मूल्य सूचियाँ बनाएँ.

> [!NOTE]
> Project Operations परियोजना मूल्य सूचियों की दिनांक प्रभावकारिता को ओवरलैप करने का समर्थन नहीं करता है. यदि किसी दिए गए दिनांक वाले ट्रांज़ैक्शन के लिए कई परियोजना मूल्य सूचियाँ हैं, तो उस ट्रांज़ैक्शन का मूल्य डिफ़ॉल्ट रूप से शून्य होगा.

### <a name="remove-a-project-price-list-association"></a>परियोजना मूल्य सूची संबद्धता निकालें

- परियोजना मूल्य सूची चुनें और उसके बाद सबग्रिड पर **अनुबंध परियोजना मूल्य सूची हटाएं** चुनें. 

  मूल्य सूची को अनुबंध की परियोजना मूल्य सूचियों से हटा दिया जाता है. मूल्य सूची स्वयं नहीं हटाई जाएगी. केवल अनुबंध की संबद्धता को हटा दिया जाएगा.

## <a name="set-up-automatic-defaulting-of-project-price-lists-on-a-contract"></a>अनुबंध पर परियोजना मूल्य सूचियों की स्वचालित डिफ़ॉल्टिंग सेट अप करें

परियोजना मूल्य सूची को परियोजना अनुबंध पर डिफ़ॉल्ट सूची के रूप में स्थापित किया जा सकता है. यह सेटअप यह सुनिश्चित करने में मदद कर सकता है कि आपके संगठन के सभी अनुबंध हमेशा उस मूल्य अवधि के लिए एक मानक मूल्य सूची के साथ शुरू होते हैं.

### <a name="set-up-the-organizational-default-for-project-price-lists"></a>परियोजना मूल्य सूचियों के लिए संगठनात्मक डिफ़ॉल्ट सेट अप करें

1. **सेटिंग** > **सामान्य** पर जाएँ और उसके बाद **पैरामीटर** चुनें.
2. **सक्रिय पैरामीटर** सूची पृष्ठ में, रिकॉर्ड को खोलने के लिए उसे चुनें और उस पर डबल-क्लिक करें. डबल-क्लिक करते समय, सुनिश्चित करें कि आप हाइपरलिंक वाले फ़ील्ड मान पर क्लिक नहीं कर रहे हैं. 
3. **सक्रिय पैरामीटर** पृष्ठ पर, **मूल्य सूची** टैब चुनें. सबग्रिड डिफ़ॉल्ट मूल्य सूचियों की एक सूची दिखाती है. यह मानक लागत और विक्रय मूल्य सूचियों की एक सूची है. उस प्रत्येक मुद्रा के लिए जिसमें आप समान बेचते हैं यहाँ एक **विक्रय** मूल्य सूची संबद्ध होना सुनिश्चित करता है कि विक्रय मूल्य सूची उस किसी भी अनुबंध के लिए डिफ़ॉल्ट है, जो आप उन ग्राहकों के लिए बनाते हैं, जो इस मुद्रा में लेनदेन करते हैं.

### <a name="set-up-a-customer-specific-project-price-list"></a>ग्राहक-विशिष्ट परियोजना मूल्य सूची सेट अप करें

जब अपने ग्राहकों के साथ मास्टर मूल्य निर्धारण समझौते पर बातचीत की होती है, तो आप ग्राहक-विशिष्ट परियोजना मूल्य सूचियाँ भी सेट अप कर सकते हैं.

1. **विक्रय** > **ग्राहक** पर जाएँ.
2. सक्रिय खातों की सूची से, वह ग्राहक चुनें, जिसके लिए आपके पास विशेष मूल्य सूची है.
3. ग्राहक रिकॉर्ड को खोलने के लिए उसे चुनें और उसके बाद **परियोजना मूल्य सूची** टैब चुनें. सबग्रिड इस ग्राहक के लिए परियोजना मूल्य सूचियों की एक सूची दिखाती है. 
4. यहाँ एक नई मूल्य सूची संबद्धता बनाएँ, ताकि इस ग्राहक के पास विशिष्ट परियोजना मूल्य सूची हो.

## <a name="custom-pricing-on-a-project-contract"></a>परियोजना अनुबंध पर कस्टम मूल्य निर्धारण

आपके पास संगठनात्मक और ग्राहक-विशिष्ट डिफ़ॉल्ट परियोजना मूल्य सूचियाँ होने के बाद, आपके परियोजना अनुबंध इन परियोजना मूल्य सूची संबद्धता के साथ स्वचालित रूप से बन जाएंगे. हालाँकि, परियोजना अनुबंध की परियोजना मूल्य सूचियाँ हमेशा दिनांक और अनुबंध नाम के साथ कॉपी की जाती हैं. उसके बाद खाता और परियोजना प्रबंधक इन प्रतियों पर मूल्यों का संपादन करना शुरू कर सकते हैं. ये बदले हुए मूल्य केवल इस परियोजना अनुबंध पर लागू होंगे.