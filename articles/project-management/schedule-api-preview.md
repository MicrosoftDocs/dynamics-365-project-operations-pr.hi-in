---
title: शेड्यूलिंग निकायों के साथ संचालन करने के लिए प्रोजेक्ट शेड्यूल API का उपयोग करें
description: यह विषय प्रोजेक्ट शेड्यूल API का उपयोग करने के लिए जानकारी और नमूने प्रदान करता है.
author: sigitac
ms.date: 06/22/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 4915261c08a3271a919e04084e92a14b297c1b35
ms.sourcegitcommit: 2f16c2bc7c8350676a6a380c61fffa9958db6a0b
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/22/2021
ms.locfileid: "6293229"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a>शेड्यूलिंग निकायों के साथ संचालन करने के लिए प्रोजेक्ट शेड्यूल API का उपयोग करें

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

> [!IMPORTANT] 
> इस विषय में नोट की गई कुछ या सभी कार्यक्षमता पूर्वावलोकन रिलीज के हिस्से के रूप में उपलब्ध है. सामग्री और कार्यक्षमता परिवर्तन के अधीन हैं. 

## <a name="scheduling-entities"></a>शेड्यूलिंग निकाय

प्रोजेक्ट शेड्यूल API **शेड्यूलिंग निकाय** के साथ ऑपरेशन बनाने, अपडेट करने और हटाने की क्षमता प्रदान करते हैं. इन निकायों को वेब के लिए परियोजना में शेड्यूलिंग इंजन के माध्यम से प्रबंधित किया जाता है. पहले Dynamics 365 Project Operations रिलीज़ में **निकाय शेड्यूलिंग** के साथ संचालन बनाएं, अपडेट करें और मिटाएं.

निम्न तालिका प्रोजेक्ट शेड्यूल निकायों की पूरी सूची प्रदान करती है.

| निकाय का नाम  | निकाय तार्किक नाम |
| --- | --- |
| Project | msdyn_project |
| परियोजना कार्य  | msdyn_projecttask  |
| परियोजना कार्य निर्भरता  | msdyn_projecttaskdependency  |
| संसाधन असाइनमेंट | msdyn_resourceassignment |
| परियोजना बकेट  | msdyn_projectbucket |
| परियोजना टीम सदस्य | msdyn_projectteam |

## <a name="operationset"></a>OperationSet

OperationSet एक यूनिट-ऑफ-वर्क पैटर्न है जिसका उपयोग तब किया जा सकता है जब शेड्यूल प्रभावित करने वाले कई अनुरोधों को लेनदेन के भीतर संसाधित किया जाना चाहिए.

## <a name="project-schedule-apis"></a>प्रोजेक्ट शेड्यूल API

निम्नलिखित वर्तमान प्रोजेक्ट शेड्यूल API की सूची है.

- **msdyn_CreateProjectV1**: इस API का उपयोग एक प्रोज़ेक्ट बनाने के लिए किया जा सकता है. प्रोज़ेक्ट और डिफॉल्ट प्रोज़ेक्ट बकेट तुरंत बनाया जाता है.
- **msdyn_CreateTeamMemberV1**: इस API का उपयोग प्रोज़ेक्ट टीम के सदस्य बनाने के लिए किया जा सकता है. टीम के सदस्य का रिकार्ड तुरंत बनाया जाता है.
- **msdyn_CreateOperationSetV1**: इस एपीआई का उपयोग कई अनुरोधों को शेड्यूल करने के लिए किया जा सकता है जिन्हें लेनदेन के भीतर किया जाना चाहिए.
- **msdyn_PSSCreateV1**: इस एपीआई का उपयोग एक निकाय बनाने के लिए किया जा सकता है. निकाय कोई भी प्रोजेक्ट शेड्यूलिंग निकाय हो सकता है, जो निर्माण कार्य का समर्थन करता है.
- **msdyn_PSSCreateV1**: इस API का उपयोग एक निकाय अपडेट के लिए किया जा सकता है. निकाय कोई भी प्रोजेक्ट शेड्यूलिंग निकाय हो सकता है, जो अपडेट कार्य का समर्थन करता है.
- **msdyn_PSSDeleteV1**: इस API को हटाने के लिए एक निकाय इस्तेमाल किया जा सकता है. निकाय कोई भी प्रोजेक्ट शेड्यूलिंग निकाय हो सकता है, जो हटाने के कार्य का समर्थन करता है.
- **msdyn_ExecuteOperationSetV1**: इस एपीआई का उपयोग दिए गए ऑपरेशन सेट के भीतर सभी संचालनों को निष्पादित करने के लिए किया जाता है.

## <a name="using-project-schedule-apis-with-operationset"></a>ऑपरेशनसेट के साथ प्रोजेक्ट शेड्यूल API का उपयोग करना

क्योंकि दोनों के साथ रिकॉर्ड **CreateProjectV1** और **CreateTeamMemberV1** तुरंत बनाए जाते हैं, इन APIs का उपयोग सीधे **OperationSet** में नहीं किया जा सकता है. हालांकि, आप आवश्यक रिकॉर्ड बनाने, **OperationSet** बनाने के लिए API का उपयोग कर सकते हैं, और फिर **OperationSet** में इन पूर्व-निर्मित रिकॉर्ड का उपयोग कर सकते हैं.

## <a name="supported-operations"></a>समर्थित संचालन

| निकाय शेड्यूलिंग | निर्माण करें | अद्यतित करें | हटाएं | महत्वपूर्ण विचार |
| --- | --- | --- | --- | --- |
परियोजना कार्य | हाँ | हाँ | हाँ | कुछ नहीं |
| प्रोज़ेक्ट कार्य निर्भरता | हाँ | हाँ | | प्रोज़ेक्ट कार्य निर्भरता रिकॉर्ड अपडेट नहीं किए गए हैं. इसके बजाय, एक पुराना रिकॉर्ड हटाया जा सकता है और एक नया रिकॉर्ड बनाया जा सकता है. |
| रिसोर्स असाइनमेंट | हाँ | हाँ | | निम्नलिखित फ़ील्ड के साथ संचालन का समर्थन नहीं किया जाता है: **BookableResourceID**, **प्रयास**,**EffortCompleted**, **EffortRemaining**, और **PlannedWork**. संसाधन असाइनमेंट रिकॉर्ड अपडेट नहीं किए गए हैं. इसके बदले पुराना रिकॉर्ड डिलीट किया जा सकता है और नया रिकॉर्ड बनाया जा सकता है. |
| प्रोज़ेक्ट बकेट | लागू नहीं | लागू नहीं | लागू नहीं | डिफ़ॉल्ट बकेट **CreateProjectV1** API का उपयोग करके बनाई गई है. |
| प्रोजेक्ट टीम सदस्य | हाँ | हाँ | हाँ | बनाने के ऑपरेशन के लिए, **CreateTeamMemberV1** API का उपयोग करें. |
| Project | हाँ | हाँ | लागू नहीं | निम्नलिखित फ़ील्ड के साथ संचालन का समर्थन नहीं किया जाता है: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **प्रयास**, **EffortCompleted**, **EffortRemaining**, **प्रगति**, **समाप्त करें**, **TaskEarliestStart**, और **अवधि**. |

इन APIs को निकाय ऑब्जेक्ट्स के साथ बुलाया जा सकता है जिसमें कस्टम फ़ील्ड शामिल हैं.

ID संपत्ति वैकल्पिक है. यदि यह प्रदान किया जाता है, तो सिस्टम इसका उपयोग करने का प्रयास करता है और यदि इसका उपयोग नहीं किया जा सकता है तो अपवाद प्रदान करता है. यदि यह प्रदान नहीं किया जाता है, तो सिस्टम इसे उत्पन्न करेगा.

## <a name="restricted-fields"></a>प्रतिबंधित फील्ड

निम्न तालिका उन क्षेत्रों को परिभाषित करती है जो **बनाएं** और **संपादित करें** से प्रतिबंधित हैं.

### <a name="project-task"></a>परियोजना कार्य

| **तार्किक नाम**                       | **बना सकते हैं** | **संपादित कर सकते हैं**     |
|----------------------------------------|----------------|------------------|
| msdyn_actualcost                       | नहीं             | नहीं               |
| msdyn_actualcost_base                  | नहीं             | नहीं               |
| msdyn_actualend                        | नहीं             | नहीं               |
| msdyn_actualsales                      | नहीं             | नहीं               |
| msdyn_actualsales_base                 | नहीं             | नहीं               |
| msdyn_actualstart                      | नहीं             | नहीं               |
| msdyn_costatcompleteestimate           | नहीं             | नहीं               |
| msdyn_costatcompleteestimate_base      | नहीं             | नहीं               |
| msdyn_costconsumptionpercentage        | नहीं             | नहीं               |
| msdyn_effortcompleted                  | नहीं             | नहीं               |
| msdyn_effortestimateatcomplete         | नहीं             | नहीं               |
| msdyn_iscritical                       | नहीं             | नहीं               |
| msdyn_iscriticalname                   | नहीं             | नहीं               |
| msdyn_ismanual                         | नहीं             | नहीं               |
| msdyn_ismanualname                     | नहीं             | नहीं               |
| msdyn_ismilestone                      | नहीं             | नहीं               |
| msdyn_ismilestonename                  | नहीं             | नहीं               |
| msdyn_LinkStatus                       | नहीं             | नहीं               |
| msdyn_linkstatusname                   | नहीं             | नहीं               |
| msdyn_msprojectclientid                | नहीं             | नहीं               |
| msdyn_plannedcost                      | नहीं             | नहीं               |
| msdyn_plannedcost_base                 | नहीं             | नहीं               |
| msdyn_plannedsales                     | नहीं             | नहीं               |
| msdyn_plannedsales_base                | नहीं             | नहीं               |
| msdyn_pluginprocessingdata             | नहीं             | नहीं               |
| msdyn_progress                         | नहीं             | नही ( P4W के लिए हां) |
| msdyn_remainingcost                    | नहीं             | नहीं               |
| msdyn_remainingcost_base               | नहीं             | नहीं               |
| msdyn_remainingsales                   | नहीं             | नहीं               |
| msdyn_remainingsales_base              | नहीं             | नहीं               |
| msdyn_requestedhours                   | नहीं             | नहीं               |
| msdyn_resourcecategory                 | नहीं             | नहीं               |
| msdyn_resourcecategoryname             | नहीं             | नहीं               |
| msdyn_resourceorganizationalunitid     | नहीं             | नहीं               |
| msdyn_resourceorganizationalunitidname | नहीं             | नहीं               |
| msdyn_salesconsumptionpercentage       | नहीं             | नहीं               |
| msdyn_salesestimateatcomplete          | नहीं             | नहीं               |
| msdyn_salesestimateatcomplete_base     | नहीं             | नहीं               |
| msdyn_salesvariance                    | नहीं             | नहीं               |
| msdyn_salesvariance_base               | नहीं             | नहीं               |
| msdyn_scheduleddurationminutes         | नहीं             | नहीं               |
| msdyn_scheduledend                     | नहीं             | नहीं               |
| msdyn_scheduledstart                   | नहीं             | नहीं               |
| msdyn_schedulevariance                 | नहीं             | नहीं               |
| msdyn_skipupdateestimateline           | नहीं             | नहीं               |
| msdyn_skipupdateestimatelinename       | नहीं             | नहीं               |
| msdyn_summary                          | नहीं             | नहीं               |
| msdyn_varianceofcost                   | नहीं             | नहीं               |
| msdyn_varianceofcost_base              | नहीं             | नहीं               |

### <a name="project-task-dependency"></a>प्रोज़ेक्ट कार्य निर्भरता

| **तार्किक नाम**              | **बना सकते हैं** | **संपादित कर सकते हैं** |
|-------------------------------|----------------|--------------|
| msdyn_linktype                | नहीं             | नहीं           |
| msdyn_linktypename            | नहीं             | नहीं           |
| msdyn_predecessortask         | हाँ            | नहीं           |
| msdyn_predecessortaskname     | हाँ            | नहीं           |
| msdyn_project                 | हाँ            | नहीं           |
| msdyn_projectname             | हाँ            | नहीं           |
| msdyn_projecttaskdependencyid | हाँ            | नहीं           |
| msdyn_successortask           | हाँ            | नहीं           |
| msdyn_successortaskname       | हाँ            | नहीं           |

### <a name="resource-assignment"></a>रिसोर्स असाइनमेंट

| **तार्किक नाम**             | **बना सकते हैं** | **संपादित कर सकते हैं** |
|------------------------------|----------------|--------------|
| msdyn_bookableresourceid     | हाँ            | नहीं           |
| msdyn_bookableresourceidname | हाँ            | नहीं           |
| msdyn_bookingstatusid        | नहीं             | नहीं           |
| msdyn_bookingstatusidname    | नहीं             | नहीं           |
| msdyn_committype             | नहीं             | नहीं           |
| msdyn_committypename         | नहीं             | नहीं           |
| msdyn_effort                 | नहीं             | नहीं           |
| msdyn_effortcompleted        | नहीं             | नहीं           |
| msdyn_effortremaining        | नहीं             | नहीं           |
| msdyn_finish                 | नहीं             | नहीं           |
| msdyn_plannedcost            | नहीं             | नहीं           |
| msdyn_plannedcost_base       | नहीं             | नहीं           |
| msdyn_plannedcostcontour     | नहीं             | नहीं           |
| msdyn_plannedsales           | नहीं             | नहीं           |
| msdyn_plannedsales_base      | नहीं             | नहीं           |
| msdyn_plannedsalescontour    | नहीं             | नहीं           |
| msdyn_plannedwork            | नहीं             | नहीं           |
| msdyn_projectid              | हाँ            | नहीं           |
| msdyn_projectidname          | नहीं             | नहीं           |
| msdyn_projectteamid          | नहीं             | नहीं           |
| msdyn_projectteamidname      | नहीं             | नहीं           |
| msdyn_start                  | नहीं             | नहीं           |
| msdyn_taskid                 | नहीं             | नहीं           |
| msdyn_taskidname             | नहीं             | नहीं           |
| msdyn_userresourceid         | नहीं             | नहीं           |

### <a name="project-team-member"></a>प्रोजेक्ट टीम सदस्य

| **तार्किक नाम**                                 | **बना सकते हैं** | **संपादित कर सकते हैं** |
|--------------------------------------------------|----------------|--------------|
| msdyn_calendarid                                 | नहीं             | नहीं           |
| msdyn_creategenericteammemberwithrequirementname | नहीं             | नहीं           |
| msdyn_deletestatus                               | नहीं             | नहीं           |
| msdyn_deletestatusname                           | नहीं             | नहीं           |
| msdyn_effort                                     | नहीं             | नहीं           |
| msdyn_effortcompleted                            | नहीं             | नहीं           |
| msdyn_effortremaining                            | नहीं             | नहीं           |
| msdyn_finish                                     | नहीं             | नहीं           |
| msdyn_hardbookedhours                            | नहीं             | नहीं           |
| msdyn_hours                                      | नहीं             | नहीं           |
| msdyn_markedfordeletiontimer                     | नहीं             | नहीं           |
| msdyn_markedfordeletiontimestamp                 | नहीं             | नहीं           |
| msdyn_msprojectclientid                          | नहीं             | नहीं           |
| msdyn_percentage                                 | नहीं             | नहीं           |
| msdyn_requiredhours                              | नहीं             | नहीं           |
| msdyn_softbookedhours                            | नहीं             | नहीं           |
| msdyn_start                                      | नहीं             | नहीं           |

### <a name="project"></a>Project

| **तार्किक नाम**                       | **बना सकते हैं** | **संपादित कर सकते हैं** |
|----------------------------------------|----------------|--------------|
| msdyn_actualexpensecost                | नहीं             | नहीं           |
| msdyn_actualexpensecost_base           | नहीं             | नहीं           |
| msdyn_actuallaborcost                  | नहीं             | नहीं           |
| msdyn_actuallaborcost_base             | नहीं             | नहीं           |
| msdyn_actualsales                      | नहीं             | नहीं           |
| msdyn_actualsales_base                 | नहीं             | नहीं           |
| msdyn_contractlineproject              | हाँ            | नहीं           |
| msdyn_contractorganizationalunitid     | हाँ            | नहीं           |
| msdyn_contractorganizationalunitidname | हाँ            | नहीं           |
| msdyn_costconsumption                  | नहीं             | नहीं           |
| msdyn_costestimateatcomplete           | नहीं             | नहीं           |
| msdyn_costestimateatcomplete_base      | नहीं             | नहीं           |
| msdyn_costvariance                     | नहीं             | नहीं           |
| msdyn_costvariance_base                | नहीं             | नहीं           |
| msdyn_duration                         | नहीं             | नहीं           |
| msdyn_effort                           | नहीं             | नहीं           |
| msdyn_effortcompleted                  | नहीं             | नहीं           |
| msdyn_effortestimateatcompleteeac      | नहीं             | नहीं           |
| msdyn_effortremaining                  | नहीं             | नहीं           |
| msdyn_finish                           | हाँ            | हाँ          |
| msdyn_globalrevisiontoken              | नहीं             | नहीं           |
| msdyn_islinkedtomsprojectclient        | नहीं             | नहीं           |
| msdyn_islinkedtomsprojectclientname    | नहीं             | नहीं           |
| msdyn_linkeddocumenturl                | नहीं             | नहीं           |
| msdyn_msprojectdocument                | नहीं             | नहीं           |
| msdyn_msprojectdocumentname            | नहीं             | नहीं           |
| msdyn_plannedexpensecost               | नहीं             | नहीं           |
| msdyn_plannedexpensecost_base          | नहीं             | नहीं           |
| msdyn_plannedlaborcost                 | नहीं             | नहीं           |
| msdyn_plannedlaborcost_base            | नहीं             | नहीं           |
| msdyn_plannedsales                     | नहीं             | नहीं           |
| msdyn_plannedsales_base                | नहीं             | नहीं           |
| msdyn_progress                         | नहीं             | नहीं           |
| msdyn_remainingcost                    | नहीं             | नहीं           |
| msdyn_remainingcost_base               | नहीं             | नहीं           |
| msdyn_remainingsales                   | नहीं             | नहीं           |
| msdyn_remainingsales_base              | नहीं             | नहीं           |
| msdyn_replaylogheader                  | नहीं             | नहीं           |
| msdyn_salesconsumption                 | नहीं             | नहीं           |
| msdyn_salesestimateatcompleteeac       | नहीं             | नहीं           |
| msdyn_salesestimateatcompleteeac_base  | नहीं             | नहीं           |
| msdyn_salesvariance                    | नहीं             | नहीं           |
| msdyn_salesvariance_base               | नहीं             | नहीं           |
| msdyn_scheduleperformance              | नहीं             | नहीं           |
| msdyn_scheduleperformancename          | नहीं             | नहीं           |
| msdyn_schedulevariance                 | नहीं             | नहीं           |
| msdyn_taskearlieststart                | नहीं             | नहीं           |
| msdyn_teamsize                         | नहीं             | नहीं           |
| msdyn_teamsize_date                    | नहीं             | नहीं           |
| msdyn_teamsize_state                   | नहीं             | नहीं           |
| msdyn_totalactualcost                  | नहीं             | नहीं           |
| msdyn_totalactualcost_base             | नहीं             | नहीं           |
| msdyn_totalplannedcost                 | नहीं             | नहीं           |
| msdyn_totalplannedcost_base            | नहीं             | नहीं           |


## <a name="limitations-and-known-issues"></a>सीमाएं और ज्ञात मुद्दे
निम्नलिखित सीमाओं और ज्ञात मुद्दों की एक लिस्ट है:

- प्रोजेक्ट शेड्यूल API का उपयोग केवल **Microsoft प्रोजेक्ट लाइसेंस वाले उपयोगकर्ता** के द्वारा किया जा सकता है. उनका इनके द्वारा उपयोग नहीं किया जा सकता है:
    - अनुप्रयोग उपयोगकर्ता
    - सिस्टम उपयोगकर्ता
    - एकीकरण उपयोगकर्ता
    - अन्य उपयोगकर्ता जिनके पास आवश्यक लाइसेंस नहीं है
- प्रत्येक **OperationSet** में अधिकतम 100 संचालन हो सकते हैं.
- प्रत्येक उपयोगकर्ता के पास अधिकतम 10 खुला **OperationSets** हो सकते हैं.
- Project Operations वर्तमान में एक प्रोज़ेक्ट पर अधिकतम 500 कुल कार्यों का समर्थन करता है.
- **OperationSet** विफलता की स्थिति और विफलता लॉग वर्तमान में उपलब्ध नहीं हैं.
- [प्रोजेक्ट और कार्यों पर लिमिट और बाउंड्री](/project-for-the-web/project-for-the-web-limits-and-boundaries)

## <a name="error-handling"></a>त्रुटि हैंडलिंग

   - ऑपरेशन सेट से उत्पन्न त्रुटियों की समीक्षा करने के लिए, **सेटिंग** \> **शेड्यूल इंटीग्रेशन** \> **ऑपरेशन सेट्स** पर जाएं.
   - प्रोजेक्ट शेड्यूल सेवा से उत्पन्न त्रुटियों की समीक्षा करने के लिए, **समायोजन** \> **अनुसूची एकीकरण** \> **PSS त्रुटि लॉग** पर जाएँ.

## <a name="sample-scenario"></a>नमूना परिदृश्य

इस परिदृश्य में, आप एक प्रोज़ेक्ट, एक टीम के सदस्य, चार कार्य और दो संसाधन कार्य बनाएंगे. इसके बाद, आप एक कार्य को अपडेट करेंगे, प्रोज़ेक्ट को अपडेट करेंगे, एक कार्य को हटा देंगे, एक संसाधन असाइनमेंट को हटा देंगे,और एक कार्य निर्भरता बनाएंगे.

```csharp
Entity project = CreateProject();
project.Id = CallCreateProjectAction(project);
var projectReference = project.ToEntityReference();

var teamMember = new Entity("msdyn_projectteam", Guid.NewGuid());
teamMember["msdyn_name"] = $"TM {DateTime.Now.ToShortTimeString()}";
teamMember["msdyn_project"] = projectReference;
var createTeamMemberResponse = CallCreateTeamMemberAction(teamMember);

var description = $"My demo {DateTime.Now.ToShortTimeString()}";
var operationSetId = CallCreateOperationSetAction(project.Id, description);

var task1 = GetTask("1WW", projectReference);
var task2 = GetTask("2XX", projectReference, task1.ToEntityReference());
var task3 = GetTask("3YY", projectReference);
var task4 = GetTask("4ZZ", projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment("R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

var assignment1Response = CallPssCreateAction(assignment1, operationSetId);
var assignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

var assignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a>अतिरिक्त नमूने

```csharp
#region Call actions --- Sample code ----

/// <summary>
/// Calls the action to create an operationSet
/// </summary>
/// <param name="projectId">project id for the operations to be included in this operationSet</param>
/// <param name="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
private string CallCreateOperationSetAction(Guid projectId, string description)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_CreateOperationSetV1");
    operationSetRequest["ProjectId"] = projectId.ToString();
    operationSetRequest["Description"] = description;
    OrganizationResponse response = organizationService.Execute(operationSetRequest);
    return response["OperationSetId"].ToString();
}

/// <summary>
/// Calls the action to create an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>

private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <param name="entity">Task or Resource Assignment</param>
/// <param name="operationSetId">operationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssUpdateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssUpdateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to update an entity, only Task and Resource Assignment for now
/// </summary>
/// <param name="recordId">Id of the record to be deleted</param>
/// <param name="entityLogicalName">Entity logical name of the record</param>
/// <param name="operationSetId">OperationSet Id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssDeleteAction(string recordId, string entityLogicalName, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssDeleteV1");
    operationSetRequest["RecordId"] = recordId;
    operationSetRequest["EntityLogicalName"] = entityLogicalName;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// Calls the action to execute requests in an operationSet
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallExecuteOperationSetAction(string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_ExecuteOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary>
/// This can be used to abandon an operationSet that is no longer needed
/// </summary>
/// <param name="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
protected OperationSetResponse CallAbandonOperationSetAction(Guid operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_AbandonOperationSetV1");
    operationSetRequest["OperationSetId"] = operationSetId.ToString();
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}


/// <summary>
/// Calls the action to create a new project
/// </summary>
/// <param name="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1");
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);
    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <param name="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
private string CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject<OperationSetResponse>((string)orgResponse.Results["OperationSetResponse"]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet("msdyn_project", "msdyn_name");
    var getDefaultBucket = new QueryExpression("msdyn_projectbucket")
    {
        ColumnSet = columnsToFetch,
        Criteria =
        {
            Conditions =
            {
                new ConditionExpression("msdyn_project", ConditionOperator.Equal, projectReference.Id),
                new ConditionExpression("msdyn_name", ConditionOperator.Equal, "Bucket 1")
            }
        }
    };

    return organizationService.RetrieveMultiple(getDefaultBucket);
}

private Entity GetBucket(EntityReference projectReference)
{
    var bucketCollection = GetDefaultBucket(projectReference);
    if (bucketCollection.Entities.Count > 0)
    {
        return bucketCollection[0].ToEntity<Entity>();
    }

    throw new Exception($"Please open project with id {projectReference.Id} in the Dynamics UI and navigate to the Tasks tab");
}

private Entity CreateProject()
{
    var project = new Entity("msdyn_project", Guid.NewGuid());
    project["msdyn_subject"] = $"Proj {DateTime.Now.ToShortTimeString()}";

    return project;
}



private Entity GetTask(string name, EntityReference projectReference, EntityReference parentReference = null)
{
    var task = new Entity("msdyn_projecttask", Guid.NewGuid());
    task["msdyn_project"] = projectReference;
    task["msdyn_subject"] = name;
    task["msdyn_effort"] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
    task["new_custom1"] = "Just my test";
    task["new_age"] = 98;
    task["new_amount"] = 591.34m;
    task["new_isready"] = new OptionSetValue(100000000);
    */

    if (parentReference == null)
    {
        task["msdyn_outlinelevel"] = 1;
    }
    else
    {
        task["msdyn_parenttask"] = parentReference;
    }

    return task;
}

private Entity GetResourceAssignment(string name, Entity teamMember, Entity task, Entity project)
{
    var assignment = new Entity("msdyn_resourceassignment", Guid.NewGuid());
    assignment["msdyn_projectteamid"] = teamMember.ToEntityReference();
    assignment["msdyn_taskid"] = task.ToEntityReference();
    assignment["msdyn_projectid"] = project.ToEntityReference();
    assignment["msdyn_name"] = name;
    assignment["msdyn_start"] = DateTime.Now;
    assignment["msdyn_finish"] = DateTime.Now;

    return assignment;
}

protected Entity GetTaskDependency(Entity project, Entity predecessor, Entity successor)
{
    var taskDependency = new Entity("msdyn_projecttaskdependency", Guid.NewGuid());
    taskDependency["msdyn_project"] = project.ToEntityReference();
    taskDependency["msdyn_predecessortask"] = predecessor.ToEntityReference();
    taskDependency["msdyn_successortask"] = successor.ToEntityReference();
    taskDependency["msdyn_linktype"] = new OptionSetValue(192350000);

    return taskDependency;
}

#endregion


#region OperationSetResponse DataContract --- Sample code ----

[DataContract]
public class OperationSetResponse
{
[DataMember(Name = "operationSetId")]
public Guid OperationSetId { get; set; }

[DataMember(Name = "operationSetDetailId")]
public Guid OperationSetDetailId { get; set; }

[DataMember(Name = "operationType")]
public string OperationType { get; set; }

[DataMember(Name = "recordId")]
public string RecordId { get; set; }

[DataMember(Name = "correlationId")]
public string CorrelationId { get; set; }
}

#endregion
```
