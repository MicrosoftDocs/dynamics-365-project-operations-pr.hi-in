---
title: एक मैनुअल प्रोफ़ॉर्मा इनवॉइस बनाएँ - लाइट
description: यह विषय Project Operations में एक मैनुअल प्रोफ़ॉर्मा इनवॉइस बनाने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 5a924de6efc377e28a20e038e7deac04616b95aa
ms.sourcegitcommit: 2b74edd31f38410024a01124c9202a4d94464d04
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 12/17/2020
ms.locfileid: "4764505"
---
# <a name="create-a-manual-proforma-invoice---lite"></a>एक मैनुअल प्रोफ़ॉर्मा इनवॉइस बनाएँ - लाइट

_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_

Dynamics 365 Project Operations में, प्रोफ़ॉर्मा इनवॉइस आवश्यकतानुसार मैन्युल रूप से बनाए जा सकते हैं. आप मैन्युअल रूप से **प्रोजेक्ट अनुबंध** सूची पृष्ठ से या **प्रोजेक्ट अनुबंध** विवरण पृष्ठ से एक प्रोफ़ॉर्मा इनवॉइस बना सकते हैं.

##  <a name="project-contracts-list-page"></a>प्रोजेक्ट अनुबंध सूची पृष्ठ

**प्रोजेक्ट अनुबंध** सूची पृष्ठ से, एक या एक से अधिक प्रोजेक्ट अनुबंधों का चयन करें, और सभी चयनित रिकॉर्ड के लिए इनवॉइस बनाएं.

सिस्टम यह देखने के लिए जांच करता है कि चयनित परियोजना अनुबंधों में से कौन सा **इनवॉइस के लिए तैयार** बैकलॉग आज के दिनांक से पहले का है. उन अनुबंधों से, सिस्टम ड्राफ्ट प्रोफ़ॉर्मा इनवॉइस बनाता है. यदि किसी प्रोजेक्ट अनुबंध में कई ग्राहक हैं, तो प्रति ग्राहक एक इनवॉइस बनाया जा सकता है, और प्रति प्रोजेक्ट अनुबंध कई इनवॉइस हो सकते हैं.

बनाए गए सभी प्रोजेक्ट इनवॉइस **सेल्स** क्षेत्र के **बिलिंग** अनुभाग में **इनवॉइस** पृष्ठ पर उपलब्ध हैं.

## <a name="project-contract-details-page"></a>प्रोजेक्ट अनुबंध विवरण पृष्ठ

प्रोफ़ॉर्मा इनवॉइस को **परियोजना अनुबंध** विवरण पृष्ठ से भी बनाया जा सकता है. सिस्टम सत्यापित करता है कि परियोजना अनुबंध **इनवॉइस के लिए तैयार** बैकलॉग आज के दिनांक से पहले का है. इन अनुबंधों से, सिस्टम प्रत्येक अनुबंध लाइन पर ग्राहकों की संख्या के आधार पर ड्राफ्ट प्रोफ़ॉर्मा इनवॉइस बनाता है.

जब एक भी प्रोफ़ॉर्मा इनवॉइस बनाया जाता है, तो **इनवॉइस** पृष्ठ खुलता है. यदि उस परियोजना अनुबंध के लिए एकाधिक इनवॉइस बनाए जाते हैं, तो**इनवॉइस** सूची पृष्ठ सभी बनाए गए इनवॉइस को बनाने के लिए खुल जाता है.