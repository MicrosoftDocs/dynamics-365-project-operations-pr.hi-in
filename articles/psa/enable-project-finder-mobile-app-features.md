---
title: Project Finder Mobile एप्लिकेशन सुविधाओं को सक्षम करें
description: Project Service के लिए Project Finder Mobile अनुप्रयोग सुविधाओं को सक्षम करने का तरीका
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 749c5682dc2e639843a0a8a085fe8af65502d433
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077707"
---
# <a name="enable-project-finder-mobile-app-features-project-service"></a>Project Finder Mobile अनुप्रयोग सुविधाएँ (Project Service) सक्षम करें

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

आपके संसाधन [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] के साथ अपने फ़ोन पर Project Finder Mobile अनुप्रयोग का उपयोग कर सकते हैं ताकि वे कार्य करने के लिए नई परियोजनाएँ ढूँढ़ सकें और अपने कौशल को अद्यतन कर सकें.  
  
 यह अनुप्रयोग [!INCLUDE[tn_Apple_iphone](../includes/tn-apple-iphone.md)] फ़ोन, और [!INCLUDE[tn_android](../includes/tn-android.md)], और [!INCLUDE[pn_windows_phone](../includes/pn-windows-phone.md)] के लिए उपलब्ध है.  
  
 आपको अपनी संगठनात्मक इकाई के लिए सेटिंग पैरामीटर सेट करने के लिए कुछ विकल्पों को सेट करना होगा, ताकि उपयोगकर्ता, परियोजनाओं की संसाधन आवश्‍यकताओं को देख सकें और अपने कौशल को अद्यतन कर सकें.  
  
> [!NOTE]
>  Project Finder Mobile अनुप्रयोग केवल [!INCLUDE[pn_crm_online_shortest](../includes/pn-crm-online-shortest.md)] के साथ कार्य करता है, ऑन-प्रिमाइसेस स्‍थापनाओं के साथ नहीं.  
  
1. **Project Service > पैरामीटर्स** पर जाएँ.  
  
2. आप Project Finder Mobile अनुप्रयोग सुविधाओं की अनुमति देने के लिए जिन पैरामीटर सेटिंग का उपयोग करना चाहते हैं, उन्‍हें क्लिक करें.  
  
3. **सामान्य** क्षेत्र में, **संसाधनों के लिए दृश्‍यमान संसाधन आवश्यकताएँ** को **हाँ** पर सेट करें.  
  
4. **संसाधन द्वारा कौशल अद्यतन की अनुमति दें** को **हाँ** पर सेट करें.  
  
   ![ProjectService_ProjectFinderEnable](../psa/media/project-service-project-finder-enable.png "ProjectService_ProjectFinderEnable")  
  
   यह एक ग्‍लोबल सेटिंग है. परियोजना प्रबंधक यह सेट कर सकते हैं कि कोई व्‍यक्तिगत परियोजना उस परियोजना के **परियोजना टीम** पृष्ठ पर दृश्‍यमान होगी या नहीं.  
  
   ![ProjectService_ProjectTeamVisible](../psa/media/project-service-project-team-visible.png "ProjectService_ProjectTeamVisible")  
  
## <a name="email-notifications"></a>ईमेल सूचनाएँ  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] संसाधन अनुरोधों के बारे में ईमेल निम्न प्राप्तकर्ताओं को निम्न समय पर भेजता है:  
  
|प्राप्तकर्ता|ईवेंट|  
|---------------|-----------|  
|परियोजना प्रबंधक|-   जब कोई संसाधन Project Finder Mobile अनुप्रयोग की सहायता से परियोजना के लिए साइन-अप करता है.|  
|संसाधन|-   जब परियोजना कार्य जिसके लिए संसाधन ने साइन अप किया है, वह पहले से किसी अन्य संसाधन द्वारा पूरा किया जा चुका होता है.<br />-   जब उनका कौशल अनुमोदन अनुरोध, स्वीकार या अस्वीकार कर दिया जाता है.<br />-   जब उनका परियोजना साइन अप अनुरोध, स्वीकार या अस्वीकार कर दिया जाता है.|  
  
## <a name="privacy-notice"></a>गोपनीयता सूचना  
 [!INCLUDE[cc_privacy_crm_project_finder_mobile_app](../includes/cc-privacy-crm-project-finder-mobile-app.md)]  
  
### <a name="see-also"></a>यह भी देखें  
 [संसाधन सेट अप करें](../psa/set-up-resources.md)
