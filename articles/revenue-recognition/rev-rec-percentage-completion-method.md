---
title: निश्चित मूल्य आय अनुमान परियोजनाएँ
description: यह विषय परियोजनाओं में निश्चित मूल्य के बारे में जानकारी प्रदान करता है.
author: sigitac
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 639c6a104f2a90366a0f477c0d7cf384f19cdd81
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013803"
---
# <a name="fixed-price-revenue-estimate-projects"></a><span data-ttu-id="05b44-103">निश्चित मूल्य आय अनुमान परियोजनाएँ</span><span class="sxs-lookup"><span data-stu-id="05b44-103">Fixed price revenue estimate projects</span></span> 

<span data-ttu-id="05b44-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="05b44-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="05b44-105">जब आप Microsoft Dataverse पर Dynamics 365 Project Operations में निम्न एट्रिब्यूट के साथ परियोजना अनुबंध पंक्ति बनाते हैं, तो सिस्टम स्वचालित रूप से एक निश्चित मूल्य आय अनुमान परियोजना बनाता है.</span><span class="sxs-lookup"><span data-stu-id="05b44-105">When you create a project contract line with the following attributes in Dynamics 365 Project Operations on Microsoft Dataverse, the system automatically creates a fixed price revenue estimate project.</span></span> <span data-ttu-id="05b44-106">इस परियोजना की जानकारी निम्नलिखित पर आधारित है:</span><span class="sxs-lookup"><span data-stu-id="05b44-106">The information in this project is based on the following:</span></span>

  - <span data-ttu-id="05b44-107">निश्चित मूल्य बिलिंग विधि.</span><span class="sxs-lookup"><span data-stu-id="05b44-107">A fixed price billing method.</span></span>
  - <span data-ttu-id="05b44-108">संबद्ध परियोजना.</span><span class="sxs-lookup"><span data-stu-id="05b44-108">An associated project.</span></span>
  - <span data-ttu-id="05b44-109">**परियोजना अनुबंध पंक्ति** पृष्ठ के **इनवॉइस शेड्यूल** टैब पर कम से कम एक माइलस्टोन परिभाषित किया गया है.</span><span class="sxs-lookup"><span data-stu-id="05b44-109">At least one milestone defined on the **Invoice schedule** tab on the **Project contract line** page.</span></span>

## <a name="review-fixed-price-revenue-estimates-projects"></a><span data-ttu-id="05b44-110">निश्चित मूल्य आय अनुमान परियोजनाओं की समीक्षा करें</span><span class="sxs-lookup"><span data-stu-id="05b44-110">Review fixed price revenue estimates projects</span></span>
<span data-ttu-id="05b44-111">निर्धारित मूल्य आय अनुमान परियोजनाओं की समीक्षा करने के लिए, निम्नलिखित चरणों को पूरा करें:</span><span class="sxs-lookup"><span data-stu-id="05b44-111">To review fixed price revenue estimates projects, complete the following steps:</span></span>

1. <span data-ttu-id="05b44-112">Dynamics 365 Finance परिवेश में, **परियोजना प्रबंधन और लेखांकन** > **परियोजनाएँ** > **निश्चित मूल्य आय अनुमान परियोजनाएँ** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="05b44-112">In the Dynamics 365 Finance environment, go to **Projects management and accounting** > **Projects** > **Fixed price revenue estimate projects**.</span></span>
2. <span data-ttu-id="05b44-113">उस परियोजना का चयन करें, जिसे आप देखना चाहते हैं और रिकॉर्ड को खोलने और परियोजना के विवरण की समीक्षा करने के लिए **अनुमान परियोजना ID** पर डबल-क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="05b44-113">Select the project that you want to view and double-click the **Estimate project ID** to open the record and review the details of the project.</span></span>
3. <span data-ttu-id="05b44-114">**परियोजना** टैब को विस्तृत करें. आपको **चयनित परियोजनाएँ** ग्रिड में एक परियोजना दिखाई देगी.</span><span class="sxs-lookup"><span data-stu-id="05b44-114">Expand the **Project** tab. You will see one project in the **Selected projects** grid.</span></span> <span data-ttu-id="05b44-115">सिस्टम इसका डिफ़ॉल्ट परियोजना के रूप में उपयोग करता है, क्योंकि यह वह परियोजना है, जो परियोजना अनुबंध पंक्ति से संबद्ध है.</span><span class="sxs-lookup"><span data-stu-id="05b44-115">The system uses this as default project because it is the project associated to the project contract line.</span></span> 
4. <span data-ttu-id="05b44-116">संबद्धता को बदलने के लिए, अतिरिक्त परियोजनाएँ चुनें और उन्हें **चयनित परियोजनाएँ** ग्रिड में जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="05b44-116">To change the association, select additional projects and add them to the **Selected projects** grid.</span></span> <span data-ttu-id="05b44-117">यदि इस ग्रिड में कई परियोजनाओं का चयन किया जाता है, तो सभी चयनित परियोजनाओं के लिए परियोजना प्रतिशत पूर्ण और आय अनुमान का एक साथ परिकलन किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="05b44-117">If multiple projects are selected in this grid, the project percentage completion and revenue estimates are calculated together for of the all selected projects.</span></span>

  <span data-ttu-id="05b44-118">परियोजना लागत, आय प्रोफ़ाइल, लागत टेम्पलेट और अवधि कोड को मैन्युअल रूप से सेट किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="05b44-118">Project cost, revenue profile, cost template, and the period code can be set manually.</span></span> <span data-ttu-id="05b44-119">यदि वे मैन्युअल रूप से सेट नहीं होते हैं, तो परियोजना लागत और आय प्रोफ़ाइल के लिए कॉन्फ़िगर किए गए नियमों का उपयोग करके पहली अनुमान गणना के दौरान मान डिफ़ॉल्ट होते हैं.</span><span class="sxs-lookup"><span data-stu-id="05b44-119">If they aren't set manually, the values default during the first estimate calculation for the project using the rules configured for project cost and revenue profiles.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]