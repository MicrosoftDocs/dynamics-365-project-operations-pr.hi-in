---
title: डेमो डेटा के साथ प्रयोग करें
description: Project Service Automation के लिए डेमो डेटा को कैसे डाउनलोड करें और कैसे प्रयोग करें.
author: JohnPBurrows
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
ms.openlocfilehash: 91cf4150c651794fe38ebf5a406cad936aa5105d
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4130489"
---
# <a name="experiment-with-demo-data-project-service"></a><span data-ttu-id="f87b3-103">डेमो डेटा के साथ प्रयोग करना (Project Service)</span><span class="sxs-lookup"><span data-stu-id="f87b3-103">Experiment with demo data (Project Service)</span></span>

<span data-ttu-id="f87b3-104">Dynamics 365 Project Service Automation से परिचित होने के लिए, एक पूर्व-कॉन्फ़िगर परिवेश होना उपयोगी होता है ताकि अन्वेषण किया जा सके.</span><span class="sxs-lookup"><span data-stu-id="f87b3-104">To become familiar with Dynamics 365 Project Service Automation, it’s useful to have a pre-configured environment to explore.</span></span> <span data-ttu-id="f87b3-105">इस उद्देश्य के लिए, हमने एक अलग नमूना डेटा स्थापना पैकेज (इस समय केवल अंग्रेज़ी-भाषा) बनाया है जो इन समाधानों के बारे में जानना आसान बनाता है.</span><span class="sxs-lookup"><span data-stu-id="f87b3-105">For this purpose, we’ve created a separate sample data installation package (English-language only at this time) that makes it easier to learn about these solutions.</span></span> 

<span data-ttu-id="f87b3-106">स्थापना पैकेज [Microsoft डाउनलोड केंद्र](https://go.microsoft.com/fwlink/?linkid=859966) में उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="f87b3-106">The installation package is available on the [Microsoft Download Center](https://go.microsoft.com/fwlink/?linkid=859966).</span></span>  

<span data-ttu-id="f87b3-107">Package Deployer स्थापना को चलाने पर निम्न कार्य होंगे:</span><span class="sxs-lookup"><span data-stu-id="f87b3-107">Running the Package Deployer install performs the following actions:</span></span> 
  
-   <span data-ttu-id="f87b3-108">डिफ़ॉल्ट पैरामीटर्स बनाता या सेट करता है जो Project Service के व्‍यवहार को बढ़ाते हैं.</span><span class="sxs-lookup"><span data-stu-id="f87b3-108">Creates or sets default parameters that drive behavior of Project Service</span></span>  
  
-   <span data-ttu-id="f87b3-109">नमूना डेटा, जैसे बुक करने योग्य संसाधन, भूमिकाएँ, Sales और लागत मूल्य सूचियाँ, संगठनात्मक इकाइयाँ, प्रासंगिक विक्रय प्रक्रिया रिकॉर्ड्स, कार्य ऑर्डर्स और परियोजनाएँ, आयात करता है</span><span class="sxs-lookup"><span data-stu-id="f87b3-109">Imports sample data such as Bookable Resources, Roles, Sales and Cost Price lists, Organizational Units, relevant sales process records, Work Orders and Projects</span></span>    
  
> [!IMPORTANT]
> <span data-ttu-id="f87b3-110">**डेमो डेटा की स्थापना रद्द करने का कोई तरीका नहीं है.**</span><span class="sxs-lookup"><span data-stu-id="f87b3-110">**There is no way to un-install the demo data.**</span></span> <span data-ttu-id="f87b3-111">इसलिए, आपको केवल प्रदर्शन, मूल्यांकन, प्रशिक्षण या परीक्षण सिस्‍टम्स पर इस पैकेज का उपयोग करना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="f87b3-111">Therefore, you should only use this package on demonstration, evaluation, training and test systems.</span></span>

<span data-ttu-id="f87b3-112">अधिक जानकारी के लिए, इसे देखें [ब्लॉग](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data).</span><span class="sxs-lookup"><span data-stu-id="f87b3-112">For more information, see this [blog](https://blogs.msdn.microsoft.com/crm/2017/10/24/microsoft-dynamics-365-for-field-service-and-project-service-automation-sample-data).</span></span>





  
### <a name="see-also"></a><span data-ttu-id="f87b3-113">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="f87b3-113">See Also</span></span>  
 <span data-ttu-id="f87b3-114">[व्यवस्थापक मार्गदर्शिका](../psa/admin-guide.md) </span><span class="sxs-lookup"><span data-stu-id="f87b3-114">[Administrator Guide](../psa/admin-guide.md) </span></span>  
 <span data-ttu-id="f87b3-115">[खाता प्रबंधक मार्गदर्शिका](../psa/account-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="f87b3-115">[Account Manager Guide](../psa/account-manager-guide.md) </span></span>  
 <span data-ttu-id="f87b3-116">[परियोजना प्रबंधक मार्गदर्शिका](../psa/project-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="f87b3-116">[Project Manager Guide](../psa/project-manager-guide.md) </span></span>  
 <span data-ttu-id="f87b3-117">[संसाधन प्रबंधक मार्गदर्शिका](../psa/resource-manager-guide.md) </span><span class="sxs-lookup"><span data-stu-id="f87b3-117">[Resource Manager Guide](../psa/resource-manager-guide.md) </span></span>  
 [<span data-ttu-id="f87b3-118">समय, व्यय और सहयोग मार्गदर्शिका</span><span class="sxs-lookup"><span data-stu-id="f87b3-118">Time, Expense, and Collaboration Guide</span></span>](../psa/time-expense-collaboration-guide.md)
