---
title: ठेका श्रमिकों और उपसंविदा क्षमता के साथ एक परियोजना का स्टाफिंग
description: यह विषय बताता है कि Microsoft में अनुबंध कर्मचारियों या उप-अनुबंधित क्षमता का उपयोग करके परियोजना आवश्यकताओं को कैसे पूरा किया जा सकता है।Dynamics 365 Project Operations
author: rumant
ms.date: 12/03/2021
ms.topic: article
ms.reviewer: tonyafehr
ms.author: rumant
ms.openlocfilehash: 7e9a0ca08f472999138589f31ca820b733b6303e
ms.sourcegitcommit: 04dc8d952e6da3ab3eb2a20131c6f7cee6040876
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 12/10/2021
ms.locfileid: "7903673"
---
# <a name="staffing-a-project-with-contract-workers-and-subcontracted-capacity"></a>ठेका श्रमिकों और उपसंविदा क्षमता के साथ एक परियोजना का स्टाफिंग

[!include [banner](../../includes/dataverse-preview.md)]

_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_

जेनेरिक प्रोजेक्ट टीम के सदस्यों को कर्मचारियों या अनुबंध श्रमिकों के साथ रखा जा सकता है। ठेका श्रमिकों के साथ एक परियोजना में काम करते समय, आप अपने स्टाफिंग विकल्पों को विशिष्ट अनुबंध श्रमिकों तक सीमित कर सकते हैं जिन्हें एक उप-ठेकेदार लाइन को सौंपा गया है। 

## <a name="search-for-staff-resource-requirements-with-contract-workers-that-belong-to-a-specific-subcontract-line"></a>एक विशिष्ट उप-अनुबंध लाइन से संबंधित अनुबंध श्रमिकों के साथ स्टाफ संसाधन आवश्यकताओं की खोज करें

एक विशिष्ट उपठेकेदार लाइन से संबंधित ठेका श्रमिकों के साथ और स्टाफ संसाधन आवश्यकताओं की खोज करने के लिए, इन चरणों का पालन करें:

1. एक सामान्य प्रोजेक्ट टीम सदस्य बनाएं जो उप-अनुबंध और उप-अनुबंध लाइन का संदर्भ देता है।
2. का उपयोग करके इस सामान्य परियोजना टीम के सदस्य के लिए संसाधन आवश्यकता उत्पन्न करें **आवश्यकता उत्पन्न करें** प्रोजेक्ट टीम के सदस्य सब ग्रिड पर बटन।
3. टीम सदस्य पंक्ति का चयन करें और फिर चुनें **पुस्तक** सब ग्रिड पर बटन। 
4. यह आवश्यकता संदर्भ के साथ शेड्यूल बोर्ड खोलता है। दिनांक, भूमिका और संगठनात्मक इकाई फ़ील्ड जैसी अन्य विशेषताओं के साथ, शेड्यूल बोर्ड फ़िल्टर भी संसाधन आवश्यकता से विक्रेता, उप-अनुबंध, और उप-अनुबंध लाइन फ़ील्ड के साथ स्वचालित रूप से भर जाते हैं।
5. सिस्टम उन संसाधनों की खोज करता है जो फ़िल्टर मानदंड को पूरा करते हैं और उन्हें सूचीबद्ध करते हैं। 
6. फ़िल्टर किए गए संसाधनों में से किसी एक का चयन करें और आवश्यकता के लिए संसाधन बुक करें। 
7. एक प्रोजेक्ट टीम सदस्य को उप-अनुबंध और उप-अनुबंध लाइन संदर्भों के साथ बनाया और अद्यतन किया जाता है। के लिए जाओ **परियोजना अनुमान** और चुनें **कीमतों को अपडेट करें** संसाधन असाइनमेंट की अद्यतन लागत देखने के लिए। 

> [!NOTE]
> प्रोजेक्ट टीम के सदस्य को उप-अनुबंध और उप-अनुबंध लाइन संदर्भ के साथ अद्यतन करना बुकिंग के दौरान हमेशा संभव नहीं हो सकता है यदि संसाधन एकाधिक उप-अनुबंध लाइनों को असाइन किया गया है। यदि सिस्टम प्रोजेक्ट टीम के सदस्य को सब-कॉन्ट्रैक्ट और सब-कॉन्ट्रैक्ट लाइन के साथ अपडेट करने में असमर्थ है, तो प्रोजेक्ट टीम मेंबर रिकॉर्ड खोलें और इन फील्ड्स को मैन्युअल रूप से अपडेट करें ताकि वित्तीय लागत अनुमान उपठेकेदार लागत को सटीक रूप से प्रतिबिंबित करे।

## <a name="search-for-and-staff-resource-requirements-with-any-contract-worker"></a>किसी भी ठेका कर्मचारी के साथ और स्टाफ संसाधन आवश्यकताओं की खोज करें

किसी ठेका कर्मचारी के साथ और स्टाफ संसाधन आवश्यकताओं की खोज करने के लिए, इन चरणों का पालन करें:

1. एक सामान्य प्रोजेक्ट टीम सदस्य बनाएँ।
2. का उपयोग करके इस सामान्य परियोजना टीम के सदस्य के लिए संसाधन आवश्यकता उत्पन्न करें **आवश्यकता उत्पन्न करें** प्रोजेक्ट टीम के सदस्य सब ग्रिड पर बटन।
3. टीम सदस्य पंक्ति का चयन करें और फिर चुनें **पुस्तक** सब ग्रिड पर बटन। 
4. यह आवश्यकता संदर्भ के साथ शेड्यूल बोर्ड खोलता है। दिनांक, भूमिका और संगठनात्मक इकाई फ़ील्ड जैसी अन्य विशेषताओं के साथ, शेड्यूल बोर्ड फ़िल्टर भी संसाधन आवश्यकता से विक्रेता, उप-अनुबंध, और उप-अनुबंध लाइन फ़ील्ड के साथ स्वचालित रूप से भर जाते हैं। चूंकि आवश्यकता में कोई उप-अनुबंध या उप-अनुबंध पंक्ति मान नहीं भरा गया था, इसलिए ये विशेषताएँ फ़िल्टर फलक पर खाली होंगी।
5. सिस्टम उन संसाधनों की खोज करता है जो फ़िल्टर मानदंड को पूरा करते हैं और उन्हें सूचीबद्ध करते हैं।
6. अपडेट करें **कार्यकर्ता प्रकार** फ़िल्टर फलक पर फ़ील्ड **संविदा कर्मचारी** खोज को ठेका श्रमिकों तक सीमित करने के लिए। अद्यतन **विक्रेता** फ़िल्टर फलक पर एक विक्रेता का चयन करने के लिए खोज को सीमित करने के लिए केवल एक विशिष्ट विक्रेता कंपनी से संबंधित अनुबंध श्रमिकों को दिखाने के लिए।
7. सूची से एक ठेका कर्मचारी का चयन करें और आवश्यकता के लिए संसाधन बुक करें।
8. एक प्रोजेक्ट टीम सदस्य बनाया गया है। हालांकि, प्रोजेक्ट टीम के सदस्य को किसी भी उप-अनुबंध या उप-अनुबंध लाइन के साथ अद्यतन नहीं किया जाता है और इसलिए उप-अनुबंध मूल्य निर्धारण का उपयोग करके संसाधन असाइनमेंट की लागत नहीं ली जाएगी। प्रोजेक्ट टीम के सदस्य को उप-अनुबंध लाइन के साथ मैन्युअल रूप से अपडेट करें और यहां जाएं **परियोजना अनुमान** और चुनें **कीमतों को अपडेट करें** संसाधन असाइनमेंट की अद्यतन लागत देखने के लिए।

> [!NOTE]
> प्रोजेक्ट टीम के सदस्य जिनके पास है **कार्यकर्ता प्रकार** जैसा**संविदा कर्मचारी** लेकिन एक उपठेकेदार संदर्भ नहीं है के रूप में चिह्नित कर रहे हैं **अमान्य** पर **प्रोजेक्ट टीम के सदस्य** ग्रिड। यदि इस स्थिति के साथ कोई प्रोजेक्ट टीम सदस्य हैं, तो प्रोजेक्ट टीम सदस्य रिकॉर्ड खोलें और उप-अनुबंध और उप-अनुबंध लाइन फ़ील्ड को मैन्युअल रूप से अपडेट करें ताकि वित्तीय लागत अनुमान सटीक रूप से उप-ठेकेदार लागत को प्रतिबिंबित कर सके **अनुमान** टैब। 


[!INCLUDE[footer-include](../../includes/footer-banner.md)]