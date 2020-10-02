---
title: मुद्रा
description: यह विषय Project Operations में मुद्रा प्रकारों को जोड़ने और हटाने के बारे में जानकारी देता है.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: d53bae2f64e7b427f762161ff08917598217bb5a
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/28/2020
ms.locfileid: "3898353"
---
# <a name="currency"></a>मुद्रा

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

मुद्राएँ उत्पाद कैटलॉग में उत्पादों के लिए मूल्यों और विक्रय ऑर्डर जैसे लेन-देनों की लागत का निर्धारण करती हैं. यदि आपके ग्राहक भौगोलिक क्षेत्रों में फैले हैं, तो अपने लेनदेन को प्रबंधित करने के लिए उनकी मुद्राओं को जोड़ें. ऐसी मुद्राएँ जोड़ें जो आपकी वर्तमान और भावी व्यावसायिक आवश्यकताओं के लिए सबसे उपयुक्त हो.  

> [!NOTE]
> यदि आपका परिवेश एक Common Data Service परिवेश है और आप Power Platform व्यवस्थापन केंद्र में हैं और आप **मुद्राएँ** पृष्ठ (**परिवेश** > [परिवेश चुनें] > **सेटिंग** > **व्यवसाय** > **मुद्राएं**) चुनते हैं, तो पृष्ठ रिक्त होगा. ऐसा इसलिए है क्योंकि Common Data Service परिस्थिति में मुद्रा स्थापन समर्थित नहीं है.

## <a name="add-a-currency"></a>एक मुद्रा जोड़ें  
आप प्रक्रिया शुरू करने से पहले यह सत्यापित करें कि आपकी सुरक्षा भूमिका में सिस्टम व्यवस्थापक अनुमतियां शामिल हैं. 

1. Power Platform व्यवस्थापक केंद्र में, एक परिवेश का चयन करें. 
2. **सेटिंग** > **व्यवसाय** चुनें
3. **मुद्राएँ** चुनें.  
4. **नया** चुनें.  
5. आवश्यकतानुसार, जानकारी भरें.  


   |          फील्ड          |                                                                                                                                                                                                                                                                                                                                                                            वर्णन                                                                                                                                                                                                                                                                                                                                                                            |
   |-------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
   |    **मुद्रा प्रकार**    | - **सिस्टम** - यदि आप Dynamics 365 में मॉडल-चालित ऐप में उपलब्ध मुद्राओं का उपयोग करना चाहते हैं, तो यह विकल्प चुनें. मुद्रा ढूंढने के लिए, **लुकअप** चुनें. जब आप कोई मुद्रा कोड चुनते हैं, तो चयनित मुद्रा के लिए **मुद्रा का नाम** और **मुद्रा का प्रतीक** स्वचालित रूप से जुड़ जाता है.<br />- **कस्टम** - यदि आप एक ऐसी मुद्रा जोड़ना चाहते हैं जो Dynamics 365 में मॉडल-चालित ऐप्स में उपलब्ध नहीं है. ऐसी स्थिति में, आपको **मुद्रा कोड**, **मुद्रा की शुद्धता**, **मुद्रा का नाम**, **मुद्रा का प्रतीक** और **मुद्रा का रूपांतरण** के मान मैन्युअल रूप से दर्ज करने होंगे. |
   |    **मुद्रा कोड**    |                                                                                                                                                                                                                                                                                                                                            मुद्रा का लघु रूप. उदाहरण के लिए युनाइटेड स्टेट्स डॉलर के लिए **USD**.                                                                                                                                                                                                                                                                                                                                            |
   | **मुद्रा शुद्धता**  |                                                                                                                                                                                  उन दशमलवों की संख्या टाइप करें जिसका आप मुद्रा के लिए उपयोग करना चाहते हैं.  आप 0 और 4 के बीच का एक मान जोड़ सकते हैं. **ध्यान दें:**  यदि आपने **सिस्टम सेटिंग** संवाद बॉक्स में कोई शुद्धता मान सेट किया है, तो वह मान यहां दिखाई देगा.                                                                                                                                                                                  |
   |    **मुद्रा नाम**    |                                                                                                                                                                                                                                         यदि आपने Dynamics 365 में मॉडल-चालित ऐप में उपलब्ध मुद्राओं की सूची से एक मुद्रा कोड चुना है, तो चयनित कोड के लिए मुद्रा का नाम यहां प्रदर्शित होता है. यदि आपने मुद्रा प्रकार के रूप में **कस्टम** का चयन किया है, तो मुद्रा का नाम टाइप करें.                                                                                                                                                                                                                                          |
   |   **मुद्रा चिह्न**   |                                                                                                                                                                                                                                                                      यदि आपने उपलब्ध मुद्राओं की सूची में से एक मुद्रा कोड चुना है, तो चयनित मुद्रा के लिए प्रतीक यहां प्रदर्शित होता है. यदि आपने मुद्रा प्रकार के रूप में **कस्टम** का चयन किया है, तो नई मुद्रा के लिए प्रतीक दर्ज करें.                                                                                                                                                                                                                                                                       |
   | **मुद्रा परिवर्तन** |                                                                                                                                                                                                                                     चयनित मुद्रा का मान एक यूएस डॉलर के रूप में दर्ज करें. यह वह राशि है जिस पर चयनित मुद्रा बेस मुद्रा पर रूपांतरित की जाति है. **महत्वपूर्ण:**  अपने लेन-देनों में किसी गलत परिकलन से बचने के लिए, इस मान को नियमित रूप से अपडेट करना न भूलें.                                                                                                                                                                                                                                      |


6. यह पूरा कर लेने के बाद, आदेश पट्टी पर, **सहेजें** या **सहेजें और बंद करें** चुनें.  

   > [!TIP]
   >  किसी मुद्रा को संपादित करने के लिए, मुद्रा चुनें और उसके बाद नए मान दर्ज करें या चुनें.  

## <a name="delete-a-currency"></a>एक मुद्रा हटाएं  

1. Power Platform व्यवस्थापक केंद्र में, एक परिवेश का चयन करें. 
2. **सेटिंग** > **व्यवसाय** चुनें.
3. **मुद्राएँ** चुनें.  
4. प्रदर्शित मुद्राओं की सूची से, हटाने के लिए मुद्रा चुनें.  
5. **हटाएँ** चुनें.  
6. हटाने की पुष्टि करें.  

> [!IMPORTANT]
>  आप ऐसी मुद्राएं नहीं हटा सकते, जिसका अन्य रिकॉर्ड द्वारा उपयोग किया जा रहा हो; आप उन्हें केवल निष्क्रिय कर सकते हैं. मुद्रा रिकॉर्ड निष्क्रिय करने से अवसर या ऑर्डर जैसे वर्तमान रिकॉर्ड में संग्रहित मुद्रा जानकारियाँ निकलती नहीं हैं. हालांकि, आप नए ट्रांज़ैक्शन के लिए निष्क्रिय की गई मुद्रा का चयन नहीं कर पाएंगे.  