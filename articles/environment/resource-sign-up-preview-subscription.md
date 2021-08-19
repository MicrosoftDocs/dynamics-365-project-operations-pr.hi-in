---
title: संसाधन/गैर-स्टॉक किए गए परिदृश्य के लिए परियोजना संचालन पूर्वावलोकन सदस्यता के लिए साइन अप करें
description: यह विषय संसाधन/गैर-स्टॉक किए गए परिदृश्यों के लिए परियोजना संचालन की सदस्यता और परिनियोजित कैसे करना है, की जानकारी देता है।
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 75ee31e67018fe2a7655d8a8f11e40b433a9a5db6f8f2addac27844f18fffe8d
ms.sourcegitcommit: 7f8d1e7a16af769adb43d1877c28fdce53975db8
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 08/06/2021
ms.locfileid: "7007868"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a>संसाधन/गैर-स्टॉक किए गए परिदृश्य के लिए परियोजना संचालन पूर्वावलोकन सदस्यता के लिए साइन अप करें

_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations_

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

यह विषय बताता है कि ट्रायल प्रस्ताव की सदस्यता कैसे लें और संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations परिवेश को कैसे परिनियोजित करें.

## <a name="prerequisites"></a>पूर्वावश्यकताएँ
- पूर्वावलोकन नियोजित करने वाले उपयोगकर्ता के पास Azure टेनेंट वैश्विक प्रशासक अधिकार होना चाहिए. आप पहले ऑफ़र रिडीम के दौरान टेनेंट बना सकते हैं. 
- वित्त परिवेश में परिनियोजन के लिए एक मान्य Azure सदस्यता की आवश्यकता होती है जिसे परिवेश के अनुसार बिल किया जाएगा। आप अपने संगठनों की मौजूदा सदस्यता का उपयोग कर सकते हैं या शुरू करने के लिए एक [Azure परीक्षण](https://azure.microsoft.com/en-us/free/) का उपयोग कर सकते हैं। CDS परिवेश को सीमित 30 दिन की अवधि के लिए मुफ्त प्रदान किया जाएगा।

> [!IMPORTANT]
> एक संगठन में केवल एक व्यक्ति, टेनेंट व्यवस्थापक को इस कार्य को करने की आवश्यकता है। यदि आप इस रिलीज़ के सदस्य नहीं हैं, तो तब तक इंतजार करें जब तक कि आपके संगठन द्वारा साइन अप नहीं किया जाता है और आपको अपना उपयोगकर्ता क्रेडेंशियल प्राप्त न हो जाए।
> 
> ट्रायल टैनेंट में एकल उपयोग के लिए हैं. आप केवल एक बार ट्रायल चला सकते हैं. हम सुझाव देते हैं कि आप ट्रायल उद्देश्य के लिए नया टैनेंट बनाएं.


### <a name="dynamics-365-project-operations-ce---preview-trial"></a>Dynamics 365 Project Operations(CE) - पूर्वावलोकन परीक्षण 

शुरू करने से पहले, सुनिश्चित करें कि आप टेनेंट में उपयोगकर्ता वर्क अकाउंट के साथ ब्राउज़र में लॉग इन कर रहे हैं जहां आप Project Operations का पूर्वावलोकन चाहते हैं.

1. पहला ऑफ़र कोड, **Dynamics 365 Project Operations** यहाँ [Project Operations परीक्षण](https://aka.ms/try-po) रिडीम करें.
2. ऑर्डर की पुष्टि करें.

  आप देखेंगे अनुमोदन प्रस्ताव सफलतापूर्वक चुका दिया गया है.

### <a name="dynamics-365-finance-preview-trial"></a>Dynamics 365 Finance पूर्वावलोकन परीक्षण

[वित्त पूर्वावलोकन परीक्षण के लिए Dynamics 365](https://aka.ms/trypoche) पर जाएँ और ऑफ़र के साथ पिछले अनुभाग के चरणों को दोहराएं, क्लाउड होस्टेड परिवेश के लिए साइन अप करें.  

## <a name="assign-licenses"></a>लाइसेंस असाइन करें

> [!IMPORTANT]
> निम्नलिखित चरणों को पूरा करने के लिए आपको अपने संगठन के Microsoft 365 पोर्टल तक प्रशासनिक पहुंच की आवश्यकता होगी.

1. अपने उपयोगकर्ताओं को लाइसेंस आवंटित करने के लिए [Microsoft 365 व्यवस्थापक केंद्र](https://portal.office.com/) पर जाएं.

2. **सक्रिय उपयोगकर्ता** पृष्ठ पर उन उपयोगकर्ताओं का चयन करें, जिन्हें आप लाइसेंस देना चाहते हैं.

3. सत्यापित करें कि **Dynamics 365 Project Operations** लाइसेंस को चुना गया है और **परिवर्तनों को सहेजें** चुनें.

> [!NOTE]
> वित्त परीक्षण प्रस्ताव को उपयोगकर्ता को सौंपने की आवश्यकता नहीं है।

## <a name="start-a-new-project-in-lcs"></a>LCS में एक नई परियोजना प्रारंभ करें

विषय LCS में एक नई परियोजना शुरू करें, [LCS में एक नई परियोजना शुरू करें](create-lcs-project.md)

## <a name="add-an-azure-subscription-to-an-lcs-project"></a>LCS परियोजना में एक Azure सदस्यता जोड़ें

इस कार्य को पूरा करने के लिए, विषय LCS परियोजना में एक Azure सदस्यता जोड़ें [LCS प्रोजेक्ट के लिए एक Azure सदस्यता जोड़ें](resource-add-azure-subscription-lcs-project.md) ।

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a>संसाधन/गैर-स्टॉक किए गए परिदृश्यों के लिए परियोजना संचालन के साथ वित्त डेमो परिवेश नियोजित करें

परिनियोजन को पूरा करने के लिए, विषय, [नए परिवेश का प्रावधान करें](resource-provision-new-environment.md) में मार्गदर्शन का पालन करें। पूर्वावलोकन के लिए [डेमो परिवेश](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) परिनियोजन प्रकार का उपयोग करें। 

## <a name="install-cds-setup-and-configuration-data"></a>CDS सेटअप और कॉन्फ़िगरेशन डेटा स्थापित करें

CDS सेटअप और कॉन्फ़िगरेशन डेटा स्थापित करें जैसा कि विषय, [सामान्य डेटा सेवा में कॉन्फ़िगरेशन डेटा सेट अप और लागू करें Common Data Service](resource-apply-pro-setup-config-data.md)में वर्णित है।
इस चरण को तभी पूरा करें, जब वित्त डेमो परिवेश परिनियोजित हो और डेमो डेटा तैयार हो.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
