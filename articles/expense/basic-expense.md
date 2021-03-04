---
title: व्यय प्रविष्टि (लाइट)
description: यह विषय लाइट परिनियोजन में व्यय प्रविष्टि के साथ काम कैसे किया जाए, यह जानकारी देता है.
author: stsporen
manager: AnnBe
ms.date: 11/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: d87094882751f0751a8d9d539fa4cdcfc6b7b0d7
ms.sourcegitcommit: 16c442258ba24c79076cf5877a0f3c1f51a85f61
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/20/2020
ms.locfileid: "4590948"
---
# <a name="expense-entry-lite"></a>व्यय प्रविष्टि (लाइट)

_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_

बेसिक, या लाइट, व्यय प्रबंधन सामान्य व्यय रिकॉर्ड करने की क्षमता है. आप परियोजना के सापेक्ष खर्च दर्ज कर सकते हैं, और फिर परियोजना अनुमोदक इसकी समीक्षा करेंगे और उन्हें स्वीकृत करेंगे.

Dynamics 365 Project Operations में व्यय क्षमताओं के बारे में अधिक जानकारी के लिए, [व्यय ओवरव्यू](expense-overview.md) देखें.

## <a name="capture-a-basic-expense"></a>मूल व्यय अधिकृत करें

आप अपने व्यय अधिकृत कर सकते/सकती हैं ताकि आप उन्हें स्वीकृति के लिए सबमिट कर सकें.

1. **व्यय** पर जाएँ, और **नया** चुनें.
2. **नया खर्च** पेज पर, ज़रूरी व्यय जानकारी दर्ज करें और **सहेजें** चुनें.

## <a name="submit-a-basic-expense"></a>मूल व्यय सबमिट करें

जब आप अपने सभी व्यय अधिकृत कर लेते/लेती हैं और आप उनको स्वीकृत कराने के लिए तैयार होते/होती हैं, तो आपको उन्हें सबमिट करना होगा.

1. **व्यय** पर जाएँ, और व्यय चुनें. या, शीर्ष लेख पर चेक बॉक्स इस्तेमाल करके सभी व्यय चुनें.
2. **सबमिट करें** चुनें. सिस्टम चुनी गई प्रविष्टियों को संसाधित करता है और फिर व्यय स्वीकृत करने के लिए अनुरोध बनाता है.

## <a name="add-an-attachment"></a>एक अनुलग्नक जोड़ें

आपको अपने व्यय के बारे में अनुमोदनकर्ता को अतिरिक्त दस्तावेज़ प्रदान करना पड़ सकता है. आप व्यय प्रविष्टि की टाइमलाइन में रसीद संलग्न कर सकते हैं. **संपादित करें** और **टाइमलाइन** सेक्शन चुनें और उसके बाद अपनी रसीद संलग्न करने के लिए पेपरक्लिप आइकन का उपयोग करें.

## <a name="recall-a-basic-expense"></a>मूल व्यय को रिकॉल करें

जब आप भूल से कोई व्यय सबमिट करते/करती हैं, तो आप इसे रिकॉल कर सकते/सकती हैं. व्यय प्रविष्टि को रिकॉल करने के लिए ज़रूरी समय इसके स्वीकृति चरण पर निर्भर करता है.  यदि अनुमोदक ने अब तक प्रविष्टि स्वीकार नहीं की है, तो रिकॉल तुरंत हो सकता है. फिर भी, अगर प्रविष्टि पहले से ही स्वीकृत हो गई है, तो अनुमोदक को लेनदेन को रिकॉल और रिवर्स करने के लिए कहा जाता है.

1. **व्यय** पर जाएं और व्यय सूची में रिकॉल करने के लिए व्यय चुनें.
2. **रीकॉल** चुनें। अगर अब तक व्यय प्रविष्टि स्वीकृत नहीं हुई है, तो सिस्टम तुरंत इसे रिकॉल करता है. अगर व्यय प्रविष्टि पहले ही स्वीकृत की जा चुकी है, तो अनुमोदक को सूचना देने के लिए रिकॉल अनुरोध बनाया जाता है कि आप व्यय को रिवर्स करना चाहते/चाहती हैं. फिर अनुमोदक पुष्टि करेगा कि रिवर्स किया जा सकता है और प्रविष्टि वापस की जाएगी.

## <a name="delete-a-basic-expense"></a>मूल व्यय हटाएं

अब तक सबमिट नहीं किये गये व्यय हटाए जा सकते हैं. पहले सबमिट किए गए व्यय को हटाने के लिए, आपको पहले इसे रिकॉल करना होगा.

## <a name="see-also"></a>इसे भी देखें

- [अनुमोदनों का अवलोकन](../approvals/approvals-overview.md)