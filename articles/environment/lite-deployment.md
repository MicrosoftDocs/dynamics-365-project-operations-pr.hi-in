---
title: प्रोजेक्ट ऑपरेशंस लाइट परिनियोजित करें
description: यह आलेख Project Operations लाइट नियोजन स्थापित करने के तरीके के बारे में जानकारी प्रदान करता है - प्रोफार्मा इनवॉयसिंग करने के लिए समझौता.
author: stsporen
ms.date: 11/29/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 2c508f56b3018b6a86fea78bcf9ee4136e90f385
ms.sourcegitcommit: 38cb012502cbd640abbc21a0912b195112b27ccb
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/30/2022
ms.locfileid: "9810980"
---
# <a name="deploy-project-operations-lite"></a>प्रोजेक्ट ऑपरेशंस लाइट परिनियोजित करें

_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_



Project Operations कई नियोजन मॉडल का समर्थन करता है. सबसे अच्छा नियोजन मॉडल निर्धारित करने के लिए, देखें [नियोजन के प्रकार](determine-deployment-type.md).


> [!IMPORTANT]
> यह नियोजन, लाइट नियोजन - प्रोफार्मा इंवॉयसिंग करने के लिए समझौता, एक **Dataverse Project Operations की नियोजन** में परिणाम है.

- [एक नए Dataverse परिवेश में Project Operations इंस्टॉल करें](#new)
- [एक मौजूदा Dataverse परिवेश में इंस्टॉल करें](#existing)
- [ऐसे मौजूदा Dataverse ऐसे वातावरण में स्थापित करें जिसमें दोहरे लेखन घटक हों](#existingdw)



## <a name="install-project-operations-lite-to-a-new-dataverse-environment"></a><a name="new"></a> Project Operations Lite को नए Dataverse पर्यावरण में स्थापित करें

1. एक Project Operations लाइसेंस के साथ [ग्लोबल या एडमिनिस्ट्रेटर Power Platform](/power-platform/admin/global-service-administrators-can-administer-without-license) के रूप में [PowerPlatform व्यवस्थापक केंद्र](https://admin.powerplatform.com) में एक नया Dataverse परिवेश बनाएँ. निश्चित करें कि **इस परिवेश के लिए एक डेटाबेस बनाएँ** तथा **Dynamics 365 ऐप्स** सक्षम हैं। अधिक जानकारी के लिए, देखें [Power Platform एडमिन सेंटर में परिवेश बनाएं और प्रबंधित करें](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
1. Dynamics 365 ऐप की परिनियोजन सूची से **Microsoft Dynamics 365 Project Operations** चुनें.


## <a name="install-project-operations-lite-to-an-existing-dataverse-environment"></a><a name="existing"></a> Project Operations Lite को मौजूदा Dataverse पर्यावरण में स्थापित करें 
1. [ग्लोबल या Power Platform एडमिनिस्ट्रेटर](/power-platform/admin/global-service-administrators-can-administer-without-license) के रूप में एक Project Operations लाइसेंस के साथ, [पावर प्लेटफॉर्म व्यवस्थापक केंद्र](https://admin.powerplatform.com) में परिवेश का पता लगाएं, जहां आप Project Operations इंस्टॉल करना चाहते हैं.
1. Dynamics 365 ऐप की परिनियोजन सूची से **Microsoft Dynamics 365 Project Operations** स्थापित करें. अधिक जानकारी के लिए, [Dynamics 365 अनुप्रयोग प्रबंधित करें](/power-platform/admin/manage-apps) देखें.

## <a name="install-project-operations-lite-to-an-existing-dataverse-environment-where-dual-write-solutions-are-already-present"></a><a name="existingdw"></a> Project Operations Lite को मौजूदा Dataverse पर्यावरण में स्थापित करें जहाँ दोहरे लेखन समाधान पहले से मौजूद हैं

यदि आप लाइट डिप्लॉयमेंट मोड में प्रोजेक्ट ऑपरेशंस चलाना जारी रखना चाहते हैं, तो आपको इन चरणों का पालन करना चाहिए:

1. [ग्लोबल या Power Platform एडमिनिस्ट्रेटर](/power-platform/admin/global-service-administrators-can-administer-without-license) के रूप में एक Project Operations लाइसेंस के साथ, [पावर प्लेटफॉर्म व्यवस्थापक केंद्र](https://admin.powerplatform.com) में परिवेश का पता लगाएं, जहां आप Project Operations इंस्टॉल करना चाहते हैं.
1. Dynamics 365 ऐप की परिनियोजन सूची से **Microsoft Dynamics 365 Project Operations** स्थापित करें. अधिक जानकारी के लिए, [Dynamics 365 अनुप्रयोग प्रबंधित करें](/power-platform/admin/manage-apps) देखें.
1. क्योंकि आपके वातावरण में दोहरे लेखन घटक हैं जो स्थापित वित्त और संचालन ऐप्स के एकीकरण में मदद करते हैं, प्रोजेक्ट संचालन स्थापना परियोजना से संबंधित डेटा को वित्त और संचालन ऐप में एकीकृत करने के लिए आवश्यक क्षमताओं और एक्सटेंशन को भी स्थापित करेगी। चूंकि आप लाइट परिनियोजन में प्रोजेक्ट संचालन चलाना चाहते हैं, इसलिए इन एकीकरण घटकों को हटा दिया जाना चाहिए क्योंकि वे लाइट परिनियोजन परिदृश्यों के लिए प्रतिबंध और ओवरहेड बनाएंगे। इन घटकों को हटाने के लिए **Dynamics 365 Project Operations ड्युअल राइट** और **Dynamics 365 Project Operations डुअल राइट एंटिटी मैप** मैन्युअल रूप से समाधान अनइंस्टॉल करें।
1.  **परियोजना संचालन -> सेटिंग -> पैरामीटर**.  **प्रोजेक्ट पैरामीटर** विवरण पृष्ठ खोलें और **समाधान अपग्रेड व्यवहार** फ़ील्ड को **लाइट पर सेट करें सिर्फ़**. यह सुनिश्चित करता है कि प्रोजेक्ट ऑपरेशंस के बाद के किसी भी अपग्रेड से इंटीग्रेशन कंपोनेंट्स को प्रोजेक्ट ऑपरेशंस में वापस नहीं लाया जाएगा।  

[!INCLUDE[footer-include](../includes/footer-banner.md)]
