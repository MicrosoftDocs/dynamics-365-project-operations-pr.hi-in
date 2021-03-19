---
title: विक्रय प्रक्रिया के दौरान एक परियोजना के लिए कार्य अनुमान प्रदान करें
description: Project Service में विक्रय प्रक्रिया के दौरान परियोजना के लिए कार्य अनुमान प्रदान करने का तरीका
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
ms.openlocfilehash: 49ea8327ae34a69eba1585f1b1b4e557fd4eac93
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5283550"
---
# <a name="provide-work-estimates-for-a-project-during-the-sales-process-project-service"></a><span data-ttu-id="4d68a-103">विक्रय प्रक्रिया के दौरान परियोजना के लिए कार्य अनुमान प्रदान करना (Project Service)</span><span class="sxs-lookup"><span data-stu-id="4d68a-103">Provide work estimates for a project during the sales process (Project Service)</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="4d68a-104">विक्रय प्रक्रिया के दौरान, आप आधार से लेकर कोट पंक्तियों तक विक्रय अनुमान की गणना कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="4d68a-104">During the sales process, you can work out sales estimates from the ground up with quote lines.</span></span> [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] <span data-ttu-id="4d68a-105">में [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] क्षमताएँ एक बेहतर वैज्ञानिक और निश्चयात्‍मक तरीके प्रदान करते हैं ताकि कार्य आइटमों को विभाजित करके, और कार्य विश्लेषण संरचना में परियोजना के लिए अनुमानों में योगदान देने वाले उचित एट्रिब्‍यूट को संबद्ध करके, विक्रय अनुमानों की गणना की जा सके.</span><span class="sxs-lookup"><span data-stu-id="4d68a-105">capabilities in [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] provide a more scientific and deterministic way of coming up with sales estimates by breaking down work items and associating relevant attributes that contribute toward the estimates for the project in the work breakdown structure.</span></span>  
  
 <span data-ttu-id="4d68a-106">एक बार जब आप विक्रय जीत जाते हैं, तब फिर आप अपने परियोजना योजना में संबंधित कार्य विश्लेषण संरचना का उपयोग कर सकते हैं, अपनी परियोजना को पूर्ण करने के लिए आवश्‍यकतानुसार उसे परिशोधित कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="4d68a-106">Once you win the sale, you can use the associated work breakdown structure in your project plan, refining it as necessary for successful completion of your project.</span></span>  
  
## <a name="link-a-project-to-a-quote-line"></a><span data-ttu-id="4d68a-107">एक परियोजना को एक कोट पंक्ति के साथ लिंक करें</span><span class="sxs-lookup"><span data-stu-id="4d68a-107">Link a project to a quote line</span></span>  
 <span data-ttu-id="4d68a-108">परियोजना आधारित कोट पंक्ति बनाते समय, आप कोट पंक्ति से एक नई परियोजना बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="4d68a-108">When creating a project-based quote line, you can create a new project from the quote line.</span></span> <span data-ttu-id="4d68a-109">उसके बाद आप परियोजना टेम्पलेट्स का उपयोग कर सकते हैं, जो आपके संगठन के लिए पूर्व कॉन्फ़िगर की गई सामान्‍य मानक परियोजना योजनाएँ और वित्तीय अनुमान होते हैं, अथवा एक परियोजना योजना की प्रतिलिपि या पिछली परियोजना के अनुमान होते हैं.</span><span class="sxs-lookup"><span data-stu-id="4d68a-109">You can then use project templates, which are either pre-configured standard project plans and financial estimates common to your organization, or a copy of a project plan and estimates from a past project.</span></span> <span data-ttu-id="4d68a-110">जब आप कोई परियोजना बनाते हैं, तब परियोजना टेम्‍पलेट चुनने से परियोजना योजना, अनुमान और भूमिका शर्तें परिशोधित करने का एक आधार मिलता है.</span><span class="sxs-lookup"><span data-stu-id="4d68a-110">When you create a project, choosing a project template provides a basis to refine the project plan, estimates, and role requirements.</span></span> <span data-ttu-id="4d68a-111">कोट से अपनी परियोजना बनाते समय, परियोजना स्‍वचालित रूप से कोट पंक्ति के साथ संबद्ध हो जाती है.</span><span class="sxs-lookup"><span data-stu-id="4d68a-111">By creating your project from the quote, the project is automatically associated with the quote line.</span></span>  
  
## <a name="project-estimate-components"></a><span data-ttu-id="4d68a-112">परियोजना अनुमान घटक</span><span class="sxs-lookup"><span data-stu-id="4d68a-112">Project estimate components</span></span>  
 <span data-ttu-id="4d68a-113">किसी परियोजना में कार्य विश्लेषण संरचना से कार्य को छोटे कार्यों में तोड़ने, कार्यों का पदानुक्रमन बनाए रखने, और प्रत्‍येक कार्य को पूर्ण करने के लिए आवश्‍यक प्रयास का अनुमान असाइन करने का एक तरीका प्राप्त होता है.</span><span class="sxs-lookup"><span data-stu-id="4d68a-113">The work breakdown structure in a project provides a way to break down work into tasks, maintain a hierarchy of tasks, and assign an estimate of effort required to complete each task.</span></span> <span data-ttu-id="4d68a-114">आप कार्यों पर भूमिकाएँ भी असाइन कर सकते हैं ताकि एक कार्य और एक शेड्यूल पूर्ण करने में आवश्‍यक संसाधन के प्रकार का अनुमान दर्शाया जा सके.</span><span class="sxs-lookup"><span data-stu-id="4d68a-114">You can also associate roles to a task to indicate an estimate of the type of resource required to complete a task and a schedule.</span></span>  
  
 <span data-ttu-id="4d68a-115">कार्य विश्लेषण संरचना से आपको कार्य प्रयास और शेड्यूल अनुमान निर्धारित करने में मदद मिलती है.</span><span class="sxs-lookup"><span data-stu-id="4d68a-115">The work breakdown structure helps you determine work effort and schedule estimates.</span></span> <span data-ttu-id="4d68a-116">डिफ़ॉल्ट रूप से, परियोजना उस डिफ़ॉल्ट मूल्य सूचियों का उपयोग करती है जिन्‍हें आपने पहले परिभाषित किया था.</span><span class="sxs-lookup"><span data-stu-id="4d68a-116">By default, the project uses default price lists that you defined earlier.</span></span> <span data-ttu-id="4d68a-117">मूल्‍य सूचियों में परिभाषित लागत और विक्रय मूल्‍यों से उस परियोजना के कार्य विश्लेषण संरचना के लिए वित्तीय अनुमान निर्धारित करने में मदद मिलती है.</span><span class="sxs-lookup"><span data-stu-id="4d68a-117">The cost and sales prices defined in the price lists help determine financial estimates for the project’s work breakdown.</span></span>  
  
 <span data-ttu-id="4d68a-118">यदि आपकी परियोजना एक कोट से संबद्ध होती है, और कोट की मूल्‍य सूची डिफ़ॉल्‍ट से भिन्न होती है, तो वित्तीय अनुमानों के लिए कोट की मूल्‍य सूची का उपयोग किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="4d68a-118">If your project is associated with a quote, and the quote has a different price list from the default, the quote’s price list is used for financial estimates.</span></span>  
  
## <a name="import-estimates-from-a-project-into-a-quote"></a><span data-ttu-id="4d68a-119">किसी परियोजना से अनुमानों को कोट में आयात करें</span><span class="sxs-lookup"><span data-stu-id="4d68a-119">Import estimates from a project into a quote</span></span>  
 <span data-ttu-id="4d68a-120">परियोजना में परियोजना अनुमान होने पर, आप इन अनुमानों को कोट पंक्ति में आयात कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="4d68a-120">Once you have project estimates in the project, you can import these estimates into the quote line:</span></span>  
  
-   <span data-ttu-id="4d68a-121">**कोट पंक्ति विवरण** में, **अनुमानों से आयात करें** क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="4d68a-121">In **Quote Line Details**, click **Import from estimates**.</span></span> 

-   <span data-ttu-id="4d68a-122">यह चयन करें कि किस प्रकार से सारांशीकृत किए गए परियोजना अनुमानों को आयात करना है, लेन देन प्रकार से, भूमिका से अथवा कार्य विश्लेषण संरचना नोड स्‍तर से.</span><span class="sxs-lookup"><span data-stu-id="4d68a-122">Select whether to import project estimates summarized by transaction type, role, or work breakdown structure node level.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="4d68a-123">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="4d68a-123">See Also</span></span>  
 [<span data-ttu-id="4d68a-124">परियोजना प्रबंधक मार्गदर्शिका</span><span class="sxs-lookup"><span data-stu-id="4d68a-124">Project Manager Guide</span></span>](../psa/project-manager-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]