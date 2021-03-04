---
title: संसाधन बुकिंग और वे कार्य असाइनमेंट से कैसे संबंधित हैं
description: यह विषय नामित संसाधनों, संसाधन बुकिंग और कार्य असाइनमेंट को प्रबंधित करने के तरीके और वे एक दूसरे से कैसे संबंधित हैं, के बारे में जानकारी प्रदान करता है।
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 9/27/2019
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
ms.openlocfilehash: c4b976b49bd643bc7a774a86b1ba89bd76d7c916
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4125000"
---
# <a name="resource-bookings-and-how-they-relate-to-task-assignments"></a>संसाधन बुकिंग और वे कार्य असाइनमेंट से कैसे संबंधित हैं


ऐसे दो तरीके हैं जिनसे नामित संसाधन किसी प्रोजेक्ट टीम के लिए बुक किए जा सकते हैं और उन्हें कार्य असाइन किए जा सकते हैं:

- संसाधन सीधे किसी प्रोजेक्ट के लिए बुक किया जा सकता है, और फिर प्रोजेक्ट कार्यों को असाइन किया जा सकता है.
- किसी ऐसे जेनेरिक संसाधन को कार्य असाइन किए जा सकते हैं, बाद में जेनेरिक को ढूँढकर उसे एक नामित संसाधन के साथ बदलने के लिए जिसका उपयोग किया जाता है. 

दोनों मामलों में, संसाधन बुक करना संसाधन की क्षमता को सुरक्षित रखता है.

प्रोजेक्ट की योजना बनाने वाला प्रोजेक्ट प्रबंधक ही प्रोजेक्ट की योजना और शेड्यूल का स्वामी होता है. असाइनमेंट के लिए जेनेरिक संसाधन का उपयोग करके और फिर उससे एक संसाधन अनुरोध जनरेट करके, प्रोजेक्ट प्रबंधक प्रोजेक्ट की योजना में निर्दिष्ट रूपरेखा के साथ प्रोजेक्ट के लिए संसाधन बुक कर सकता है. वे किसी प्रोजेक्ट के लिए संसाधन बुक कर सकते हैं और फिर उन्हें कार्यों को असाइन कर सकते हैं, लेकिन बुकिंग की रूपरेखा को कार्यों की रूपरेखा के साथ संरेखित करने का कोई तरीका नहीं है. बुकिंग प्रोजेक्ट शेड्यूल को प्रभावित नहीं करती है।

एकाधिक ओवरलैपिंग कार्यों वाले एक जटिल प्रोजेक्ट पर विचार करें जहाँ समान प्रकार के एकाधिक संसाधनों को एक साथ कार्य करने की आवश्यकता होगी. यदि किसी संसाधन को ऐसी रूपरेखा प्रदान की जाती है जो उसकी कुल असाइनमेंट्स से अलग है, तो बुकिंग्स की रूपरेखा को उसके डिस्क्रीट कार्यों और उसकी मूल रूपरेखा के अनुरूप बनाने के लिए कार्यों को संशोधित करना कठिन होता है.

नीचे दिए गए उदाहरण में, दो सप्ताह की अवधि में चार कार्यों के एक सेट से समान संसाधन के लिए आवश्यक कुल प्रयास 62 घंटे है और एक विशिष्ट रूपरेखा मौजूद है. यदि समान दो सप्ताहों के दौरान संसाधन बॉब को 62 घंटे के लिए, लेकिन भिन्न रूपरेखा के साथ, बुक किया जाता है, तो आवश्यकता और बुकिंग संरेखित नहीं हैं.

| **कार्य की रूपरेखा**    | **कुल घंटे** | सोम 6/4 | मंगल 6/5 | बुध 6/6 | गुरू 6/7 | शुक्र 6/8 | शनि 6/9 | रवि 6/10 | सोम 6/11 | मंगल 6/12 | बुध 6/13 | गुरू 6/14 | शुक्र 6/15 |
|----------------------|-----------------|--------|--------|--------|--------|--------|--------|---------|---------|---------|---------|---------|---------|
| कार्य 1               | 24              | 8      | 8      | 4      |        |        |        |         |         |         | 4       |         |         |
| कार्य 2               | 16              |        |        | 4      | 4      |        |        |         | 8       |         |         |         |         |
| कार्य 3               | 10              |        |        |        |        | 4      |        |         |         | 4       |         | 2       |         |
| कार्य 4               | 12              |        |        |        |        |        |        |         |         |         | 4       |         | 8       |
|                      |                 |        |        |        |        |        |        |         |         |         |         |         |         |
| **कुल**           | 62              | 8      | 8      | 8      | 4      | 4      |        |         | 8       | 4       | 8       | 2       | 8       |
|                      |                 |        |        |        |        |        |        |         |         |         |         |

### <a name="bobs-availability"></a>बॉब की उपलब्धता
| **संसाधन बुकिंग** | **कुल घंटे** | सोम 6/4 | मंगल 6/5 | बुध 6/6 | गुरू 6/7 | शुक्र 6/8 | शनि 6/9 | रवि 6/10 | सोम 6/11 | मंगल 6/12 | बुध 6/13 | गुरू 6/14 | शुक्र 6/15 |
|------------------------|-----------------|--------|--------|--------|--------|--------|--------|---------|---------|---------|---------|---------|---------|
| बॉब                    | 62              | 4      | 4      | 8      | 8      | 8      |        |         | 4       | 4       | 8       | 8       | 6       |

हालाँकि, प्रति-दिन के आधार पर कार्यों को बुक किए गए घंटों की रूपरेखा असाइन करने करने का कोई व्यवस्थित तरीका नहीं है. यदि प्रोजेक्ट प्रबंधक संसाधन की उपलब्धता को पूरा करने के लिए प्रोजेक्ट के शेड्यूल में बदलाव करने के लिए तैयार है, तो उसे असाइनमेंट को हटाना होगा और बुकिंग की रूपरेखा से मेल खाने के लिए सभी कार्यों को संशोधित करना होगा.

ऐसी स्थिति में जहाँ किसी संगठन ने एक प्रोजेक्ट प्रबंधक और एक संसाधन प्रबंधक, दोनों को प्रोजेक्ट की योजना बनाने का कार्य दिया है, तो प्रोजेक्ट प्रबंधक शेड्यूल सेट करता है और उसमें आवश्यक कार्य की रूपरेखा शामिल होती है. ऐसा नहीं होना चाहिए कि वास्तविक संसाधनों को बुक करते हुए प्रोजेक्ट प्रबंधक की जानकारी के बिना संसाधन प्रबंधक शेड्यूल को प्रभावित कर सके. यदि संसाधन प्रबंधक प्रोजेक्ट मैनेजर द्वारा अनुरोध किए गए कार्य से अलग है, तो उसे इस बारे में सहमत होना होगा कि प्रोजेक्ट के शेड्यूल में क्या परिवर्तन करने की आवश्यकता है.

चूँकि बुकिंग्स और असाइनमेंट्‍स बहुत अधिक युग्मित नहीं हैं, इसलिए कार्य की रूपरेखाओं से अलग रूपरेखाओं को बुक करना या असाइनमेंट्स में ऐसे बदलाव करना संभव है जिसके परिणामस्वरूप ऐसी स्थितियाँ उत्पन्न होती हैं जहाँ बुकिंग्स और असाइनमेंट्स संरेखित नहीं हैं.

**समन्वय दृश्य** प्रोजेक्ट प्रबंधक प्रोजेक्ट टीम के प्रत्येक सदस्य के लिए बुकिंग्स और असाइनमेंट्स देखने की अनुमति देता है. दृश्य यह दिखाने के लिए रंगों और छाया का उपयोग करता है कि टीम के सदस्य की बुकिंग्स और असाइनमेंट्स कहाँ बेमेल हैं. इस जानकारी के आधार पर, प्रोजेक्ट प्रबंधक सुधारात्मक कार्रवाई कर सकता है जिसमें असाइनमेंट्स होने और बुकिंग्स न होने पर संसाधन बुकिंग्स का विस्तार करना या संसाधन बुक होने लेकिन कोई असाइनमेंट न होने की स्थितियों में बुकिंग्स रद्द करना शामिल है.

> [!NOTE]
> यदि आप किसी ऐसे कार्य को हटाते हैं, आपने स्वयं जिसकी रूपरेखा तैयार की है, तो ये रूपरेखाएँ कायम नहीं रखी जातीं. कार्य के घंटों और छुट्टियों में परिवर्तन को शामिल करने के लिए प्रोजेक्ट कैलेंडर के अनुसार रूपरेखाएँ पुन: जनरेट की जाती हैं. यह डिज़ाइन के अनुसार होता है क्योंकि सिस्टम मूल रूपरेखा का प्रयोजन नहीं जानता और यह निर्धारित नहीं कर सकता कि किसी नई समय अवधि में उस रूपरेखा को कायम रखना सही है या नहीं. चूँकि बुकिंग्स और असाइनमेंट्‍स अलग होती हैं, बुकिंग्स मूल बुकिंग रूपरेखाओं को कायम रखती हैं. इस स्थिति में, यदि आपको बुकिंग रद्द करके नई असाइनमेंट रूपरेखा के साथ पुन: बुक करना होगा.
