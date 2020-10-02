---
title: पूर्णता पर अनुमानित लागत अद्यतित करें
description: यह विषय परियोजना पर प्रयास के अनुमान को अद्यतन करने के बारे में जानकारी देता है.
author: ruhercul
manager: AnnBe
ms.date: 09/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-customerservice
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 42824cc4cfc2b934f69d319944fe7ee43183955c
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/28/2020
ms.locfileid: "3897768"
---
# <a name="update-estimate-at-completion"></a>पूर्णता पर अनुमानित लागत अद्यतित करें

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

टास्क के मूल अनुमानों को संशोधित करना प्रोजेक्ट मैनेजर के लिए आम बात है। परियोजना की चालू अवस्था के बारे में, परियोजना का दोबारा अनुमान लगाना, दृष्टिकोण को लेकर परियोजना प्रबंधक के विचार होते हैं. बहरहाल, हम इस बात की सिफारिश नहीं करते कि प्रोजेक्ट मैनेजर बेसलाइन अंकों को बदलें क्योंकि प्रोजेक्ट की बेसलाइन प्रोजेक्ट के शेड्यूल और लागत के प्राक्कलनों की सच्चाई के स्थापित स्रोत होती है और लागत अनुमान और प्रोजेक्ट के सभी भागीदार उस पर सहमत होते हैं।

ऐसे दो तरीके हैं जिससे परियोजना प्रबंधक कार्यों के प्रयासों का दोबारा अनुमान लगा सकता है:

- कार्य में वास्तविक बाकी प्रयास के नए अनुमान के साथ (ETC) को पूरा करने के लिए डिफ़ॉल्ट अनुमान को ओवरराइड करें. 
- टास्क पर सही प्रगति के एक नए अनुमान के साथ डिफ़ॉल्ट प्रगति प्रतिशत को ओवरराइड करें।

इनमें से प्रत्येक दृष्टिकोण कार्य के ETC,पूर्ण होने पर अनुमान (EAC) और प्रगति प्रतिशत और कार्य के लिए अनुमानित प्रयास भिन्नता की पुनर्गणना का कारण बनता है. समरी टास्क पर EAC, ETC और प्रगति के प्रतिशत का दोबारा परिकलन किया जाता है और प्रयास की भिन्नता का नया अनुमान किया जाता है.