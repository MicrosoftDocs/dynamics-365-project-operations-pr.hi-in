---
title: Project Service Automation वर्ज़न 3.x wave 1 2020 में क्या क्या नया है या बदल गया है
description: यह टॉपिक Project Service Automation वर्ज़न 3 wave 1 2020 में क्या नया है और क्या बदला है, इसके बारे में जानकारी प्रदान करता है.
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 01/24/2020
ms.topic: article
ms.prod: ''
ms.technology: Dynamics 365 Project Service Automation 3.x wave 1 2020
author: stsporen
ms.assetid: 48b408c1-11e7-4005-abac-8fd7c0b064b1
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 478080c0570b71188c9f1e12b18b5aadc13903e5
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3752011"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a>Project Service Automation वर्ज़न 3 wave 1 2020 में क्या क्या नया है या बदल गया है
यह टॉपिक Project Service Automation (PSA) वर्ज़न 3.x wave 1 2020 की नवीनतम रिलीज़ के लिए आगे बढ़ने पर मुख्य अपडेट विचारों पर प्रकाश डालता है.

## <a name="time-entry"></a>समय प्रविष्टि
समय प्रविष्टि अनुभव को अधिक ग्राहक परिदृश्यों में समय प्रविष्टि के विस्तार की क्षमता प्रदान करने के लिए बढ़ाया गया है. इसमें प्रविष्टि प्रकार जोड़ने की क्षमता शामिल है, जो अब फील्ड स्कीमा नाम के आधार पर विशिष्ट व्यवहार को चलाते हैं **समय प्रविष्टि सेटिंग**, **समय स्रोत** के रूप में प्रदर्शित.

### <a name="upgrade-consideration"></a>नवीनीकरण विचार
इस कार्यक्षमता का समर्थन करने के लिए, PSA के भीतर की भूमिकाओं को नए विशेषाधिकार शामिल करने के लिए अपडेट किया गया है. ये विशेषाधिकार नई इकाई, **समय प्रविष्टि सेटिंग** तक पहुँच प्रदान करते हैं.

जिन उपयोगकर्ताओं को समय को रिकॉर्ड करने की क्षमता की आवश्यकता होती है, उन्हें मौजूदा भूमिकाओं के साथ-साथ उपयोगकर्ता भूमिका **समय प्रविष्टि उपयोगकर्ता** दी जानी चाहिए. इस भूमिका में नई कार्यक्षमता शामिल है और यह सुनिश्चित करती है कि समय प्रविष्टि काम करना जारी रखेगी.

### <a name="currently-extended-time-entry-changes"></a>वर्तमान में विस्तारित समय प्रविष्टि परिवर्तन
समय प्रविष्टि के वर्तमान उपयोगकर्ताओं पर प्रभाव को कम करने के लिए, यह भूमिका परिवर्तन समय प्रविष्टि का उपयोग जारी रखने के लिए आवश्यक एकमात्र कोर आवश्यकता है. यदि आपने कस्टम दृश्य या अलग समय प्रविष्टि अनुभव बनाए हैं, तो आपको **समय प्रविष्टि सेटिंग** फील्ड को सही PSA मान पीआर सेट करना होगा.
