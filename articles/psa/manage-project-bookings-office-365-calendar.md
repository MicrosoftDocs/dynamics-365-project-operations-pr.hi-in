---
title: अपने Office 365 कैलेंडर में प्रोजेक्ट और बुकिंग को व्यवस्थित करना
description: अपने Office 365 कैलेंडर में प्रोजेक्ट और बुकिंग को कैसे व्यवस्थित करें
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
- D365PS
- ProjectOperations
ms.openlocfilehash: 575f3c94f886d12717496445d0e6357fdc01246b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000393"
---
# <a name="manage-projects-and-bookings-in-your-calendar-project-service"></a>अपने कैलेंडर में प्रोजेक्ट और बुकिंग को व्यवस्थित करना (Project Service)

> [!Note]
> मूल्यह्रास किया गया – इस विशेषता का मूल्यह्रास किया गया और अब उपलब्ध नहीं है।

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] 

[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] कैलेंडर का उपयोग करके व्यक्तिगत अपॉइंटमेंट, परियोजना-कार्य बुकिंग और field service कार्य ऑर्डर असाइनमेंट देखें.  
  
 जब सब कुछ एक ही स्थान पर हो, तो आपके दिन को प्रबंधित करना आसान बन जाता है. आपकी मीटिंग, अपॉइंटमेंट, बुकिंग और कार्य सभी आपके [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] कैलेंडर में उपलब्ध हैं.  
  
 यदि आप [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] उपयोग कर रहे हैं, तो आप Project Service समय प्रविष्टि दृश्य में अपनी व्यक्तिगत अपॉइंटमेंट्स भी दर्ज कर सकते हैं. यह परियोजना और संसाधन प्रबंधकों को परियोजनाओं के लिए आपकी उपलब्धता की जानकारी देता है. यह आपके समय की बचत भी करता है क्योंकि आपको दो बार अपनी व्यक्तिगत अपॉइंटमेंट्स के बारे में जानकारी दर्ज नहीं करनी पड़ती. आप बस अपने कैलेंडर से Project Service समय प्रविष्टि दृश्य में अपनी व्यक्तिगत अपॉइंटमेंट्स को आयात कर सकते हैं.  
  
 आपका कैलेंडर आज से लेकर आने वाले चार सप्ताहों तक परियोजना और कार्य ऑर्डर बुकिंग्स को सिंक्रनाइज़ करेगा. यह सेटिंग बदली नहीं जा सकती.  
  
 सिंक्रनाइज़ करना केवल PSA से आपके [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] कैलेंडर तक एक तरफ़ा समर्थित है,. आप रिवर्स ऑर्डर में सिंक कर सकते हैं। 
  
 अपने [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] कैलेंडर का उपयोग करने का तरीका जानने के लिए, [व्‍यवसाय के लिए वेब पर Outlook में कैलेंडर देखें](https://support.office.com/article/Calendar-in-Outlook-on-the-web-for-business-5219c457-d1fe-4c2f-9032-1a816b88e936).  
  
## <a name="setup"></a>सेटअप  
 इससे पहले कि आप अपने [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] कैलेंडर में अपनी बुकिंग देख सकें और उन्हें प्रबंधित कर सकें, आपको कुछ चीज़ें सेट अप करने की आवश्यकता होगी.  
  
- आपको [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] ग्‍लोबल व्यवस्थापक या सिस्टम व्यवस्थापक क्रेडेंशियल्स की आवश्यकता होगी.  
  
- आपके व्यवस्थापक को ईमेल सर्वर प्रोफ़ाइल कॉन्फ़िगर करना होगा और प्रत्येक उपयोगकर्ता को उसके मेलबॉक्स को कॉन्फ़िगर करने की आवश्यकता होगी. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [सर्वर-साइड सिंक्रनाइज़ेशन का उपयोग करके ईमेल संसाधन सेट अप करें](/dynamics365/customerengagement/on-premises/admin/set-up-server-side-synchronization-of-email-appointments-contacts-and-tasks)  
  
## <a name="turn-on-synchronization-for-your-organization-admin-task"></a>अपने संगठन के लिए सिंक्रनाइज़ेशन चालू करें (व्यवस्थापन कार्य)  
  
1.  मुख्य मेनू से, **सेटिंग्‍स** > **व्यवस्थापन** पर क्लिक करें.  
  
2.  **सिस्टम सेटिंग** पर क्लिक करें.  
  
3.  **सिंक्रनाइज़ेशन** टैब पर क्लिक करें.  
  
4.  **चुनें कि क्या संसाधन बुकिंग का निम्न के साथ सिंक्रनाइज़ेशन सक्षम करना है** के अंतर्गत, **Outlook के साथ संसाधन बुकिंग को सिंक्रनाइज़ करें** को चेक करें.  
  
## <a name="turn-on-synchronization-for-your-user-profile-user-task"></a>आपके उपयोगकर्ता प्रोफ़ाइल के लिए सिंक्रनाइज़ेशन चालू करें (उपयोगकर्ता कार्य)  
  
1.  स्क्रीन के ऊपरी-दाएँ कोने में **सेटिंग्स** बटन पर क्लिक करें.  
  
2.  **विकल्प** पर क्लिक करें.  
  
3.  **सिंक्रनाइज़ेशन** टैब पर क्लिक करें.  
  
4.  **Outlook के साथ संसाधन बुकिंग सिंक्रनाइज़ेशन** के अंतर्गत, **Outlook के साथ संसाधन बुकिंग सिंक्रनाइज़ेशन** को चेक करें.  
  
## <a name="import-your-personal-appointments-user-task"></a>अपनी व्यक्तिगत अपॉइंटमेंट्स आयात करें (उपयोगकर्ता कार्य)  
 आप अपने कैलेंडर से Project Service Automation समय प्रविष्टि दृश्य में अपनी व्यक्तिगत अपॉइंटमेंट्स को आयात कर सकते हैं.  
  
1. [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] कैलेंडर खोलें और **डेटा आयात करें** पर क्लिक करें.  
  
2. फ़िल्टर स्क्रीन पर, **Exchange से अपॉइंटमेंट्स** का चयन करें और फिर **लागू करें** पर क्लिक करें.  
  
3. सिस्टम वर्तमान सप्ताह से सुझाई गई प्रविष्टियों के रूप में अपॉइंटमेंट्स को समय प्रविष्टि दृश्य में खींचेगा. किसी अन्य सप्ताह के लिए प्रविष्टियाँ जोड़ने हेतु, **पिछला** या **अगला** पर क्लिक करें.  
  
4. उस अपॉइंटमेंट का चयन करें जिसे आप Project Service Automation समय प्रविष्टि दृश्य में जोड़ना चाहते हैं.  
  
5. **समय प्रविष्टि** पॉपअप बॉक्स में, अपॉइंटमेंट को Project Service Automation समय प्रविष्टि दृश्य में परिवर्तित करने के लिए उपयुक्त विकल्पों का चयन करें.  
  
6. **सहेजें** पर क्लिक करें.  
  
### <a name="see-also"></a>यह भी देखें  
 [समय, व्यय और सहयोग मार्गदर्शिका](../psa/time-expense-collaboration-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]