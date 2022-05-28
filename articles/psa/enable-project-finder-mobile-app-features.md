---
title: Project Finder Mobile एप्लिकेशन सुविधाओं को सक्षम करें
description: Project Service के लिए Project Finder Mobile अनुप्रयोग सुविधाओं को सक्षम करने का तरीका
author: JohnPBurrows
ms.prod: ''
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
ms.openlocfilehash: 3f8f23c1f32d94a514de9ae40bd07b3d8063824c
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/14/2022
ms.locfileid: "8593687"
---
# <a name="enable-project-finder-mobile-app-features-project-service"></a>Project Finder Mobile अनुप्रयोग सुविधाएँ (Project Service) सक्षम करें

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

आपके संसाधन [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] के साथ अपने फ़ोन पर Project Finder Mobile ऐप का उपयोग कर सकते हैं, ताकि वे कार्य करने के लिए नई परियोजनाएँ ढूँढ़ सकें और अपने स्किलसेट अद्यतन कर सकें.  
  
 यह अनुप्रयोग [!INCLUDE[tn_Apple_iphone](../includes/tn-apple-iphone.md)] फ़ोन, और [!INCLUDE[tn_android](../includes/tn-android.md)], और [!INCLUDE[pn_windows_phone](../includes/pn-windows-phone.md)] के लिए उपलब्ध है.  
    
 उपयोगकर्ताओं को परियोजना संसाधन आवश्यकताएँ देखने और स्किल अद्यतन करने की अनुमति देने के लिए, आपकी संगठनात्मक इकाई हेतु पैरामीटर सेटिंग में विकल्प चुने जाने चाहिए.
  
> [!NOTE]
>  Project Finder Mobile अनुप्रयोग केवल [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)] के साथ कार्य करता है, ऑन-प्रिमाइसेस स्‍थापनाओं के साथ नहीं.  
  
1. **Project Service > पैरामीटर्स** पर जाएँ.  
  
2. आप Project Finder Mobile अनुप्रयोग सुविधाओं की अनुमति देने के लिए जिन पैरामीटर सेटिंग का उपयोग करना चाहते हैं, उन्‍हें क्लिक करें.  
  
3. **सामान्य** क्षेत्र में, **संसाधनों के लिए दृश्‍यमान संसाधन आवश्यकताएँ** को **हाँ** पर सेट करें.  
  
4. **संसाधन द्वारा कौशल अद्यतन की अनुमति दें** को **हाँ** पर सेट करें.  
  
   ![परियोजना सेवा&#95; प्रोजेक्टफाइंडर सक्षम करें।](../psa/media/project-service-project-finder-enable.png "ProjectService_ProjectFinderEnable")  
  
   यह एक ग्‍लोबल सेटिंग है. परियोजना प्रबंधक यह सेट कर सकते हैं कि कोई व्‍यक्तिगत परियोजना उस परियोजना के **परियोजना टीम** पृष्ठ पर दृश्‍यमान होगी या नहीं.  
  
   ![परियोजना सेवा&#95; प्रोजेक्ट टीम दृश्यमान।](../psa/media/project-service-project-team-visible.png "ProjectService_ProjectTeamVisible")  
  
## <a name="email-notifications"></a>ईमेल सूचनाएँ  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] संसाधन अनुरोधों के बारे में ईमेल निम्न प्राप्तकर्ताओं को निम्न समय पर भेजता है:  
  
|प्राप्तकर्ता|ईवेंट|  
|---------------|-----------|  
|परियोजना प्रबंधक|- संसाधन Project Finder Mobile ऐप के साथ परियोजना के लिए साइन-अप करता है.|  
|संसाधन|- संसाधन जिस परियोजना कार्य के लिए साइन अप करता है, वह कार्य पहले ही अन्‍य संसाधन द्वारा पूर्ण हो चुका है.<br />- स्किल अनुमोदन अनुरोध, अनुमोदित या अस्‍वीकृत हो चुका है.<br />- परियोजना साइन अप अनुरोध अनुमोदित या अस्‍वीकृत हो चुका है.|  
  
## <a name="privacy-notice"></a>गोपनीयता सूचना  
 [!INCLUDE[cc_privacy_crm_project_finder_mobile_app](../includes/cc-privacy-crm-project-finder-mobile-app.md)]  
  
### <a name="see-also"></a>यह भी देखें  
 [संसाधन सेट अप करें](../psa/set-up-resources.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
