---
title: Microsoft Project में अपने कार्य की योजना बनाने के लिए Project Service ऐड-इन का उपयोग करना | MicrosoftDocs
description: यह विषय Microsoft Project Service के लिए Microsoft प्रोजेक्ट ऐड-इन को जोड़ना, कॉन्फ़िगर और उपयोग कैसे करना है के बारे में जानकारी प्रदान करता है।
author: ruhercul
ms.custom:
- dyn365-projectservice
ms.date: 04/06/2019
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
ms.openlocfilehash: 460b5bb7baabcb804b9745f5fddae9bcc3fc7541
ms.sourcegitcommit: 30242d7754bca300b594b0887eb4212d10bea1c4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/07/2022
ms.locfileid: "8727960"
---
# <a name="use-the-project-service-automation-add-in-to-plan-your-work-in-microsoft-project"></a>Microsoft Project में आपके कार्य की योजना बनाने के लिए Project Service Automation ऐड-इन का उपयोग करें

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] आपके लिए अनुमान सहित आपकी परियोजना को नियोजित करना आसान बनाता है. आप कार्य को परिभाषित कर सकते हैं ताकि अंतिम प्रस्ताव प्रस्तुत किए जाने पर लागत, प्रयास और विक्रय मान स्पष्ट हों.  

 अब आप [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] स्थापित कर सकते हैं और [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] के परिचित परिवेश में अपना नियोजन कार्य कर सकते हैं. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] की मज़बूत नियोजन और प्रबंधन क्षमताओं का उपयोग करें और उसके बाद Project Service Automation में अपनी परियोजना की योजना का अद्यतन करें.  

> [!IMPORTANT]
> - [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] परियोजनाओं के लिए अपनी [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] फ़ाइलों को स्टोर करने के लिए SharePoint दस्तावेज़ प्रबंधन का उपयोग करने के लिए आपके [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] व्यवस्थापक को दस्तावेज़ प्रबंधन विकल्प चालू करना होगा. 
> - [!INCLUDE[pn_ms_dyn_365_psa_for_ms_project](../includes/pn-ms-dyn-365-psa-for-ms-project.md)] केवल [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] 2016 Professional Edition के साथ संगत है.  

## <a name="download-and-install-the-add-in"></a>ऐड-इन डाउनलोड और स्थापित करें  
 अपनी [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] साइन-इन जानकारी तैयार रखें. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] से [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] पर कनेक्ट करने के लिए आपको इस जानकारी की आवश्यकता होगी.  

1.  डाउनलोड केंद्र से आप, Project Service के अपने समर्थित संस्करण [V2.X](/dynamics365/project-operations/psa/overview#guidance-for-earlier-versions-app-version-2x-or-1x) या [V3.4+](https://www.microsoft.com/download/details.aspx?id=57956) के लिए ऐड-इन डाउनलोड कर सकते हैं.  

2.  डाउनलोड लिंक पर क्लिक करें.  

3.  जब डाउनलोड पूरा हो जाए, तो ऐड-इन इंस्टॉल करने के लिए **हां** पर क्लिक करें।  

## <a name="configure-the-add-in"></a>ऐड-इन को कॉन्फ़िगर करें  

1. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] खोलें और **Project Service** टैब पर क्लिक करें.  

2. **कनेक्ट करें** क्लिक करें.  

3. अपनी साइन-इन जानकारी दर्ज करें और फिर **साइन इन करें** पर क्लिक करें.  

   अब आप ऐड-इन का उपयोग करना प्रारंभ कर सकते हैं.  

## <a name="read-from-a-template"></a>टेम्पलेट से पढ़ें  
 उस टेम्पलेट से पढ़ें, जो आपने [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] में बनाया था और जिसकी आपने अपनी परियोजना योजना प्रारंभ करने के लिए [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] में प्रतिलिपि बनाई थी. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [एक परियोजना टेम्पलेट बनाएँ (Project Service Automation)](../psa/create-project-template.md)  

1.  **Project Service** टैब से, **पढ़ें** > **Project Service Automation परियोजना टेम्पलेट** पर क्लिक करें.  

2.  सूची से परियोजना टेम्पलेट चुनें और फिर **खोलें** पर क्लिक करें.  

    > [!NOTE]
    >  डिफ़ॉल्ट रूप से, टेम्पलेट से परियोजना में जिन कार्यों की प्रतिलिपि बनाई जाती है, वे मैन्युअल रूप से शेड्यूल किए गए के रूप में सेट किए जाते हैं.  

## <a name="assign-pn_project_service_auto-roles-to-project-resources"></a>परियोजना संसाधनों को [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] भूमिकाएँ असाइन करें  

1.  परियोजना खोलें और **कार्य** रिबन पर क्लिक करें.  

2.  **गैंट चार्ट** मेनू पर क्लिक करें और फिर **संसाधन पत्रक** चुनें.  

3.  संसाधन पत्रक पर, **Project Service संसाधन भूमिका** ड्रॉप-डाउन मेनू पर क्लिक करें और Project Service Automation भूमिका चुनें.  

## <a name="staff-your-project-with-resources"></a>अपनी परियोजना में संसाधनों के साथ कर्मचारी जोड़ें  

1.  Project Service टैब से, किसी पंक्ति का चयन करें और **संसाधन ढूँढें** पर क्लिक करें.  

2.  **संसाधन बुक करें** स्क्रीन पर, उस संसाधन का चयन करें जिसका उपयोग आप परियोजना के लिए करना चाहते हैं.  

3.  **बुक करें** पर क्लिक करें और फिर **ठीक** पर क्लिक करें.  

## <a name="publish-your-project"></a>अपनी परियोजना प्रकाशित करें  
आपका परियोजना नियोजन पूर्ण होने पर, अगला चरण परियोजना को [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] में आयात और प्रकाशित करना है.  

परियोजना [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] में आयात हो जाएगी. मूल्य निर्धारण और टीम जनरेशन प्रक्रिया लागू की जाती है. यह देखने के लिए [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] में परियोजना को खोलें कि टीम, परियोजना अनुमान और कार्य विश्लेषण संरचना जनरेट किए गए हैं. निम्न तालिका दिखाती है कि परिणामों को कहाँ खोजना है:

| Project | Details |
| ---- | --- |
|  [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **गैंट चार्ट**   | [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **कार्य विश्लेषण संरचना** स्क्रीन में आयात करता है. |
| [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **संसाधन पत्रक** |   [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **परियोजना Team Members** स्क्रीन में आयात करता है.   |
|   [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] **उपयोग का उपयोग करें**    |    [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] **परियोजना अनुमान** स्क्रीन में आयात करता है.     |

**अपनी परियोजना को आयात और प्रकाशित करने के लिए**  
1. **Project Service** टैब से, **प्रकाशित करें** > **नई Project Service Automation परियोजना** पर क्लिक करें.  

2. **Project Service में नई परियोजना पर प्रकाशित करें** संवाद बॉक्‍स पर, **परियोजना का नाम** दर्ज करें और **ग्राहक** चुनें.  

3. वैकल्पिक रूप से योजना Project फ़ाइल को Project Service Automation से लिंक करने के लिए **परियोजना की योजना को Project Service Automation से लिंक करें** को चेक करें.  

4. **प्रकाशित करें** क्लिक करें.  

   Project फ़ाइल को [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] से लिंक करना परियोजना फ़ाइल को मास्टर बनाता है और [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] में कार्य विश्लेषण संरचना को केवल पढ़ने के लिए पर सेट करता है.  परियोजना की योजना में परिवर्तन करने के लिए, वे परिवर्तन आपको [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] में करने होंगे और उन्हें [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] के अद्यतन के रूप में प्रकाशित करना होगा.  

## <a name="edit-a-project-thats-been-imported"></a>ऐसी कोई परियोजना संपादित करें जिसे आयात किया गया है  
 [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] में आयात की गई परियोजना की योजना में परिवर्तन करने के लिए, आपके पास दो विकल्प हैं:  

- मास्टर फ़ाइल खोलें और उसे [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] में संपादित करें.  

- फ़ाइल को अनलिंक करें और उसे सीधे Project Service में संपादित करें. डिफ़ॉल्ट रूप से, [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] से अपलोड की गई परियोजना लॉक होती है और केवल परियोजना में संपादित की जा सकती है. [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] में फ़ाइल संपादित करने के लिए, फ़ाइल को अनलिंक करना होगा.  

### <a name="edit-in-pn_microsoft_project"></a>[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] में संपादित करें  

1. मुख्य मेनू से, **Project Service** > **परियोजनाएँ** पर क्लिक करें.  

2. परियोजनाओं की सूची से, उस परियोजना को खोलें, जो आपने [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] में बनाई थी.  

3. रिबन से **MS Project में खोलें** पर क्लिक करें. यह लिंक की गई मास्टर फ़ाइल को [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] में खोले देगा.  

### <a name="unlink-a-file-and-edit-in-pn_microsoft_project-service"></a>फ़ाइल को अनलिंक करें और उसे [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] Service में संपादित करें  

1. मुख्य मेनू से, **Project Service** > **परियोजनाएँ** पर क्लिक करें.  

2. परियोजनाओं की सूची से, उस परियोजना को खोलें, जो आपने [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] में बनाई थी.  

3. रिबन से **MS Project से अनलिंक करें** पर क्लिक करें.  

## <a name="upload-a-project-file-to-sharepoint-or-office-groups"></a>SharePoint या Office समूहों के लिए एक प्रोजेक्ट फ़ाइल अपलोड करें  
 आप अपनी प्रोजेक्ट फ़ाइल को SharePoint पर अपलोड कर सकते हैं और इसे अपने [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] प्रोजेक्ट के लिए संबद्ध दस्तावेज़ों के तहत पा सकते हैं।  आपको चाहिए कि आपका व्यवस्थापक SharePoint दस्तावेज़ प्रबंधन को कॉन्फ़िगर करे और इसे परियोजना इकाई के लिए चालू करे. 

 यदि आपके पास Office समूह सेट अप है, तो आप अपनी परियोजना फ़ाइल को [!INCLUDE[pn_onedrive_for_business](../includes/pn-onedrive-for-business.md)] में भी अपलोड कर सकते हैं.

### <a name="upload-a-file-for-sharepoint"></a>SharePoint के लिए एक फ़ाइल अपलोड करें  

1. मुख्य मेनू से, **Project Service** > **अपलोड करें** पर क्लिक करें.  

2. **Project Service Automation परियोजना दस्तावेज़ के लिए** का चयन करें.  

3. **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] में खोलें सक्षम करें** संवाद में, **हाँ** या **नहीं** चुनें.  

   - अगर आप **हाँ** पर क्लिक करते हैं, तो आप Project Service Automation में **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** बटन में खोलें चुन पाएंगे और [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] लॉन्च करें और SharePoint दस्तावेज़ लाइब्रेरी से परियोजना फ़ाइल लोड करें.  

   - अगर आप **नहीं** पर क्लिक करते हैं, तो **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** बटन में खोलें के लिए लिंक काम नहीं करेगा.  

4. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] फ़ाइल विशिष्ट [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] परियोजना के लिए **दस्तावेज़** के अंतर्गत [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] में मिल सकती है.  

### <a name="upload-a-file-for-office-groups"></a>Office समूह के लिए फ़ाइल अपलोड करें  

1. मुख्य मेनू से, **Project Service** > **अपलोड करें** पर क्लिक करें.  

2. **Project Service Automation परियोजना दस्तावेज़ के लिए** का चयन करें.  

3. **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] में खोलें सक्षम करें** संवाद में, **हाँ** या **नहीं** चुनें.  

   - अगर आप **हाँ** पर क्लिक करते हैं, तो आप Project Service Automation में **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** बटन में खोलें चुन पाएंगे और [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] लॉन्च करें और SharePoint दस्तावेज़ लाइब्रेरी से परियोजना फ़ाइल लोड करें.  

   - अगर आप **नहीं** पर क्लिक करते हैं, तो **[!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)]** बटन में खोलें के लिए लिंक काम नहीं करेगा.  

4. [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] फ़ाइल विशिष्ट [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] परियोजना के लिए **दस्तावेज़** के अंतर्गत [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] में मिल सकती है.  

## <a name="publish--your-project-as-a-template"></a>अपनी परियोजना को टेम्पलेट के रूप में प्रकाशित करें  
 आप अपनी परियोजना को सहेज सकते हैं और [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] में परियोजना टेम्पलेट के रूप में उसे सहेज कर उसका पुन: प्रयोग कर सकते हैं.  परियोजना टेम्पलेट्स [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] में पुनः उपयोग योग्य परियोजना की योजनाएँ हैं. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [एक परियोजना टेम्पलेट बनाएँ (Project Service Automation)](../psa/create-project-template.md)  

1. **Project Service** टैब से, **प्रकाशित करें** > **नई Project Service Automation परियोजना टेम्पलेट** पर क्लिक करें.  

2. **Project Service टेम्पलेट में नई परियोजना प्रकाशित करें** संवाद बॉक्‍स में, **परियोजना टेम्पलेट का नाम** दर्ज करें.  

3. वैकल्पिक रूप से, परियोजना फ़ाइल को [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] से लिंक करने के लिए **परियोजना योजना को Project Service Automation से लिंक करें** को चेक करें.  

4. **प्रकाशित करें** क्लिक करें.  

Project फ़ाइल को [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] से लिंक करना परियोजना फ़ाइल को मास्टर बनाता है और [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] टेम्पलेट में कार्य विश्लेषण संरचना को केवल पढ़ने के लिए पर सेट करता है.  परियोजना की योजना में परिवर्तन करने के लिए, वे परिवर्तन आपको [!INCLUDE[pn_microsoft_project](../includes/pn-microsoft-project.md)] में करने होंगे और उन्हें [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] के अद्यतन के रूप में प्रकाशित करना होगा.

## <a name="read-a-resource-loaded-schedule"></a>संसाधन लोड हुआ शेड्यूल पढ़ें

Project Service Automation से किसी परियोजना को पढ़ते समय, संसाधन का कैलेंडर डेस्कटॉप क्लाइंट के लिए सिंक्रनाइज़ नहीं किया जाता है. यदि कार्य अवधि, प्रयास, या अंत में अंतर हैं, तो यह संभवतः इसलिए है, क्योंकि संसाधन और डेस्कटॉप क्लाइंट के पास परियोजना पर लागू समान कार्य समय टेम्पलेट कैलेंडर नहीं है.


## <a name="data-synchronization"></a>डेटा सिंक्रोनाइज़ेशन

निम्न तालिका बताती है कि Project Service Automation और Microsoft Project डेस्कटॉप ऐड-इन के बीच डेटा को कैसे सिंक्रनाइज़ किया जाता है.

| **निकाय** | **फ़ील्ड** | **Microsoft Project से Project Service Automation में** | **Project Service Automation से Microsoft Project में** |
| --- | --- | --- | --- |
| परियोजना कार्य | नियत तिथि | ● | - |
| परियोजना कार्य | अनुमानित प्रयास | ● | - |
| परियोजना कार्य | MS Project क्लाइंट ID | ● | - |
| परियोजना कार्य | पैरेंट कार्य | ● | - |
| परियोजना कार्य | Project | ● | - |
| परियोजना कार्य | परियोजना कार्य | ● | - |
| परियोजना कार्य | परियोजना कार्य का नाम | ● | - |
| परियोजना कार्य | संसाधन इकाई (v3.0 में डेप्रिकेटेड) | ● | - |
| परियोजना कार्य | शेड्यूल की गई अवधि | ● | - |
| परियोजना कार्य | प्रारंभ तिथि | ● | - |
| परियोजना कार्य | WBS ID | ● | - |

| **निकाय** | **फ़ील्ड** | **Microsoft Project से Project Service Automation में** | **Project Service Automation से Microsoft Project में** |
| --- | --- | --- | --- |
| टीम सदस्य | MS Project क्लाइंट ID | ● | - |
| टीम सदस्य | पद का नाम | ● | - |
| टीम सदस्य | प्रोजेक्ट | ● | ● |
| टीम सदस्य | परियोजना टीम | ● | ● |
| टीम सदस्य | संसाधन इकाई | - | ● |
| टीम सदस्य | भूमिका | - | ● |
| टीम सदस्य | कार्य घंटे | सिंक्रनाइज़्ड नहीं | सिंक्रनाइज़्ड नहीं |

| **निकाय** | **फ़ील्ड** | **Microsoft Project से Project Service Automation में** | **Project Service Automation से Microsoft Project में** |
| --- | --- | --- | --- |
| संसाधन असाइनमेंट | प्रारंभ दिनांक | ● | - |
| संसाधन असाइनमेंट | घंटे | ● | - |
| संसाधन असाइनमेंट | MS Project क्लाइंट ID | ● | - |
| संसाधन असाइनमेंट | नियोजित कार्य | ● | - |
| संसाधन असाइनमेंट | Project | ● | - |
| संसाधन असाइनमेंट | परियोजना टीम | ● | - |
| संसाधन असाइनमेंट | संसाधन असाइनमेंट | ● | - |
| संसाधन असाइनमेंट | कार्य | ● | - |
| संसाधन असाइनमेंट | आज तक | ● | - |

| **निकाय** | **फ़ील्ड** | **Microsoft Project से Project Service Automation में** | **Project Service Automation से Microsoft Project में** |
| --- | --- | --- | --- |
| परियोजना कार्य निर्भरताएँ | परियोजना कार्य निर्भरता | ● | - |
| परियोजना कार्य निर्भरताएँ | लिंक प्रकार | ● | - |
| परियोजना कार्य निर्भरताएँ | पूर्वगामी कार्य | ● | - |
| परियोजना कार्य निर्भरताएँ | Project | ● | - |
| परियोजना कार्य निर्भरताएँ | उत्तरवर्ती कार्य | ● | - |

### <a name="see-also"></a>यह भी देखें  
 [परियोजना प्रबंधक मार्गदर्शिका](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
