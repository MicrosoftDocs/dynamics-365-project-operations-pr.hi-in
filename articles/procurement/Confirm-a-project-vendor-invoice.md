---
title: परियोजना विक्रेता चालान की पुष्टि करें
description: यह आलेख बताता है कि Microsoft में प्रोजेक्ट विक्रेता इनवॉइस की पुष्टि कैसे करें Dynamics 365 Project Operations और एक परियोजना विक्रेता चालान की पुष्टि के वित्तीय प्रभाव का वर्णन करता है।
author: suvaidya
ms.date: 8/25/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: suvaidya
ms.openlocfilehash: 9739b15753aa34c51a0aa1e6dfeb7f590655ca7a
ms.sourcegitcommit: 60a34a00e2237b377c6f777612cebcd6380b05e1
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/13/2022
ms.locfileid: "9475481"
---
# <a name="confirm-project-vendor-invoices"></a>परियोजना विक्रेता चालान की पुष्टि करें

_ **इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन

जब **पीएम द्वारा मैन्युअल पुष्टि की आवश्यकता है** पैरामीटर सक्षम है, विक्रेता इनवॉइस जो में बनाए गए हैं Microsoft Dataverse पास होना**प्रारूप** दर्जा। इस तरह से बनाए गए विक्रेता चालान की समीक्षा की जानी चाहिए और मैन्युअल रूप से पुष्टि की जानी चाहिए। जब **पीएम द्वारा मैन्युअल पुष्टि की आवश्यकता है** पैरामीटर अक्षम है, विक्रेता इनवॉइस जो में बनाए गए हैं Dataverse स्वतः पुष्टि हो जाती है। अब किसी कार्रवाई की आवश्यकता नहीं। 

आपके द्वारा विक्रेता इनवॉइस पर सभी पंक्तियों को सत्यापित करने के बाद Dynamics 365 Project Operations, चुनते हैं **पुष्टि करें** विक्रेता चालान की पुष्टि करने के लिए।

जब आप चुनते हैं **पुष्टि करें** विक्रेता इनवॉइस पर, निम्न व्यवहार होता है:

1. विक्रेता इनवॉइस की स्थिति को अद्यतन किया जाता है **की पुष्टि की**.
1. पुष्टि किए गए विक्रेता चालान और इससे संबंधित रिकॉर्ड केवल पढ़ने के लिए बन जाते हैं, और इन्हें संपादित या हटाया नहीं जा सकता है।
1. यदि कोई वास्तविक लागत विक्रेता इनवॉइस लाइन को मिलान प्रक्रिया के भाग के रूप में संदर्भित करती है, तो संदर्भित विक्रेता इनवॉइस लाइन से संबद्ध सभी वास्तविक लागत उलट जाती हैं।
1. नई लागत वास्तविक विक्रेता इनवॉइस लाइन पर जानकारी का उपयोग करके बनाए जाते हैं।
1. अब आप सुधार जर्नल नहीं बना सकते हैं, समय प्रविष्टियों की प्रक्रिया को याद नहीं कर सकते हैं, या मूल समय, व्यय, या सामग्री वास्तविक जो उलट गए थे, के अनुमोदन को रद्द कर सकते हैं।
1. Dynamics 365 Finance में, **परियोजना की लागत** प्रोजेक्ट इंटीग्रेशन जर्नल का उपयोग करके मूल्य को अपडेट किया जाता है, और प्रोक्योरमेंट इंटीग्रेशन अकाउंट है *औंधा* प्रोजेक्ट इंटीग्रेशन जर्नल पोस्ट करने के बाद।

> [!NOTE]
> यदि विक्रेता इनवॉइस पर किसी भी लाइन की सत्यापन स्थिति के अलावा अन्य है **पूरा**, विक्रेता चालान की पुष्टि नहीं की जा सकती।

[!INCLUDE[footer-include](../includes/footer-banner.md)]