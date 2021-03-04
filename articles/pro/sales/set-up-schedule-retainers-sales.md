---
title: रिटेनर शेड्यूल सेट अप करें
description: यह विषय Project Operations में रिटेनर शेड्यूल सेट अप करने के तरीके के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/22/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 1c264b544660cf7a0b116f09b6bd7c94fcf0457e
ms.sourcegitcommit: 250270409412ba4cad95fbd4c345a80d3d2b3e53
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/21/2020
ms.locfileid: "4596374"
---
# <a name="set-up-a-retainer-schedule"></a>रिटेनर शेड्यूल सेट अप करें

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

Dynamics 365 Project Operations में **परियोजना अनुबंध** पृष्ठ पर रिटेनर शेड्यूल सेट अप किए जाते हैं.

1. **परियोजना अनुबंध** पृष्ठ पर, **एडवांस और रिटेनर्स** टैब पर, **रिटेनर शेड्यूल सेट अप करें** चुनें.
2. खुलने वाले संवाद पृष्ठ पर, निम्न तालिका में सूचीबद्ध फ़ील्ड दिखाई जाती हैं. तालिका इस बात का अंदाजा देती है कि दर्ज किए गए मान उस रिटेनर शेड्यूल को कैसे प्रभावित करते हैं या असर डालते हैं, जो बनाया जाएगा.

| क्षेत्र | विवरण | डाउनस्ट्रीम प्रभाव |
| --- | --- | --- |
| परियोजना अनुबंध ग्राहक | अनुबंध पर वह ग्राहक, जिसे रिटेनर या एडवांस के लिए इनवॉइस किया जाएगा. | यदि आपके पास अनुबंध पर एकाधिक ग्राहक हैं और यदि आपको उनमें से प्रत्येक को एक विशिष्ट रिटेनर या एडवांस राशि के लिए इनवॉइस करने की आवश्यकता हो, तो प्रत्येक ग्राहक के लिए मैनुअल रूप से एक इनवॉइस बनाएं. |
| रिटेनर शेड्यूल प्रारंभ | रिटेनर शेड्यूल का प्रारंभ दिनांक दर्ज करें. | यह दिनांक, वह दिनांक हो सकता है, जब पहला रिटेनर या एडवांस बनाया गया हो. वह दिनांक, जब पहला रिटेनर या एडवांस बनाया गया होता है, वह इनवॉइस आवृत्ति से भी प्रभावित होता है. |
| रिटेनर शेड्यूल समाप्त | रिटेनर शेड्यूल का समाप्ति दिनांक दर्ज करें. | यह दिनांक, हो सकता है कि वह दिनांक न हो, जब अंतिम रिटेनर या एडवांस बनाया गया था. वह दिनांक, जब अंतिम रिटेनर या एडवांस बनाया गया होता है, वह इनवॉइस आवृत्ति से भी प्रभावित होता है. |
| बनाए जाने वाले रिटेनर्स की संख्या | जब आप बनाने के लिए रिटेनर्स की संख्या दर्ज करते हैं, तो सिस्टम इस फ़ील्ड में संख्या बनाने के लिए प्रारंभ दिनांक और आवृत्ति का उपयोग करता है. | जब इस फ़ील्ड को मैन्युअल रूप से अद्यतन किया जाता है, तो सिस्टम **रिटेनर शेड्यूल समाप्ति** फ़ील्ड में मान को अनदेखा कर देता है और इसके बजाय रिटेनर्स या एडवांस की विशिष्ट संख्या बनाता है. |
| इनवॉइस आवृत्ति | एप्लिकेशन कितनी बार रिटेनर्स और एडवांस बनाएगा. | यह मान रिटेनर्स और एडवांस की संख्या और निर्माण दिनांकों को सीधे प्रभावित करता है. |
| कुल राशि | कुल राशि वह राशि होती है, जिसे उन व्यक्तिगत रिटेनर या एडवांस भुगतानों में विभाजित किया जाता है, जो बनाए जाएंगे. | इस फील्ड का प्रवाह की दिशा में कोई प्रभाव नहीं होता है. |