---
title: कार्य विश्लेषण संरचना वाली एक परियोजना शेड्यूल करें
description: Project Service में कार्य विश्लेषण संरचना वाली एक परियोजना को शेड्यूल करने का तरीका
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
ms.openlocfilehash: cf12cc3bcf061e1daffafb248cfd76809c6444ec
ms.sourcegitcommit: 418fa1fe9d605b8faccc2d5dee1b04b4e753f194
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/10/2021
ms.locfileid: "5149815"
---
# <a name="schedule-a-project-with-a-work-breakdown-structure-project-service"></a><span data-ttu-id="14e48-103">कार्य विश्लेषण संरचना वाली एक परियोजना को शेड्यूल करना (Project Service)</span><span class="sxs-lookup"><span data-stu-id="14e48-103">Schedule a project with a work breakdown structure (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="14e48-104">परियोजना शेड्यूल यह बताता है कि कौन-कौन से कार्य किए जाने हैं, कौन-कौन से संसाधन कार्य करेंगे, और उस कार्य को किस समय सीमा में पूरा किया जाना आवश्यक है.</span><span class="sxs-lookup"><span data-stu-id="14e48-104">A project schedule communicates what work needs to be performed, which resources will perform the work, and the timeframe in which that work needs to be completed.</span></span> <span data-ttu-id="14e48-105">परियोजना शेड्यूल में परियोजना को समय पर डिलीवर करने से संबंधित सभी कार्य दर्शाए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="14e48-105">The project schedule reflects all the work associated with delivering the project on time.</span></span> <span data-ttu-id="14e48-106">परियोजना की शुरूआती अवस्‍था का एक प्रथम चरण पर यह है कि परियोजना शेड्यूल बनाया जाए.</span><span class="sxs-lookup"><span data-stu-id="14e48-106">One of the first steps in the initiation phase of the project is to come up with a project schedule.</span></span> <span data-ttu-id="14e48-107">एक परियोजना शेड्यूल स्थापित करने के लिए, आपको एक कार्य विश्लेषण संरचना बनानी होगी.</span><span class="sxs-lookup"><span data-stu-id="14e48-107">To establish a project schedule, you need to create a work breakdown structure.</span></span>  
  
 <span data-ttu-id="14e48-108">कार्य विश्लेषण संरचना के साथ एक परियोजना संरचना बनाएँ, इससे आपको निम्न में मदद मिलेगी:</span><span class="sxs-lookup"><span data-stu-id="14e48-108">Create a project structure with a work breakdown structure, which helps you:</span></span>  
  
- <span data-ttu-id="14e48-109">कार्य को प्रबंध किए जा सकने योग्‍य कार्यों में विभाजित करने में</span><span class="sxs-lookup"><span data-stu-id="14e48-109">Break down work into manageable tasks</span></span>  
  
- <span data-ttu-id="14e48-110">किसी कार्य को पूरा करने के लिए आवश्यक समय का अनुमान लगाने में</span><span class="sxs-lookup"><span data-stu-id="14e48-110">Estimate the time required to complete a task</span></span>  
  
- <span data-ttu-id="14e48-111">कार्य निर्भरताएँ और कार्य अवधि सेट करने में</span><span class="sxs-lookup"><span data-stu-id="14e48-111">Set task dependencies and task duration</span></span>  
  
- <span data-ttu-id="14e48-112">प्रत्येक कार्य को पूर्ण करने के लिए आवश्यक भूमिकाएँ निर्धारित करने में</span><span class="sxs-lookup"><span data-stu-id="14e48-112">Determine the roles required to complete each task</span></span>  
  
  <span data-ttu-id="14e48-113">कार्य विश्लेषण संरचना में परियोजना शेड्यूल का रूप और अनुभव जाना-पहचाना होता है, एक इंटरैक्टिव गैंट चार्ट के साथ पूर्ण होता है.</span><span class="sxs-lookup"><span data-stu-id="14e48-113">The project schedule in the work breakdown structure has a familiar look and feel, complete with an interactive Gantt chart.</span></span>  
  
## <a name="create-a-work-breakdown-structure-for-a-project"></a><span data-ttu-id="14e48-114">परियोजना के लिए एक कार्य विश्लेषण संरचना बनाएँ</span><span class="sxs-lookup"><span data-stu-id="14e48-114">Create a work breakdown structure for a project</span></span>  
 <span data-ttu-id="14e48-115">परियोजना में कार्यों का अनुक्रम बताने के लिए कार्य विश्लेषण संरचना बनाएँ.</span><span class="sxs-lookup"><span data-stu-id="14e48-115">Create a work breakdown structure to represent the sequence of tasks in a project.</span></span> <span data-ttu-id="14e48-116">कार्य विश्लेषण संरचना में कार्य, प्रत्येक कार्य के लिए आवश्‍यकताएँ, और आय और लागत की जानकारी शामिल होती है.</span><span class="sxs-lookup"><span data-stu-id="14e48-116">The work breakdown structure includes tasks, requirements for each task, and revenue and cost information.</span></span> <span data-ttu-id="14e48-117">अपनी कार्य विश्लेषण संरचना में, आप जोड़ सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="14e48-117">In your work breakdown structure, you can add:</span></span>  
  
-   <span data-ttu-id="14e48-118">पदानुक्रम में कार्यों का क्रम</span><span class="sxs-lookup"><span data-stu-id="14e48-118">The sequence of tasks in a hierarchy</span></span>  
  
-   <span data-ttu-id="14e48-119">अन्‍य ऐसे कार्य, यदि कोई हों तो, जिन्‍हें किसी कार्य को शुरू करने के पहले पूर्ण किया जाना आवश्‍यक है</span><span class="sxs-lookup"><span data-stu-id="14e48-119">Other tasks, if any, that must be completed before a task can be started</span></span>  
  
-   <span data-ttu-id="14e48-120">किसी कार्य का प्रारंभ दिनांक, समाप्ति दिनांक, और कार्य की अवधि</span><span class="sxs-lookup"><span data-stu-id="14e48-120">The starting date, ending date, and duration of a task</span></span>  
  
-   <span data-ttu-id="14e48-121">कार्य के लिए आवश्यक घंटों की संख्या</span><span class="sxs-lookup"><span data-stu-id="14e48-121">The number of hours required for a task</span></span>  
  
-   <span data-ttu-id="14e48-122">कार्यकर्ता के लिए आवश्यक कोई कौशल और शिक्षा</span><span class="sxs-lookup"><span data-stu-id="14e48-122">Any required worker skills and education</span></span>  
  
-   <span data-ttu-id="14e48-123">वे कार्यकर्ता, जिन्हें एक कार्य असाइन किया गया है</span><span class="sxs-lookup"><span data-stu-id="14e48-123">The workers who are assigned to a task</span></span>  
  
-   <span data-ttu-id="14e48-124">अनुमानित आय और लागत</span><span class="sxs-lookup"><span data-stu-id="14e48-124">Estimated revenue and costs</span></span>  
  
## <a name="task-types"></a><span data-ttu-id="14e48-125">कार्य प्रकार</span><span class="sxs-lookup"><span data-stu-id="14e48-125">Task types</span></span>  
<span data-ttu-id="14e48-126">आप कार्य विश्लेषण संरचना बनाते समय निम्न प्रकार के कार्यों का उपयोग करेंगे:</span><span class="sxs-lookup"><span data-stu-id="14e48-126">You’ll use the following types of tasks when creating your work breakdown structure:</span></span>  

| | | 
|---------------------------------------|-----------------------------------------------------------------| 
| <span data-ttu-id="14e48-127">**परियोजना रूट नोड**</span><span class="sxs-lookup"><span data-stu-id="14e48-127">**Project root node**</span></span> | <span data-ttu-id="14e48-128">परियोजना के लिए शीर्ष-स्तरीय सारांश कार्य.</span><span class="sxs-lookup"><span data-stu-id="14e48-128">The top-level summary task for the project.</span></span> <span data-ttu-id="14e48-129">सभी अन्य परियोजना कार्य इसके अंतर्गत बनाए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="14e48-129">All other project tasks are created under it.</span></span> <span data-ttu-id="14e48-130">रूट कार्य का नाम परियोजना का नाम होता है.</span><span class="sxs-lookup"><span data-stu-id="14e48-130">The name of the root task is the project name.</span></span> <span data-ttu-id="14e48-131">रूट नोड का प्रयास, दिनांक, और अवधि, इससे नीचे के पदानुक्रम के मानों पर आधारित होती है.</span><span class="sxs-lookup"><span data-stu-id="14e48-131">The effort, dates, and duration of the root node are based on the values on the hierarchy below it.</span></span> <span data-ttu-id="14e48-132">आप रूट नोड गुण को संपादित नहीं कर सकते या रूट नोड नहीं हटा सकते.</span><span class="sxs-lookup"><span data-stu-id="14e48-132">You can’t edit root node properties or delete the root node.</span></span> | 
| <span data-ttu-id="14e48-133">**सारांश या कंटेनर कार्य**</span><span class="sxs-lookup"><span data-stu-id="14e48-133">**Summary or container tasks**</span></span> | <span data-ttu-id="14e48-134">सारांश कार्य वह कार्य है जिसके अंतर्गत उप-कार्य आते हैं.</span><span class="sxs-lookup"><span data-stu-id="14e48-134">A summary task is a task that has sub-tasks under it.</span></span> <span data-ttu-id="14e48-135">सारांश कार्य का स्‍वयं का कोई कार्य प्रभाव या लागत नहीं होती.</span><span class="sxs-lookup"><span data-stu-id="14e48-135">A summary task doesn’t have any work effort or cost of its own.</span></span> <span data-ttu-id="14e48-136">इसके कार्य प्रभाव और लागत इसके उप कार्यों के रोलअप होते हैं.</span><span class="sxs-lookup"><span data-stu-id="14e48-136">Its work effort and cost are a rollup of its sub-tasks.</span></span> <span data-ttu-id="14e48-137">आप एक सारांश कार्य का नाम परिवर्तित कर सकते हैं, परंतु आप प्रयास, दिनांक या अवधि परिवर्तित नहीं कर सकते, क्‍योंकि इनकी गणना स्‍वचालित रूप से होती है.</span><span class="sxs-lookup"><span data-stu-id="14e48-137">You can change the name of a summary task, but you can’t change the effort, dates, or duration, because those are automatically calculated.</span></span> <span data-ttu-id="14e48-138">किसी सारांश कार्य को हटाने से वह कार्य और उसके सभी उप-कार्य हट जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="14e48-138">Deleting a summary task deletes the task and all of its sub-tasks.</span></span>|  
| <span data-ttu-id="14e48-139">**लीफ़ नोड कार्य**</span><span class="sxs-lookup"><span data-stu-id="14e48-139">**Leaf node tasks**</span></span> | <span data-ttu-id="14e48-140">लीफ़ नोड कार्य परियोजना पर सर्वाधिक विस्तृत कार्य का प्रतिनिधित्व करता है.</span><span class="sxs-lookup"><span data-stu-id="14e48-140">A leaf node task represents the most detailed work on the project.</span></span> <span data-ttu-id="14e48-141">इसके पास एक अनुमानित प्रयास, संसाधनों की नियोजित संख्‍या, नियोजित प्रारंभ और समाप्ति दिनांक, और एक अवधि होती है.</span><span class="sxs-lookup"><span data-stu-id="14e48-141">It has an estimated effort, a planned number of resources, planned start and end dates, and a duration.</span></span>|

  
## <a name="task-hierarchy"></a><span data-ttu-id="14e48-142">कार्य पदानुक्रम</span><span class="sxs-lookup"><span data-stu-id="14e48-142">Task hierarchy</span></span>  
 <span data-ttu-id="14e48-143">आपके पास एक कार्य पदानुक्रम बनाते समय निम्नलिखित विकल्‍प होते हैं:</span><span class="sxs-lookup"><span data-stu-id="14e48-143">You have the following options when creating a task hierarchy:</span></span>  
  
- <span data-ttu-id="14e48-144">**कार्य जोड़ें**.</span><span class="sxs-lookup"><span data-stu-id="14e48-144">**Add task**.</span></span>   <span data-ttu-id="14e48-145">आप एक कार्य को उस स्थिति पर जोड़ सकते हैं, जिसे आप कार्य पदानुक्रम में चुनते हैं.</span><span class="sxs-lookup"><span data-stu-id="14e48-145">You can add a task at a position you choose in the task hierarchy.</span></span> <span data-ttu-id="14e48-146">यदि आप स्थिति का चयन नहीं करते, तो नया कार्य अंत में दिखाई देता है.</span><span class="sxs-lookup"><span data-stu-id="14e48-146">If you don’t select a position, your new task appears at the end.</span></span>  
  
- <span data-ttu-id="14e48-147">**इंडेंट कार्य**।</span><span class="sxs-lookup"><span data-stu-id="14e48-147">**Indent task**.</span></span>   <span data-ttu-id="14e48-148">किसी कार्य को उसके ठीक ऊपर के कार्य का चाइल्‍ड बनाने के लिए उसे इंडेंट करें.</span><span class="sxs-lookup"><span data-stu-id="14e48-148">Indent a task to make it a child of the task directly above it.</span></span>  
  
- <span data-ttu-id="14e48-149">**आउटडेंट कार्य**।</span><span class="sxs-lookup"><span data-stu-id="14e48-149">**Outdent task**.</span></span>   <span data-ttu-id="14e48-150">किसी कार्य को बनाने के लिए आउटडेंट करें जिससे वह अब अपने मूल पैरेंट कार्य का उप-कार्य नहीं रहता.</span><span class="sxs-lookup"><span data-stu-id="14e48-150">Outdent a task to make it so it’s no longer a sub-task of its original parent task.</span></span>  
  
- <span data-ttu-id="14e48-151">**ऊपर ले जाएँ और नीचे ले जाएँ**.</span><span class="sxs-lookup"><span data-stu-id="14e48-151">**Move up and Move down**.</span></span>   <span data-ttu-id="14e48-152">कार्यों को उसके पैरेंट कार्य के पदानुक्रम में ऊपर या नीचे ले जाएँ.</span><span class="sxs-lookup"><span data-stu-id="14e48-152">Move tasks up and down in the hierarchy of its parent task.</span></span> <span data-ttu-id="14e48-153">किसी कार्य को ऊपर या नीचे ले जाने से उसके प्रयास, लागत, दिनांक, या अवधि पर कोई प्रभाव नहीं पड़ता.</span><span class="sxs-lookup"><span data-stu-id="14e48-153">Moving a task up or down has no effect on its effort, cost, dates, or duration.</span></span>  
  
## <a name="task-attributes"></a><span data-ttu-id="14e48-154">कार्य एट्रिब्‍यूट</span><span class="sxs-lookup"><span data-stu-id="14e48-154">Task attributes</span></span>  
 <span data-ttu-id="14e48-155">किसी कार्य के नाम में पूर्ण किए जाने वाले कार्य का वर्णन होता है.</span><span class="sxs-lookup"><span data-stu-id="14e48-155">A task’s name describes the work that needs to be completed.</span></span> <span data-ttu-id="14e48-156">आप कार्य के शेड्यूल और उसके लिए स्‍टाफ़िंग आवश्‍यकता का वर्णन करने के लिए विभिन्न कार्य एट्रिब्‍यूट का उपयोग करते हैं.</span><span class="sxs-lookup"><span data-stu-id="14e48-156">You use various task attributes to describe the schedule and staffing requirements for the task.</span></span>  
  
### <a name="schedule-attributes"></a><span data-ttu-id="14e48-157">शेड्यूल एट्रिब्‍यूट</span><span class="sxs-lookup"><span data-stu-id="14e48-157">Schedule attributes</span></span>

 - <span data-ttu-id="14e48-158">कार्य का शेड्यूल निर्धारित करने के लिए **प्रयास के घंटे**, **संसाधनों की संख्या**, **प्रारंभ दिनांक**, **समाप्त दिनांक**, और **अवधि** पर मान असाइन करें.</span><span class="sxs-lookup"><span data-stu-id="14e48-158">Assign values to **Effort hours**, **Number of resources**, **Start date**, **End date**, and **Duration** to determine the schedule for the task.</span></span> 
 - <span data-ttu-id="14e48-159">**प्रयास** वह अनुमानित घंटे हैं जो कार्य को पूर्ण करने के लिए लगते हैं.</span><span class="sxs-lookup"><span data-stu-id="14e48-159">**Effort** is an estimate of the hours it takes to complete the task.</span></span>
 - <span data-ttu-id="14e48-160">**संसाधनों की संख्या** परियोजना प्रबंधक द्वारा कार्य पर लगने वाला वह अनुमान है ताकि यथासंभव उत्तम शेड्यूल बनाने में मदद मिल सके.</span><span class="sxs-lookup"><span data-stu-id="14e48-160">**Number of resources** is an estimate that the project manager puts in the task to help come up with the best possible schedule.</span></span> 
 - <span data-ttu-id="14e48-161">**अवधि** (दिनों में) दिनों की संख्या बताता है जो कार्य को पूर्ण करने में लगेंगे.</span><span class="sxs-lookup"><span data-stu-id="14e48-161">**Duration** (in days) indicates the number of work days it will take to complete the task.</span></span>  
  
### <a name="staffing-attributes"></a><span data-ttu-id="14e48-162">स्‍टाफ़िंग एट्रिब्‍यूट</span><span class="sxs-lookup"><span data-stu-id="14e48-162">Staffing attributes</span></span>

 - <span data-ttu-id="14e48-163">**भूमिका**, **संसाधन संगठनात्मक इकाई**, **संसाधनों की संख्या**, और **संसाधन** कार्य के लिए स्‍टाफ़िंग आवश्यकताओं का वर्णन करते हैं.</span><span class="sxs-lookup"><span data-stu-id="14e48-163">**Role**, **Resource organizational unit**, **Number of resources**, and **Resources** describe the staffing requirements for the task.</span></span> 
 - <span data-ttu-id="14e48-164">**भूमिका** कार्य करने के लिए आवश्यक संसाधन के प्रकार का वर्णन करता है.</span><span class="sxs-lookup"><span data-stu-id="14e48-164">**Role** describes the type of resource needed to perform the task.</span></span> 
 - <span data-ttu-id="14e48-165">**संसाधन संगठनात्मक इकाई** उस संगठनात्मक इकाई को इंगित करता है जिससे उस कार्य के लिए संसाधनों को स्‍टाफ़ किया जाना चाहिए; इससे कार्य के लागत और विक्रय अनुमान पर भी प्रभाव पड़ता है, क्‍योंकि संसाधन के लिए इकाई विक्रय मूल्य का निर्धारण करते समय इसे ध्‍यान में रखा जाता है.</span><span class="sxs-lookup"><span data-stu-id="14e48-165">**Resource organizational unit** indicates the organizational unit from which resources should be staffed for that task; this also impacts the cost and sales estimate of the task, since this is accounted for when determining the unit sales price for the resource.</span></span> 
 - <span data-ttu-id="14e48-166">**संसाधन** को जब कोई जेनेरिक संसाधन या नामयुक्त संसाधन मिलता है, तो यह उसे धारण कर लेता है.</span><span class="sxs-lookup"><span data-stu-id="14e48-166">**Resources** holds a generic resource or a named resource when one is found.</span></span>  
  
## <a name="task-dependencies"></a><span data-ttu-id="14e48-167">कार्य निर्भरताएँ</span><span class="sxs-lookup"><span data-stu-id="14e48-167">Task dependencies</span></span>  
 <span data-ttu-id="14e48-168">आप कार्य विश्लेषण संरचना में एक या अधिक कार्यों के बीच पूर्वगामी संबंध बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="14e48-168">You can create predecessor relationships between one or more tasks in the work breakdown structure.</span></span> <span data-ttu-id="14e48-169">आप कार्यों पर पूर्वगामी फ़ील्ड के लिए एक या अधिक मान सेट कर सकते हैं ताकि उन कार्यों को इंगित किया जा सके जिन पर निर्भर हुआ जाएगा.</span><span class="sxs-lookup"><span data-stu-id="14e48-169">You can set one or more values for the predecessor field on tasks to indicate the tasks that it will be dependent on.</span></span> <span data-ttu-id="14e48-170">जब आप किसी कार्य पर एक पूर्वगामी मान असाइन करते हैं, तो वह कार्य केवल तभी प्रारंभ हो सकता है जब सभी पूर्वगामी कार्य पूर्ण हो जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="14e48-170">When you assign a predecessor value to a task, the task can only start when all the predecessor tasks have completed.</span></span> <span data-ttu-id="14e48-171">किसी कार्य पर यह निर्भरता सेट करने से उस कार्य के नियोजित प्रारंभ दिनांक की पुन: गणना होगी, जिसमें इस प्रारंभ दिनांक को इसके सभी पूर्वगामियों के नवीनतम समाप्ति दिनांक के रूप में लिया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="14e48-171">Setting this dependency on a task will result in the recalculation of the planned start date of the task as the latest end of all of its predecessors.</span></span> <span data-ttu-id="14e48-172">शेड्यूल पर पूर्वगामी-संबंधित प्रभाव, कार्य मोड, जिसे कार्य पर परिभाषित किया जाता है, द्वारा सीमित नहीं रहते.</span><span class="sxs-lookup"><span data-stu-id="14e48-172">Predecessor-related impacts on a schedule are not limited by the task mode defined on the task.</span></span>  
  
## <a name="task-mode"></a><span data-ttu-id="14e48-173">कार्य मोड</span><span class="sxs-lookup"><span data-stu-id="14e48-173">Task mode</span></span>  
 <span data-ttu-id="14e48-174">कार्य मोड एक ऐसा महत्वपूर्ण कारक है जो लीफ़ नोड कार्यों की शेड्यूलिंग निर्धारित करता है.</span><span class="sxs-lookup"><span data-stu-id="14e48-174">Task mode is one of the important factors that determine scheduling leaf node tasks.</span></span> <span data-ttu-id="14e48-175">प्रत्येक कार्य के लिए दो कार्य मोड हैं: स्‍वतः शेड्यूलिंग मोड और मैन्युअल शेड्यूलिंग मोड.</span><span class="sxs-lookup"><span data-stu-id="14e48-175">There are two task modes for every task: auto scheduling mode and manual scheduling mode.</span></span>  
  
-   <span data-ttu-id="14e48-176">**ऑटो शेड्यूलिंग**.</span><span class="sxs-lookup"><span data-stu-id="14e48-176">**Auto scheduling**.</span></span>   <span data-ttu-id="14e48-177">जब आप कार्य मोड को स्‍वचालित शेड्यूल पर सेट करते हैं, तो कार्य शेड्यूलिंग इंजन निम्न कार्य एट्रिब्‍यूट पर शेड्यूलिंग नियमों का उपयोग करता है, ताकि कार्य के लिए शेड्यूल निर्धारित किया जा सके:</span><span class="sxs-lookup"><span data-stu-id="14e48-177">When you set the task mode to Automatically Scheduled, the task scheduling engine uses the scheduling rules on the following task attributes to determine the schedule for the task:</span></span>  
  
    -   <span data-ttu-id="14e48-178">पूर्वगामी</span><span class="sxs-lookup"><span data-stu-id="14e48-178">Predecessors</span></span>  
  
    -   <span data-ttu-id="14e48-179">प्रयास</span><span class="sxs-lookup"><span data-stu-id="14e48-179">Effort</span></span>  
  
    -   <span data-ttu-id="14e48-180">संसाधनों की संख्या</span><span class="sxs-lookup"><span data-stu-id="14e48-180">Number of resources</span></span>  
  
    -   <span data-ttu-id="14e48-181">आरंभ और समाप्ति दिनांक</span><span class="sxs-lookup"><span data-stu-id="14e48-181">Start and end dates</span></span>  
  
-   <span data-ttu-id="14e48-182">**शेड्यूलिंग नियम**.</span><span class="sxs-lookup"><span data-stu-id="14e48-182">**Scheduling rules**.</span></span>   <span data-ttu-id="14e48-183">ऐसे लीफ़ नोड कार्य, जिसका कोई पूर्वगामी नहीं होता, का प्रारंभ दिनांक डिफ़ॉल्ट रूप से परियोजना के शेड्यूलिंग प्रारंभ दिनांक के समान होता है.</span><span class="sxs-lookup"><span data-stu-id="14e48-183">The start date of a leaf node task that does not have predecessors defaults to the project’s scheduling start date.</span></span> <span data-ttu-id="14e48-184">लीफ़ नोड कार्य की अवधि की गणना हमेशा उसके प्रारंभ और समाप्ति दिनांकों के बीच कार्य दिवसों की संख्या के रूप में की जाती है.</span><span class="sxs-lookup"><span data-stu-id="14e48-184">The duration of a leaf node task is always calculated as the number of working days between its start and end dates.</span></span> <span data-ttu-id="14e48-185">जब कोई कार्य स्वचालित रूप से शेड्यूल किया गया है, तो शेड्यूलिंग इंजन निम्न नियमों का पालन करता है:</span><span class="sxs-lookup"><span data-stu-id="14e48-185">When a task is automatically scheduled, the scheduling engine follows the rules below:</span></span>  
  
    -   <span data-ttu-id="14e48-186">कार्य का प्रारंभ और समाप्ति दिनांक हमेशा वे कार्य दिवस होने चाहिए, जो परियोजना के शेड्यूलिंग कैलेंडर के अनुसार हों</span><span class="sxs-lookup"><span data-stu-id="14e48-186">Start and end dates of a task must always be working days according to the project’s scheduling calendar</span></span>  
  
    -   <span data-ttu-id="14e48-187">जिस कार्य के पूर्वगामी होते हैं, उसका प्रारंभ दिनांक डिफ़ॉल्‍ट रूप से उसके पूर्वगामियों के नवीनतम समाप्ति दिनांक के समान होता है</span><span class="sxs-lookup"><span data-stu-id="14e48-187">The start date of a task that has predecessors defaults to the latest end date of its predecessors</span></span>  
  
    -   <span data-ttu-id="14e48-188">प्रयास = व्‍यक्तियों की संख्‍या \* अवधि \* परियोजना कैलेंडर के मानक कार्य दिवस में घंटे</span><span class="sxs-lookup"><span data-stu-id="14e48-188">Effort = Number of people \* Duration \* hours in a standard work day of the project calendar</span></span>  
  
-   <span data-ttu-id="14e48-189">**मैन्युअल शेड्यूलिंग**.</span><span class="sxs-lookup"><span data-stu-id="14e48-189">**Manual scheduling**.</span></span>   <span data-ttu-id="14e48-190">कुछ मामलों में, हो सकता है कि आप इन नियमों से विचलन करना चाहें.</span><span class="sxs-lookup"><span data-stu-id="14e48-190">In some cases, you might want to deviate from these rules.</span></span> <span data-ttu-id="14e48-191">इन मामलों में, आप कार्य के लिए कार्य मोड को मैन्युअल रूप से शेड्यूल करने के लिए सेट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="14e48-191">In these cases, you can set the task mode for the task to be manually scheduled.</span></span> <span data-ttu-id="14e48-192">इससे शेड्यूलिंग इंजन के अन्‍य शेड्यूलिंग एट्रिब्‍यूट के मानों की गणना करने पर रोक लगती है.</span><span class="sxs-lookup"><span data-stu-id="14e48-192">This stops the scheduling engine from calculating the values for other scheduling attributes.</span></span> <span data-ttu-id="14e48-193">कार्यों पर पूर्वगामी सेट करने से हमेशा निर्भरों के कार्य के प्रारंभ दिनांक पर प्रभाव पड़ता है.</span><span class="sxs-lookup"><span data-stu-id="14e48-193">Setting predecessors on tasks always impacts the dependent task’s start date.</span></span>  
  
## <a name="create-a-work-breakdown-structure"></a><span data-ttu-id="14e48-194">एक कार्य विश्लेषण संरचना बनाएँ</span><span class="sxs-lookup"><span data-stu-id="14e48-194">Create a work breakdown structure</span></span>  
  
1.  <span data-ttu-id="14e48-195">**Project Service > परियोजना** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="14e48-195">Go to **Project Service > Projects**.</span></span>  
  
2.  <span data-ttu-id="14e48-196">जिस परियोजना पर आप काम करना चाहते हैं, उस पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="14e48-196">Click the project you want to work on.</span></span>  
  
3.  <span data-ttu-id="14e48-197">स्क्रीन के ऊपर दी गई पट्टी में, परियोजना नाम के आगे स्थित नीचे तीर का चयन करें और उसके बाद कार्य विश्लेषण संरचना पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="14e48-197">In the bar across the top of the screen, select the down arrow next to the project name, and then click Work breakdown structure.</span></span>  
  
4.  <span data-ttu-id="14e48-198">कार्य जोड़ने के लिए, **कार्य जोड़ें** क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="14e48-198">To add a task, click **Add Task**.</span></span> <span data-ttu-id="14e48-199">कार्य के लिए फ़ील्ड भरें, और फिर **सहेजें** क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="14e48-199">Fill in the fields for the task, and then click **Save**.</span></span>  
  
5.  <span data-ttu-id="14e48-200">कार्य जोड़ना तब तक जारी रखें जब तक कार्य विश्लेषण संरचना पूर्ण न हो जाए.</span><span class="sxs-lookup"><span data-stu-id="14e48-200">Continue adding tasks until your work breakdown structure is complete.</span></span> <span data-ttu-id="14e48-201">अपनी कार्य विश्लेषण संरचना बनाते समय, आप अपने कार्यों को व्यवस्थित करने के लिए निम्न कार्य कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="14e48-201">While creating your work breakdown structure, you can do the following to organize your tasks:</span></span>  
  
    -   <span data-ttu-id="14e48-202">किसी कार्य का चयन करें और उसे अन्‍य कार्य के अंतर्गत ले जाने के लिए **इंडेंट** पर क्लिक करें या उसे एक स्‍तर बाहर ले जाने के लिए आउटडेंट पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="14e48-202">Select a task and click **Indent** to move it under another task or click Outdent to move it out a level.</span></span>  
  
    -   <span data-ttu-id="14e48-203">एक कार्य का चयन करें, और उसे सूची में ऊपर या नीचे ले जाने के लिए **ऊपर ले जाएँ** या **नीचे ले जाएँ** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="14e48-203">Select a task and click **Move Up** or **Move Down** to move it up or down in the list.</span></span>  
  
    -   <span data-ttu-id="14e48-204">गैंट चार्ट छिपाने के लिए **गैंट छिपाएँ** पर क्लिक करें और उसे पुनः प्रदर्शित करने के लिए **गैंट दिखाएँ** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="14e48-204">Click **Hide Gantt** to hide the Gantt chart, and click **Show Gantt** to display it again.</span></span>  
  
    -   <span data-ttu-id="14e48-205">गैंट चार्ट के लिए समय की विभिन्न अवधि को **समय स्केल** में चुनें.</span><span class="sxs-lookup"><span data-stu-id="14e48-205">Select a different period of time for the Gantt chart in **Time Scale**.</span></span>  
  
6.  <span data-ttu-id="14e48-206">आपने अपने कार्य विश्लेषण संरचना में जो भूमिकाएँ निर्दिष्ट की हैं, उन्‍हें अपनी परियोजना के टीम सदस्‍यों पर जोड़ने के लिए, **परियोजना टीम उत्पन्न करें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="14e48-206">To add the roles you specified in your work breakdown structure to your project’s team members, click **Generate Project Team**.</span></span>  
  
7.  <span data-ttu-id="14e48-207">परिवर्तन करने के बाद, स्‍क्रीन के निचले दाएँ कोने में स्थित **सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="14e48-207">Click **Save** at the bottom right corner of the screen when you’re done making changes.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="14e48-208">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="14e48-208">See Also</span></span>  
 [<span data-ttu-id="14e48-209">परियोजना प्रबंधक मार्गदर्शिका</span><span class="sxs-lookup"><span data-stu-id="14e48-209">Project manager guide</span></span>](../psa/project-manager-guide.md)
