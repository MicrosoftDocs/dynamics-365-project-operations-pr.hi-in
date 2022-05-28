---
title: शेड्यूलिंग निकायों के साथ संचालन करने के लिए प्रोजेक्ट शेड्यूल API का उपयोग करें
description: यह विषय प्रोजेक्ट शेड्यूल API का उपयोग करने के लिए जानकारी और नमूने प्रदान करता है.
author: sigitac
ms.date: 01/13/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: cabdf9716e4e25ed682368b99a87b3a3bf483cca
ms.sourcegitcommit: c0792bd65d92db25e0e8864879a19c4b93efb10c
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/14/2022
ms.locfileid: "8592050"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a>शेड्यूलिंग निकायों के साथ संचालन करने के लिए प्रोजेक्ट शेड्यूल API का उपयोग करें

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_



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

- **msdyn_CreateProjectV1**: इस API का उपयोग एक प्रोज़ेक्ट बनाने के लिए किया जा सकता है. प्रोजेक्ट और डिफ़ॉल्ट प्रोजेक्ट बकेट तुरंत बनाए जाते हैं।
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
परियोजना कार्य | हां | हां | हां | **प्रगति**, **ास पूर्ण**, और **प्रयास शेष** वेब के लिए प्रोजेक्ट में फ़ील्ड संपादित किए जा सकते हैं, लेकिन उन्हें प्रोजेक्ट ऑपरेशंस में संपादित नहीं किया जा सकता है।  |
| प्रोज़ेक्ट कार्य निर्भरता | हां |  | हां | प्रोज़ेक्ट कार्य निर्भरता रिकॉर्ड अपडेट नहीं किए गए हैं. इसके बजाय, एक पुराना रिकॉर्ड हटाया जा सकता है, और एक नया रिकॉर्ड बनाया जा सकता है। |
| रिसोर्स असाइनमेंट | हां | हां | | निम्नलिखित फ़ील्ड के साथ संचालन का समर्थन नहीं किया जाता है: **BookableResourceID**, **प्रयास**,**EffortCompleted**, **EffortRemaining**, और **PlannedWork**. संसाधन असाइनमेंट रिकॉर्ड अपडेट नहीं किए गए हैं. इसके बजाय, पुराने रिकॉर्ड को हटाया जा सकता है, और एक नया रिकॉर्ड बनाया जा सकता है। |
| प्रोज़ेक्ट बकेट | हां | हां | हां | डिफ़ॉल्ट बकेट का उपयोग करके बनाया जाता है **प्रोजेक्ट बनाएंV1** एपीआई। अद्यतन रिलीज़ 16 में प्रोजेक्ट बकेट बनाने और हटाने के लिए समर्थन जोड़ा गया था। |
| प्रोजेक्ट टीम सदस्य | हां | हां | हां | बनाने के ऑपरेशन के लिए, **CreateTeamMemberV1** API का उपयोग करें. |
| Project | हां | हां |  | निम्नलिखित फ़ील्ड के साथ संचालन का समर्थन नहीं किया जाता है: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **प्रयास**, **EffortCompleted**, **EffortRemaining**, **प्रगति**, **समाप्त करें**, **TaskEarliestStart**, और **अवधि**. |

इन APIs को निकाय ऑब्जेक्ट्स के साथ बुलाया जा सकता है जिसमें कस्टम फ़ील्ड शामिल हैं.

ID संपत्ति वैकल्पिक है. यदि यह प्रदान किया जाता है, तो सिस्टम इसका उपयोग करने का प्रयास करता है और यदि इसका उपयोग नहीं किया जा सकता है तो अपवाद प्रदान करता है. यदि यह प्रदान नहीं किया जाता है, तो सिस्टम इसे उत्पन्न करेगा.

## <a name="restricted-fields"></a>प्रतिबंधित फील्ड

निम्न तालिकाएँ उन फ़ील्ड्स को परिभाषित करती हैं जो प्रतिबंधित हैं **सृजन करना** और **संपादन करना**.

### <a name="project-task"></a>परियोजना कार्य

| तार्किक नाम                           | बना सकते हैं     | संपादित कर सकते हैं         |
|----------------------------------------|----------------|------------------|
| msdyn_actualcost                       | No             | No               |
| msdyn_actualcost_base                  | No             | No               |
| msdyn_actualend                        | No             | No               |
| msdyn_actualsales                      | No             | No               |
| msdyn_actualsales_base                 | No             | No               |
| msdyn_actualstart                      | No             | No               |
| msdyn_costatcompleteestimate           | No             | No               |
| msdyn_costatcompleteestimate_base      | No             | No               |
| msdyn_costconsumptionpercentage        | No             | No               |
| msdyn_effortcompleted                  | नहीं (हाँ परियोजना के लिए)             | नहीं (हाँ परियोजना के लिए)               |
| msdyn_effortremaining                  | नहीं (हाँ परियोजना के लिए)              | नहीं (हाँ परियोजना के लिए)                |
| msdyn_effortestimateatcomplete         | No             | No               |
| msdyn_iscritical                       | No             | No               |
| msdyn_iscriticalname                   | No             | No               |
| msdyn_ismanual                         | No             | No               |
| msdyn_ismanualname                     | No             | No               |
| msdyn_ismilestone                      | No             | No               |
| msdyn_ismilestonename                  | No             | No               |
| msdyn_LinkStatus                       | No             | No               |
| msdyn_linkstatusname                   | No             | No               |
| msdyn_msprojectclientid                | No             | No               |
| msdyn_plannedcost                      | No             | No               |
| msdyn_plannedcost_base                 | No             | No               |
| msdyn_plannedsales                     | No             | No               |
| msdyn_plannedsales_base                | No             | No               |
| msdyn_pluginprocessingdata             | No             | No               |
| msdyn_progress                         | नहीं (हाँ परियोजना के लिए)             | नहीं (हाँ परियोजना के लिए) |
| msdyn_remainingcost                    | No             | No               |
| msdyn_remainingcost_base               | No             | No               |
| msdyn_remainingsales                   | No             | No               |
| msdyn_remainingsales_base              | No             | No               |
| msdyn_requestedhours                   | No             | No               |
| msdyn_resourcecategory                 | No             | No               |
| msdyn_resourcecategoryname             | No             | No               |
| msdyn_resourceorganizationalunitid     | No             | No               |
| msdyn_resourceorganizationalunitidname | No             | No               |
| msdyn_salesconsumptionpercentage       | No             | No               |
| msdyn_salesestimateatcomplete          | No             | No               |
| msdyn_salesestimateatcomplete_base     | No             | No               |
| msdyn_salesvariance                    | No             | No               |
| msdyn_salesvariance_base               | No             | No               |
| msdyn_scheduleddurationminutes         | No             | No               |
| msdyn_scheduledend                     | No             | No               |
| msdyn_scheduledstart                   | No             | No               |
| msdyn_schedulevariance                 | No             | No               |
| msdyn_skipupdateestimateline           | No             | No               |
| msdyn_skipupdateestimatelinename       | No             | No               |
| msdyn_summary                          | No             | No               |
| msdyn_varianceofcost                   | No             | No               |
| msdyn_varianceofcost_base              | No             | No               |

### <a name="project-task-dependency"></a>प्रोज़ेक्ट कार्य निर्भरता

| तार्किक नाम                  | बना सकते हैं     | संपादित कर सकते हैं     |
|-------------------------------|----------------|--------------|
| msdyn_linktype                | No             | No           |
| msdyn_linktypename            | No             | No           |
| msdyn_predecessortask         | हां            | No           |
| msdyn_predecessortaskname     | हां            | No           |
| msdyn_project                 | हां            | No           |
| msdyn_projectname             | हां            | No           |
| msdyn_projecttaskdependencyid | हां            | No           |
| msdyn_successortask           | हां            | No           |
| msdyn_successortaskname       | हां            | No           |

### <a name="resource-assignment"></a>रिसोर्स असाइनमेंट

| तार्किक नाम                 | बना सकते हैं     | संपादित कर सकते हैं     |
|------------------------------|----------------|--------------|
| msdyn_bookableresourceid     | हां            | No           |
| msdyn_bookableresourceidname | हां            | No           |
| msdyn_bookingstatusid        | No             | No           |
| msdyn_bookingstatusidname    | No             | No           |
| msdyn_committype             | No             | No           |
| msdyn_committypename         | No             | No           |
| msdyn_effort                 | No             | No           |
| msdyn_effortcompleted        | No             | No           |
| msdyn_effortremaining        | No             | No           |
| msdyn_finish                 | No             | No           |
| msdyn_plannedcost            | No             | No           |
| msdyn_plannedcost_base       | No             | No           |
| msdyn_plannedcostcontour     | No             | No           |
| msdyn_plannedsales           | No             | No           |
| msdyn_plannedsales_base      | No             | No           |
| msdyn_plannedsalescontour    | No             | No           |
| msdyn_plannedwork            | No             | No           |
| msdyn_projectid              | हां            | No           |
| msdyn_projectidname          | No             | No           |
| msdyn_projectteamid          | No             | No           |
| msdyn_projectteamidname      | No             | No           |
| msdyn_start                  | No             | No           |
| msdyn_taskid                 | No             | No           |
| msdyn_taskidname             | No             | No           |
| msdyn_userresourceid         | No             | No           |

### <a name="project-team-member"></a>प्रोजेक्ट टीम सदस्य

| तार्किक नाम                                     | बना सकते हैं     | संपादित कर सकते हैं     |
|--------------------------------------------------|----------------|--------------|
| msdyn_calendarid                                 | No             | No           |
| msdyn_creategenericteammemberwithrequirementname | No             | No           |
| msdyn_deletestatus                               | No             | No           |
| msdyn_deletestatusname                           | No             | No           |
| msdyn_effort                                     | No             | No           |
| msdyn_effortcompleted                            | No             | No           |
| msdyn_effortremaining                            | No             | No           |
| msdyn_finish                                     | No             | No           |
| msdyn_hardbookedhours                            | No             | No           |
| msdyn_hours                                      | No             | No           |
| msdyn_markedfordeletiontimer                     | No             | No           |
| msdyn_markedfordeletiontimestamp                 | No             | No           |
| msdyn_msprojectclientid                          | No             | No           |
| msdyn_percentage                                 | No             | No           |
| msdyn_requiredhours                              | No             | No           |
| msdyn_softbookedhours                            | No             | No           |
| msdyn_start                                      | No             | No           |

### <a name="project"></a>Project

| तार्किक नाम                           | बना सकते हैं     | संपादित कर सकते हैं     |
|----------------------------------------|----------------|--------------|
| msdyn_actualexpensecost                | No             | No           |
| msdyn_actualexpensecost_base           | No             | No           |
| msdyn_actuallaborcost                  | No             | No           |
| msdyn_actuallaborcost_base             | No             | No           |
| msdyn_actualsales                      | No             | No           |
| msdyn_actualsales_base                 | No             | No           |
| msdyn_contractlineproject              | हां            | No           |
| msdyn_contractorganizationalunitid     | हां            | No           |
| msdyn_contractorganizationalunitidname | हां            | No           |
| msdyn_costconsumption                  | No             | No           |
| msdyn_costestimateatcomplete           | No             | No           |
| msdyn_costestimateatcomplete_base      | No             | No           |
| msdyn_costvariance                     | No             | No           |
| msdyn_costvariance_base                | No             | No           |
| msdyn_duration                         | No             | No           |
| msdyn_effort                           | No             | No           |
| msdyn_effortcompleted                  | No             | No           |
| msdyn_effortestimateatcompleteeac      | No             | No           |
| msdyn_effortremaining                  | No             | No           |
| msdyn_finish                           | हां            | हां          |
| msdyn_globalrevisiontoken              | No             | No           |
| msdyn_islinkedtomsprojectclient        | No             | No           |
| msdyn_islinkedtomsprojectclientname    | No             | No           |
| msdyn_linkeddocumenturl                | No             | No           |
| msdyn_msprojectdocument                | No             | No           |
| msdyn_msprojectdocumentname            | No             | No           |
| msdyn_plannedexpensecost               | No             | No           |
| msdyn_plannedexpensecost_base          | No             | No           |
| msdyn_plannedlaborcost                 | No             | No           |
| msdyn_plannedlaborcost_base            | No             | No           |
| msdyn_plannedsales                     | No             | No           |
| msdyn_plannedsales_base                | No             | No           |
| msdyn_progress                         | No             | No           |
| msdyn_remainingcost                    | No             | No           |
| msdyn_remainingcost_base               | No             | No           |
| msdyn_remainingsales                   | No             | No           |
| msdyn_remainingsales_base              | No             | No           |
| msdyn_replaylogheader                  | No             | No           |
| msdyn_salesconsumption                 | No             | No           |
| msdyn_salesestimateatcompleteeac       | No             | No           |
| msdyn_salesestimateatcompleteeac_base  | No             | No           |
| msdyn_salesvariance                    | No             | No           |
| msdyn_salesvariance_base               | No             | No           |
| msdyn_scheduleperformance              | No             | No           |
| msdyn_scheduleperformancename          | No             | No           |
| msdyn_schedulevariance                 | No             | No           |
| msdyn_taskearlieststart                | No             | No           |
| msdyn_teamsize                         | No             | No           |
| msdyn_teamsize_date                    | No             | No           |
| msdyn_teamsize_state                   | No             | No           |
| msdyn_totalactualcost                  | No             | No           |
| msdyn_totalactualcost_base             | No             | No           |
| msdyn_totalplannedcost                 | No             | No           |
| msdyn_totalplannedcost_base            | No             | No           |

### <a name="project-bucket"></a>प्रोज़ेक्ट बकेट

| तार्किक नाम          | बना सकते हैं      | संपादित कर सकते हैं     |
|-----------------------|-----------------|--------------|
| msdyn_displayorder    | हां             | No           |
| msdyn_name            | हां             | हां          |
| msdyn_project         | हां             | No           |
| msdyn_projectbucketid | हां             | No           |

## <a name="limitations-and-known-issues"></a>सीमाएं और ज्ञात मुद्दे
निम्नलिखित सीमाओं और ज्ञात मुद्दों की एक लिस्ट है:

- प्रोजेक्ट शेड्यूल API का उपयोग केवल इसके द्वारा किया जा सकता है **Microsoft प्रोजेक्ट लाइसेंस वाले उपयोगकर्ता**. उनका इनके द्वारा उपयोग नहीं किया जा सकता है:

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
