---
title: परियोजना शेड्यूलिंग लॉग
description: यह आलेख जानकारी और नमूने प्रदान करता है जो परियोजना शेड्यूलिंग लॉग का उपयोग करके परियोजना शेड्यूलिंग सेवा और परियोजना शेड्यूलिंग API से संबंधित विफलताओं को ट्रैक करने में आपकी सहायता करेगा।
author: ruhercul
ms.date: 11/30/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: ruhercul
ms.openlocfilehash: c57419642e90e4def01f2cd2474c9e82dc162b86
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8923697"
---
# <a name="project-scheduling-logs"></a>परियोजना शेड्यूलिंग लॉग

_**इस पर लागू होता है**: संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, लाइट परिनियोजन - प्रोफार्मा चालान-प्रक्रिया के लिए सौदा_, _Project for the Web_

Microsoft Dynamics 365 Project Operations इसके प्राथमिक शेड्यूलिंग इंजन के रूप में [Project for the Web](https://support.microsoft.com/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5) का उपयोग करता है। मानक Microsoft Dataverse का उपयोग करने के बजाय वेब एप्लिकेशन प्रोग्रामिंग इंटरफेस (एपीआई), Project Operations परियोजना टास्क, रिसोर्स असाइनमेंट, टास्क डिपेंडेंसी, परियोजना बकेट और परियोजना टीम के सदस्यों को बनाने, अपडेट करने और हटाने के लिए नए परियोजना शेड्यूलिंग एपीआई का उपयोग करता है। हालांकि, जब कार्य विश्लेषण संरचना (WBS) निकायों पर प्रोग्रामेटिक रूप से क्रिएट, अपडेट या डिलीट ऑपरेशन चलाए जाते हैं, तो त्रुटियां हो सकती हैं। इन त्रुटियों और संचालन के इतिहास को ट्रैक करने के लिए, दो नए प्रशासनिक लॉग लागू किए गए हैं: **ऑपरेशन सेट** तथा **परियोजना निर्धारण सेवा (पीएसएस)**। इन लॉग्स तक पहुँचने के लिए, **सेटिंग्स** \> **शेड्यूल एकीकरण** पर जाएँ।

निम्न उदाहरण परियोजना शेड्यूलिंग लॉग के लिए डेटा मॉडल दिखाता है।

![परियोजना शेड्यूलिंग मोड के लिए डेटा मॉडल](media/LOGDATAMODEL.jpg)

## <a name="operation-set-log"></a>ऑपरेशन सेट लॉग

ऑपरेशन सेट लॉग एक ऑपरेशन सेट के निष्पादन को ट्रैक करता है जिसका उपयोग प्रोजेक्ट्स, परियोजना टास्क, रिसोर्स असाइनमेंट, टास्क डिपेंडेंसी, परियोजना बकेट या परियोजना टीम के सदस्यों के बैच में एक या कई क्रिएट, अपडेट या डिलीट ऑपरेशन को चलाने के लिए किया जाता है। **स्थिति में संचालन** फ़ील्ड ऑपरेशन सेट की समग्र स्थिति दिखाता है। ऑपरेशन सेट पेलोड का विवरण संबंधित ऑपरेशन सेट विवरण रिकॉर्ड में दर्ज किया गया है।

### <a name="operation-set"></a>ऑपरेशन सेट

निम्न तालिका **ऑपरेशन सेट** निकाय से संबंधित फ़ील्ड को दिखाती है.

| स्कीमा का नाम            | विवरण                                                                                                  | DisplayName            |
|-----------------------|--------------------------------------------------------------------------------------------------------------|------------------------|
| msdyn_completedon     | तिथि/समय जब ऑपरेशन सेट पूरा या विफल हुआ था।                                                | CompletedOn            |
| msdyn_correlationid   | अनुरोध की **correlationId** वैल्यू।                                                                  | CorrelationId          |
| msdyn_description     | ऑपरेशन सेट का वर्णन.                                                                        | विवरण            |
| msdyn_executedon      | वह तिथि/समय जब रिकॉर्ड चला था.                                                                       | निष्पादन दिनांक            |
| msdyn_operationsetId  | निकाय आवृतियों का विशिष्ट पहचानकर्ता.                                                                   | OperationSet           |
| msdyn_Project         | परियोजना जो ऑपरेशन सेट से संबंधित है.                                                            | Project                |
| msdyn_projectid       | अनुरोध की **projectId** वैल्यू।                                                                      | ProjectId (अप्रचलित) |
| msdyn_projectName     | लागू नहीं.                                                                                              | लागू नहीं         |
| msdyn_PSSErrorLog     | परियोजना शेड्यूलिंग सेवा त्रुटि लॉग का विशिष्ट पहचानकर्ता जो ऑपरेशन सेट से संबद्ध है। | PSS त्रुटि लॉग          |
| msdyn_PSSErrorLogName | लागू नहीं.                                                                                              | लागू नहीं         |
| msdyn_status          | ऑपरेशन सेट की स्थिति                                                                             | स्थिति                 |
| msdyn_statusName      | लागू नहीं.                                                                                              | लागू नहीं         |
| msdyn_useraadid       | Azure Active Directory (Azure AD) उपयोगकर्ता की  ऑब्जेक्ट ID जिससे अनुरोध संबंधित है।                     | UserAADID              |

### <a name="operation-set-detail"></a>ऑपरेशन सेट विवरण

निम्न तालिका **ऑपरेशन सेट विवरण** निकाय से संबंधित फ़ील्ड को दिखाती है.

| स्कीमा का नाम                 | विवरण                                                                                 | DisplayName           |
|----------------------------|---------------------------------------------------------------------------------------------|-----------------------|
| msdyn_cdspayload           | अनुरोध के लिए क्रमाकृत Dataverse फ़ील्ड।                                            | CdsPayload            |
| msdyn_entityname           | अनुरोध के लिए निकाय का नाम.                                                     | EntityName            |
| msdyn_httpverb             | अनुरोध विधि।                                                                         | HTTP क्रिया (अप्रचलित) |
| msdyn_httpverbName         | लागू नहीं.                                                                             | लागू नहीं        |
| msdyn_operationset         | उस ऑपरेशन सेट का विशिष्ट पहचानकर्ता, जिसके साथ यह रिकॉर्ड संबंधित है।                      | OperationSet          |
| msdyn_operationsetdetailId | निकाय आवृतियों का विशिष्ट पहचानकर्ता.                                                  | OperationSet विवरण   |
| msdyn_operationsetName     | लागू नहीं.                                                                             | लागू नहीं        |
| msdyn_operationtype        | ऑपरेशन सेट विवरण का ऑपरेशन प्रकार.                                             | OperationType         |
| msdyn_operationtypeName    | लागू नहीं.                                                                             | लागू नहीं        |
| msdyn_psspayload           | अनुरोध के लिए क्रमबद्ध परियोजना शेड्यूलिंग सेवा फ़ील्ड।                           | PssPayload            |
| msdyn_recordid             | अनुरोध रिकॉर्ड का पहचानकर्ता.                                                       | रिकॉर्ड ID             |
| msdyn_requestnumber        | उस क्रम की पहचान करने वाला स्वतः जनरेट किया गया नंबर, जिसके अनुरोध प्राप्त हुए थे। | अनुरोध संख्या        |

## <a name="project-scheduling-service-error-logs"></a>परियोजना शेड्यूलिंग सेवा प्रवाह लॉग्स

परियोजना शेड्यूलिंग सेवा त्रुटि लॉग विफलताओं को कैप्चर करते हैं जो तब होती हैं जब परियोजना शेड्यूलिंग सेवा **सहेजे** या **खोलें** ऑपरेशन की कोशिश करती है। तीन समर्थित परिदृश्य हैं जहाँ ये लॉग उत्पन्न होते हैं:

- उपयोगकर्ता द्वारा शुरू की गई कार्रवाइयां गंभीर रूप से विफल हो जाती हैं (उदाहरण के लिए, अनुपलब्ध विशेषाधिकारों के कारण असाइनमेंट नहीं बनाया जा सकता)।
- परियोजना शेड्यूलिंग सेवा किसी निकाय पर प्रोग्रामेटिक रूप से कोई अन्य कैस्केडिंग ऑपरेशन नहीं बना सकती, अपडेट नहीं कर सकती, हटा सकती है या निष्पादित नहीं कर सकती है।
- जब कोई रिकॉर्ड खोलने में विफल रहता है तो उपयोगकर्ता त्रुटियों का अनुभव करता है (उदाहरण के लिए, जब कोई परियोजना खोला जाता है या टीम के सदस्य की जानकारी अपडेट की जाती है)।

### <a name="project-scheduling-service-log"></a>परियोजना शेड्यूलिंग सेवा लॉग

निम्न तालिका परियोजना शेड्यूलिंग सेवा लॉग में शामिल फ़ील्ड को दिखाती है.

| स्कीमा का नाम          | विवरण                                                                    | DisplayName    |
|---------------------|--------------------------------------------------------------------------------|----------------|
| msdyn_CallStack     | अपवाद का कॉल स्टैक.                                               | कॉल स्टैक     |
| msdyn_correlationid | त्रुटि की सहसंबंध id.                                               | CorrelationId  |
| msdyn_errorcode     | एक फ़ील्ड जिसका उपयोग Dataverse त्रुटि कोड या HTTP त्रुटि कोड स्टोर करने के लिए किया जाता है। | त्रुटि कोड     |
| msdyn_HelpLink      | सार्वजनिक सहायता दस्तावेज के लिए लिंक.                                       | सहायता लिंक      |
| msdyn_log           | परियोजना शेड्यूलिंग सेवा से लॉग।                                   | लॉग            |
| msdyn_project       | त्रुटि लॉग से सम्बद्ध परियोजना।                             | Project        |
| msdyn_projectName   | परियोजना का नाम यदि ऑपरेशन सेट का पेलोड बना रहेगा। | लागू नहीं |
| msdyn_psserrorlogId | निकाय आवृतियों का विशिष्ट पहचानकर्ता.                                     | PSS त्रुटि लॉग  |
| msdyn_SessionId     | परियोजना सत्र ID.                                                        | सत्र आईडी     |

## <a name="error-log-cleanup"></a>त्रुटि लॉग क्लीनअप

डिफ़ॉल्ट रूप से, परियोजना शेड्यूलिंग सेवा त्रुटि लॉग और ऑपरेशन सेट लॉग दोनों को हर 90 दिनों में साफ़ किया जा सकता है। 90 दिनों से पुराने सभी रिकॉर्ड्स हटा दिए जाएंगे. हालांकि, **परियोजना पैरामीटर** पृष्ठ पर **msdyn_StateOperationSetAge** फ़ील्ड के मूल्य को बदलकर, व्यवस्थापक क्लीनअप श्रेणी को इस प्रकार समायोजित कर सकते हैं कि यह 1 से 120 दिनों के बीच हो। इस मान को बदलने की कई विधियाँ उपलब्ध हैं:

- एक कस्टम पृष्ठ बनाकर **परियोजना पैरामीटर** निकाय को अनुकूलित करें और **स्टेल ऑपरेशन सेट एज** फ़ील्ड जोड़कर।
- क्लाइंट कोड का उपयोग करें जो [WebApi सॉफ्टवेयर डेवलपमेंट किट (एसडीके)](/powerapps/developer/model-driven-apps/clientapi/reference/xrm-webapi/updaterecord) का उपयोग करता है.
- सेवा SDK कोड का उपयोग करें जो **updateRecord** विधि (क्लाइंट API संदर्भ) मॉडल-चालित ऐप्स में Xrm SDK का उपयोग करता है। **updateRecord** तरीका के लिए Power Apps में एक विवरण और समर्थित पैरामीटर शामिल हैं।

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
