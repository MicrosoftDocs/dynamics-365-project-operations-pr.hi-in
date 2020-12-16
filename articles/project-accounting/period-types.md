---
title: अवधि प्रकार
description: इस विषय में आय अनुमान के लिए अवधि प्रकार को सेट अप करने के तरीके के बारे में बताया गया है.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6bcd988fbd074c66d64f7e327b4329d3de27e950
ms.sourcegitcommit: 2d399bc9d07807626f0d6b2d0cf304240c47591c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/17/2020
ms.locfileid: "4531449"
---
# <a name="period-types"></a><span data-ttu-id="78e58-103">अवधि प्रकार</span><span class="sxs-lookup"><span data-stu-id="78e58-103">Period types</span></span>

<span data-ttu-id="78e58-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="78e58-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="78e58-105">अवधि प्रकार परिभाषित करता है कि किसी परियोजना पर कितनी बार आय का अनुमान लगाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="78e58-105">A period type defines how frequently revenue on a project is estimated.</span></span> <span data-ttu-id="78e58-106">इस विषय में आय अनुमान के लिए अवधि प्रकार को सेट अप करने के तरीके के बारे में बताया गया है.</span><span class="sxs-lookup"><span data-stu-id="78e58-106">This topic provides information about how to set up period types for revenue estimation.</span></span> 

## <a name="create-and-work-with-period-types"></a><span data-ttu-id="78e58-107">अवधि प्रकार बनाएँ और उसके साथ कार्य करें</span><span class="sxs-lookup"><span data-stu-id="78e58-107">Create and work with period types</span></span>
<span data-ttu-id="78e58-108">अवधि प्रकार बनाने और उनके साथ कार्य करने के लिए, निम्नलिखित चरणों को पूरा करें:</span><span class="sxs-lookup"><span data-stu-id="78e58-108">To create and work with period types, complete the following steps:</span></span>

1. <span data-ttu-id="78e58-109">अपने Dynamics 365 Finance परिवेश में, **परियोजना प्रबंधन और लेखांकन** > **सेटअप** > **अनुमान** > **अवधि प्रकार** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="78e58-109">In your Dynamics 365 Finance environment, go to **Project management and accounting** > **Setup** > **Estimates** > **Period types**.</span></span>
2. <span data-ttu-id="78e58-110">नया अवधि प्रकार बनाने के लिए, **नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="78e58-110">Select **New** to create new period type.</span></span> <span data-ttu-id="78e58-111">एक नाम और एक विवरण दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="78e58-111">Enter a name and description.</span></span>
3. <span data-ttu-id="78e58-112">**आवृत्ति** फ़ील्ड में, एक मान चुनें:</span><span class="sxs-lookup"><span data-stu-id="78e58-112">In the **Frequency** field, select a value:</span></span>

    - <span data-ttu-id="78e58-113">यदि आप **सप्ताह**, **द्वि-साप्ताहिक**, **अर्ध मासिक**, **महीना**, **दिन**, **तिमाही** या **साल** चुनते हैं, तो अवधियाँ जनरेट करने के लिए कैलेंडर का उपयोग किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="78e58-113">If you select **Week**, **Bi-weekly**, **Semi-monthly**, **Month**, **Day**, **Quarter**, or **Year**, the calendar will be used to generate the periods.</span></span> 
    - <span data-ttu-id="78e58-114">यदि आप **लेज़र अवधि** चुनते हैं, तो अवधियाँ जनरेट करने के लिए सामान्य लेज़र कॉन्फ़िगरेशन से लेज़र अवधियों का उपयोग किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="78e58-114">If you select **Ledger period**, ledger periods from the General ledger configuration will be used to generate periods.</span></span>
    - <span data-ttu-id="78e58-115">यदि आप **असीमित** चुनते हैं, तो आप कस्टम अवधियाँ निर्दिष्ट कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="78e58-115">If you select **Unlimited**, you can specify custom periods.</span></span>
4. <span data-ttu-id="78e58-116">अवधि प्रकार के लिए अवधियाँ बनाने हेतु, अवधि प्रकार रिकॉर्ड को चुनें और उसके बाद **अवधियाँ जनरेट करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="78e58-116">Select the period type record and then select **Generate periods** to create periods for the period type.</span></span> <span data-ttu-id="78e58-117">आपके द्वारा चुनी गई अवधि आवृत्ति के आधार पर, आपके पास प्रारंभ दिनांक या जनरेट की जाने वाली अवधियों की संख्या निर्दिष्ट करने का विकल्प हो सकता है.</span><span class="sxs-lookup"><span data-stu-id="78e58-117">Based on the period frequency that you selected, you might have the option to specify a start date or the number of periods to generate.</span></span>
5. <span data-ttu-id="78e58-118">जनरेट की गई अवधियों की समीक्षा करने के लिए, **अवधियाँ** चुनें.</span><span class="sxs-lookup"><span data-stu-id="78e58-118">Select **Periods** to review generated periods.</span></span>

