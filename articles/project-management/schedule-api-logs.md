---
title: प्रोजेक्ट शेड्यूलिंग लॉग
description: यह विषय जानकारी और नमूने प्रदान करता है जो प्रोजेक्ट शेड्यूलिंग लॉग का उपयोग करके प्रोजेक्ट शेड्यूलिंग सेवा और प्रोजेक्ट शेड्यूलिंग API से संबंधित विफलताओं को ट्रैक करने में आपकी सहायता करेगा।
author: ruhercul
ms.date: 11/30/2021
ms.topic: article
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 1c5632a880fa30d1b863c326b22e3d930c9564dc
ms.sourcegitcommit: 844ec8eacd0fc10d1659b437cc5cbb4480ec9e1e
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 12/01/2021
ms.locfileid: "7877510"
---
# <a name="project-scheduling-logs"></a>प्रोजेक्ट शेड्यूलिंग लॉग

_**पर लागू होता है:** संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए परियोजना संचालन, लाइट परिनियोजन - प्रोफार्मा चालान-प्रक्रिया के लिए सौदा_, _के लिए परियोजना_

माइक्रोसॉफ्ट Dynamics 365 Project Operations उपयोग करता है [वेब के लिए परियोजना](https://support.microsoft.com/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5) इसके प्राथमिक शेड्यूलिंग इंजन के रूप में। मानक Microsoft Dataverse वेब एप्लिकेशन प्रोग्रामिंग इंटरफेस (API) का उपयोग करने के बजाय, प्रोजेक्ट ऑपरेशंस प्रोजेक्ट कार्यों, संसाधन असाइनमेंट, कार्य निर्भरता, प्रोजेक्ट बकेट और प्रोजेक्ट टीम के सदस्यों को बनाने, अपडेट करने और हटाने के लिए नए प्रोजेक्ट शेड्यूलिंग API का उपयोग करता है। हालांकि, जब वर्क ब्रेकडाउन स्ट्रक्चर (WBS) निकायों पर प्रोग्रामेटिक रूप से क्रिएट, अपडेट या डिलीट ऑपरेशन चलाए जाते हैं, तो त्रुटियां हो सकती हैं। इन त्रुटियों और संचालन के इतिहास को ट्रैक करने के लिए, दो नए प्रशासनिक लॉग लागू किए गए हैं: **ऑपरेशन सेट** तथा**परियोजना निर्धारण सेवा (पीएसएस)**. इन लॉग्स तक पहुँचने के लिए, यहाँ जाएँ **समायोजन** \> **अनुसूची एकीकरण**.

निम्न उदाहरण प्रोजेक्ट शेड्यूलिंग लॉग के लिए डेटा मॉडल दिखाता है।

![प्रोजेक्ट शेड्यूलिंग लॉग के लिए डेटा मॉडल।](media/LOGDATAMODEL.jpg)

## <a name="operation-set-log"></a>ऑपरेशन सेट लॉग

ऑपरेशन सेट लॉग एक ऑपरेशन सेट के निष्पादन को ट्रैक करता है जिसका उपयोग प्रोजेक्ट्स, प्रोजेक्ट टास्क, रिसोर्स असाइनमेंट, टास्क डिपेंडेंसी, प्रोजेक्ट बकेट या प्रोजेक्ट टीम के सदस्यों के बैच में एक या कई क्रिएट, अपडेट या डिलीट ऑपरेशन को चलाने के लिए किया जाता है। NS **स्थिति में संचालन** फ़ील्ड ऑपरेशन सेट की समग्र स्थिति दिखाता है। ऑपरेशन सेट पेलोड का विवरण संबंधित ऑपरेशन सेट विवरण रिकॉर्ड में दर्ज किया गया है।

### <a name="operation-set"></a>ऑपरेशन सेट

निम्न तालिका उन क्षेत्रों को दिखाती है जो संबंधित हैं **ऑपरेशन सेट** कंपनी।

| SchemaName            | विवरण                                                                                                  | DisplayName            |
|-----------------------|--------------------------------------------------------------------------------------------------------------|------------------------|
| msdyn_completedon     | वह तारीख/समय जब ऑपरेशन सेट पूरा हुआ या विफल रहा।                                                | CompletedOn            |
| msdyn_correlationid   | NS **सहसंबंध आईडी** अनुरोध का मूल्य।                                                                  | CorrelationId          |
| msdyn_description     | ऑपरेशन सेट का विवरण।                                                                        | विवरण            |
| msdyn_executedon      | दिनांक/समय जब रिकॉर्ड चलाया गया था।                                                                       | निष्पादन दिनांक            |
| msdyn_operationsetId  | इकाई उदाहरणों की विशिष्ट पहचानकर्ता।                                                                   | OperationSet           |
| msdyn_परियोजना         | प्रोजेक्ट जो ऑपरेशन सेट से संबंधित है।                                                            | Project                |
| msdyn_projectid       | NS **प्रोजेक्ट आईडी** अनुरोध का मूल्य।                                                                      | ProjectId (अप्रचलित) |
| msdyn_projectName     | लागू नहीं.                                                                                              | लागू नहीं         |
| msdyn_PSSErrorLog     | प्रोजेक्ट शेड्यूलिंग सेवा त्रुटि लॉग का विशिष्ट पहचानकर्ता जो ऑपरेशन सेट से संबद्ध है। | PSS त्रुटि लॉग          |
| msdyn_PSSErrorLogName | लागू नहीं.                                                                                              | लागू नहीं         |
| msdyn_status          | ऑपरेशन सेट की स्थिति।                                                                             | स्थिति                 |
| msdyn_statusName      | लागू नहीं.                                                                                              | लागू नहीं         |
| msdyn_useraadid       | उस उपयोगकर्ता का Azure Active Directory (Azure AD) ऑब्जेक्ट आईडी जिससे अनुरोध संबंधित है।                     | UserAADID              |

### <a name="operation-set-detail"></a>ऑपरेशन सेट विवरण

निम्न तालिका उन क्षेत्रों को दिखाती है जो संबंधित हैं **ऑपरेशन सेट विवरण** कंपनी।

| SchemaName                 | विवरण                                                                                 | DisplayName           |
|----------------------------|---------------------------------------------------------------------------------------------|-----------------------|
| msdyn_cdspayload           | अनुरोध के लिए क्रमबद्ध Dataverse फ़ील्ड।                                            | CdsPayload            |
| msdyn_entityname           | अनुरोध के लिए निकाय का नाम.                                                     | EntityName            |
| msdyn_httpverb             | अनुरोध विधि।                                                                         | HTTP क्रिया (अप्रचलित) |
| msdyn_httpverbName         | लागू नहीं.                                                                             | लागू नहीं        |
| msdyn_ऑपरेशनसेट         | ऑपरेशन का विशिष्ट पहचानकर्ता सेट करता है कि रिकॉर्ड किसका है।                      | OperationSet          |
| msdyn_operationsetdetailId | इकाई उदाहरणों की विशिष्ट पहचानकर्ता।                                                  | OperationSet विवरण   |
| msdyn_operationsetName     | लागू नहीं.                                                                             | लागू नहीं        |
| msdyn_ऑपरेशन प्रकार        | ऑपरेशन सेट का ऑपरेशन प्रकार विवरण।                                             | OperationType         |
| msdyn_operationtypeName    | लागू नहीं.                                                                             | लागू नहीं        |
| msdyn_psspayload           | अनुरोध के लिए क्रमबद्ध प्रोजेक्ट शेड्यूलिंग सेवा फ़ील्ड।                           | PssPayload            |
| msdyn_recordid             | अनुरोध रिकॉर्ड की पहचानकर्ता।                                                       | रिकॉर्ड ID             |
| msdyn_requestnumber        | एक स्वचालित रूप से जेनरेट की गई संख्या जो उस क्रम की पहचान करती है जिसमें अनुरोध प्राप्त हुए थे। | अनुरोध संख्या        |

## <a name="project-scheduling-service-error-logs"></a>प्रोजेक्ट शेड्यूलिंग सेवा त्रुटि लॉग

प्रोजेक्ट शेड्यूलिंग सेवा त्रुटि लॉग कैप्चर विफलताओं को कैप्चर करते हैं जो तब होती हैं जब प्रोजेक्ट शेड्यूलिंग सेवा कोशिश करती है a **सहेजें** या**खोलना** कार्यवाही। तीन समर्थित परिदृश्य हैं जहाँ ये लॉग उत्पन्न होते हैं:

- उपयोगकर्ता द्वारा शुरू की गई कार्रवाइयां गंभीर रूप से विफल हो जाती हैं (उदाहरण के लिए, विशेषाधिकार अनुपलब्ध होने के कारण असाइनमेंट नहीं बनाया जा सकता है)।
- प्रोजेक्ट शेड्यूलिंग सेवा किसी निकाय पर प्रोग्रामेटिक रूप से कोई अन्य कैस्केडिंग ऑपरेशन नहीं बना सकती, अपडेट नहीं कर सकती, हटा सकती है या निष्पादित नहीं कर सकती है।
- जब कोई रिकॉर्ड खुलने में विफल रहता है तो उपयोगकर्ता त्रुटियों का अनुभव करता है (उदाहरण के लिए, जब कोई प्रोजेक्ट खोला जाता है या टीम के सदस्य की जानकारी अपडेट की जाती है)।

### <a name="project-scheduling-service-log"></a>परियोजना निर्धारण सेवा लॉग

निम्न तालिका प्रोजेक्ट शेड्यूलिंग सेवा लॉग में शामिल फ़ील्ड दिखाती है।

| SchemaName          | विवरण                                                                    | DisplayName    |
|---------------------|--------------------------------------------------------------------------------|----------------|
| msdyn_CallStack     | अपवाद का कॉल स्टैक.                                               | कॉल स्टैक     |
| msdyn_correlationid | त्रुटि का सहसंबंध आईडी।                                               | CorrelationId  |
| msdyn_errorcode     | एक फ़ील्ड जिसका उपयोग Dataverse त्रुटि कोड या HTTP त्रुटि कोड को संग्रहीत करने के लिए किया जाता है। | त्रुटि कोड     |
| msdyn_HelpLink      | सार्वजनिक सहायता दस्तावेज़ीकरण का लिंक।                                       | सहायता लिंक      |
| msdyn_log           | प्रोजेक्ट शेड्यूलिंग सेवा से लॉग।                                   | लॉग            |
| msdyn_project       | प्रोजेक्ट जो त्रुटि लॉग के साथ संबद्ध है।                             | Project        |
| msdyn_projectName   | प्रोजेक्ट का नाम यदि ऑपरेशन सेट का पेलोड बना रहेगा। | लागू नहीं |
| msdyn_psserrorlogId | इकाई उदाहरणों की विशिष्ट पहचानकर्ता।                                     | PSS त्रुटि लॉग  |
| msdyn_SessionId     | परियोजना सत्र आईडी।                                                        | सत्र आईडी     |

## <a name="error-log-cleanup"></a>त्रुटि लॉग सफाई

डिफ़ॉल्ट रूप से, प्रोजेक्ट शेड्यूलिंग सेवा त्रुटि लॉग और ऑपरेशन सेट लॉग दोनों को हर 90 दिनों में साफ़ किया जा सकता है। 90 दिनों से अधिक पुराने किसी भी रिकॉर्ड को हटा दिया जाएगा। हालांकि, के मूल्य को बदलकर **msdyn_StateOperationSetAge** मैदान पर **परियोजना पैरामीटर्स** पृष्ठ पर, व्यवस्थापक क्लीनअप श्रेणी को इस प्रकार समायोजित कर सकते हैं कि यह 1 से 120 दिनों के बीच हो। इस मान को बदलने की कई विधियाँ उपलब्ध हैं:

- अनुकूलित करें **परियोजना पैरामीटर** निकाय एक कस्टम पृष्ठ बनाकर और जोड़ कर **बासी संचालन निर्धारित आयु** खेत।
- क्लाइंट कोड का उपयोग करें जो का उपयोग करता है [वेबएपी सॉफ्टवेयर डेवलपमेंट किट (एसडीके)](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/updaterecord).
- सेवा एसडीके कोड का उपयोग करें जो एक्सआरएम एसडीके का उपयोग करता है **अद्यतन रिकॉर्ड** विधि (क्लाइंट API संदर्भ) मॉडल-चालित ऐप्स में। Power Apps में इसके लिए एक विवरण और समर्थित पैरामीटर शामिल हैं **अद्यतन रिकॉर्ड** तरीका।

    ```C#
    Xrm.WebApi.retrieveMultipleRecords('msdyn_projectparameter').then(function (response) {
        parameter = response.entities[0];
        var staleOperationValue = prompt("All records older than (x) days will be deleted, please enter X between 1 to 90 days", 1)
        var newData = {};
        newData.msdyn_projectparameterid = parameter.msdyn_projectparameterid;
        newData.msdyn_staleoperationsetage = parseInt(staleOperationValue);
        Xrm.WebApi.updateRecord("msdyn_projectparameter", parameter.msdyn_projectparameterid, newData).then(
            function success(result) {
                console.log("Project Parameter: Stale Operation Expiry is set to: " + newData.msdyn_staleoperationsetage);
                // perform operations on record update
                Xrm.WebApi.retrieveMultipleRecords('msdyn_projectparameter')
                .then(function (response2) { console.log("Confirmed Project Parameter: Stale Operation Expiry is set to: " + response2.entities[0].msdyn_staleoperationsetage) });
            },
            function (error) {
                console.log("Failed to Update Project Ednpoint with error: " + error.message);
            // handle error conditions
            }
        );
    });
    ```
