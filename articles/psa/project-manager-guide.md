---
title: परियोजना प्रबंधक मार्गदर्शिका
description: Project Service के लिए परियोजना प्रबंधन मार्गदर्शिका
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
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
ms.openlocfilehash: e3ac30b8fb8a6c6b4f4a6dc658cbdaca5271a214
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/14/2022
ms.locfileid: "8596328"
---
# <a name="project-manager-guide-project-service"></a>परियोजना प्रबंधक मार्गदर्शिका (Project Service)

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] में [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] क्षमताएँ, आपके परियोजना कोट और अनुबंधों को बनाने में आपकी मदद करती हैं और आपके द्वारा अनुबंध जीतने के बाद आपके क्‍लाइंट्स के लिए परियोजनाएँ बनाती हैं और प्रबंधित करती हैं. वे आपकी यह सुनिश्चित करने में मदद करने के लिए कि परियोजना संगत और लाभदायक हैं, विश्लेषण भी प्रदान करती हैं. आप परियोजनाओं को समय और सामग्री या निर्धारित मूल्य के आधार पर सेट कर सकते हैं.  
  
 परियोजना प्रबंधन निम्न करने में आपकी मदद करता है:  
  
-   प्रभावी रूप से कार्य का अनुमान लगाना  
  
-   परियोजनाओं के पाइपलाइन में होने पर, संसाधन आवश्यकताओं का पूर्वानुमान लगाना  
  
-   टीम सदस्यों को परियोजनाओं पर सहयोग करने और हर समय परियोजना की स्थिति को नवीनतम और सटीक रखने में सक्षम करना  
  
-   प्रत्येक और सभी सहभागिता की सफलता के लिए संभावित खतरों की तुरंत पहचान करना और उन्हें हल करना.  
  
यह मार्गदर्शिका परियोजना बनाने और प्रबंधित करने के लिए आवश्यक जानकारी प्रदान करती है:  
  
-   [विक्रय प्रक्रिया के दौरान एक परियोजना के लिए कार्य अनुमान प्रदान करें](../psa/provide-estimates-project-during-sales-process.md)  
  
-   [परियोजना बनाएँ](../psa/create-project.md)  
  
-   [Microsoft Project में अपने कार्य की योजना बनाने के लिए Project Service Automation ऐड-इन का उपयोग करें](../psa/add-plan-work-microsoft-project.md)  
  
-   [कार्य विश्लेषण संरचना वाली एक परियोजना शेड्यूल करें](../psa/schedule-project-work-breakdown-structure.md)  
  
-   [परियोजना लागत और आय अनुमान निर्धारित करें](../psa/determine-project-cost-revenue-estimates.md)  
  
-   [परियोजना प्रगति और लागत ट्रैक करें](../psa/track-project-progress-cost.md)  
  
-   [कोई परियोजना टेम्पलेट बनाएँ](../psa/create-project-template.md)  
  
-   [संसाधन अनुरोध सबमिट करें](../psa/submit-resource-requests.md)  
  
-   [किसी परियोजना के लिए एक Office 365 समूह बनाएँ](../psa/create-office-365-group-project.md)  
  
-   [किसी परियोजना में दस्तावेज़ जोड़ें](../psa/add-documents-project.md)  
  
-   [परियोजना की स्थिति ट्रैक करें](../psa/track-project-status.md)  
  
-   [परियोजना के टीम सदस्यों को देखें और बुकिंग प्रबंधित करें](../psa/view-project-team-members-manage-bookings.md)  
  
-   [परियोजना अनुमान देखें और संपादित करें](../psa/view-edit-project-estimates.md)  
  
-   [समय और व्यय अनुमोदित करें](../psa/approve-time-expenses.md)  
  
-   [परियोजना वास्तविक की समीक्षा करें](../psa/review-project-actuals.md)  
  
-   [इनवॉइस देखें और भेजें](../psa/view-send-invoices.md)  
  
-   [डैशबोर्ड और रिपोर्ट देखें](../psa/view-dashboards-reports.md)  
  
## <a name="prerequisites"></a>पूर्वावश्यकताएँ  
 यदि आपने पहले से नहीं किए हैं, तो परियोजनाएँ बनाना प्रारंभ करने से पहले आपको निम्न आइटम्स पूर्ण करने होंगे:  
  
-   [कार्य घंटों का एक टेम्पलेट बनाएँ](../psa/create-work-hours-template.md). एक ऐसा परियोजना कैलेंडर सेट अप करे, जो शेड्यूल और किसी भी व्यवसाय बंदी के दौरान प्रति दिन समायोजित किए जाने वाले कार्य के घंटों की संख्या निर्धारित करें.  
  
-   [एक मूल्य सूची बनाएँ](../psa/create-price-list.md). अपने संगठन में संसाधन भूमिकाओं और साथ ही अन्य श्रेणियों जैसे व्यय और उत्पाद के लिए लागत और विक्रय मूल्य सेट करें.  
  
-   [संसाधन भूमिकाएँ जोड़ें](../psa/add-resource-roles.md). संसाधन आवश्यकताओं और परियोजना लागत को निर्धारित करने में मदद करने के लिए भूमिकाएँ परिभाषित करें.  
  
### <a name="see-also"></a>यह भी देखें  
 [Project Service का ओवरव्यू](../psa/overview.md)   
 [व्यवस्थापक मार्गदर्शिका](../psa/admin-guide.md)   
 [खाता प्रबंधक मार्गदर्शिका](../psa/account-manager-guide.md)   
 [संसाधन प्रबंधक मार्गदर्शिका](../psa/resource-manager-guide.md)   
 [समय, व्यय और सहयोग मार्गदर्शिका](../psa/time-expense-collaboration-guide.md)



[!INCLUDE[footer-include](../includes/footer-banner.md)]
