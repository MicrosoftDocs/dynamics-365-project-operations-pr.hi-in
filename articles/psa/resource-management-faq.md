---
title: संसाधन प्रबंधन FAQ
description: यह लेख संसाधन प्रबंधन के बारे में अक्सर पूछे जाने वाले प्रश्नों के उत्तर प्रदान करता है।
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 03/28/2019
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
ms.reviewer: johnmichalak
ms.openlocfilehash: 6610098737b79d76b38c3d467135b9118c2a8ec7
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8913346"
---
# <a name="resource-management-faq"></a>संसाधन प्रबंधन FAQ

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

## <a name="what-is-the-difference-between-a-team-member-and-a-resource-requirement"></a>टीम के सदस्य और संसाधन की आवश्यकता के बीच क्या अंतर है?

एक परियोजना टीम के सदस्य को कार्य सौंपा जा सकता है, बुक किया जा सकता है या ओवरबुक किया जा सकता है, और एक अनुमोदनकर्ता के रूप में स्थापित किया जा सकता है। एक संसाधन की आवश्यकता डिमांड के ड्राफ्ट नोट के रूप में, एक परियोजना टीम के सदस्य के बिना मौजूद हो सकती है। 

## <a name="what-is-the-difference-between-proposed-and-soft-booked-hours"></a>प्रस्तावित और सॉफ्ट-बुक किए गए घंटों के बीच क्या अंतर है?

प्रस्तावित घंटे और सॉफ्ट-बुक किए गये घंटे दृश्यता में भिन्न होते हैं। प्रस्तावित घंटे केवल संसाधन प्रबंधकों और परियोजना प्रबंधक को दिखाई देते हैं जिन्होंने संसाधन अनुरोध का उपयोग करके मांग आरंभ की है। सॉफ्ट-बुक घंटे अनुसूची बोर्ड तक पहुंच रखने वाले किसी भी व्यक्ति को दिखाई देते हैं।

## <a name="how-can-i-see-the-soft-booked-hours-for-resources-on-a-team"></a>मैं किसी टीम पर संसाधनों के लिए सॉफ्ट-बुक किए गए घंटे कैसे देख सकता हूं?

जब आप संसाधन की आवश्यकता को बुक करते हैं तो सॉफ्ट बुकिंग की जा सकती है। संसाधन जो किसी प्रोजेक्ट टीम पर सॉफ्ट-बुक किए जाते हैं, टीम के सदस्यों के रूप में दिखाई देते हैं, जिनके पास सॉफ्ट-बुक्ड घंटे हैं। वे शेड्यूल बोर्ड में भी दिखाई देते हैं।

## <a name="how-do-i-change-the-required-hours-and-the-start-and-end-dates-for-a-resource-generic-or-named-that-i-booked"></a>संसाधन (सामान्य या नामित) जिसे मैंने बुक किया था, उसके लिए मैं आवश्यक घंटों और आरंभ और समाप्ति तिथियों को कैसे बदल सकता हूँ?

संसाधन बुक होने के बाद, आवश्यक परिवर्तन करने के लिए **बुकिंग बनाए रखें** का चयन करें।

## <a name="what-resources-types-does-project-service-automation-support"></a>Project Service Automation कौन से संसाधन प्रकार का समर्थन करते हैं?

**उपयोगकर्ता** और **संपर्क** ही केवल वे संसाधन प्रकार हैं, जो Microsoft Dynamics 365 Project Service Automation में समर्थित हैं। यद्यपि आप अन्य प्रकार के संसाधन बना सकते हैं (उदाहरण के लिए, **उपकरण** और **समूह**), उनके लिए कोई आद्योपान्त प्रक्रिया नहीं है।

## <a name="what-is-the-difference-between-an-assignment-and-a-booking"></a>असाइनमेंट और बुकिंग में क्या अंतर है?

असाइनमेंट्स, प्रोजेक्ट शेड्यूल में प्रोजेक्ट कार्यों के लिए संसाधनों का असाइनमेंट हैं। संसाधन, वास्तविक या सामान्य संसाधन हो सकते हैं। बुकिंग किसी परियोजना के लिए संसाधनों का कठिन या आसान आवंटन है। हार्ड बुकिंग किसी संसाधन की क्षमता का उपभोग करते हैं। आदर्श रूप से, वास्तविक संसाधनों के लिए, बुकिंग और असाइनमेंट आपस में सहमत होना चाहिए, क्योंकि वे अलग नहीं हैं। हालाँकि, PSA इस समझौते को लागू नहीं करता है। समायोजन दृश्य एक परियोजना प्रबंधक स्थानों को दिखाता है, जहां संसाधन की बुकिंग और असाइनमेंट सहमत नहीं होते हैं।


[!INCLUDE[footer-include](../includes/footer-banner.md)]
