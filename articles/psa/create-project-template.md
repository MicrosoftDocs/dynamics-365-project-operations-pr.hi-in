---
title: परियोजना टेम्पलेट बनाएँ
description: Project Service में परियोजना टेम्पलेट बनाने का तरीका
author: ruhercul
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
ms.openlocfilehash: 148bf1d42b640ff7b58b13bb0c30c7e583d803c8
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5997243"
---
# <a name="create-a-project-template-project-service"></a><span data-ttu-id="0df1c-103">परियोजना टेम्पलेट बनाना (Project Service)</span><span class="sxs-lookup"><span data-stu-id="0df1c-103">Create a project template (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="0df1c-104">यदि आपकी कंपनी नियमित रूप से समान प्रकार की परियोजनाओं पर बिड करती है, तो परियोजना टेम्पलेट आपका समय बचाते हैं.</span><span class="sxs-lookup"><span data-stu-id="0df1c-104">Project templates save you time if your company regularly bids on similar types of projects.</span></span> <span data-ttu-id="0df1c-105">वे भूमिकाओं के मानक सेट और एक परियोजना प्रकार के लिए अनुमानित घंटे प्रदान करते हैं.</span><span class="sxs-lookup"><span data-stu-id="0df1c-105">They provide a standard set of roles and estimated hours for a type of project.</span></span> <span data-ttu-id="0df1c-106">खाता प्रबंधक और परियोजना प्रबंधक, एक परियोजना टेम्पलेट के आधार पर परियोजनाएँ बना सकते हैं, या वे अपना स्‍वयं का टेम्‍पलेट बनाने के लिए उसकी प्रतिलिपि ले सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="0df1c-106">Account managers and project managers can create projects based on a project template, or they can copy the template and make one of their own.</span></span>  
  
## <a name="components-of-project-template"></a><span data-ttu-id="0df1c-107">परियोजना टेम्पलेट के घटक</span><span class="sxs-lookup"><span data-stu-id="0df1c-107">Components of project template</span></span>
 <span data-ttu-id="0df1c-108">एक परियोजना टेम्पलेट के तीन घटक होते हैं:</span><span class="sxs-lookup"><span data-stu-id="0df1c-108">A project template consists of three components:</span></span>  
  
- <span data-ttu-id="0df1c-109">**कार्य विश्लेषण संरचना**: एक परियोजना टेम्‍पलेट में कार्य विश्लेषण संरचना के तत्‍वों के वही सेट होते हैं जैसा परियोजना के पास हैं.</span><span class="sxs-lookup"><span data-stu-id="0df1c-109">**Work breakdown structure**: A work breakdown structure in a project template has the same set of elements as in the project.</span></span> <span data-ttu-id="0df1c-110">आप एक कार्य पदानुक्रम बना सकते हैं, कार्य पर भूमिकाएँ संबद्ध कर सकते हैं, शेड्यूल एट्रिब्‍यूट परिभाषित कर सकते हैं, और निर्भरताएँ सेट कर सकते हैं और गैंट में सभी डेटा देख सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="0df1c-110">You can create a task hierarchy, associate roles to task, define schedule attributes, set dependencies and view all the data in the Gantt.</span></span> <span data-ttu-id="0df1c-111">परियोजना टेम्‍पलेट्स में कार्य विश्लेषण संरचना प्रत्‍येक कार्य के लिए कार्य मोड का भी समर्थन करती है.</span><span class="sxs-lookup"><span data-stu-id="0df1c-111">The work breakdown structure in project templates also support task modes for each task.</span></span> <span data-ttu-id="0df1c-112">कार्य शेड्यूल बनाते समय एक परियोजना टेम्पलेट और परियोजना के बीच कोई अंतर नहीं है.</span><span class="sxs-lookup"><span data-stu-id="0df1c-112">There is no difference between a project template and a project when creating work schedule.</span></span>  
  
- <span data-ttu-id="0df1c-113">**परियोजना अनुमान**: टेम्पलेट्स में परियोजना अनुमान उसी तरह कार्य करता है जैसा परियोजना में करता है, सिवाय इसके की लागत और विक्रय मूल्‍यों को डिफ़ॉल्ट करने वाली मूल्‍य सूचियाँ हमेशा [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] पैरामीटर में परिभाषित डिफ़ॉल्ट लागत और मूल्‍य सूचियों होती हैं.</span><span class="sxs-lookup"><span data-stu-id="0df1c-113">**Project estimates**: Project estimates in templates work the same way as they do in projects, except the price lists for defaulting the cost and sales prices are always the default cost and sales price lists defined in [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] parameters.</span></span> <span data-ttu-id="0df1c-114">शेष सभी कार्यक्षमता किसी परियोजना के समान ही होती है.</span><span class="sxs-lookup"><span data-stu-id="0df1c-114">The rest of the functionality is the same as in a project.</span></span>  
  
- <span data-ttu-id="0df1c-115">**परियोजना टीम निर्माण**: परियोजना टेम्‍पलेट के लिए परियोजना टीम बनाते समय, आप टेम्पलेट में एक नामयुक्त संसाधन बुक नहीं कर सकते.</span><span class="sxs-lookup"><span data-stu-id="0df1c-115">**Project team formation**: When forming a project team for a project template, you can’t book a named resource in a template.</span></span> <span data-ttu-id="0df1c-116">आप जेनेरिक संसाधनों के सेट उत्‍पन्न करने के लिए कार्य विश्लेषण संरचना में **परियोजना टीम उत्‍पन्न करें** का उपयोग कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="0df1c-116">You can use **Generate Project Team** in the work breakdown structure to generate a set of generic resources.</span></span> <span data-ttu-id="0df1c-117">आप जेनेरिक संसाधनों के लिए आवश्यक कौशल और दक्षताएँ भी निर्दिष्ट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="0df1c-117">You can also specify required skills and proficiencies for generic resources.</span></span> <span data-ttu-id="0df1c-118">आप एक जेनेरिक संसाधन को एक बुक होने योग्‍य संसाधन से स्थानापन्न नहीं कर सकते.</span><span class="sxs-lookup"><span data-stu-id="0df1c-118">You can’t substitute a generic resource with a bookable resource in project templates.</span></span>  
  
## <a name="create-a-project-from-a-template"></a><span data-ttu-id="0df1c-119">एक टेम्पलेट से एक परियोजना बनाएँ</span><span class="sxs-lookup"><span data-stu-id="0df1c-119">Create a project from a template</span></span>  
 <span data-ttu-id="0df1c-120">आप किसी टेम्पलेट से कोई परियोजना निम्न तरीकों से बना सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="0df1c-120">You can create a project from a template in these following ways:</span></span>  
  
-   <span data-ttu-id="0df1c-121">कोट से परियोजना बनाते समय, आप परियोजना त्‍वरित बनाएँ प्रपत्र में एक परियोजना टेम्पलेट चुन सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="0df1c-121">When creating a project from the quote, you can choose a project template in the project quick create form.</span></span>  
  
-   <span data-ttu-id="0df1c-122">**नई परियोजना** में क्लिक करके एक परियोजना बनाते समय, परियोजना प्रपत्र आपके रिकॉर्ड सहेजने से पहले दिखाई देता है.</span><span class="sxs-lookup"><span data-stu-id="0df1c-122">When creating a project by clicking **New Project**, the project form displays before you save the record.</span></span> <span data-ttu-id="0df1c-123">यहाँ से, आप अपने संगठन के लिए पूर्व-परिभाषित परियोजना टेम्‍पलेट की सूची से चुनने के लिए **एक टेम्पलेट चुनें** फ़ील्ड क्लिक कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="0df1c-123">From here, you can click **Pick a template** field to choose from the list of pre-defined project templates in your organization.</span></span>  
  
-   <span data-ttu-id="0df1c-124">टेम्‍पलेट से परियोजना बनाने के लिए, **परियोजना टेम्‍पलेट** पृष्ठ पर **एक टेम्पलेट से परियोजना बनाएँ** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="0df1c-124">Click **Create project from a template** on the **Project Template** page to create a project from the template.</span></span>  
  
## <a name="copying-components-of-a-template-to-a-project"></a><span data-ttu-id="0df1c-125">टेम्पलेट के घटकों की प्रतिलिपि एक परियोजना में बनाई जा रही है</span><span class="sxs-lookup"><span data-stu-id="0df1c-125">Copying components of a template to a project</span></span>  
 <span data-ttu-id="0df1c-126">जब आप परियोजना से एक टेम्पलेट के घटकों की प्रतिलिपि बनाते हैं, तो कुछ ऐसी चीज़ें हैं जिनके बारे में आपको जानना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="0df1c-126">When you copy components of a template into a project, there are a few things you should know about.</span></span>  
  
 <span data-ttu-id="0df1c-127">**कार्य विश्लेषण संरचना की प्रतिलिपि बनाना**: आपके एक परियोजना टेम्‍पलेट से कार्य विश्लेषण संरचना की प्रतिलिपि बनाते समय, यदि परियोजना के पास टेम्‍पलेट की तुलना में एक भिन्न परियोजना कैलेंडर होता है, तो कार्य शेड्यूल करने के लिए कार्य के घंटे परियोजना के कैलेंडर से लागू होंगे.</span><span class="sxs-lookup"><span data-stu-id="0df1c-127">**Copying a work breakdown structure**: When you copy the work breakdown structure from a project template, if the project has a different project calendar than the template, the work hours from the project’s calendar will be applied to the schedule of tasks.</span></span> <span data-ttu-id="0df1c-128">इससे परियोजना कैलेंडर को बैक करने के लिए शेड्यूल समायोजित होता है.</span><span class="sxs-lookup"><span data-stu-id="0df1c-128">This adjusts the schedule to the backing project calendar.</span></span> <span data-ttu-id="0df1c-129">इसी प्रकार, परियोजना विश्लेषण संरचना पर पहला कार्य परियोजना की प्रारंभ तिथि लेता है, ताकि शेष कार्य पदानुक्रम टेम्‍पलेट की कार्य विश्लेषण संरचना में निर्दिष्ट शेड्यूल अवधि और निर्भरताओं के आधार पर अद्यतन हो जाएँ.</span><span class="sxs-lookup"><span data-stu-id="0df1c-129">Similarly, the first task on the work breakdown structure takes the project’s start date, so the rest of the task hierarchy schedule is updated based on the duration and dependencies specified in the template’s work breakdown structure.</span></span>  
  
 <span data-ttu-id="0df1c-130">**परियोजना अनुमानों की प्रतिलिपि बनाना**: जब आप परियोजना अनुमान रेखाओं के ऊपर प्रतिलिपि बनाते हैं, तो मूल्य सूचियाँ लागत मूल्य सूची और ग्राहक के लिए बिक्री मूल्य सूची के लिए परियोजना की स्वामित्व इकाई के आधार पर अद्यतन की जाती हैं.</span><span class="sxs-lookup"><span data-stu-id="0df1c-130">**Copying project estimates**: When you copy across project estimate lines, price lists are updated based on the owning unit of the project for the cost price list and customer for the sales price list.</span></span> <span data-ttu-id="0df1c-131">इकाई लागत और बिक्री मूल्य, इन परियोजनाओं पर मूल्य सूचियों से निर्धारित किए जाते हैं, जो विक्रय निकाय पर संबद्ध हैं.</span><span class="sxs-lookup"><span data-stu-id="0df1c-131">The unit cost and sales prices are determined from these price lists on projects that are associated to a sales entity.</span></span>  
  
 <span data-ttu-id="0df1c-132">**एक परियोजना टीम की प्रतिलिपि बनाना**: जब आप एक परियोजना टीम से प्रतिलिपि बनाते हैं, तो समूचे जेनेरिक संसाधनों की, टेम्‍पलेट में परिभाषित कौशल और दक्षताओं के साथ प्रतिलिपि बनाई जाती है.</span><span class="sxs-lookup"><span data-stu-id="0df1c-132">**Copying a project team**: When you copy the project team from the template to a project, the generic resources are copied across, along with the skills and proficiencies defined in the template.</span></span> <span data-ttu-id="0df1c-133">जेनेरिक संसाधन असाइनमेंट को भी परियोजना टेम्पलेट के रूप में रखा जाता है.</span><span class="sxs-lookup"><span data-stu-id="0df1c-133">Generic resource assignments are also maintained as in the project template.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="0df1c-134">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="0df1c-134">See Also</span></span>  
 [<span data-ttu-id="0df1c-135">परियोजना प्रबंधक मार्गदर्शिका</span><span class="sxs-lookup"><span data-stu-id="0df1c-135">Project Manager Guide</span></span>](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]