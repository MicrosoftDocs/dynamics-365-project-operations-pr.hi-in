---
title: प्रोजेक्ट सेटिंग्‍स
description: इस विषय में प्रोजेक्ट प्रबंधन सेटिंग की जानकारी दी गई है।
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
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
ms.openlocfilehash: c9b8659f3b7ee81d2e21ef52743debd521fa9bb9
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077863"
---
# <a name="project-settings"></a><span data-ttu-id="b351f-103">प्रोजेक्ट सेटिंग्‍स</span><span class="sxs-lookup"><span data-stu-id="b351f-103">Project settings</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="b351f-104">प्रोजेक्ट प्लानिंग सुविधाएँ प्राप्त करने के लिए निम्नलिखित सेटिंग का इस्तेमाल करें।</span><span class="sxs-lookup"><span data-stu-id="b351f-104">Use the following settings to access the project planning features.</span></span>

## <a name="work-template"></a><span data-ttu-id="b351f-105">कार्य टेम्‍पलेट</span><span class="sxs-lookup"><span data-stu-id="b351f-105">Work template</span></span>

<span data-ttu-id="b351f-106">प्रोजेक्ट शेड्यूल बनाने के लिए, आपको प्रोजेक्ट कैलेंडर टैम्पलेट बनाना होगा जिसमें प्रति दिन के कार्य घंटे और किसी कारोबार के बंद होने की संख्या परिभाषित की जाती है।</span><span class="sxs-lookup"><span data-stu-id="b351f-106">To create a project schedule, you create a project calendar template that defines the number of working hours per day and any business closures.</span></span> <span data-ttu-id="b351f-107">प्रोजेक्ट कैलेंडर टैम्पलेट बनाने के लिए, आपको प्रोजेक्ट के **कैलेंडर टैम्पलेट** फील्ड के साथ कार्य टैम्पलेट से जुड़ना होगा.</span><span class="sxs-lookup"><span data-stu-id="b351f-107">To create a project calendar template, you associate a work template with the **Calendar template** field for the project.</span></span> <span data-ttu-id="b351f-108">कार्य टैम्पलेट बनाने के लिए निम्नलिखित चरणों को पूरा करें।</span><span class="sxs-lookup"><span data-stu-id="b351f-108">Follow these steps to create a work template.</span></span>

1. <span data-ttu-id="b351f-109">PSA में, बाएँ नेवीगेशन पैन में, **संसाधन** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="b351f-109">In PSA, in the left navigation pane, click **Resources**.</span></span> 
2. <span data-ttu-id="b351f-110">**संसाधन** लिस्ट पेज में, यूज़र रिकार्ड खालें और उसके बाद **काम के घंटे दिखाएं** चुनें।</span><span class="sxs-lookup"><span data-stu-id="b351f-110">On the **Resources** list page, open a user record, and then select **Show Work Hours**.</span></span>

  > [!NOTE]
  > <span data-ttu-id="b351f-111">सुनिश्चित करें कि आप ब्राउज़र पेज में पॉप-अप को अनुमत करते हैं।</span><span class="sxs-lookup"><span data-stu-id="b351f-111">Make sure that you allow pop-ups on the browser page.</span></span> <span data-ttu-id="b351f-112">इससे आप संसाधन के कार्य के घंटे देख सकेंगे।</span><span class="sxs-lookup"><span data-stu-id="b351f-112">This lets you see the work hours set for the resource.</span></span>
  
3. <span data-ttu-id="b351f-113">**मासिक दृश्य** टैब पर, **सेट अप** क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="b351f-113">On the **Monthly View** tab, click **Set Up**.</span></span> <span data-ttu-id="b351f-114">तीन विकल्पों की सूची दिखेगा:</span><span class="sxs-lookup"><span data-stu-id="b351f-114">A list of three options appears:</span></span> 

  - <span data-ttu-id="b351f-115">नया साप्ताहिक शेड्यूल</span><span class="sxs-lookup"><span data-stu-id="b351f-115">New Weekly Schedule</span></span>
  - <span data-ttu-id="b351f-116">एक दिन के लिए कार्य शेड्यूल</span><span class="sxs-lookup"><span data-stu-id="b351f-116">Work Schedule for One Day</span></span>
  - <span data-ttu-id="b351f-117">समय समाप्त</span><span class="sxs-lookup"><span data-stu-id="b351f-117">Time Off</span></span>

> ![सेट अप विकल्प](media/project-13.png)

4. <span data-ttu-id="b351f-119">**नया साप्ताहिक शेड्यूल** चुनें और उसके बाद इस रिसोर्स के शेड्यूल के लिए ऑप्शन सेट करें।</span><span class="sxs-lookup"><span data-stu-id="b351f-119">Select **New Weekly Schedule** , and then set the options for this resource schedule.</span></span> <span data-ttu-id="b351f-120">इसमें आप आवर्ती साप्ताहिक शेड्यूल, दैनिक घंटा पैरामीटर, कारोबार समाप्ति जैसी कई सुविधाएँ सेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="b351f-120">You can set a recurring weekly schedule, daily hour parameters, business closures, and more.</span></span>
5. <span data-ttu-id="b351f-121">डेट रेंज सेट करें, **सहेजें** चुनें और उसके बाद **बंद करें** क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="b351f-121">Set the date range, select **Save** , and then click **Close**.</span></span> 
6. <span data-ttu-id="b351f-122">**संसाधन** लिस्ट पेज पर वापस जाएँ और उस संसाधन को चुनें जिसे आपने कार्य घंटों के लिए सेट किया था।</span><span class="sxs-lookup"><span data-stu-id="b351f-122">Go back to the **Resources** list page, and select the resource that you set the work hours for.</span></span> 
7. <span data-ttu-id="b351f-123">कार्य टैम्पलेट सेट करने के लिए **कैलेंडर को इस रूप में सेट करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="b351f-123">Select **Set Calendar As** to set the work template.</span></span> 
8. <span data-ttu-id="b351f-124">**कार्य टेम्‍पलेट** डॉयलॉग बॉक्स में कार्य टैम्पलेट का नाम दर्ज करें और उसके बाद **लागू करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="b351f-124">In the **Work Template** dialog box, enter a name for the work template, and then select **Apply**.</span></span> 

<span data-ttu-id="b351f-125">अब आप वर्क टैम्पलेट को प्रोजेक्ट कैलेंडर के टैम्पलेट से जोड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="b351f-125">You can now associate the work template with a project calendar template.</span></span>

## <a name="resource-roles"></a><span data-ttu-id="b351f-126">संसाधन भूमिकाएं</span><span class="sxs-lookup"><span data-stu-id="b351f-126">Resource roles</span></span>

<span data-ttu-id="b351f-127">शब्द *संसाधन भूमिकाएं* उन कौशल, सक्षमताओं और प्रमाणीकरणों से संबंधित है जिन्हें प्रोजेक्ट पर विशेष प्रकार के टास्क करने के लिए एक व्यक्ति में होने चाहिए।</span><span class="sxs-lookup"><span data-stu-id="b351f-127">The term *resource role* refers to the set of skills, competencies, and certifications that a person must have to perform a specific set of tasks on a project.</span></span> <span data-ttu-id="b351f-128">PSA से आप उस भूमिका पर रिसोर्स के समय पर आधारित लागत और बिल बना सकते हैं जिससे रिसोर्स संबद्ध है।</span><span class="sxs-lookup"><span data-stu-id="b351f-128">PSA lets you cost and bill a resource's time based on the role that the resource is associated with.</span></span> <span data-ttu-id="b351f-129">प्रत्येक संगठन को **Project Service** मेन्यू में बाएँ नेवीगेशन का इस्तेमाल करते हुए इन भूमिकाओं को सेट करना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="b351f-129">Every organization must set up these roles by using the left navigation on the **Project Service** menu.</span></span>

<span data-ttu-id="b351f-130">प्रत्येक संगठन को **सक्रिय संसाधन श्रेणियाँ** पेज पर इन भूमिकाओं को सेट करना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="b351f-130">Every organization must set up these roles on the **Active Resource Categories** page.</span></span> <span data-ttu-id="b351f-131">इस पेज को खोलने के लिए, बाएँ नेवीगेशन पैन में, **संसाधन की भूमिकाएं** चुनें।</span><span class="sxs-lookup"><span data-stu-id="b351f-131">To open this page, in the left navigation pane, select **Resource Roles**.</span></span>

## <a name="price-lists"></a><span data-ttu-id="b351f-132">मूल्य सूचियाँ</span><span class="sxs-lookup"><span data-stu-id="b351f-132">Price lists</span></span>

<span data-ttu-id="b351f-133">कीमत की सूचियों से आप एक संगठन में संसाधन की भूमिकाओं, खर्च के वर्गों, प्रॉडक्ट और अन्य तत्वों के लिए लागत और बिक्री की कीमत सेट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="b351f-133">Price lists let you set cost and sales prices for resource roles, expense categories, products, and other elements in an organization.</span></span> <span data-ttu-id="b351f-134">किसी प्रोजेक्ट के लिए किए जाने वाले कार्य का वित्तीय आकलन सेट करने से पहले, आपको बैकिंग लागत और बिक्री कीमत सूची तैयार करनी चाहिए।</span><span class="sxs-lookup"><span data-stu-id="b351f-134">Before you set financial estimates for the work that must be delivered for a project, you should create a backing cost and sales price list.</span></span> <span data-ttu-id="b351f-135">पैरामीटर खंड में, आपको डिफाल्ट लागत और बिक्री कीमत सूची भी सेट करनी चाहिए जो संगठन में बनाए गए सभी प्रोजेक्ट के लिए लागू होते हैं।</span><span class="sxs-lookup"><span data-stu-id="b351f-135">In the parameters section, you should also set up a default cost and sales price list that applies to all projects that are created in the organization.</span></span> <span data-ttu-id="b351f-136">**सक्रिय परियोजना पैरामीटर्स** पेज में यह सुनिश्चित करें कि आपने डिफाल्ट लागत और बिक्री कीमत सूची सेट कर ली है।</span><span class="sxs-lookup"><span data-stu-id="b351f-136">On the **Active Project Parameters** page, make sure that you set up a default cost and sales price list.</span></span>
