---
title: निकाय शेड्यूलिंग के साथ संचालन करने के लिए शेड्यूल APIs का उपयोग करें
description: यह विषय अनुसूची APIs का उपयोग करने के लिए जानकारी और नमूने प्रदान करता है.
author: sigitac
manager: Annbe
ms.date: 04/07/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a50a2c6220bb49de8146d0758019827e120e0526
ms.sourcegitcommit: 8ff9fe396db6dec581c21cd6bb9acc2691c815b0
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/07/2021
ms.locfileid: "5868131"
---
# <a name="use-schedule-apis-to-perform-operations-with-scheduling-entities"></a>निकाय शेड्यूलिंग के साथ संचालन करने के लिए शेड्यूल APIs का उपयोग करें

_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_

> [!IMPORTANT] 
> इस विषय में नोट की गई कुछ या सभी कार्यक्षमता पूर्वावलोकन रिलीज के हिस्से के रूप में उपलब्ध है. सामग्री और कार्यक्षमता परिवर्तन के अधीन हैं. 

## <a name="scheduling-entities"></a>शेड्यूलिंग निकाय

शेड्यूल APIs **निकाय शेड्यूलिंग** के साथ निर्माण, अपडेट और हटाने के संचालन को करने की क्षमता प्रदान करता है. इन निकायों को वेब के लिए परियोजना में शेड्यूलिंग इंजन के माध्यम से प्रबंधित किया जाता है. पहले Dynamics 365 Project Operations रिलीज़ में **निकाय शेड्यूलिंग** के साथ संचालन बनाएं, अपडेट करें और मिटाएं.

निम्नलिखित तालिका **निकाय शेड्यूलिंग** की पूरी लिस्ट प्रदान करती है.

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

## <a name="schedule-apis"></a>APIs शेड्यूल करें

यह वर्तमान शेड्यूल APIs की लिस्ट है.

- **msdyn_CreateProjectV1**: इस API का उपयोग एक प्रोज़ेक्ट बनाने के लिए किया जा सकता है. प्रोज़ेक्ट और डिफॉल्ट प्रोज़ेक्ट बकेट तुरंत बनाया जाता है.
- **msdyn_CreateTeamMemberV1**: इस API का उपयोग प्रोज़ेक्ट टीम के सदस्य बनाने के लिए किया जा सकता है. टीम के सदस्य का रिकार्ड तुरंत बनाया जाता है.
- **msdyn_CreateOperationSetV1**: इस एपीआई का उपयोग कई अनुरोधों को शेड्यूल करने के लिए किया जा सकता है जिन्हें लेनदेन के भीतर किया जाना चाहिए.
- **msdyn_PSSCreateV1**: इस एपीआई का उपयोग एक निकाय बनाने के लिए किया जा सकता है. निकाय शेड्यूलिंग संस्थाओं में से कोई भी हो सकता है जो निर्माण ऑपरेशन का समर्थन करता है.
- **msdyn_PSSCreateV1**: इस API का उपयोग एक निकाय अपडेट के लिए किया जा सकता है. निकाय शेड्यूलिंग संस्थाओं में से कोई भी हो सकता है जो अपडेट ऑपरेशन का समर्थन करता है.
- **msdyn_PSSDeleteV1**: इस API को हटाने के लिए एक निकाय इस्तेमाल किया जा सकता है. निकाय शेड्यूलिंग संस्थाओं में से कोई भी हो सकता है जो डिलीट ऑपरेशन का समर्थन करता है.
- **msdyn_ExecuteOperationSetV1**: इस एपीआई का उपयोग दिए गए ऑपरेशन सेट के भीतर सभी संचालनों को निष्पादित करने के लिए किया जाता है.

## <a name="using-schedule-apis-with-operationset"></a>OperationSet के साथ शेड्यूल APIs का उपयोग करना

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

## <a name="limitations-and-known-issues"></a>सीमाएं और ज्ञात मुद्दे
निम्नलिखित सीमाओं और ज्ञात मुद्दों की एक लिस्ट है:

- शेड्यूल एपीआई का उपयोग केवल **Microsoft प्रोज़ेक्ट लाइसेंस वाले** उपयोगकर्ताओं द्वारा किया जा सकता है. उनका इनके द्वारा उपयोग नहीं किया जा सकता है:
    - अनुप्रयोग उपयोगकर्ता
    - सिस्टम उपयोगकर्ता
    - एकीकरण उपयोगकर्ता
    - अन्य उपयोगकर्ता जिनके पास आवश्यक लाइसेंस नहीं है
- प्रत्येक **OperationSet** में अधिकतम 100 संचालन हो सकते हैं.
- प्रत्येक उपयोगकर्ता के पास अधिकतम 10 खुला **OperationSets** हो सकते हैं.
- Project Operations वर्तमान में एक प्रोज़ेक्ट पर अधिकतम 500 कुल कार्यों का समर्थन करता है.
- **OperationSet** विफलता की स्थिति और विफलता लॉग वर्तमान में उपलब्ध नहीं हैं.
- शेड्यूल एपीआई सार्वजनिक पूर्वावलोकन में हैं. उत्पादन परिवेश में इन एपीआई का उपयोग करना Microsoft द्वारा समर्थित नहीं है.

## <a name="sample-scenario"></a>नमूना परिदृश्य

इस परिदृश्य में, आप एक प्रोज़ेक्ट, एक टीम के सदस्य, चार कार्य और दो संसाधन कार्य बनाएंगे. इसके बाद, आप एक कार्य को अपडेट करेंगे, प्रोज़ेक्ट को अपडेट करेंगे, एक कार्य को हटा देंगे, एक संसाधन असाइनमेंट को हटा देंगे,और एक कार्य निर्भरता बनाएंगे.

```C#
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
var task4 = GetTask("4ZZ";, projectReference);

var assignment1 = GetResourceAssignment("R1", teamMember, task2, project);
var assignment2 = GetResourceAssignment"R2", teamMember, task3, project);

var task1Response = CallPssCreateAction(task1, operationSetId);
var task2Response = CallPssCreateAction(task2, operationSetId);
var task3Response = CallPssCreateAction(task3, operationSetId);
var task4Response = CallPssCreateAction(task4, operationSetId);

varassignment1Response = CallPssCreateAction(assignment1, operationSetId);
varassignment2Response = CallPssCreateAction(assignment2, operationSetId);

task2["msdyn_subject"] = "Updated Task";
var task2UpdateResponse = CallPssUpdateAction(task2, operationSetId);

project["msdyn_subject"] = $"Proj update {DateTime.Now.ToShortTimeString()}";
var projectUpdateResponse = CallPssUpdateAction(project, operationSetId);

var task4DeleteResponse = CallPssDeleteAction(task4.Id.ToString(), task4.LogicalName, operationSetId);

varassignment2DeleteResponse = CallPssDeleteAction(assignment2.Id.ToString(), assignment2.LogicalName, operationSetId);

var dependency1 = GetTaskDependency(project, task2, task3);
var dependency1Response = CallPssCreateAction(dependency1, operationSetId);

CallExecuteOperationSetAction(operationSetId);
Console.WriteLine("Done....");
```

## <a name="additional-samples"></a>अतिरिक्त नमूने

```C#
#region Call actions 

///<summary>
/// Calls the action to create an operationSet
/// </summary>
/// <paramname="projectId">project id for the operations to be included in this operationSet>/param>
/// <paramname="description">description of this operationSet</param>
/// <returns>operationSet id</returns>
privatestring CallCreateOperationSetAction(Guid projectId, string description)
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
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet id</param>
/// <returns>OperationSetResponse</returns>
private OperationSetResponse CallPssCreateAction(Entity entity, string operationSetId)
{
    OrganizationRequest operationSetRequest = new OrganizationRequest("msdyn_PssCreateV1");
    operationSetRequest["Entity"] = entity;
    operationSetRequest["OperationSetId"] = operationSetId;
    return GetOperationSetResponseFromOrgResponse(organizationService.Execute(operationSetRequest));
}

/// <summary<
/// Calls the action to update an entity, only Task for now
/// </summary>
/// <paramname="entity">Task or Resource Assignment</param>
/// <paramname="operationSetId">operationSet Id</param>
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
/// <summary>
/// <paramname="recordId">Id of the record to be deleted</param>
/// <paramname="entityLogicalName">Entity logical name of the record</param>
/// <paramname="operationSetId">OperationSet Id</param>
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
/// <summary>
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="operationSetId">operationSet id</param>
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
/// <paramname="project">Project</param>
/// <returns>project Id</returns>
private Guid CallCreateProjectAction(Entity project)
{
    OrganizationRequest createProjectRequest = new OrganizationRequest("msdyn_CreateProjectV1";
    createProjectRequest["Project"] = project;
    OrganizationResponse response = organizationService.Execute(createProjectRequest);
    var projectId = Guid.Parse((string)response["ProjectId"]);

    return projectId;
}

/// <summary>
/// Calls the action to create a new project team member
/// </summary>
/// <paramname="teamMember">Project team member</param>
/// <returns>project team member Id</returns>
privatestring CallCreateTeamMemberAction(Entity teamMember)
{
    OrganizationRequest request = new OrganizationRequest("msdyn_CreateTeamMemberV1");
    request["TeamMember"] = teamMember;
    OrganizationResponse response = organizationService.Execute(request);
    return (string)response["TeamMemberId"];
}

private OperationSetResponse GetOperationSetResponseFromOrgResponse(OrganizationResponse orgResponse)
{
    return JsonConvert.DeserializeObject><OperationSetResponse>
    ((string)orgResponse.Results["OperationSetResponse";]);
}

private EntityCollection GetDefaultBucket(EntityReference projectReference)
{
    var columnsToFetch = new ColumnSet(";msdyn_project", "msdyn_name");
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
    task["msdyn_effort";] = 4d;
    task["msdyn_scheduledstart"] = DateTime.Today;
    task["msdyn_scheduledend"] = DateTime.Today.AddDays(5);
    task["msdyn_progress"] = 0.34m;
    task["msdyn_start"] = DateTime.Now.AddDays(1);
    task["msdyn_projectbucket"] = GetBucket(projectReference).ToEntityReference();
    task["msdyn_LinkStatus"] = new OptionSetValue(192350000);

    //Custom field handling
    /*
        task["new_custom1"] = "Just my test";
        task[";new_age"] = 98;
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
publicclassOperationSetResponse
{
    [DataMember(Name = "operationSetId")]
    public Guid OperationSetId { get; set; }

    [DataMember(Name = "operationSetDetailId")]
    public Guid OperationSetDetailId { get; set; }

    [DataMember(Name = "operationType")]
    publicstring OperationType { get; set; }

    [DataMember(Name = "recordId")]
    publicstring RecordId { get; set; }

    [DataMember(Name = "correlationId")]
    publicstring CorrelationId { get; set; }
}

#endregion
```
