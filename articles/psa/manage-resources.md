---
title: संसाधनों का प्रबंधन करें
description: यह विषय संसाधनों को व्यवस्थित करने की जानकारी देता है।
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 05/13/2019
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
ms.openlocfilehash: 5b34ad66750dba9459d551a2527c13111196511e
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077901"
---
# <a name="manage-resources"></a><span data-ttu-id="e266a-103">संसाधनों का प्रबंधन करें</span><span class="sxs-lookup"><span data-stu-id="e266a-103">Manage resources</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="e266a-104">Dynamics 365 Project Service Automation में एक रिसोर्स मैनेजर डैशबोर्ड होता है जो रिसोर्स की मांग और पूरे संगठन में उसकी उपयोगिता की दृश्यगत जानकारी प्रदान करता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-104">Dynamics 365 Project Service Automation includes a resource manager dashboard that provides a visual overview of resource demand and utilization throughout the organization.</span></span> <span data-ttu-id="e266a-105">आप निम्नलिखित जानकारी देखने के लिए इस डैशबोर्ड पर दिए गए चार्ट का इस्तेमाल कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="e266a-105">You can use the charts on this dashboard to visualize the following information:</span></span>

- <span data-ttu-id="e266a-106">**रिसोर्स डिमांड** – **एक्टिव रिसोर्स रिक्वेस्ट** चार्ट उन संसाधनों को दिखाता है जिन्हें सबमिट किया गया है।</span><span class="sxs-lookup"><span data-stu-id="e266a-106">**Resource demand** – The **Active Resource Request** chart shows resources that have been submitted.</span></span> <span data-ttu-id="e266a-107">इन संसाधनों को भूमिका या प्रोजेक्ट द्वारा इकट्ठा किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-107">The resources are aggregated by either role or project.</span></span>
- <span data-ttu-id="e266a-108">**सबमिट नहीं किया गया संसाधन डिमांड** – **असाइन नहीं किया गया संसाधन डिमांड** चार्ट उन सभी संसाधन आवश्यकताओं को दर्शाता है जिन्हें सबमिट नहीं किया गया है।</span><span class="sxs-lookup"><span data-stu-id="e266a-108">**Unsubmitted resource demand** – The **Unassigned Resource Demand** chart shows all the resource requirements that haven't been submitted.</span></span> <span data-ttu-id="e266a-109">इससे रिसोर्ट मैनेजर ऐसी मांग को देख सकते हैं जो स्थिर नहीं है और जिन्हें रिसोर्स रिक्वेस्ट द्वारा सबमिट किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-109">It helps resource managers view demand that isn't firm and might be submitted through a resource request.</span></span>
- <span data-ttu-id="e266a-110">**पिछले सप्ताह की बिल योग्य उपयोगिता** – **भूमिका द्वारा उपयोगिता** चार्ट भूमिका द्वारा बिल योग्य उपयोगिता के लक्ष्य के समक्ष भूमिका द्वारा संगठन की वास्तविक बिल योग्य उपयोगिता का प्रतिशत दर्शाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-110">**Billable utilization for the past week** – The **Utilization by Role** chart shows the percentage of the organization's actual billable utilization by role against its target billable utilization by role.</span></span>

    > [!NOTE]
    > <span data-ttu-id="e266a-111">**भूमिका द्वारा उपयोगिता** चार्ट उपलब्ध कराने के लिए, ऐसा जॉब तैयार करें जो अपडेट रोल यूटिलाइज़ेशन वर्कफ्लो चलाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-111">To make the **Utilization by Role** chart available, create a job that runs the UpdateRoleUtilization workflow.</span></span> <span data-ttu-id="e266a-112">यह आवर्ती जॉब पिछले सात दिनों के बिल योग्य उपयोगिता का परिकलन करने के लिए प्रत्येक सात दिन चलाया जाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-112">This recurring job runs every seven days to calculate billable utilization for the previous seven days.</span></span> <span data-ttu-id="e266a-113">परिणाम भूमिका द्वारा इकट्ठे किए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-113">The results are aggregated by role.</span></span>

## <a name="manage-project-team-members"></a><span data-ttu-id="e266a-114">परियोजना टीम के सदस्यों का प्रबंध करना।</span><span class="sxs-lookup"><span data-stu-id="e266a-114">Manage project team members</span></span>

<span data-ttu-id="e266a-115">प्रोजेक्ट मैनेजर प्रोजेक्ट में संसाधनों का प्रबंध करने के लिए रिसोर्स मैनेजरों के डैशबोर्ड का इस्तेमाल कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-115">Project managers can use the resource manager dashboard to manage the resources on projects.</span></span> <span data-ttu-id="e266a-116">उदाहरण के लिए, वे किसी प्रोजेक्ट में टीम के सदस्य को सीधे शामिल कर सकते हैं या टीम के सदस्य को सामान्य रिसोर्स द्वारा बताई गई आवश्यकताओं को पूरा करने के लिए कह सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-116">For example, they can add a team member directly to a project and book a team member to fulfill the resource requirements that were captured by a generic resource.</span></span>

### <a name="add-a-team-member-directly-to-a-project"></a><span data-ttu-id="e266a-117">किसी प्रोजेक्ट में टीम के सदस्य को सीधे शामिल करना</span><span class="sxs-lookup"><span data-stu-id="e266a-117">Add a team member directly to a project</span></span>

<span data-ttu-id="e266a-118">किसी प्रोजेक्ट में टीम के सदस्य को सीधे शामिल करने के लिए, **प्रोजेक्ट** पेज पर, **टीम** टैब पर, **न्यू** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-118">To add a team member directly to a project, on the **Projects** page, on the **Team** tab, select **New**.</span></span> <span data-ttu-id="e266a-119">**क्विक क्रिएट: प्रोजेक्ट टीम मेम्बर** डॉयलॉग बॉक्स दिखेगा।</span><span class="sxs-lookup"><span data-stu-id="e266a-119">The **Quick Create:Project Team Member** dialog box appears.</span></span> <span data-ttu-id="e266a-120">इस डॉयलॉग बॉक्स में, आप निम्नलिखित काम कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="e266a-120">In this dialog box, you can perform these tasks:</span></span>

- <span data-ttu-id="e266a-121">**नामित रिसोर्स को बुक करें** – **बुक करने योग्य रिसोर्स** फील्ड में, रिसोर्स का नाम चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-121">**Book a named resource** – In the **Bookable Resource** field, select the name of the resource.</span></span> <span data-ttu-id="e266a-122">इसके बाद भूमिका चुनें, अवधि तयक रें और आबंटन की विधि चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-122">Then select the role, set the period, and select an allocation method.</span></span> <span data-ttu-id="e266a-123">आपके द्वारा चयनित नामित रिसोर्स को चयनित आबंटन विधि और रिसोर्स कैलेंडर का उपयोग करते हुए प्रोजेक्ट में शामिल किया जाएगा।</span><span class="sxs-lookup"><span data-stu-id="e266a-123">The named resource that you selected is added to the project by using the selected allocation method and the resources calendar.</span></span>
- <span data-ttu-id="e266a-124">**सामान्य रिसोर्स जोड़ें** – **बुक करने योग्य रिसोर्स** फील्ड को खाली छोड़ें, उसके बाद भूमिका चुनें, अवधि तय करें और वरीय आबंटन विधि चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-124">**Add a generic resource** – Leave the **Bookable resource** field blank, and then select the role, set the period, and select the preferred allocation method.</span></span> <span data-ttu-id="e266a-125">टीम में नामित रिसोर्स बुक करने में प्रयुक्त मांग पैटर्न धारित करने के लिए प्लेसहोल्डर के रूप में टीम में एक सामान्य रिसोर्स जोड़ दिया जाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-125">A generic resource is added to the team as a placeholder to hold the demand pattern that is used to book named resources on the team.</span></span> <span data-ttu-id="e266a-126">प्रोजेक्ट कैलेंडर के अनुसार आवश्यकता बताई जाती है।</span><span class="sxs-lookup"><span data-stu-id="e266a-126">The requirement is made according to the project calendar.</span></span>
- <span data-ttu-id="e266a-127">**रिसोर्स की क्षमता का उपयोग किए बिना टीम में नामित रिसोर्स जोड़ना** – **बुक करने योग्य रिसोर्स** फील्ड में, रिसोर्स चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-127">**Add a named resource to the team without consuming resource capacity** – In the **Bookable Resource** field, select a resource.</span></span> <span data-ttu-id="e266a-128">इसके बाद अवधि चुनें, आबंटित विधि के रूप में **कोई नहीं** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-128">Then select the period, and select **None** as the allocation method.</span></span> <span data-ttu-id="e266a-129">टीम में रिसोर्स जोड़ दिया जाता है लेकिन बुकिंग द्वारा रिसोर्स की क्षमता का उपयोग नहीं किया जाता।</span><span class="sxs-lookup"><span data-stu-id="e266a-129">The resource is added to the team, but the resource's capacity isn't consumed through a booking.</span></span>

### <a name="book-a-team-member-to-fulfill-resource-requirements-for-a-generic-resource"></a><span data-ttu-id="e266a-130">सामान्य रिसोर्स की आवश्यकताओं को पूरा करने के लिए टीम सदस्य को बुक करना।</span><span class="sxs-lookup"><span data-stu-id="e266a-130">Book a team member to fulfill resource requirements for a generic resource</span></span>

<span data-ttu-id="e266a-131">PSA में, आप एक परियोजना टीम में सामान्य रिसोर्स को बुक कर सकते हैं और उसकी भूमिका, अपेक्षित क्षमता और उस क्षमता का वितरण कैसे किया जाए, तय कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-131">In PSA, you can book a generic resource on a project team, and can specify the role, the required capacity, and how that capacity is distributed.</span></span> <span data-ttu-id="e266a-132">संसाधन की आवश्यकता में, आप उन गुणों को बता सकते हैं जो उस सामान्य संसाधन से संबंधित हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-132">On the resource requirement, you can specify attributes that are associated with the generic resource.</span></span> <span data-ttu-id="e266a-133">इन गुणों में कौशल, वरीय संगठन की यूनिट और वरीय रिसोर्स शामिल होते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-133">These attributes include required skills, the preferred organizational unit, and preferred resources.</span></span>

<span data-ttu-id="e266a-134">डेवलपर के लिए सामान्य रिसोर्स पर अपेक्षित कौशल बताने के लिए इन कदमों का पालन करें।</span><span class="sxs-lookup"><span data-stu-id="e266a-134">Follow these steps to specify required skills on a generic resource for a developer.</span></span>

1. <span data-ttu-id="e266a-135">**प्रोजेक्ट्स** पेज में, **टीम** टैब पर, एक सामान्य रिसोर्स बुक करने के लिए **न्यू** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-135">On the **Projects** page, on the **Team** tab, select **New** to book a generic resource.</span></span>

    ![टीम में बुक किया गया सामान्य रिसोर्स](media/Resource-Management-image9.png)

2. <span data-ttu-id="e266a-137">**ऑल टीम मेम्बर्स** व्यू में, **रिसोर्स रिक्वायरमेंट** कॉलम में, सामान्य रिसोर्स के लिए आवश्यक कौशल जोड़ने के लिए लिंक चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-137">In the **All Team Members** view, in the **Resource Requirement** column, select the link to add required skills for the generic resource.</span></span>

    ![आवश्यकता लिंक](media/Resource-Management-image10.png)

3. <span data-ttu-id="e266a-139">दिखने वाले **रिसोर्स रिक्वायरमेंट** पेज में, **स्किल्स** ग्रिड में, एल्लिप्सिस ( **...** ) चुनें और उसके बाद, अपने डेवलपर के लिए आवश्यक कौशल जोड़ने के लिए **एड न्यू रिक्वायरमेंट कैरेक्टरिस्टिक** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-139">On the **Resource Requirement** page that appears, in the **Skills** grid, select the ellipsis ( **...** ) and then select **Add New Requirement Characteristic** to add the required skills for your developer.</span></span>

    ![एड न्यू रिक्वायरमेंट कैरेक्टरिस्टिक कमांड जोड़ना](media/Resource-Management-image11.png)

4. <span data-ttu-id="e266a-141">दिखने वाले **क्विक व्यू: रिक्वायरमेंट कैरेक्टरिस्टिक** डॉयलॉग बॉक्स में, **कैरेक्टरिस्टिक** फील्ड में, आवश्यक कौशल चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-141">In the **Quick Create: Requirement Characteristic** dialog box that appears, in the **Characteristic** field, select the required skill.</span></span> <span data-ttu-id="e266a-142">इसके बाद, **रेटिंग वैल्यू** फील्ड में, उस कौशल का प्रवीणता स्तर चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-142">Then, in the **Rating value** field, select the proficiency level for that skill.</span></span> <span data-ttu-id="e266a-143">अंत में, **रिसोर्स रिक्वायरमेंट** फील्ड में, संगठन की यूनिट से रिसोर्स प्राप्त करने या नामित रिसोर्स की आवश्यकता तय करें।</span><span class="sxs-lookup"><span data-stu-id="e266a-143">Finally, in the **Resource Requirement** field, set the requirement to source resources from organizational units or even named resources.</span></span> <span data-ttu-id="e266a-144">जब आप अपना काम समाप्त कर लें, तो **सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="e266a-144">When you've finished, select **Save**.</span></span>

    ![क्विक क्रिएट: रिक्वायरमेंट कैरेक्टरिस्टिक डॉयलॉग बॉक्स](media/Resource-Management-image12.png)

5. <span data-ttu-id="e266a-146">**रिसोर्स रिक्वायरमेंट** पेज में, रिसोर्स की आवश्यकता पूरी करने के लिए **बुक** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-146">On the **Resource Requirement** page, select **Book** to fulfill the resource requirement.</span></span>

    ![रिसोर्स रिक्वायरमेंट पेज में बुक बटन](media/Resource-Management-image13.png)

    <span data-ttu-id="e266a-148">आप **ऑल टीम मेम्बर्स** ग्रिड में सामान्य रिसोर्स भी चुन सकते हैं और उसके बाद **बुक** चुन सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-148">You can also select the generic resource in the **All Team Members** grid and then select **Book**.</span></span>

    ![ऑल टीम मेम्बर्स ग्रिड के ऊपर बुक बटन](media/Resource-Management-image14.png)

    > [!NOTE]
    > <span data-ttu-id="e266a-150">इस उदाहरण में, 40 घंटे आवश्यक होते हैं लेकिन कोई वास्तविक बुक किया गया घंटा नहीं होता है क्योंकि सामान्य रिसोर्स की बुकिंग नहीं होती है।</span><span class="sxs-lookup"><span data-stu-id="e266a-150">In this example, there are 40 required hours but no actual booked hours, because generic resources don't have bookings.</span></span> <span data-ttu-id="e266a-151">इसके अलावा, कोई निर्धारित घंटे नहीं होते हैं क्योंकि सामान्य रिसोर्स को टीम द्वारा सीधे शामिल किया गया था।</span><span class="sxs-lookup"><span data-stu-id="e266a-151">Additionally, there are no assigned hours, because the generic resource was added directly to the team.</span></span> <span data-ttu-id="e266a-152">टास्क असाइनमेंट का उपयोग करते हुए इसे जोड़ा नहीं गया था।</span><span class="sxs-lookup"><span data-stu-id="e266a-152">It wasn't added by using task assignment.</span></span>

    <span data-ttu-id="e266a-153">**शेड्यूलिंग असिस्टेंट** पेज में, आप रिसोर्स की आवश्यकता में निर्दिष्ट आवश्यकता द्वारा उपलब्ध रिसोर्स को फिल्टर कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-153">On the **Scheduling Assistant** page, you can filter available resources by the requirements that are specified on the resource requirement.</span></span> <span data-ttu-id="e266a-154">रिसोर्स को शेड्लूय बोर्ड पर निर्दिष्ट सॉर्टिंग परिमापियों के अनुसार छांटा जाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-154">Resources are sorted according to the sorting parameters that are specified on the Schedule Board.</span></span>

    ![शेड्यूलिंग असिस्टेंट पेज](media/Resource-Management-image15.png)

    <span data-ttu-id="e266a-156">अक्सर प्रयोग किए जाने वाले कुछ फिल्टर इस प्रकार हैं:</span><span class="sxs-lookup"><span data-stu-id="e266a-156">Here are some filters that are often used:</span></span>

    - <span data-ttu-id="e266a-157">**रेटिंग के साथ कैरेक्टरिस्टिक्स** – प्रवीणता की रेटिंग के अलावा, कौशल, प्रमाण-पत्रों और अन्य क्वालिटी द्वारा फिल्टर करता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-157">**Characteristics along with a rating** – Filter by skills, certifications, and other resource qualities, in addition to ratings of proficiency.</span></span>
    - <span data-ttu-id="e266a-158">**रोल्स** – बुक करने योग्य रिसोर्स को दी गई भूमिकाओं द्वारा फिल्टर करता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-158">**Roles** – Filter by the default roles that are assigned to bookable resources.</span></span>
    - <span data-ttu-id="e266a-159">**ऑर्गेनाइज़ेशनल यूनिट्स** – ऑर्गेनाइज़ेशनल यूनिट जिन्हें संसाधन सौंपा गया है, द्वारा बुक योग्य संसाधन फिल्टर करता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-159">**Organizational units** – Filter bookable resources by the organizational units that they are assigned to.</span></span>

6. <span data-ttu-id="e266a-160">यदि आप प्रारंभिक खोज के परिणामों से संतुष्ट नहीं हैं तो आप फिल्टर मानदंड बदल सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-160">If you aren't satisfied with the results of the initial requirement search, you can change the filter criteria.</span></span> <span data-ttu-id="e266a-161">बाईं ओर **फिल्टर व्यू** पैन को विस्तारित करें और अतिरिक्त संसाधन खोजने के लिए **सर्च** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-161">Expand the **Filter View** pane on the left, and then select **Search** to find additional resources.</span></span>

    ![व्यू पैन फिल्टर करना](media/Resource-Management-image16.png)

7. <span data-ttu-id="e266a-163">परिणाम छांटने की विधि बदलने के लिए, **सॉर्ट** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-163">To change how the results are sorted, select **Sort**.</span></span>

    ![सॉर्ट कमांड](media/Resource-Management-image17.png)

8. <span data-ttu-id="e266a-165">ग्रिड के ऊपर दर्शाए गए अनुसार, आवश्यता में बताई गई मांग के अनुसार रिसोर्स चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-165">Select resources according to the demand that is specified on the requirement, as indicated at the top of the grid.</span></span> <span data-ttu-id="e266a-166">आप ग्रिड में सेल का चयन हटा सकते हैं और उस रिसोर्स क्षमता को खुला रख सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-166">You can clear the selection of cells in the grid and leave that resource capacity open.</span></span> <span data-ttu-id="e266a-167">एक बार में केवल एक रिसोर्स को बुक किए गए के रूप में चुना जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-167">Only one resource at a time can be selected as booked.</span></span>

9. <span data-ttu-id="e266a-168">चुने गए रिसोर्स को बुक करने के लिए **बुक** चुनें और स्केड्यूल बोर्ड को खुला छोड़े ताकि आप अतिरिक्त रिसोर्स का चयन कर सकें।</span><span class="sxs-lookup"><span data-stu-id="e266a-168">Select **Book** to book the selected resource and leave the Schedule Board open, so that you can select additional resources.</span></span> <span data-ttu-id="e266a-169">वैकल्पिक रूप से, चुने गए रिसोर्स को बुक करने के लिए **बुक एंड एक्ज़िट** चुनें और स्केड्यूल बोर्ड को बंद करें।</span><span class="sxs-lookup"><span data-stu-id="e266a-169">Alternatively, select **Book & Exit** to book the selected resource and close the Schedule Board.</span></span>

    ![बुक करने के लिए रिसोर्स](media/Resource-Management-image19.png)

    <span data-ttu-id="e266a-171">आपको बुक किए गए घंटों के बारे में सूचना मिलेगी।</span><span class="sxs-lookup"><span data-stu-id="e266a-171">You receive a notification about booked hours.</span></span> <span data-ttu-id="e266a-172">मांग संसूचक यह दर्शाते हैं कि बुकिंग की कितनी आवश्यकता पूरी की गई है और कितनी शेष है।</span><span class="sxs-lookup"><span data-stu-id="e266a-172">The demand indicators show how much the booking requirement is satisfied and how much remains.</span></span> <span data-ttu-id="e266a-173">आप यह भी देख सकते हैं कि चयनित रिसोर्स की कितनी क्षमता का उपभोग किया गया है।</span><span class="sxs-lookup"><span data-stu-id="e266a-173">You can also see how much of the selected resource's capacity is consumed.</span></span> <span data-ttu-id="e266a-174">रिसोर्स बुकिंग के बारे में अधिक विवरण देखने के लिए **एक्सपैंड** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-174">Select **Expand** to view more details about resource bookings.</span></span>

9. <span data-ttu-id="e266a-175">**ऑल टीम मेम्बर्स** व्यू में वापस जाएँ।</span><span class="sxs-lookup"><span data-stu-id="e266a-175">Return to the **All Team Members** view.</span></span> <span data-ttu-id="e266a-176">ग्रिड में, ध्यान दें कि सामान्य रिसोर्स को बदकर नामित रिसोर्स कर दिया गया है और उस रिसोर्स के लिए 40 घंटे बुक किए गए हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-176">In the grid, notice that the generic resource has been replaced by the named resource, and 40 hours are listed as booked for that resource.</span></span>

    ![ऑल टीम मेम्बर्स ग्रिड अपडेट हो गया है](media/Resource-Management-image20.png)

    > [!NOTE]
    > <span data-ttu-id="e266a-178">कोई असाइन किए गए घंटे नहीं दिखाए गये हैं क्योंकि उन्हें सीधे टीम पर बुक कर दिया गया है।</span><span class="sxs-lookup"><span data-stu-id="e266a-178">No assigned hours are shown, because they were booked directly on the team.</span></span> <span data-ttu-id="e266a-179">उन्हें टास्क असाइनमेंट का इस्तेमाल करते हुए बुक नहीं किया गया है।</span><span class="sxs-lookup"><span data-stu-id="e266a-179">They weren't booked by using task assignment.</span></span>

## <a name="assign-generic-resources-to-tasks-and-generate-resource-requirements"></a><span data-ttu-id="e266a-180">सामान्य रिसोर्स को टास्क के लिए असाइन करें और रिसोर्स की आवश्यकताएँ बताएँ</span><span class="sxs-lookup"><span data-stu-id="e266a-180">Assign generic resources to tasks and generate resource requirements</span></span>

<span data-ttu-id="e266a-181">PSA में, आप टास्क बना सकते हैं और उन्हें सामान्य रिसोर्स असाइन कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-181">In PSA, you can create tasks and then assign generic resources to them.</span></span> <span data-ttu-id="e266a-182">इस तरह, अपने स्केड्यूल और वित्तीय अंकों का प्राक्कलन करते समय रिसोर्स की मांग को प्लेसहोल्डर द्वारा दर्शाया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-182">In this way, resource demand can be represented by placeholders while you estimate your schedule and financial numbers.</span></span> <span data-ttu-id="e266a-183">इसके बाद आप सामान्य संसाधनों के लिए संसाधन की आवश्यकताएँ बना सकते हैं और उन्हें पूरा कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-183">You can then generate resource requirements for the generic resources and fulfill them.</span></span>

1. <span data-ttu-id="e266a-184">**प्रोजेक्ट्स** पेज पर, **शिड्यूल** टैब पर, टास्क बनाने के लिए, **एड** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-184">On the **Projects** page, on the **Schedule** tab, select **Add** to create a task.</span></span>

    ![नया टास्क बन जाएगा](media/Resource-Management-image21.png)

2. <span data-ttu-id="e266a-186">**रिसोर्सेस** फील्ड में, **रिसोर्स पिकर** प्रतीक चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-186">In the **Resources** field, select the **Resource Picker** symbol.</span></span> <span data-ttu-id="e266a-187">रिसोर्स पिकर प्रकट होगा जो प्रोजेक्ट के विद्यमान टीम सदस्यों को दिखाएगा।</span><span class="sxs-lookup"><span data-stu-id="e266a-187">The Resource Picker appears and shows existing team members for the project.</span></span>

    ![रिसोर्स पिकर](media/Resource-Management-image22.png)

3. <span data-ttu-id="e266a-189">नए सामान्य रिसोर्स का नाम दर्ज करें और **क्रिएट** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-189">Enter the name of the new generic resource, and then select **Create**.</span></span>

    ![नए सामान्य रिसोर्स का नाम दर्ज हो जाएगा](media/Resource-Management-image23.png)

4. <span data-ttu-id="e266a-191">**क्विक क्रिएट: प्रोजेक्ट टीम मेम्बर** डॉयलॉग बॉक्स में, **रोल** फील्ड में, सामान्य रिसोर्स का नाम चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-191">In the **Quick Create: Project Team Member** dialog box that appears, in the **Role** field, select the role for the generic resource.</span></span> <span data-ttu-id="e266a-192">**रिसोर्सिंग यूनिटे** फील्ड में, सामान्य रिसोर्स के लिए ऑर्गेनाइजेशनल यूनिट चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-192">In the **Resourcing Unit** field, select the organizational unit for the generic resource.</span></span> <span data-ttu-id="e266a-193">फिर **सेव** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-193">Then select **Save**.</span></span>

    ![क्विक क्रिएट: प्रोजेक्ट टीम मेम्बर डॉयलॉग बॉक्स](media/Resource-Management-image24.png)

    <span data-ttu-id="e266a-195">सामान्य टीम सदस्य को अब टास्क असाइन कर दिया गया है।</span><span class="sxs-lookup"><span data-stu-id="e266a-195">The generic team member is now assigned to the task.</span></span>

    ![सामान्य टीम सदस्य को टास्क असाइन कर दिया गया है](media/Resource-Management-image25.png)

    <span data-ttu-id="e266a-197">**टीम** टैब में, आप नए सामान्य टीम सदस्य को देखेंगे।</span><span class="sxs-lookup"><span data-stu-id="e266a-197">On the **Team** tab, you will see the new generic team member.</span></span> <span data-ttu-id="e266a-198">ध्यान दें कि इसमें केवल असाइन किए गए घंटे हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-198">Notice that it has only assigned hours.</span></span> <span data-ttu-id="e266a-199">ये घंटे उन सभी टास्क का योग है जिन्हें सामान्य टीम सदस्य को असाइन किए गए हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-199">These hours are the sum of all tasks that are assigned to the generic team member.</span></span> <span data-ttu-id="e266a-200">सामान्य टीम सदस्य को अब तक आवश्यक घंटों की या रिसोर्स की आवश्यकता नहीं है।</span><span class="sxs-lookup"><span data-stu-id="e266a-200">The generic team member doesn't yet have required hours or a resource requirement.</span></span>

    ![टीम टैब पर सामान्य टीम सदस्य](media/Resource-Management-image26.png)

5. <span data-ttu-id="e266a-202">अब आप रिसोर्स पिकर का इस्तेमाल करते हुए सामान्य टीम सदस्य को अन्य टास्क सौंप सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-202">You can now assign the generic team member to other tasks by using the Resource Picker.</span></span>

    ![रिसोर्स पिकर में सामान्य टीम सदस्य](media/Resource-Management-image27.png)

    <span data-ttu-id="e266a-204">जब आप सामान्य रिसोर्स को टास्क दे चुके होते हैं, तो आप सामान्य रिसोर्स के लिए रिसोर्स की आवश्यकता बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-204">When you've finished assigning the generic resource to tasks, you can generate a resource requirement for the generic resource.</span></span>

5. <span data-ttu-id="e266a-205">**टीम** टैब पर, सामान्य रिसोर्स चुनें फिर **जनरेट रिक्वायरमेंट** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-205">On the **Team** tab, select the generic resource, and then select **Generate Requirement**.</span></span>

    ![जनरल रिक्वायरमेंट कमांड](media/Resource-Management-image28.png)

    <span data-ttu-id="e266a-207">जब आवश्यकता बना दी जाती है, तो सामान्य टीम सदस्य को अपेक्षित घंटों और रिसोर्स आवश्यकता के लिए लिंक की आवश्यकता होगी।</span><span class="sxs-lookup"><span data-stu-id="e266a-207">When the requirement is generated, the generic team member will have required hours and a link for the resource requirement.</span></span>

    ![रिसोर्स आवश्यकता का लिंक](media/Resource-Management-image29.png)

    <span data-ttu-id="e266a-209">नामित रिसोर्स को बुक करने के बाद, सामान्य रिसोर्स को टीम से हटा दिया जाता है और उसे नामित रिसोर्स से स्थानापित कर दिया जाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-209">After you book a named resource, the generic resource is removed from the team and replaced by the named resource.</span></span>

    ![नामित रिसोर्स से स्थानापित किया गया सामान्य रिसोर्स](media/Resource-Management-image30.png)

    <span data-ttu-id="e266a-211">**स्केड्यूल** टैब पर, सामान्य रिसोर्स के असाइनमेंट को हटा दिया जाता है और उसे नामित रिसोर्स से स्थानापित कर दिया जाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-211">On the **Schedule** tab, the generic resource assignments are removed and replaced by the named resource.</span></span>

    ![स्केड्यूल टैब पर, नामित रिसोर्स से स्थानापित सामान्य रिसोर्स असाइनमेंट](media/Resource-Management-image31.png)

    > [!NOTE]
    > <span data-ttu-id="e266a-213">ऐसा तभी होता है जब नामित रिसोर्स को सामान्य रिसोर्स की आवश्यकता के लिए पूरी तरह बुक किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-213">This behavior occurs only when a named resource is fully booked for the generic resource requirement.</span></span> <span data-ttu-id="e266a-214">जब नामित रिसोर्स आंशिक रूप से सामान्य रिसोर्स की आवश्यकता को स्थानापित करता है या एक से अधिक नामित रिसोर्स सामान्य रिसोर्स की आवश्यकता को स्थानापित करते हैं, तो टास्क को सामान्य रिसोर्स असाइन किया बना रहता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-214">When either a named resource partially replaces the generic resource requirement or multiple named resources replace the generic resource requirement, the generic resource remains assigned to the task.</span></span>

    <span data-ttu-id="e266a-215">निम्नलिखित उदाहरण में, पाँच-दिनों की अवधि (पाँच दिनों में प्रत्येक दिन 16 घंटे) के लिए 80-घंटों के टास्क की योजना बनाई गई है और **फंक्शनल** नामक सामान्य रिसोर्स को सौंपा गया है।</span><span class="sxs-lookup"><span data-stu-id="e266a-215">In the following illustration, an 80-hour task has been planned for a five-day duration (16 hours per day over five days) and assigned to the generic resource that is named **Functional**.</span></span>

    ![फंक्शनल सामान्य रिसोर्स को अस्सी-घंटों का, पाँच दिवसीय टॉस्क सौंपा गया है](media/Resource-Management-image32.png)

    <span data-ttu-id="e266a-217">जब आप आवश्यकता बनाते हैं, तो यह पाँच दिनों के लिए 80 घंटों का होगा।</span><span class="sxs-lookup"><span data-stu-id="e266a-217">When you generate the requirement, it's for 80 hours over five days.</span></span>

    ![पाँच दिनों के ले 80 घंटों की आवश्यकता बनाई गई है](media/Resource-Management-image33.png)

    <span data-ttu-id="e266a-219">क्योंकि उपलब्ध रिसोर्स प्रति दिन केवल आठ घंटे काम करते हैं, इस आवश्यकता को पूरा करने के लिए दो रिसोर्स की आवश्यकता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-219">Because available resources work only eight hours per day, two resources are needed to fulfill the requirement.</span></span>

    ![दूसरा रिसोर्स](media/Resource-Management-image35.png)

    <span data-ttu-id="e266a-221">**टीम** टैब पर, अब आप देख सकते हैं कि सामान्य रिसोर्स को घंटों की आवश्यकता नहीं है लेकिन सौंपे गए घंटे अब भी दो नामित रिसोर्स के साथ दिखते हैं जो आवश्यकता को पूरा करेंगे।</span><span class="sxs-lookup"><span data-stu-id="e266a-221">On the **Team** tab, you can now see that the generic resource has no required hours, but the assigned hours still appear together with the two named resources that make up the fulfillment.</span></span>

    ![टीम टैब पर दो नामित रिसोर्स](media/Resource-Management-image36.png)

    <span data-ttu-id="e266a-223">**शिड्यूल** टैब पर, सामान्य रिसोर्स को सौंपा गया टास्क बना रहता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-223">On the **Schedule** tab, the generic resource remains assigned to the task.</span></span>

    ![स्केड्यूल टैब पर सामान्य रिसोर्स](media/Resource-Management-image37.png)

<span data-ttu-id="e266a-225">PSA दोनों रिसोर्स को टास्क नहीं सौंपता है क्योंकि ऐसा करने से कम पूर्वानुमान का स्केड्यूल बनेगा।</span><span class="sxs-lookup"><span data-stu-id="e266a-225">PSA doesn't assign both resources to the task, because that behavior would produce a less predictable schedule.</span></span> <span data-ttu-id="e266a-226">इस आसान से उदाहरण में, दोनों रिसोर्स के बीच घंटों को समान रूप से बांटना आसान होता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-226">In this simple example, it's easy to divide the hours equally between two resources.</span></span> <span data-ttu-id="e266a-227">बहरहाल, अधिक जटिल मामले में जिसमें एक से अधिक टास्क और रिसोर्स होते हैं, PSA को एक से अधिक टास्क में एक से अधिक रिसोर्स के लिए प्राप्त होने वाली बुकिंग को आबंटित करना के बार में सोचना पड़ता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-227">However, in more complex scenarios that involve multiple tasks and multiple resources, PSA would have to make assumptions about how it should allocate the bookings that are received for multiple resources across multiple tasks.</span></span>

<span data-ttu-id="e266a-228">इसलिए, ऐसे मामलो में, प्रोजेक्ट मैनेजर एक से अधिक बुकिंग को बांटने और उन्हें ज़रूरत के अनुसार सौंपने के लिए जिम्मेदार होते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-228">Therefore, in these scenarios, the project manager is responsible for parsing the multiple bookings and assigning them as needed.</span></span> <span data-ttu-id="e266a-229">बुकिंग आबंटित करने के लिए, प्रोजेक्ट मैनेजर टास्क को सामान्य रिसोर्स से नामित रिसोर्स को सौंपते हैं और उसके बाद यह सुनिश्चित करने के लिए कि आबंटन बुकिंग के अनुसार किया गया है, **रिकनसीलिएशन** व्यू का इस्तेमाल करते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-229">To allocate the bookings, the project manager assigns the tasks from the generic resources to the named resources and then uses the **Reconciliation** view to make sure that the allocation works with the bookings.</span></span>

### <a name="edit-a-resource-requirement"></a><span data-ttu-id="e266a-230">रिसोर्स की आवश्यकता के एडिट करना</span><span class="sxs-lookup"><span data-stu-id="e266a-230">Edit a resource requirement</span></span>

<span data-ttu-id="e266a-231">किसी रिसोर्स की आवश्यकता बनाने के बाद, हो सकता है कि प्रोजेक्ट मैनेजर या रिसोर्स मैनेजर स्केड्यूल बोर्ड का इस्तेमाल करने के बाद सर्च के मानदंड को रिफाइन करने के लिए विवरणों के एडिट करना चाहें।</span><span class="sxs-lookup"><span data-stu-id="e266a-231">After a resource requirement has been created, a project manager or resource manager might want to edit the details to refine the search criteria when the Schedule Board is used.</span></span> <span data-ttu-id="e266a-232">रिसोर्स आवश्यकता को एडिट करने के लिए, इन चरणों को पूरा करें।</span><span class="sxs-lookup"><span data-stu-id="e266a-232">To edit the resource requirement, follow these steps.</span></span>

1. <span data-ttu-id="e266a-233">**प्रोजेक्ट्स** पेज पर, **टीम** टैब पर, सामान्य रिसोर्स की किसी भी आवश्यकता के लिंक को चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-233">On the **Projects** page, on the **Team** tab, select the link to any requirement on a generic resource.</span></span>
2. <span data-ttu-id="e266a-234">**रिसोर्स रिक्वायरमेंट** पेज पर, आप अनेक गुणों को अपडेट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-234">On the **Resource Requirement** page that appears, you can update several attributes.</span></span> <span data-ttu-id="e266a-235">यहाँ कुछ उदाहरण दिए गए हैं:</span><span class="sxs-lookup"><span data-stu-id="e266a-235">Here are some examples:</span></span>

    - <span data-ttu-id="e266a-236">Name</span><span class="sxs-lookup"><span data-stu-id="e266a-236">Name</span></span>
    - <span data-ttu-id="e266a-237">प्रारंभ दिनांक</span><span class="sxs-lookup"><span data-stu-id="e266a-237">From Date</span></span>
    - <span data-ttu-id="e266a-238">इस दिनांक तक</span><span class="sxs-lookup"><span data-stu-id="e266a-238">To Date</span></span>
    - <span data-ttu-id="e266a-239">अवधि</span><span class="sxs-lookup"><span data-stu-id="e266a-239">Duration</span></span>
    - <span data-ttu-id="e266a-240">संसाधन प्रकार</span><span class="sxs-lookup"><span data-stu-id="e266a-240">Resource Type</span></span>

<span data-ttu-id="e266a-241">**रिसोर्स रिक्वायरमेंट** पेज पर, प्रोजेक्ट मैनेजर या रिसोर्स मैनेजर भी निम्नलिखित सूचनाओं को परिभाषित कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="e266a-241">On the **Resource Requirement** page, the project manager or resource manager can also define the following information:</span></span>

- <span data-ttu-id="e266a-242">कौशल</span><span class="sxs-lookup"><span data-stu-id="e266a-242">Skills</span></span>
- <span data-ttu-id="e266a-243">भूमिकाएँ</span><span class="sxs-lookup"><span data-stu-id="e266a-243">Roles</span></span>
- <span data-ttu-id="e266a-244">रिसोर्स की प्राथमिकताएं</span><span class="sxs-lookup"><span data-stu-id="e266a-244">Resource preferences</span></span>
- <span data-ttu-id="e266a-245">वरीय संगठनात्मक यूनिट</span><span class="sxs-lookup"><span data-stu-id="e266a-245">Preferred organizational unit</span></span>

### <a name="update-resource-bookings-after-they-are-booked-on-a-project"></a><span data-ttu-id="e266a-246">किसी प्रोजेक्ट में रिसोर्स को बुक करने के बाद रिसोर्स बुकिंग को अपडेट करना</span><span class="sxs-lookup"><span data-stu-id="e266a-246">Update resource bookings after they are booked on a project</span></span>

<span data-ttu-id="e266a-247">प्रोजेक्ट टीम में सामान्य या नामित रिसोर्स को शामिल करने के बाद, आप रिसोर्स की बुकिंग को बदल सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-247">After you've added a generic or named resource to a project team, you can change the resource's bookings.</span></span>

1. <span data-ttu-id="e266a-248">**प्रोजेक्ट्स** पेज पर, **टीम** टैब पर, टीम सदस्य चुनें फिर **मेंटेन बुकिंग्स** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-248">On the **Projects** page, on the **Team** tab, select a team member, and then select **Maintain Bookings**.</span></span>

    ![चुने गए टीम मेम्बर के लिए स्केड्यूल बोर्ड खुलेगा](media/Resource-Management-image40.png)

    <span data-ttu-id="e266a-250">स्केड्यूल बोर्ड दिखेगा जो प्रोजेक्ट टीम के मेम्बरों की बुकिंग दिखाएगा।</span><span class="sxs-lookup"><span data-stu-id="e266a-250">The Schedule Board appears and shows the project team member's bookings.</span></span> <span data-ttu-id="e266a-251">इस प्रोजेक्ट तथा अन्य प्रोजेक्ट जिसमें टीम के मेम्बर की क्षमता का उपयोग किया जाता है, के समक्ष बुक किए गए घंटों को देखने के लिए टीम मेम्बर के रिकार्ड को एक्सपैंड करें।</span><span class="sxs-lookup"><span data-stu-id="e266a-251">Expand the team member's record to view the hours that have been booked against this project and other projects that are consuming the team member's capacity.</span></span>

2. <span data-ttu-id="e266a-252">इसे एक्सपैंड करने या छोटा करने के लिए बुकिंग को चुनें और ड्रैग करें।</span><span class="sxs-lookup"><span data-stu-id="e266a-252">Select and drag the booking to extend or shorten it.</span></span> <span data-ttu-id="e266a-253">एक **क्रिएट रिसोर्स बुकिंग** डॉयलॉग बॉक्स दिखेगा जिसमें आप बुकिंग को एडजस्ट कर सकेंगे।</span><span class="sxs-lookup"><span data-stu-id="e266a-253">A **Create Resource Booking** dialog box appears that lets you adjust the booking.</span></span>

    ![क्रिएट रिसोर्स बुकिंग डॉयलॉग बॉक्स](media/Resource-Management-image41.png)

3. <span data-ttu-id="e266a-255">बुकिंग पर राइट-क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e266a-255">Right-click the booking.</span></span> <span data-ttu-id="e266a-256">इसके बाद आप निम्नलिखित काम करने के लिए शॉर्टकट मेन्यू का इस्तेमाल कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="e266a-256">You can then use the shortcut menu to complete the following actions:</span></span>

    - <span data-ttu-id="e266a-257">बुकिंग स्टेटस को बदलना।</span><span class="sxs-lookup"><span data-stu-id="e266a-257">Change the booking status.</span></span>
    - <span data-ttu-id="e266a-258">बुकिंग को एडिट करना।</span><span class="sxs-lookup"><span data-stu-id="e266a-258">Edit the booking.</span></span>
    - <span data-ttu-id="e266a-259">प्रोजेक्ट टीम पर रिसोर्स को स्थानापित करना।</span><span class="sxs-lookup"><span data-stu-id="e266a-259">Substitute a resource on the project team.</span></span>

### <a name="change-the-booking-status"></a><span data-ttu-id="e266a-260">बुकिंग स्टेटस को बदलना</span><span class="sxs-lookup"><span data-stu-id="e266a-260">Change the booking status</span></span>

<span data-ttu-id="e266a-261">आप किसी भी डिफाल्ट या कस्टम बुकिंग स्टेटस को बदल सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-261">You can change any default or custom booking status.</span></span>

![स्टेटस कमांड को बदलना](media/Resource-Management-image42.png)

<span data-ttu-id="e266a-263">PSA में निम्नलिखित स्टेटस शामिल होते हैं:</span><span class="sxs-lookup"><span data-stu-id="e266a-263">The following statuses are included in PSA:</span></span>

- <span data-ttu-id="e266a-264">**कैनसल्ड** – यह स्टेटस रिसोर्स की बुकिंग को कैंसल करता है और रिसोर्स की क्षमता को मुक्त करता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-264">**Canceled** – This status cancels a resource's booking and frees up the resource's capacity.</span></span>
- <span data-ttu-id="e266a-265">**हार्ड बुक** – यह स्टेटस रिसोर्स की क्षमता का उपभोग करता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-265">**Hard Book** – This status consumes a resource's capacity.</span></span> <span data-ttu-id="e266a-266">एक बुकिंग में आम तौर पर यह स्टेटस तब होता है जब आप **प्रोजेक्ट्स** पेज पर **ऑल टीम मेम्बर्स** ग्रिड से **मेनटेन बुकिंग्स** को खोलते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-266">A booking typically has this status when you open **Maintain Bookings** from the **All Team Members** grid on the **Projects** page.</span></span>
- <span data-ttu-id="e266a-267">**साफ्ट बुक** – यह स्टेटस टीम में एक रिसोर्स को शामिल करता है लेकिन रिसोर्स की क्षमता का उपभोग नहीं करता।</span><span class="sxs-lookup"><span data-stu-id="e266a-267">**Soft Book** – This status adds a resource to a team but doesn't consume the resource's capacity.</span></span> <span data-ttu-id="e266a-268">यह दर्शाता है कि रिसोर्स को किसी संभावित कार्य के लिए आरक्षित रखा गया है लेकिन अन्य जॉब में उसकी ज़रूरत पड़ने पर उसमें अब भी क्षमता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-268">It indicates that the resource has been reserved for potential work but still has capacity if it's needed on other jobs.</span></span> <span data-ttu-id="e266a-269">समग्र रिसोर्स उपलब्धता के व्यू में, साफ्ट बुकिंग का स्टेटस हार्ड बुकिंग के स्टेटस से अलग होता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-269">In the view of overall resource availability, soft bookings have a different status than hard bookings.</span></span>
- <span data-ttu-id="e266a-270">**प्रपोज़्ड** – यह स्टेटस किसी रिसोर्स के लिए रिसोर्स मैनेजर या प्रोजेक्ट मैनेजर के प्रस्ताव को बताता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-270">**Proposed** – This status represents a resource manager's or project manager's proposal for a resource.</span></span> <span data-ttu-id="e266a-271">प्रपोज़ल में रिसोर्स की क्षमता का उपभोग नहीं होता और रिसोर्स को प्रोजेक्ट टीम में शामिल नहीं किया जाता।</span><span class="sxs-lookup"><span data-stu-id="e266a-271">Proposals don't consume the capacity of a resource, and the resource isn't added to the project team.</span></span> <span data-ttu-id="e266a-272">टीम में रिसोर्स को हार्ड-बुक करने के लिए, प्रोजेक्ट मैनेजर को प्रपोज़ल स्वीकार करना होगा।</span><span class="sxs-lookup"><span data-stu-id="e266a-272">To hard-book the resource on the team, the project manager must accept the proposal.</span></span>

### <a name="submit-resource-requests"></a><span data-ttu-id="e266a-273">संसाधन अनुरोध सबमिट करें</span><span class="sxs-lookup"><span data-stu-id="e266a-273">Submit resource requests</span></span>

<span data-ttu-id="e266a-274">रिसोर्स के अनुरोधों का इस्तेमाल ऐसी मांग (रिसोर्स की आवश्यकता) पूरी करने के लिए किया जाता है जिसे रिसोर्स के मैनेजर द्वारा पूरा करना ज़रूरी होता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-274">Resource requests are used to carry the demand (resource requirement) that must be fulfilled by a resource manager.</span></span> <span data-ttu-id="e266a-275">किसी ऐसे जेनरिक संसाधन के लिए, जो टीम में पहले से है, आप सीधे संसाधन अनुरोध सबमिट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="e266a-275">For a generic resource that is already on the team, you can submit a resource request directly.</span></span> <span data-ttu-id="e266a-276">रिसोर्स का अनुरोध दो तरीकों से पूरा किया जा सकता है:</span><span class="sxs-lookup"><span data-stu-id="e266a-276">A resource request can be fulfilled in two ways:</span></span>

- <span data-ttu-id="e266a-277">रिसोर्स मैनेजर अनुरोध को सीधे ही पूरा कर सकता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-277">The resource manager directly fulfills the request.</span></span> <span data-ttu-id="e266a-278">इस मामले में, सामान्य रिसोर्स को हार्ड बुकिंग जिसमें नामित रिसोर्स होता है, से स्थानापित किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-278">In this case, the generic resource is replaced by a hard booking that has a named resource.</span></span>
- <span data-ttu-id="e266a-279">रिसोर्स मैनेजर एक रिसोर्स का प्रस्ताव प्रोजेक्ट मैनेजर को करता है और प्रोजेक्ट मैनेजर ऐसे प्रस्तावित रिसोर्स को स्वीकार या अस्वीकार कर सकता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-279">The resource manager proposes a resource to the project manager, and the project manager approves or rejects the proposed resource.</span></span>

#### <a name="direct-fulfillment-of-resource-requests"></a><span data-ttu-id="e266a-280">रिसोर्स के अनुरोधों को सीधे ही पूरा करना</span><span class="sxs-lookup"><span data-stu-id="e266a-280">Direct fulfillment of resource requests</span></span>

<span data-ttu-id="e266a-281">जब एक रिसोर्स की आवश्यकता बनाई जाती है, प्रोजेक्ट मैनेजर से रिसोर्स को चुनते हुए सामान्य रिसोर्स के लिए उसका अनुरोध सबमिट कर सकता है और उसके बाद **सबमिट रिक्वेस्ट** का चयन करता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-281">When a resource requirement is generated, a project manager can submit a resource request for a generic resource by selecting the resource and then selecting **Submit Request**.</span></span>

![रिक्वेस्ट बटन सबमिट करना](media/Resource-Management-image45.png)

<span data-ttu-id="e266a-283">अनुरोध को पूरा करने वाले रिसोर्स मैनेजर को रिसोर्स के बारे में टिप्पणी दी जा सकती है।</span><span class="sxs-lookup"><span data-stu-id="e266a-283">Comments about the resource can be provided to the resource manager who is fulfilling the request.</span></span> <span data-ttu-id="e266a-284">रिक्वेस्ट सबमिट होने के बाद, टीम मेम्बर के लिए **स्टेटस** फील्ड को बदलकर **सबमिटेड** कर दिया जाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-284">After the request is submitted, the **Status** field for the team member is changed to **Submitted**.</span></span>

![वैकल्पिक टिप्पणियाँ दर्ज करना](media/Resource-Management-image46.png)

<span data-ttu-id="e266a-286">जब रिसोर्स मैनेजर अनुरोध को पूरा करता है, तो सामान्य टीम सदस्य को **ऑल टीम मेम्बर्स** ग्रिड में नामित रिसोर्स में स्थानापित कर दिया जाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-286">When the resource manager fulfills the request, the generic team member is replaced by the named resource in the **All Team Members** grid.</span></span>

![सामान्य टीम सदस्य को ऑल टीम मेम्बर्स ग्रिड में नामित रिसोर्स से स्थानापित किया जाता है।](media/Resource-Management-image47.png)

#### <a name="use-a-resource-proposal-for-resource-requests"></a><span data-ttu-id="e266a-288">रिसोर्स के अनुरोधों के लिए रिसोर्स के प्रस्ताव का इस्तेमाल करना</span><span class="sxs-lookup"><span data-stu-id="e266a-288">Use a resource proposal for resource requests</span></span>

<span data-ttu-id="e266a-289">किसी रिसोर्स के अनुरोध पर रिसोर्स की सीधे बुकिंग करने के बजाय, रिसोर्स मैनेजर प्रोजेक्ट मैनेजर को रिसोर्स का प्रस्ताव रख सकता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-289">Instead of directly booking a resource on a resource request, a resource manager can propose a resource to the project manager.</span></span> <span data-ttu-id="e266a-290">यदि आवश्यकता के लिए सटीक मेल उपलब्ध न हो तो रिसोर्स मैनेजर इस विकल्प का इस्तेमाल कर सकता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-290">A resource manager might use this option when an exact match for the requirements isn't available.</span></span> <span data-ttu-id="e266a-291">जब रिसोर्स मैनेजर किसी रिसोर्स का प्रस्ताव करता है तो प्रोजेक्ट मैनेजर यह देखता है कि सामान्य टीम सदस्य का **स्टेटस** फील्ड **नीड्स रिव्यू** में बदल गया है।</span><span class="sxs-lookup"><span data-stu-id="e266a-291">When a resource manager proposes a resource, the project manager sees that the **Status** field for the generic team member is changed to **Needs Review**.</span></span>

![सामान्य टीम के सदस्य का स्टेटस बदलकर नीड्य रिव्यू हो जाता है।](media/Resource-Management-image48.png)

<span data-ttu-id="e266a-293">प्रस्ताव की बुकिंग के प्रभाव को देखने के साथ-साथ प्रस्तावित रिसोर्स को देखने के लिए, **नीड्स रिव्यू** की स्टेटस वाले टीम सदस्य पर डबल-क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="e266a-293">To view the proposed resource together with a visualization of the effect of the proposal's booking, double-click the team member that has a status of **Needs Review**.</span></span> <span data-ttu-id="e266a-294">इसके बाद **प्रपोज़्ड रिसोर्सेस** टैब चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-294">Then select the **Proposed Resources** tab.</span></span>

![प्रपोज़्ड रिसोर्सेस टैब](media/Resource-Management-image49.png)

<span data-ttu-id="e266a-296">सभी प्रस्तावित रिसोर्स को स्वीकार करने के लिए **एक्सेप्ट ऑल प्रपोज़ल्स** चुनें और उन्हें अस्वीकार करने के लिए **रिजेक्ट ऑल प्रपोज़ल्स** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-296">Select **Accept All Proposals** to accept all proposed resources or **Reject All Proposals** to reject them.</span></span> <span data-ttu-id="e266a-297">यदि आप प्रस्तावित रिसोर्स को स्वीकार करते हैं तो उन्हें टीम के सदस्य के रूप में प्रोजेक्ट पर हार्ड-बुक किया जाता है और सामान्य रिसोर्स से स्थानापित किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-297">If you accept the proposed resources, they are hard-booked on the project as team members and replace the generic resources.</span></span>

> [!NOTE]
> <span data-ttu-id="e266a-298">आपको सभी प्रस्तावित रिसोर्स को स्वीकार या अस्वीकार करना होगा।</span><span class="sxs-lookup"><span data-stu-id="e266a-298">You must either accept or reject all proposed resources.</span></span> <span data-ttu-id="e266a-299">आप उन्हें आंशिक रूप से स्वीकार या अस्वीकार नहीं कर सकते।</span><span class="sxs-lookup"><span data-stu-id="e266a-299">You can't partially accept or reject them.</span></span>

### <a name="substitute-a-resource-on-the-project-team"></a><span data-ttu-id="e266a-300">प्रोजेक्ट टीम पर रिसोर्स को स्थानापित करना</span><span class="sxs-lookup"><span data-stu-id="e266a-300">Substitute a resource on the project team</span></span>

<span data-ttu-id="e266a-301">कभी-कभी, प्रोजेक्ट मैनेजर को प्रोजेक्ट में बुक किए गए टीम सदस्य को स्थानापित करना होता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-301">Sometimes, a project manager must substitute a booked team member on a project.</span></span>

1. <span data-ttu-id="e266a-302">**प्रोजेक्ट्स** पेज पर, **टीम** टैब पर, स्थानापित करने वाले रिसोर्स को चुनें और उसके बाद **मेनटेन बुकिंग्स** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-302">On the **Projects** page, on the **Team** tab, select the resource that needs a substitute, and then select **Maintain Bookings**.</span></span>
2. <span data-ttu-id="e266a-303">असाइन किए गए प्रोजेक्ट को देखने के लिए रिसोर्स को एक्सपैंड करें।</span><span class="sxs-lookup"><span data-stu-id="e266a-303">Expand the resource to view the projects that it's assigned to.</span></span>

    ![असाइन किए गए प्रोजेक्ट को दिखाने के लिए रिसोर्स को एक्सपैंड करें](media/Resource-Management-image50.png)

3. <span data-ttu-id="e266a-305">प्रोजेक्ट पर राइट-क्लिक करें और उसके बाद **सबस्टीट्यूट रिसोर्स** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-305">Right-click the project, and then select **Substitute Resource**.</span></span>
4. <span data-ttu-id="e266a-306">यदि आप चालू रिसोर्स के लिए स्थानापित किए जाने वाले रिसोर्स को जानते हैं तो नाम चुनें या टाइप करें और उसके बाद **री-असाइन** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-306">If you know the resource that you want to substitute for the current resource, select or type the name, and then select **Re-assign**.</span></span>

    ![स्थानापित रिसोर्स को निर्दिष्ट करना](media/Resource-Management-image51.png)

    <span data-ttu-id="e266a-308">वैकल्पिक रूप से, रिसोर्स की खोज करने के लिए इन चरणों का पालन करें:</span><span class="sxs-lookup"><span data-stu-id="e266a-308">Alternatively, follow these steps to search for a resource:</span></span>

    1. <span data-ttu-id="e266a-309">**फाइंड सबस्टीट्यूशन** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-309">Select **Find Substitution**.</span></span>

        ![स्थानापित रिसोर्स की खोज करना](media/Resource-Management-image52.png)

        <span data-ttu-id="e266a-311">स्केड्यू असिस्टेंट उपलब्ध स्थानापन्न की सूची वापस देगा।</span><span class="sxs-lookup"><span data-stu-id="e266a-311">The Schedule Assistant returns a list of available substitutes.</span></span> <span data-ttu-id="e266a-312">स्केड्यू असिस्टेंट में, आप उपयुक्त स्थानापन्न का पता लगाने के लिए उपलब्ध रिसोर्स को आगे फिल्टर कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-312">In the Schedule Assistant, you can further filter the available resources to find a suitable substitute.</span></span>

        ![उपलब्ध स्थानापन्न की सूची](media/Resource-Management-image53.png)

    2. <span data-ttu-id="e266a-314">रिसोर्स को स्थानापित करने के लिए, वांछित रिसोर्स को चुनें और उसके बाद **सबस्टीट्यूट** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-314">To substitute the resource, select the resource that you want, and then select **Substitute**.</span></span>

        ![चुने गए रिसोर्स को स्थानापित करना](media/Resource-Management-image54.png)

    <span data-ttu-id="e266a-316">इन बुकिंग और असाइनमेंट को नए रिसोर्स के साथ स्थानापित किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-316">The bookings and assignments are substituted with the new resource.</span></span>

    ![नए रिसोर्स के साथ स्थानापित बुकिंग और असाइनमेंट](media/Resource-Management-image55.png)

## <a name="reconcile-team-member-bookings-and-assignments"></a><span data-ttu-id="e266a-318">टीम सदस्य की बुकिंग और असाइनमेंट का समाधान करना</span><span class="sxs-lookup"><span data-stu-id="e266a-318">Reconcile team member bookings and assignments</span></span>

<span data-ttu-id="e266a-319">टीम सदस्यों के लिए, बुकिंग और असाइनमेंट आपस में उतने संबंधित नहीं होते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-319">For team members, bookings and assignments are loosely coupled.</span></span> <span data-ttu-id="e266a-320">दूसरे शब्दों में, रिसोर्स के पास असाइनमेंट हो सकते हैं लेकिन कोई बुकिंग नहीं या उनके पास बुकिंग हो सकती है लेकिन असाइनमेंट नहीं।</span><span class="sxs-lookup"><span data-stu-id="e266a-320">In other words, resources can have assignments but no bookings, or they can have bookings but no assignments.</span></span> <span data-ttu-id="e266a-321">आदर्श स्थिति वह होगी कि बुकिंग और असाइनमेंट संतुलित हो ताकि रिसोर्स के पास टास्क असाइनमेंट पूरा करने की प्रतिबद्ध क्षमता हो।</span><span class="sxs-lookup"><span data-stu-id="e266a-321">Ideally, bookings and assignments should be aligned, so that resources have committed capacity to perform the task assignments.</span></span> <span data-ttu-id="e266a-322">बहरहाल, बुकिंग उपलब्धता पर आधारित हो सकते हैं और टास्क का समय परियोजना के जारी रहने पर बदल सकता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-322">However, the bookings might be based on availability, and task timings might change as the project continues.</span></span> <span data-ttu-id="e266a-323">इसलिए, बुकिंग और असाइनमेंट का आपस में अधिक संबंधित न होने से लोचता रहती है।</span><span class="sxs-lookup"><span data-stu-id="e266a-323">Therefore, the loose coupling of bookings and assignments provides flexibility.</span></span>

<span data-ttu-id="e266a-324">PSA में **रीकन्सीलिएशन** टैब होता है जिससे प्रोजेक्ट मैनेजर टीम के सदस्यों की बुकिंग और प्रोजेक्ट टीमों के लिए उनके असाइनमेंट का समाधान कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-324">PSA has a **Reconciliation** tab that lets project managers reconcile team members' bookings and their assignments for project teams.</span></span>

![रीकन्सीलिएशन टैब](media/Resource-Management-image56.png)

<span data-ttu-id="e266a-326">**रीकन्सीलिएशन** टैब टीम के प्रत्येक सदस्य को सौंपे गए टास्क के स्तर तक के बुकिंग और असाइनमेंट दिखाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-326">The **Reconciliation** tab shows bookings and assignments down to the level of the individual task assignment for each team member.</span></span> <span data-ttu-id="e266a-327">यह सेल में उन घंटों को दिखाता है जो माह से लेकर दिनों तक की समय अवधि बताता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-327">It shows hours in cells that represent time periods from months down to days.</span></span>

<span data-ttu-id="e266a-328">यह टैब कुल कॉलम के साथ-साथ प्रोजेक्ट का समग्र निवल कुल भी दिखाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-328">The tab also shows an overall net total for the project, together with a total column.</span></span>

<span data-ttu-id="e266a-329">प्रत्येक रिसोर्स के लिए, यह टैब टीम के सदस्य की बुकिंग और टीम सदस्य के टास्क असाइनमेंट के रोलअप के बीच के अंतर का भी परिकलन करता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-329">For each resource, the tab calculates the difference between the team member's bookings and a rollup of the team member's task assignments.</span></span> <span data-ttu-id="e266a-330">आदर्श रूप में यह अंतर 0 (शून्य) होना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="e266a-330">Ideally, this difference should be 0 (zero).</span></span> <span data-ttu-id="e266a-331">दूसरे शब्दों में, बुकिंग और असाइनमेंट के बीच कोई अंतर नहीं होना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="e266a-331">In other words, there should be no difference between bookings and assignments.</span></span> <span data-ttu-id="e266a-332">अंतरों को रंग और छाया से दिखाया जाता है ताकि दो परिस्थितियों की ओर ध्यान जाए:</span><span class="sxs-lookup"><span data-stu-id="e266a-332">Differences are colored and shaded to draw attention to two conditions:</span></span>

- <span data-ttu-id="e266a-333">**बुकिंग शॉर्टेज** – बुकिंग की कमी तब होती है जब किसी रिसोर्स के पास बुकिंग से अधिक असाइनमेंट होते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-333">**Booking shortage** – A booking shortage occurs when a resource has more assignments than bookings.</span></span> <span data-ttu-id="e266a-334">क्योंकि इस क्षमता को आरक्षित नहीं किया गया, प्रोजेक्ट मैनेजर इस कमी को दूर करने के लिए रिसोर्स की बुकिंग को बढ़ाते हुए इस परिस्थिति को ठीक करना चाहेंगे।</span><span class="sxs-lookup"><span data-stu-id="e266a-334">Because this capacity hasn't been reserved, a project manager might want to correct this condition by extending the resource's bookings to cover the deficit.</span></span>
- <span data-ttu-id="e266a-335">**बुकिंग विस्तारित करें** – एक्सेस बुकिंग तब होती है जब रिसोर्स को प्रोजेक्ट के लिए बुक तो किया गया है लेकिन उसे टास्क नहीं दिया गया।</span><span class="sxs-lookup"><span data-stu-id="e266a-335">**Excess bookings** – Excess bookings occur when a resource has been booked to the project but hasn't been assigned to tasks.</span></span> <span data-ttu-id="e266a-336">यह परिस्थिति ऐसे मामलों में स्वीकार्य होगी जहाँ रिसोर्स को टास्क असाइनमेंट से पहले ही प्रोजेक्ट के लिए बुक किया गया हो।</span><span class="sxs-lookup"><span data-stu-id="e266a-336">This condition might be acceptable in the cases where the resource was booked to the project before task assignment occurred.</span></span> <span data-ttu-id="e266a-337">बहरहाल, दूसरे मामलों में, रिसोर्स को टास्क सौंपने की योजना नहीं है।</span><span class="sxs-lookup"><span data-stu-id="e266a-337">However, in other cases, the resource isn't planned to be assigned to tasks.</span></span> <span data-ttu-id="e266a-338">इन मामलों में, परियोजना प्रबंधक को रिसोर्स की बुकिंग कैंसल करने पर विचार करना चाहिए ताकि क्षमता का उपयोग दूसरे प्रोजेक्ट में किया जा सके।</span><span class="sxs-lookup"><span data-stu-id="e266a-338">In these cases, the project manager should consider canceling the resource's bookings, so that the capacity can be used for another project.</span></span>

<span data-ttu-id="e266a-339">कुछ मामलों में, जब आप दिन के स्तर की तुलना में अधिक स्तर पर समय देखते हैं (जैसे माह का स्तर), तो हो सकता है कि आप रिसोर्स के लिए शून्य का निवल अंतर देखें (दूसरे शब्दों में, बुकिंग = असाइनमेंट)।</span><span class="sxs-lookup"><span data-stu-id="e266a-339">In some cases, when you view time at a higher level than the day level (for example, the month level), you might see a net difference of zero for a resource (in other words, bookings = assignments).</span></span> <span data-ttu-id="e266a-340">बहरहाल, यदि आप सप्ताह के स्तर पर समय देखते हैं, तो आप पहले सप्ताह शून्य घंटे का असाइनमेंट और 40 घंटों की बुकिंग देख सकते हैं लेकिन वहीं दूसरे सप्ताह 40 घंटों का असाइनमेंट और शून् घंटे की बुकिंग भी दिख सकती है।</span><span class="sxs-lookup"><span data-stu-id="e266a-340">However, if you view time at the week level, you might see that there are assignments of zero hours and bookings of 40 hours in the first week, but assignments of 40 hours and bookings of zero hours in the second week.</span></span> <span data-ttu-id="e266a-341">कुल मिलाकर, बुकिंग और असाइमेंट का समाधान किया जाता है लेकिन एक सप्ताह से दूसरे सप्ताह में उनमें अंतर होता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-341">Overall, the bookings and assignments are reconciled, but they differ from one week to the next.</span></span>

<span data-ttu-id="e266a-342">जब आप समय को उच्चतर स्तरों पर देखते हैं, तो **रीकन्सीलिएशन** टैब के सेल में आपको सूचना देने के लिए एक इंडीकेटर होता है कि निम्नतर स्तरों में अंतर है।</span><span class="sxs-lookup"><span data-stu-id="e266a-342">When you view time at higher levels, cells in the **Reconciliation** tab have an indicator to inform you that there are differences at lower levels.</span></span> <span data-ttu-id="e266a-343">सेल पर डबल-क्लिक करते हुए, आप इस अंतर को ज़ूम कर देख सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-343">By double-clicking in a cell, you can zoom in to view the difference.</span></span> <span data-ttu-id="e266a-344">इसके बाद आप ज़ूम से वापस आने के लिए उस पर राइट-क्लिक कर सकते हैं। रिसोर्स को चुनते हुए और ग्रिड के टूलबार पर **नेक्स्ट डिफरेंस** कंट्रोल का इस्तेमाल करते हुए, आप उस रिसोर्स की बुकिंग और असाइनमेंट के बीच के अगले अंतर में जा सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-344">You can then right-click to zoom out. By selecting a resource and then using the **Next difference** control on the grid toolbar, you can go to the next difference between bookings and assignments for that resource.</span></span> <span data-ttu-id="e266a-345">वापस जाने के लिए आप **प्रिवियस डिफरेंस** कंट्रोल का इस्तेमाल कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-345">You can then use the **Previous difference** control to go back.</span></span> <span data-ttu-id="e266a-346">आप **सेटिंग्स** के तहत डिफरेंस इंडीकेटर और नेवीगेशन बिहेवियर को बंद भी कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-346">You can also turn off the difference indicator and navigation behavior under **Settings**.</span></span>

![डिफरेंस इंडीकेटर](media/Resource-Management-image57.png)

<span data-ttu-id="e266a-348">यदि आपके पास रिसोर्स के लिए टास्क असाइनमेंट तो है लेकिन कोई बुकिंग नहीं है, तो **प्रोजेक्ट्स** पेज पर, **रीकन्सीलिएशन** टैब पर, बुकिंग शॉर्टेज चुनें और उसके बाद **एक्सटेंड बुकिंग** चुनें।</span><span class="sxs-lookup"><span data-stu-id="e266a-348">If you have task assignments for a resource but no bookings, on the **Projects** page, on the **Reconciliation** tab, select the booking shortage, and then select **Extend Booking**.</span></span> <span data-ttu-id="e266a-349">**एक्सटेंड बुकिंग** डॉयलॉग बॉक्स दिखेगा जो रिसोर्स की कमी को पूरा करने के लिए आवश्यक बुकिंग दिखाएगा।</span><span class="sxs-lookup"><span data-stu-id="e266a-349">The **Extend Booking** dialog box appears and shows the booking that is needed to address the resource's shortage.</span></span> <span data-ttu-id="e266a-350">यह सभी प्रोजेक्ट में या अन्य स्केड्यूल योग्य संस्थानों में रिसोर्स की मौजूदा बुकिंग भी दिखाता है।</span><span class="sxs-lookup"><span data-stu-id="e266a-350">It also shows the resource's existing bookings across all projects or other schedulable entities.</span></span> <span data-ttu-id="e266a-351">यदि आप रिसोर्स के लिए बुकिंग करने के लिए **ओके** चुनते हैं, तो उस रिसोर्स की उपलब्धता से संबंध न रखते हुए, हो सकता है कि आप ओवरबुकिंग कर लें।</span><span class="sxs-lookup"><span data-stu-id="e266a-351">If you select **OK** to create the booking for the resource, regardless of that resource's availability, you might cause overbooking.</span></span>

![बुकिंग डॉयलॉग बॉक्स को बढ़ाना](media/Resource-Management-image58.png)

<span data-ttu-id="e266a-353">इसके बाद प्रोजेक्ट मैनेजर या रिसोर्स मैनेजर किसी भी परिस्थिति जिसमें किसी रिसोर्स की क्षमता से अधिक ओवरबुकिंग की गई है, से निपटने के लिए स्केड्यूल बोर्ड का इस्तेमाल कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e266a-353">The project manager or resource manager can then use the Schedule Board to manage any situations where a resource is overbooked beyond its capacity.</span></span>
