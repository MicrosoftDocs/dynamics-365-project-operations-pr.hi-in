---
title: इनवॉइस करने की प्रक्रिया का अवलोकन
description: यह विषय संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations में इनवॉइस करने की प्रक्रिया का अवलोकन प्रदान करता है.
author: sigitac
manager: Annbe
ms.date: 01/29/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: fbc1519b6cbcf231cfa89df8b7843d11a8904e49
ms.sourcegitcommit: b4298ca4729643c1040ef35dde8c67f829461ce7
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 01/29/2021
ms.locfileid: "5089250"
---
# <a name="invoicing-process-overview"></a>इनवॉइस करने की प्रक्रिया का अवलोकन

_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_

संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, परियोजना प्रबंधक और लेनदारी लेखे क्लर्क/ परियोजना लेखापाल, दोनों की आवश्यकताओं के अनुरूप व्यापक क्षमताएं प्रदान करता है. इनवॉइस की प्रक्रिया के लिए, परियोजना प्रबंधक परियोजना बिलिंग बैकलॉग का प्रबंधन करता है और लेनदारी लेखे क्लर्क/ परियोजना लेखापाल एक अनुपालक और सटीक ग्राहक-संबंधी इनवॉइस दस्तावेज़ बनाता है.

![इनवॉइस करने का प्रवाह आरेख](./media/invoicing-flow.png)

परियोजना अनुबंध पंक्ति, संबद्ध परियोजना लेनदेन के लिए बिलिंग विधि को परिभाषित करती है. जब परियोजना प्रबंधक समय और व्यय लेनदेन को स्वीकृति देता है, तो सिस्टम लेनदेन को **परियोजना वास्तविक** निकाय में रिकॉर्ड करता है और जानकारी को Dynamics 365 Finance में **परियोजना प्रबंधन और लेखांकन** में भेजता है. परियोजना लेखापाल तब [Project Operations एकीकरण जर्नल](../project-accounting/project-operations-integration-journal.md) का उपयोग करके रिकॉर्ड की समीक्षा करता है और उसे पोस्ट करता है. इस जर्नल में बिलिंग, विक्रय कर समूह, बिलिंग आइटम विक्रय कर समूह और वित्तीय आयाम जैसे परियोजना वास्तविक के महत्वपूर्ण लेखांकन विवरण शामिल हैं.

परियोजना प्रबंधक, [समय और सामग्री बिलिंग बैकलॉग](../proforma-invoicing/manage-billing-backlog.md#time-and-material-billing-backlog) में समय और सामग्री बिलिंग विधि और [निश्चित मूल्य माइलस्टोन](../proforma-invoicing/manage-billing-backlog.md#fixed-price-milestones) में निश्चित मूल्य बिलिंग का उपयोग करके बिना बिल किए गए विक्रय लेनदेन की समीक्षा कर सकता है. ये दृश्य आपको ऐसे लेनदेन को फ़िल्टर करने और चुनने की अनुमति देते हैं जिन्हें अगले बिलिंग चक्र में शामिल करने और फिर उन्हें **इनवॉइस के लिए तैयार** चिह्नित करने की आवश्यकता होती है.

आप [मैन्युअल रूप से प्रोफ़ॉर्मा इनवॉइस बना सकते हैं](../proforma-invoicing/create-manual-proforma-invoice.md) या [ आवधिक प्रक्रिया](../proforma-invoicing/configure-automated-invoice-creation.md) का उपयोग कर सकते हैं. परियोजना प्रबंधक आवश्यकतानुसार [ड्राफ्ट प्रोफ़ॉर्मा इनवॉइस को समायोजित कर](../proforma-invoicing/manage-proforma-invoice.md) सकता है और फिर इसकी पुष्टि कर सकता है.

पुष्टि किए गए प्रोफ़ॉर्मा इनवॉइस को वित्त्त में **परियोजना प्रबंधन और लेखांकन** मॉड्यूल में भेजा जाता है. परियोजना लेखापाल, परियोजना इनवॉइस प्रस्ताव को फ़ॉर्मेट और अद्यतित करता है, और फिर दस्तावेज़ को पोस्ट और प्रिंट करता है. पोस्ट किए गए परियोजना इनवॉइस को सामान्य लेजर के साथ-साथ ग्राहक और परियोजना सबलेजर में दर्ज किया जाता है.