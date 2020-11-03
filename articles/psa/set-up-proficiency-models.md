---
title: दक्षता मॉडल्स सेट अप करें
description: Project Service में दक्षता मॉडल सेट अप करने का तरीका
author: JohnPBurrows
manager: kfend
ms.service: dynamics-365-customerservice
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
ms.openlocfilehash: 653b7eef12c57203fbc6853e97d3be43bdb85b9d
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077917"
---
# <a name="set-up-proficiency-models-project-service"></a><span data-ttu-id="6db08-103">दक्षता मॉडल सेट अप करना (Project Service)</span><span class="sxs-lookup"><span data-stu-id="6db08-103">Set up proficiency models (Project Service)</span></span>

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

<span data-ttu-id="6db08-104">अब जैसा की आपने अपने क्लायंट की परियोजनाओं के लिए कौशल को जोड़ दिया है, इसलिए अब आपको अपने सलाहकार के कौशल को रेट करने के लिए किसी तरीके की आवश्यकता होगी ताकि आप परियोजना की आवश्यकताओं के अनुसार उनका मेल मिला सकें.</span><span class="sxs-lookup"><span data-stu-id="6db08-104">Now that you’ve added the skills for your clients’ projects, you need a way to rate your consultants’ skills so you can match them to project requirements.</span></span> <span data-ttu-id="6db08-105">आप डिफ़ॉल्ट दक्षता मॉडल का उपयोग कर सकते हैं, संपादित कर सकते हैं या अपने संगठन की आवश्यकताओं से मेल मिलाने के लिए एक नया बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="6db08-105">You can use the default proficiency model, edit it, or create a new one to match the needs of your organization.</span></span>  
  
1.  <span data-ttu-id="6db08-106">**Project Service > दक्षता मॉडल्स** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="6db08-106">Go to **Project Service > Proficiency Models**.</span></span>  
  
2.  <span data-ttu-id="6db08-107">डिफ़ॉल्ट दक्षता मॉडल को देखने या संपादित करने के लिए, सूची में **डिफ़ॉल्ट रेटिंग मॉडल** पर क्लिक करें या नया दक्षता मॉडल बनाने के लिए, **नया** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="6db08-107">To view or edit the default proficiency model, click **Default Rating Model** in the list, or to create a new proficiency model, click **New**.</span></span>  
  
3.  <span data-ttu-id="6db08-108">यदि आप एक नया दक्षता मॉडल बना रहे हैं, तो **सामान्य** क्षेत्र में फ़ील्ड भरें और उसके बाद रिकॉर्ड बनाने के लिए ताकि आप उसे संपादित करना जारी रख सकें **सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="6db08-108">If you’re creating a new proficiency model, fill in the fields in the **General** area, and then click **Save** to create the record so you can continue editing it.</span></span> <span data-ttu-id="6db08-109">अपना दक्षता मॉडल बनाते समय ध्यान रखें कि उच्च नंबर बेहतर होते हैं.</span><span class="sxs-lookup"><span data-stu-id="6db08-109">When you create your own proficiency model, keep in mind that higher numbers are better.</span></span>  
  
     <span data-ttu-id="6db08-110">उदाहरण के लिए, यदि आप डिफ़ॉल्ट रेटिंग मॉडल को देख रहे हैं या संपादित कर रहे हैं, तो आपको **रेटिंग मान** में निम्न दक्षता स्तर दिखाई देंगे.</span><span class="sxs-lookup"><span data-stu-id="6db08-110">For example, if you’re viewing or editing the default rating model, you’ll see the following proficiency levels in **Rating Values**.</span></span>  
  
    |<span data-ttu-id="6db08-111">नाम</span><span class="sxs-lookup"><span data-stu-id="6db08-111">Name</span></span>|<span data-ttu-id="6db08-112">मान</span><span class="sxs-lookup"><span data-stu-id="6db08-112">Value</span></span>|  
    |----------|-----------|  
    |<span data-ttu-id="6db08-113">परिचित</span><span class="sxs-lookup"><span data-stu-id="6db08-113">Familiar</span></span>|<span data-ttu-id="6db08-114">1</span><span class="sxs-lookup"><span data-stu-id="6db08-114">1</span></span>|  
    |<span data-ttu-id="6db08-115">अच्छा</span><span class="sxs-lookup"><span data-stu-id="6db08-115">Good</span></span>|<span data-ttu-id="6db08-116">2</span><span class="sxs-lookup"><span data-stu-id="6db08-116">2</span></span>|  
    |<span data-ttu-id="6db08-117">दक्षता</span><span class="sxs-lookup"><span data-stu-id="6db08-117">Proficient</span></span>|<span data-ttu-id="6db08-118">3</span><span class="sxs-lookup"><span data-stu-id="6db08-118">3</span></span>|  
  
4.  <span data-ttu-id="6db08-119">दक्षता स्तर को जोड़ने या परिवर्तित करने के लिए, तालिका बटन पर क्लिक करें और इच्छित परिवर्तन करें.</span><span class="sxs-lookup"><span data-stu-id="6db08-119">To add or change a proficiency level, click the table button and make the changes you want.</span></span>  
  
5.  <span data-ttu-id="6db08-120">स्‍क्रीन के निचले दाएँ कोने में दिए गए **सहेजें** बटन पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="6db08-120">Click the **Save** button in the bottom right corner of the screen.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="6db08-121">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="6db08-121">See Also</span></span>  
 [<span data-ttu-id="6db08-122">संसाधन सेट अप करें</span><span class="sxs-lookup"><span data-stu-id="6db08-122">Set up resources</span></span>](../psa/set-up-resources.md)
