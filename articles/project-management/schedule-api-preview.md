---
title: शेड्यूलिंग निकायों के साथ संचालन करने के लिए प्रोजेक्ट शेड्यूल API का उपयोग करें
description: यह आलेख प्रोजेक्ट शेड्यूल API का उपयोग करने के लिए जानकारी और नमूने प्रदान करता है.
author: sigitac
ms.date: 01/13/2022
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 159d395efff98f2af780e5ed1e5ab3d6483cba89
ms.sourcegitcommit: b1c26ea57be721c5b0b1a33f2de0380ad102648f
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/20/2022
ms.locfileid: "9541126"
---
# <a name="use-project-schedule-apis-to-perform-operations-with-scheduling-entities"></a>शेड्यूलिंग निकायों के साथ संचालन करने के लिए प्रोजेक्ट शेड्यूल API का उपयोग करें

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_


**शेड्यूलिंग निकाय**

प्रोजेक्ट शेड्यूल API **शेड्यूलिंग निकाय** के साथ ऑपरेशन बनाने, अपडेट करने और हटाने की क्षमता प्रदान करते हैं. इन निकायों को वेब के लिए परियोजना में शेड्यूलिंग इंजन के माध्यम से प्रबंधित किया जाता है. पहले Dynamics 365 Project Operations रिलीज़ में **निकाय शेड्यूलिंग** के साथ संचालन बनाएं, अपडेट करें और मिटाएं.

निम्न तालिका प्रोजेक्ट शेड्यूल निकायों की पूरी सूची प्रदान करती है.

| **एंटिटी नाम**         | **निकाय तार्किक नाम**     |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| परियोजना कार्य            | msdyn_projecttask           |
| परियोजना कार्य निर्भरता | msdyn_projecttaskdependency |
| संसाधन असाइनमेंट     | msdyn_resourceassignment    |
| परियोजना बकेट          | msdyn_projectbucket         |
| परियोजना टीम सदस्य     | msdyn_projectteam           |
| प्रोजेक्ट चेकलिस्ट      | msdyn_projectchecklist      |
| प्रोजेक्ट लेबल           | msdyn_projectlabel          |
| लेबल करने के लिए प्रोजेक्ट कार्य   | msdyn_projecttasktolabel    |
| प्रोजेक्ट स्प्रिंट          | msdyn_projectsprint         |

**OperationSet**

OperationSet एक यूनिट-ऑफ-वर्क पैटर्न है जिसका उपयोग तब किया जा सकता है जब शेड्यूल प्रभावित करने वाले कई अनुरोधों को लेनदेन के भीतर संसाधित किया जाना चाहिए.

**प्रोजेक्ट शेड्यूल API**

निम्नलिखित वर्तमान प्रोजेक्ट शेड्यूल API की सूची है.

| **API**                                 | विवरण                                                                                                                       |
|-----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| **msdyn_CreateProjectV1**               | इस API का उपयोग प्रोजेक्ट बनाने के लिए किया जाता है. प्रोज़ेक्ट और डिफॉल्ट प्रोज़ेक्ट बकेट तुरंत बनाए जाते हैं.                         |
| **msdyn_CreateTeamMemberV1**            | इस API का उपयोग टीम के सदस्य बनाने के लिए किया जाता है. टीम के सदस्य का रिकार्ड तुरंत बनाया जाता है.                                  |
| **msdyn_CreateOperationSetV1**          | इस API का उपयोग ऐसे कई अनुरोधों को शेड्यूल करने के लिए किया जा सकता है, जिन्हें लेनदेन के भीतर किया जाना चाहिए.                                        |
| **msdyn_PssCreateV1**                   | इस API का उपयोग एक निकाय बनाने के लिए किया जाता है. निकाय कोई भी प्रोजेक्ट शेड्यूलिंग निकाय हो सकता है, जो निर्माण कार्य का समर्थन करता है. |
| **msdyn_PssUpdateV1**                   | इस API का उपयोग एक निकाय अद्यतन करने के लिए किया जाता है. निकाय कोई भी प्रोजेक्ट शेड्यूलिंग निकाय हो सकता है, जो अद्यतन संचालन का समर्थन करता है  |
| **msdyn_PssDeleteV1**                   | इस API का उपयोग एक निकाय हटाने के लिए किया जाता है. निकाय कोई भी प्रोजेक्ट शेड्यूलिंग निकाय हो सकता है, जो हटाने के कार्य का समर्थन करता है. |
| **msdyn_ExecuteOperationSetV1**         | इस API का उपयोग दिए गए ऑपरेशन सेट के भीतर सभी ऑपरेशन को निष्पादित करने के लिए किया जाता है.                                                 |
| **msdyn_PssUpdateResourceAssignmentV1** | इस API का उपयोग संसाधन असाइनमेंट नियोजित कार्य रूपरेखा को अद्यतन करने के लिए किया जाता है.                                                        |



**ऑपरेशनसेट के साथ प्रोजेक्ट शेड्यूल API का उपयोग करना**

क्योंकि दोनों के साथ रिकॉर्ड **CreateProjectV1** और **CreateTeamMemberV1** तुरंत बनाए जाते हैं, इन APIs का उपयोग सीधे **OperationSet** में नहीं किया जा सकता है. हालांकि, आप आवश्यक रिकॉर्ड बनाने, **OperationSet** बनाने के लिए API का उपयोग कर सकते हैं, और फिर **OperationSet** में इन पूर्व-निर्मित रिकॉर्ड का उपयोग कर सकते हैं.

**समर्थित संचालन**

| **निकाय शेड्यूलिंग**   | **निर्माण करें** | **अद्यतित करें** | **हटाएं** | **महत्वपूर्ण विचार**                                                                                                                                                                                                                                                                                                                            |
|-------------------------|------------|------------|------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| परियोजना कार्य            | हां        | हां        | हां        | **प्रगति**, **EffortCompleted** तथा **EffortRemaining** फ़ील्ड को Project for the Web में संपादित किया जा सकता है, लेकिन उन्हें Project Operations में संपादित नहीं किया जा सकता.                                                                                                                                                                                             |
| प्रोज़ेक्ट कार्य निर्भरता | हां        | No         | हां        | प्रोज़ेक्ट कार्य निर्भरता रिकॉर्ड अपडेट नहीं किए गए हैं. इसके बजाय, एक पुराना रिकॉर्ड हटाया जा सकता है और एक नया रिकॉर्ड बनाया जा सकता है.                                                                                                                                                                                                                                 |
| रिसोर्स असाइनमेंट     | हां        | हां\*      | हां        | निम्नलिखित फ़ील्ड के साथ संचालन का समर्थन नहीं किया जाता है: **BookableResourceID**, **प्रयास**,**EffortCompleted**, **EffortRemaining**, और **PlannedWork**. संसाधन असाइनमेंट रिकॉर्ड अपडेट नहीं किए गए हैं. इसके बदले पुराना रिकॉर्ड डिलीट किया जा सकता है और नया रिकॉर्ड बनाया जा सकता है. संसाधन असाइनमेंट की रूपरेखा को अद्यतन करने के लिए एक अलग API प्रदान किया गया है. |
| प्रोज़ेक्ट बकेट          | हां        | हां        | हां        | डिफ़ॉल्ट बकेट **CreateProjectV1** API का उपयोग करके बनाई जाती है. अद्यतन रिलीज़ 16 में प्रोजेक्ट बकेट बनाने और हटाने के लिए सहायता जोड़ी गई थी.                                                                                                                                                                                                   |
| प्रोजेक्ट टीम सदस्य     | हां        | हां        | हां        | बनाने के ऑपरेशन के लिए, **CreateTeamMemberV1** API का उपयोग करें.                                                                                                                                                                                                                                                                                           |
| Project                 | हां        | हां        |            | निम्नलिखित फ़ील्ड के साथ संचालन का समर्थन नहीं किया जाता है: **StateCode**, **BulkGenerationStatus**, **GlobalRevisionToken**, **CalendarID**, **प्रयास**, **EffortCompleted**, **EffortRemaining**, **प्रगति**, **समाप्त करें**, **TaskEarliestStart**, और **अवधि**.                                                                                       |
| प्रोजेक्ट चेकलिस्ट      | हां        | हां        | हां        |                                                                                                                                                                                                                                                                                                                                                         |
| प्रोजेक्ट लेबल           | No         | हां        | No         | लेबल के नाम बदले जा सकते हैं. यह सुविधा केवल Project for the Web में ही उपलब्ध है                                                                                                                                                                                                                                                                      |
| लेबल करने के लिए प्रोजेक्ट कार्य   | हां        | No         | हां        | यह सुविधा केवल Project for the Web में ही उपलब्ध है                                                                                                                                                                                                                                                                                                  |
| प्रोजेक्ट स्प्रिंट          | हां        | हां        | हां        | **प्रारंभ करें** फ़ील्ड में **खत्म करें** फ़ील्ड से पहले एक तिथि होनी चाहिए. एक ही प्रोजेक्ट के लिए स्प्रिंट एक दूसरे के साथ ओवरलैप नहीं हो सकते. यह सुविधा केवल Project for the Web में ही उपलब्ध है                                                                                                                                                                    |




ID संपत्ति वैकल्पिक है. यदि यह प्रदान किया जाता है, तो सिस्टम इसका उपयोग करने का प्रयास करता है और यदि इसका उपयोग नहीं किया जा सकता है तो अपवाद प्रदान करता है. यदि यह प्रदान नहीं किया जाता है, तो सिस्टम इसे उत्पन्न करेगा.

**सीमाएं और ज्ञात मुद्दे**

निम्नलिखित सीमाओं और ज्ञात मुद्दों की एक लिस्ट है:

-   प्रोजेक्ट शेड्यूल API का उपयोग केवल **Microsoft Project लाइसेंस** वाले उपयोगकर्ताओं द्वारा किया जा सकता है. उनका इनके द्वारा उपयोग नहीं किया जा सकता है:
    -   अनुप्रयोग उपयोगकर्ता
    -   सिस्टम उपयोगकर्ता
    -   एकीकरण उपयोगकर्ता
    -   अन्य उपयोगकर्ता जिनके पास आवश्यक लाइसेंस नहीं है
-   प्रत्येक **OperationSet** में अधिकतम 100 संचालन हो सकते हैं.
-   प्रत्येक उपयोगकर्ता के पास अधिकतम 10 खुला **OperationSets** हो सकते हैं.
-   Project Operations वर्तमान में एक प्रोज़ेक्ट पर अधिकतम 500 कुल कार्यों का समर्थन करता है.
-   प्रत्येक अद्यतन संसाधन असाइनमेंट रूपरेखा ऑपरेशन को एकल ऑपरेशन के रूप में गिना जाता है.
-   अद्यतन रूपरेखाओं की प्रत्येक सूची में अधिकतम 100 समय खंड हो सकते हैं.
-   **OperationSet** विफलता की स्थिति और विफलता लॉग वर्तमान में उपलब्ध नहीं हैं.
-   प्रति प्रोजेक्ट अधिकतम 400 स्प्रिंट है.
-   [प्रोजेक्ट और कार्यों पर सीमाएं और बाउंड्री](/project-for-the-web/project-for-the-web-limits-and-boundaries).
-   लेबल फिलहाल केवल Project for the Web के लिए ही उपलब्ध है.

**त्रुटि हैंडलिंग**

-   ऑपरेशन सेट से उत्पन्न त्रुटियों की समीक्षा करने के लिए, **सेटिंग** \> **शेड्यूल इंटीग्रेशन** \> **ऑपरेशन सेट्स** पर जाएं.
-   प्रोजेक्ट शेड्यूल सेवा से उत्पन्न त्रुटियों की समीक्षा करने के लिए, **समायोजन** \> **अनुसूची एकीकरण** \> **PSS त्रुटि लॉग** पर जाएँ.

**संसाधन असाइनमेंट रूपरेखाएँ संपादित करना**

किसी निकाय को अद्यतन करने वाले अन्य सभी प्रोजेक्ट शेड्यूलिंग API के विपरीत, संसाधन असाइनमेंट रूपरेखा API एकल फ़ील्ड, msdyn_plannedwork, एकल निकाय, msydn_resourceassignment के अद्यतन के लिए पूरी तरह से ज़िम्मेदार है.

दिया गया शेड्यूल मोड है:

-   **निश्चित इकाइयाँ**
-   प्रोजेक्ट कैलेंडर 9-5p है 9-5pst, सोम, मंगल, गुरुवार, शुक्रवार (कोई कार्य वाले बुधवार नहीं)
-   और संसाधन कैलेंडर 9-1p PST सोम से शुक्र तक है

यह असाइनमेंट एक सप्ताह, चार घंटे एक दिन के लिए है. ऐसा इसलिए है क्योंकि संसाधन कैलेंडर 9-1 PST से या दिन में चार घंटे है.

| &nbsp;     | कार्य | प्रारंभ दिनांक | समाप्ति तिथि  | मात्रा | 6/13/2022 | 6/14/2022 | 6/15/2022 | 6/16/2022 | 6/17/2022 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| 9-1 कर्मचारी |  T1  | 6/13/2022  | 6/17/2022 | 20       | 4         | 4         | 4         | 4         | 4         |

उदाहरण के लिए, यदि आप चाहते हैं कि कर्मचारी इस सप्ताह प्रत्येक दिन केवल तीन घंटे काम करे और अन्य कार्यों के लिए एक घंटे का समय दे.

#### <a name="updatedcontours-sample-payload"></a>UpdatedContours नमूना पेलोड:

```json
[{

"minutes":900.0,

"start":"2022-06-13T00:00:00-07:00",

"end":"2022-06-18T00:00:00-07:00"

}]
```

यह असाइनमेंट अद्यतन रूपरेखा शेड्यूल API चलाने के बाद का है.

| &nbsp;     | कार्य | प्रारंभ दिनांक | समाप्ति तिथि  | मात्रा | 6/13/2022 | 6/14/2022 | 6/15/2022 | 6/16/2022 | 6/17/2022 |
|------------|------|------------|-----------|----------|-----------|-----------|-----------|-----------|-----------|
| 9-1 कर्मचारी | T1   | 6/13/2022  | 6/17/2022 | 15       | 3         | 3         | 3         | 3         | 3         |


**नमूना परिदृश्य**

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

** अतिरिक्त नमूने

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
