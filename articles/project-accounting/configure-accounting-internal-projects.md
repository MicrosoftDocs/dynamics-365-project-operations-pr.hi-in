---
title: आंतरिक परियोजनाओं के लिए लेखांकन कॉन्फ़िगर करें
description: यह विषय परियोजना संचालन की आंतरिक परियोजनाओं के लिए किस तरह लेखांकन प्रथाओं को तैयार किया जाए, पर जानकारी प्रदान करता है.
author: sigitac
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ea04178d4327ccd701ab431f172463a13a55154e
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4132380"
---
# <a name="configure-accounting-for-internal-projects"></a>आंतरिक परियोजनाओं के लिए लेखांकन कॉन्फ़िगर करें

_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_

आंतरिक परियोजनाएं कंपनियों को गतिविधियों संबंधित लागत ट्रैक करने की अनुमति प्रदान करती हैं, जिनका बिल ग्राहक को नहीं दिया जाता. आंतरिक परियोजनाओं के उदाहरण, जिनमें शामिल हैं:

- किसी प्रोडक्ट को बनाना जैसे कि मोबाइल ऐप और विकास से जुड़ी लागत को ट्रैक करना.
- बिक्री से पहले के समय और व्यय का प्रबंधन करना. यदि निविदा को जीत लिया जाता है तो बिक्री से पहले की इस आंतरिक परियोजना को बाद में बिल योग्य परियोजना में परिवर्तित किया जा सकता है.

जो परियोजना Dynamics 365 Project Operations के अनुबंध से नहीं जुड़ी होती है, उसे आंतरिक माना जाता है. परियोजना की लागत और राजस्व प्रोफाइल का उपयोग परियोजना के लेखांकन नियमों को निर्धारित करने के लिए नहीं किया जाता है. लाभ और घाटा/हानि सिद्धांतों का उपयोग करके आंतरिक परियोजना लागत को हमेशा पोस्ट किया जाता है. **लेजर पोस्टिंग सेटअप** पृष्ठ/पन्ने पर पोस्टिंग के लिए लेजर खातों को परिभाषित किया गया है.

- **लागत** खाता को डेबिट करके और **पेरोल एलोकेशन** खाता को क्रेडिट करके समय के लेन-देन को पोस्ट किया जाता है.
- **लागत** खाता को डेबिट करके और **खर्च के लिए ऑफसेट खाता** को क्रेडिट करके खर्च के लेन-देन को पोस्ट किया जाता है.

परियोजना के लिए लेन-देन को पोस्ट करने के बाद, यदि परियोजना अनुबंध से जुड़ी परियोजना है तो सिस्टम सभी जमा लेन-देन को बदल देता है और नए बिल योग्य लेन-देन बना देता है. बिल योग्य लेनदेन संबंधित परियोजना लागत और राजस्व प्रोफ़ाइल में परिभाषित लेखांकन नियमों का पालन करते हैं।

