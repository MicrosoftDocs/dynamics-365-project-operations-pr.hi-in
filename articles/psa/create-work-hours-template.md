---
title: कार्य घंटों का एक टेम्पलेट बनाएँ
description: Project Service में कार्य घंटों का टेम्पलेट बनाने का तरीका
author: ruhercul
manager: kfend
ms.service: project-operations
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
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: a0fce327587940e557e0214c8c0897116ac91901
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4133055"
---
# <a name="create-a-work-hours-template-project-service"></a><span data-ttu-id="3d2f9-103">कार्य घंटों का टेम्पलेट बनाना (Project Service)</span><span class="sxs-lookup"><span data-stu-id="3d2f9-103">Create a work hours template (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="3d2f9-104">परियोजना शेड्यूल बनाने से पहले, आपको एक ऐसा परियोजना कैलेंडर सेट अप करना होगा, जो शेड्यूल और किसी भी व्यवसाय बंदी के दौरान प्रति दिन समायोजित किए जाने वाले कार्य के घंटों की संख्या निर्धारित करें.</span><span class="sxs-lookup"><span data-stu-id="3d2f9-104">Before you can create project schedules, you need to set up a project calendar that defines the number of working hours to accommodate per day in the schedule and any business closures.</span></span> <span data-ttu-id="3d2f9-105">आप ऐसा कार्य घंटे टेम्पलेट के साथ कर सकते हैं, जिसमें प्रति दिन के कार्य घंटे, कार्य बंदी वाले दिन और अन्य व्यवसाय बंदी का विवरण शामिल होता है.</span><span class="sxs-lookup"><span data-stu-id="3d2f9-105">You do this with a work hours template, which contains details about work hours per day, days off, and any other business closures.</span></span>  
  
 <span data-ttu-id="3d2f9-106">जब आप कोई परियोजना बनाते हैं, तो आप परियोजना के लिए शेड्यूल लागू करने हेतु परियोजना कैलेंडर के साथ एक कार्य टेम्पलेट संबद्ध करते हैं.</span><span class="sxs-lookup"><span data-stu-id="3d2f9-106">When you’re creating a project, you associate a work template to the project calendar to apply the schedule for the project.</span></span>  
  
 <span data-ttu-id="3d2f9-107">आप कार्य घंटे टेम्पलेट को दो तरीकों से बना सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="3d2f9-107">There are two ways you can create a work hours template:</span></span>  
  
-   <span data-ttu-id="3d2f9-108">संसाधन के कैलेंडर के आधार पर कार्य घंटों का एक टेम्पलेट बनाएँ.</span><span class="sxs-lookup"><span data-stu-id="3d2f9-108">Create a work hours template based on a resource’s calendar.</span></span>  
  
-   <span data-ttu-id="3d2f9-109">कार्य घंटों का एक नया टेम्पलेट बनाएँ.</span><span class="sxs-lookup"><span data-stu-id="3d2f9-109">Create a new work hours template.</span></span>  
  
#### <a name="to-create-a-work-hours-template-based-on-a-resources-calendar"></a><span data-ttu-id="3d2f9-110">संसाधन के कैलेंडर पर आधारित कार्य घंटे टेम्पलेट बनाने के लिए</span><span class="sxs-lookup"><span data-stu-id="3d2f9-110">To create a work hours template based on a resource’s calendar</span></span>  
  
1.  <span data-ttu-id="3d2f9-111">**Project Service > संसाधन** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="3d2f9-111">Go to **Project Service > Resources**.</span></span>  
  
2.  <span data-ttu-id="3d2f9-112">वह संसाधन चुनें, जिस पर आप अपने कार्य घंटों को आधारित करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="3d2f9-112">Select the resource you want to base your work hours on.</span></span>  
  
3.  <span data-ttu-id="3d2f9-113">**कैलेंडर को इस रूप में सहेजें** पर क्लिक करें, कार्य घंटों के टेम्पलेट के लिए कोई नाम दर्ज करें और उसके बाद **सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="3d2f9-113">Click **Save Calendar As**, enter a name for the work hours template, and then click **Save**.</span></span>  
  
4.  <span data-ttu-id="3d2f9-114">विकल्पों को बदलना पूर्ण करने के बाद, **सहेजें और बंद करें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="3d2f9-114">When you’re done changing options, click **Save and Close**.</span></span>  
  
5.  <span data-ttu-id="3d2f9-115">स्‍क्रीन के निचले दाएँ कोने में स्थित **सहेजें** बटन पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="3d2f9-115">Click the **Save** button at the bottom right corner of the screen.</span></span>  
  
#### <a name="to-create-a-new-work-hours-template"></a><span data-ttu-id="3d2f9-116">नया कार्य घंटे टेम्पलेट बनाने के लिए</span><span class="sxs-lookup"><span data-stu-id="3d2f9-116">To create a new work hours template</span></span>  
  
1.  <span data-ttu-id="3d2f9-117">**Project Service > कार्य घंटों का टेम्पलेट** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="3d2f9-117">Go to **Project Service > Work Hours Templates**.</span></span>  
  
2.  <span data-ttu-id="3d2f9-118">**नया** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="3d2f9-118">Click **New**.</span></span>  
  
3.  <span data-ttu-id="3d2f9-119">कार्य घंटों के टेम्पलेट के लिए कोई नाम दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="3d2f9-119">Enter a name for the work hours template.</span></span>  
  
4.  <span data-ttu-id="3d2f9-120">कार्य घंटों को संसांधन पर आधारित करने के लिए कोई संसाधन चुनें और उसके बाद **सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="3d2f9-120">Select a resource to base the work hours on, and then click **Save**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="3d2f9-121">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="3d2f9-121">See Also</span></span>  
 [<span data-ttu-id="3d2f9-122">संसाधन सेट अप करें</span><span class="sxs-lookup"><span data-stu-id="3d2f9-122">Set up resources</span></span>](../psa/set-up-resources.md)
