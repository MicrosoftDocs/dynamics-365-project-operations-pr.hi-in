---
title: डेमो डेटा के साथ प्रयोग करें
description: Project Service Automation के लिए डेमो डेटा को कैसे डाउनलोड करें और कैसे प्रयोग करें.
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.prod: ''
ms.technology: ''
ms.assetid: b195e5c8-63bc-4e90-914c-f29b8d565942
ms.author: jburrows
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 76dd5ff14cbafbfc5341885f0469a6e3e71dd66f
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3752049"
---
# <a name="experiment-with-demo-data-project-service"></a><span data-ttu-id="05a01-103">डेमो डेटा के साथ प्रयोग करना (Project Service)</span><span class="sxs-lookup"><span data-stu-id="05a01-103">Experiment with demo data (Project Service)</span></span>

<span data-ttu-id="05a01-104">Dynamics 365 Project Service Automation से परिचित होने के लिए, एक पूर्व-कॉन्फ़िगर परिवेश होना उपयोगी होता है ताकि अन्वेषण किया जा सके.</span><span class="sxs-lookup"><span data-stu-id="05a01-104">To become familiar with Dynamics 365 Project Service Automation, it’s useful to have a pre-configured environment to explore.</span></span> <span data-ttu-id="05a01-105">इस उद्देश्य के लिए, हमने एक अलग नमूना डेटा स्थापना पैकेज (इस समय केवल अंग्रेज़ी-भाषा) बनाया है जो इन समाधानों के बारे में जानना आसान बनाता है.</span><span class="sxs-lookup"><span data-stu-id="05a01-105">For this purpose, we’ve created a separate sample data installation package (English-language only at this time) that makes it easier to learn about these solutions.</span></span> 

<span data-ttu-id="05a01-106">स्थापना पैकेज [Microsoft डाउनलोड केंद्र](https://go.microsoft.com/fwlink/?linkid=859966) में उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="05a01-106">The installation package is available on the [Microsoft Download Center](https://go.microsoft.com/fwlink/?linkid=859966).</span></span>  

<span data-ttu-id="05a01-107">Package Deployer स्थापना को चलाने पर निम्न कार्य होंगे:</span><span class="sxs-lookup"><span data-stu-id="05a01-107">Running the Package Deployer install performs the following actions:</span></span> 
  
-   <span data-ttu-id="05a01-108">डिफ़ॉल्ट पैरामीटर्स बनाता या सेट करता है जो Project Service के व्‍यवहार को बढ़ाते हैं.</span><span class="sxs-lookup"><span data-stu-id="05a01-108">Creates or sets default parameters that drive behavior of Project Service</span></span>  
  
-   <span data-ttu-id="05a01-109">नमूना डेटा, जैसे बुक करने योग्य संसाधन, भूमिकाएँ, Sales और लागत मूल्य सूचियाँ, संगठनात्मक इकाइयाँ, प्रासंगिक विक्रय प्रक्रिया रिकॉर्ड्स, कार्य ऑर्डर्स और परियोजनाएँ, आयात करता है</span><span class="sxs-lookup"><span data-stu-id="05a01-109">Imports sample data such as Bookable Resources, Roles, Sales and Cost Price lists, Organizational Units, relevant sales process records, Work Orders and Projects</span></span>    
  
> [!IMPORTANT]
> <span data-ttu-id="05a01-110">**डेमो डेटा की स्थापना रद्द करने का कोई तरीका नहीं है.**</span><span class="sxs-lookup"><span data-stu-id="05a01-110">**There is no way to un-install the demo data.**</span></span> <span data-ttu-id="05a01-111">इसलिए, आपको केवल प्रदर्शन, मूल्यांकन, प्रशिक्षण या परीक्षण सिस्‍टम्स पर इस पैकेज का उपयोग करना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="05a01-111">Therefore, you should only use this package on demonstration, evaluation, training and test systems.</span></span>

<span data-ttu-id="05a01-112">अधिक जानकारी के लिए, इसे देखें [ब्लॉग](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data).</span><span class="sxs-lookup"><span data-stu-id="05a01-112">For more information, see this [blog](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data).</span></span>





  
### <a name="see-also"></a><span data-ttu-id="05a01-113">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="05a01-113">See Also</span></span>  
 <span data-ttu-id="05a01-114">[व्यवस्थापक मार्गदर्शिका](../project-service/admin-guide.md) </span><span class="sxs-lookup"><span data-stu-id="05a01-114">[Administrator Guide](../project-service/admin-guide.md) </span></span>  
 <span data-ttu-id="05a01-115">[खाता प्रबंधक मार्गदर्शिका](../project-service/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="05a01-115">[Account Manager Guide](../project-service/account-manager-guide.md) </span></span>  
 <span data-ttu-id="05a01-116">[परियोजना प्रबंधक मार्गदर्शिका](../project-service/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="05a01-116">[Project Manager Guide](../project-service/project-manager-guide.md) </span></span>  
 <span data-ttu-id="05a01-117">[संसाधन प्रबंधक मार्गदर्शिका](../project-service/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="05a01-117">[Resource Manager Guide](../project-service/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="05a01-118">समय, व्यय और सहयोग मार्गदर्शिका</span><span class="sxs-lookup"><span data-stu-id="05a01-118">Time, Expense, and Collaboration Guide</span></span>](../project-service/time-expense-collaboration-guide.md)
