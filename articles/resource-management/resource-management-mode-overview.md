---
title: संसाधन प्रबंधन मोड का अवलोकन
description: यह विषय Dynamics 365 Project Operations में संसाधन प्रबंधन कार्यक्षमता के बारे में जानकारी प्रदान करता है.
author: ruhercul
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 4d132bcbef5421202d2f4899091f0dc75166dd66
ms.sourcegitcommit: 3d78338773929121d17ec3386f6cb67bfb2272cc
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/27/2021
ms.locfileid: "5949951"
---
# <a name="resource-management-modes-overview"></a>संसाधन प्रबंधन मोड ओवरव्यू

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_


Dynamics 365 Project Operations समग्र बुकिंग प्रवाह को निष्पादित करने हेतु आपके लिए दो मोड का समर्थन करता है. प्रबंधन के मोड को एक परियोजना मापदंड के रूप में परिभाषित किया गया है और यदि आपके व्यवसाय को बदलने की आवश्यकता है, तो इसे संशोधित किया जा सकता है।    

## <a name="central-mode"></a>केंद्रीय मोड
परियोजनाओं के लिए संसाधनों के आवंटन को केंद्रीकृत करने वाले संगठनों के लिए, केंद्रीय मोड यह सुनिश्चित करने का एक तरीका प्रदान करता है कि परियोजना प्रबंधक परियोजना स्तर पर संसाधन आवश्यकताओं को परिभाषित कर सकें। संसाधन आवश्यकताओं की पूर्ति एक संसाधन प्रबंधक को सौंप दी जाती है। परियोजना प्रबंधक संसाधन प्रबंधक द्वारा प्रस्तावित संसाधनों को स्वीकार या अस्वीकार कर सकते हैं।

![केंद्रीय मोड](./media/resource-management-central.png)

केंद्रीय मोड वाले संसाधनों का प्रबंधन करने के लिए, देखें:

- [किसी भी कार्य में जेनेरिक बुक करने-योग्य संसाधनों को असाइन करें और संसाधनों की ज़रूरतों को जेनरेट करें](/dynamics365/project-service/assign-generic-bookable-resource)
- [संसाधनों की आवश्यकताओं से नामित संसाधनों को बुक करें](/dynamics365/project-service/book-named-resource)
- [कोई संसाधन अनुरोध सबमिट करें](/dynamics365/project-service/submit-resource-request)
- [संसाधन अनुरोध को पूरा करें](/dynamics365/project-service/resource-management-fulfill-requests)
- [संसाधनों हेतु अनुरोध में से प्रस्तावित परियोजना के किसी संसाधन को स्वीकार या अस्वीकार करें](/dynamics365/project-service/accept-reject-proposed-resource)

## <a name="hybrid-mode"></a>हाइब्रिड मोड
संसाधनों के आवंटन में लचीलापन चाहने वाले संगठनों के लिए, हाइब्रिड मोड परियोजना प्रबंधकों और संसाधन प्रबंधकों दोनों को संसाधनों को बुक करने की क्षमता देता है।

![हाइब्रिड मोड](./media/resource-management-hybrid.png)

समर्थित केंद्रीय मोड प्रक्रिया के अलावा, हाइब्रिड मोड में अन्य सभी समर्थित बुकिंग प्रवाह को प्रबंधित करने के लिए निम्नलिखित विषयों को देखें:

एक संसाधन सीधे परियोजना में बुक करें:
- [एक प्रोजेक्ट टीम को बुक करने योग्य संसाधनों का नाम और कार्यों को असाइन करें](/dynamics365/project-service/assign-named-bookable-resource)

संसाधन आवश्यकता से संसाधन बुक करें:
- [किसी भी कार्य में जेनेरिक बुक करने-योग्य संसाधनों को असाइन करें और संसाधनों की ज़रूरतों को जेनरेट करें](/dynamics365/project-service/assign-generic-bookable-resource)
- [संसाधनों की आवश्यकताओं से नामित संसाधनों को बुक करें](/dynamics365/project-service/book-named-resource)


[!INCLUDE[footer-include](../includes/footer-banner.md)]