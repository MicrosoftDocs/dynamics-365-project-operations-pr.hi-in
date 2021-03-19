---
title: प्रति कानूनी निकाय, प्रकल्प के परिचालन का एकीकरण कॉन्फिगर करें
description: यह विषय कानूनी निकाय द्वारा प्रकल्प परिचालन में एकीकरण संबंधी जानकारी देता है.
author: sigitac
manager: Annbe
ms.date: 10/21/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: ccdbdce6b7d006adc9be2b5f3573dd8e79dd2b8d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5276980"
---
# <a name="configure-project-operations-integration-per-legal-entity"></a><span data-ttu-id="2ee6d-103">प्रति कानूनी निकाय, प्रकल्प के परिचालन का एकीकरण कॉन्फिगर करें</span><span class="sxs-lookup"><span data-stu-id="2ee6d-103">Configure Project Operations integration per legal entity</span></span> 

<span data-ttu-id="2ee6d-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="2ee6d-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="2ee6d-105">यह विषय आपको प्रति कानूनी निकाय Dynamics 365 Project Operationsको कॉन्फ़िगर करने के लिए आवश्यक चरणों से ले जाता है.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-105">This topic walks you through the steps required to configure Dynamics 365 Project Operations per legal entity.</span></span>

## <a name="enable-feature-keys-in-dynamics-365-finance"></a><span data-ttu-id="2ee6d-106">Dynamics 365 Finance सुविधा कुंजियाँ सक्षम करें</span><span class="sxs-lookup"><span data-stu-id="2ee6d-106">Enable feature keys in Dynamics 365 Finance</span></span>

<span data-ttu-id="2ee6d-107">आवश्यक विशेषताओं को सक्रिय करने के लिये निम्न चरणों का अनुपालन करें.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-107">Complete the following steps to enable required features.</span></span>

1. <span data-ttu-id="2ee6d-108">Dynamics 365 Finance में, **फीचर प्रबंधन** कार्यक्षेत्र पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-108">In Dynamics 365 Finance, go to the **Feature Management** workspace.</span></span>
2. <span data-ttu-id="2ee6d-109">**विशेषता सूची** में, निम्न विशेषताओं को खोजिये और सक्रिय कीजिये:</span><span class="sxs-lookup"><span data-stu-id="2ee6d-109">In **Feature list**, find and enable the following features:</span></span>
  
    - <span data-ttu-id="2ee6d-110">**प्रकल्प के लिये एकाधिक अनुबन्ध लाइन्स सक्रिय कीजिये**</span><span class="sxs-lookup"><span data-stu-id="2ee6d-110">**Enable multiple contract lines for a project**</span></span>
    - <span data-ttu-id="2ee6d-111">**Dynamics 365 Customer Engagement पर प्रोजेक्ट संचालन सक्षम करें**</span><span class="sxs-lookup"><span data-stu-id="2ee6d-111">**Enable Project Operations on Dynamics 365 Customer Engagement**</span></span>

> [!NOTE]
> <span data-ttu-id="2ee6d-112">यदि आपको **विशेषता कुंजी** सूचीबद्ध दिखाई देती है, सत्यापित करें कि आपके फायनान्स संस्करण न्यूनतम संस्करण आवश्यकता के अनुरुप हैं (एप्लीकेशन संस्करण 10.0.13 जिसके साथ सारी गुणवत्ता जानकारी लागू की जाती है या इससे अद्यतन स्थिति होती है).</span><span class="sxs-lookup"><span data-stu-id="2ee6d-112">If you don't see **Feature keys** listed, verify that your Finance version meets the minimum version requirement (application version 10.0.13 with all quality updates applied or higher).</span></span> <span data-ttu-id="2ee6d-113">विशेषता सूची को रिफ्रेश करने के लिये **नवीन की जांच करना** को चुनें.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-113">Select **Check for updates** to refresh the feature list.</span></span>

## <a name="define-the-project-operations-deployment-scenario-for-a-legal-entity"></a><span data-ttu-id="2ee6d-114">एक कानूनी निकाय के लिये प्रकल्प परिचालन प्रकार को परिभाषित करें</span><span class="sxs-lookup"><span data-stu-id="2ee6d-114">Define the Project Operations deployment scenario for a legal entity</span></span>

<span data-ttu-id="2ee6d-115">आप प्रकल्प परिचालन को Dynamics 365 Customer Engagement की स्थिति में कानूनी निकाय के स्तर पर ले सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-115">You can enable Project Operations on Dynamics 365 Customer Engagement on a legal entity level.</span></span> <span data-ttu-id="2ee6d-116">आपके पास एक कानूनी निकाय हो सकता है जिसमें प्रकल्प परिचालन को Dynamics 365 Customer Engagement संबंधी स्थिति में, स्रोत/गैर स्टॉक आधारित स्थिति में लिया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-116">You can have one legal entity using Project Operations on Dynamics 365 Customer Engagement for resource/non-stocked based scenarios.</span></span> <span data-ttu-id="2ee6d-117">इसी परिवेश में, आपके पास एक अन्य कानूनी निकाय हो सकता है जिसमें प्रकल्प परिचालन का उपयोग स्टॉक किये हुए/ उत्पादन आदेश के स्वरुप में हो सकता है.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-117">In the same environment, you can have another legal entity using Project Operations for stocked/production order scenarios.</span></span>

1. <span data-ttu-id="2ee6d-118">Dynamics 365 Finance में, **परियोजना प्रबंधन और लेखांकन** > **सेट अप** > **ग्लोबल परियोजना प्रबंधन और लेखा मापदंड** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-118">In Dynamics 365 Finance, go to **Project management and accounting** > **Setup** > **Global project management and accounting parameters**.</span></span>
2. <span data-ttu-id="2ee6d-119">उपलब्ध कानूनी निकायों में से, उन निकायों को चुनिये जहां पर एकाधिक अनुबन्ध लाइन्स और प्रकल्प परिचालन Dynamics 365 Customer Engagement की विशेषताओं के साथ सक्रिय है.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-119">In the list of available legal entities, select entities where multiple contract lines and Project Operations on Dynamics 365 Customer Engagement features will be enabled.</span></span> <span data-ttu-id="2ee6d-120">उन कानूनी निकायों को छोड़ दीजिये जिनमें प्रकल्प परिचालन का उपयोग स्टॉक किये हुए/उत्पादन आदेश संबंधी प्रकारों को चुना नही गया है.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-120">Leave legal entities that will be using Project Operations for stocked/production order scenarios unselected.</span></span>

> [!NOTE]
> <span data-ttu-id="2ee6d-121">एक कानूनी निकाय को केवल तभी चुना जा सकता है यदि उसमें पहले से कोई जारी प्रकल्प नही हो.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-121">A legal entity can be selected only if it doesn't have any existing projects.</span></span>

## <a name="configure-project-management-and-accounting-parameters"></a><span data-ttu-id="2ee6d-122">प्रकल्प प्रबन्धन और लेखांकन मापदन्डों को कॉन्फिगर करें</span><span class="sxs-lookup"><span data-stu-id="2ee6d-122">Configure Project management and accounting parameters</span></span>

<span data-ttu-id="2ee6d-123">प्रत्येक कानूनी निकाय जिसमें प्रकल्प परिचालन को Dynamics 365 Customer Engagement की जरुरतों के अनुसार डीफॉल्ट मापदन्डों के अनुरुप बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-123">Each legal entity using Project Operations on Dynamics 365 Customer Engagement needs a set of default parameters.</span></span> <span data-ttu-id="2ee6d-124">ये मापदंड **प्रकल्प परिचालन** टैब पर कॉन्फिगर होते हैं जो कि **प्रकल्प प्रबन्धन और लेखांकन मापदंड** पेज पर होते हैं.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-124">These parameters are configured on the **Project Operations** tab on the **Project management and accounting parameters** page.</span></span> <span data-ttu-id="2ee6d-125">पैरामीटर हैं:</span><span class="sxs-lookup"><span data-stu-id="2ee6d-125">The parameters are:</span></span>

  - <span data-ttu-id="2ee6d-126">**बिलिंग प्रकार डिफॉल्ट्स**: प्रकल्प परिचालन में तयशुदा बिलिंग प्रकारों को डिफॉल्ट के रुप में चुना जाता है जिसे लाइन फायनास विशेषताओं के साथ मैप किया जाना आवश्यक है.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-126">**Billing type defaults**: Project Operations uses a fixed set of billing type defaults that must be mapped to line properties Finance.</span></span> <span data-ttu-id="2ee6d-127">प्रत्येक बिलिंग प्रकार के लिये रेकॉर्ड तैयार करें: **बताया नही गया**, **सशुल्क**, **निशुल्क**, **मुफ्त**, और **अनुपलब्ध**.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-127">Create a record for each billing type: **Not specified**, **Chargeable**, **Non-chargeable**, **Complimentary**, and **Not available**.</span></span>
  - <span data-ttu-id="2ee6d-128">**प्रकल्प श्रेणी डिफॉल्ट्स**: डिफॉल्ट प्रकल्प श्रेणियों को चुनिये जिन्हे प्रत्येक लेन देन के प्रकार के लिये उपयोग में लाया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-128">**Project category defaults**: Select the default project categories to be used for each transaction type.</span></span> <span data-ttu-id="2ee6d-129">ये डिफॉल्ट्स भी इस प्रकार से उपयोग में आएंगे **प्रकल्प परिचालन एकीकरण जर्नल** और अनुमान के साथ जहां पर किसी प्रकार की लेन देन की श्रेणी बताई नही गई होगी, वह वास्तविक प्रकल्प हेतु संबद्ध श्रेणी होती है.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-129">These defaults will be used in the **Project Operations Integration journal** and in estimates where no transaction category is specified for the project actual.</span></span>
  - <span data-ttu-id="2ee6d-130">**अनुमान**: अनुमान मॉडल को चुनिये जिसे समय और खर्च अनुमान के लिये इस्तेमाल किया जाना है.</span><span class="sxs-lookup"><span data-stu-id="2ee6d-130">**Forecasts**: Select the forecast model to be used for time and expense estimates.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]