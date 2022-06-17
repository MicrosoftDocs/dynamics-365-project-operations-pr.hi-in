---
title: Project Operations परिनियोजित करें - लाइट
description: यह आलेख प्रोजेक्ट ऑपरेशंस लाइट परिनियोजन - डील टू प्रोफार्मा इनवॉइसिंग को स्थापित करने के तरीके के बारे में जानकारी प्रदान करता है।
author: stsporen
ms.date: 02/28/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: stsporen
ms.openlocfilehash: 86293b725e86db3d4b8bdaf5810b16b7c670e8a3
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8930320"
---
# <a name="deploy-project-operations---lite"></a>Project Operations परिनियोजित करें - लाइट

_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_



Project Operations कई नियोजन मॉडल का समर्थन करता है. सबसे अच्छा नियोजन मॉडल निर्धारित करने के लिए, देखें [नियोजन के प्रकार](determine-deployment-type.md).


> [!IMPORTANT]
> यह नियोजन, लाइट नियोजन - प्रोफार्मा इंवॉयसिंग करने के लिए समझौता, एक **Dataverse Project Operations की नियोजन** में परिणाम है.

- [प्रोजेक्ट ऑपरेशंस को एक नए में स्थापित करें Dataverse वातावरण](#new)
- [मौजूदा में स्थापित करें Dataverse वातावरण](#existing)



## <a name="install-project-operations-to-a-new-dataverse-environment"></a><a name="new"></a> प्रोजेक्ट ऑपरेशंस को एक नए में स्थापित करें Dataverse वातावरण

1. के रूप में [वैश्विक याPower Platform प्रशासक](/power-platform/admin/global-service-administrators-can-administer-without-license) प्रोजेक्ट संचालन लाइसेंस के साथ, एक नया बनाएं Dataverse में पर्यावरण [PowerPlatform व्यवस्थापन केंद्र](https://admin.powerplatform.com). निश्चित करें कि**इस परिवेश के लिए एक डेटाबेस बनाएँ** तथा**डायनेमिक्स 365 ऐप्स** सक्षम हैं। अधिक जानकारी के लिए, देखें [Power Platform एडमिन सेंटर में परिवेश बनाएं और प्रबंधित करें](/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).
2. Dynamics 365 ऐप की परिनियोजन सूची से **Microsoft Dynamics 365 Project Operations** चुनें.


## <a name="install-project-operations-to-an-existing-dataverse-environment"></a><a name="existing"></a> किसी मौजूदा के लिए प्रोजेक्ट ऑपरेशंस स्थापित करें Dataverse वातावरण
1. सुनिश्चित करें कि पर्यावरण को इसके साथ कॉन्फ़िगर नहीं किया गया है [दोहरा लिखना](/dynamics365/fin-ops-core/dev-itpro/data-entities/dual-write/dual-write-overview) स्थापना के रूप में स्थापित होगा[संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए परियोजना संचालन](project-operations-integrated-deployment-overview.md) क्षमताएं।
2. [ग्लोबल या Power Platform एडमिनिस्ट्रेटर](/power-platform/admin/global-service-administrators-can-administer-without-license) के रूप में एक Project Operations लाइसेंस के साथ, [पावर प्लेटफॉर्म व्यवस्थापक केंद्र](https://admin.powerplatform.com) में परिवेश का पता लगाएं, जहां आप Project Operations इंस्टॉल करना चाहते हैं.
3. Dynamics 365 ऐप की परिनियोजन सूची से **Microsoft Dynamics 365 Project Operations** स्थापित करें. अधिक जानकारी के लिए, [Dynamics 365 अनुप्रयोग प्रबंधित करें](/power-platform/admin/manage-apps) देखें.




[!INCLUDE[footer-include](../includes/footer-banner.md)]
