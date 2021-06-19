---
title: प्रोजेक्ट संसाधन शेड्यूलिंग प्रदर्शन
description: यह विषय बड़ी संख्या में परियोजनाओं के लिए संसाधन निर्धारण के प्रदर्शन को बेहतर बनाने के बारे में जानकारी देता है.
author: Yowelle
ms.date: 08/31/2020
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.14
ms.search.validFrom: 2020-09-01
ms.openlocfilehash: 113023909f88cb4dd498190ef21b6955482b25dd
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6010023"
---
# <a name="project-resource-scheduling-performance"></a><span data-ttu-id="9228a-103">प्रोजेक्ट संसाधन शेड्यूलिंग प्रदर्शन</span><span class="sxs-lookup"><span data-stu-id="9228a-103">Project resource scheduling performance</span></span>

[!include [banner](../includes/banner.md)]
[!include [banner](../includes/preview-banner.md)]


<span data-ttu-id="9228a-104">संसाधन शेड्यूलिंग से संबंधित प्रदर्शन समस्याएँ तब हो सकती हैं, जब परियोजनाओं की संख्या हज़ारों में पहुंच जाती है.</span><span class="sxs-lookup"><span data-stu-id="9228a-104">Performance issues related to resource scheduling can occur when the number of projects reaches into the thousands.</span></span> <span data-ttu-id="9228a-105">संसाधन शेड्यूलिंग प्रदर्शन को बेहतर बनाने के लिए, फ़ीचर उपलब्ध है जो उपयोगकर्ताओं को संसाधन उपलब्धता प्रपत्र को लॉन्च करने में लगने वाले समय को कम करने की अनुमति देता है.</span><span class="sxs-lookup"><span data-stu-id="9228a-105">To improve resource scheduling performance, a feature is available that allows users to reduce the time that it takes to launch the resource availability form.</span></span> <span data-ttu-id="9228a-106">विशेष रूप से, यह संसाधन क्षमता रोल-अप सिंक्रनाइज़ेशन प्रक्रिया को हटाता है और संसाधन लुकअप को गति देने के लिए **ResProjectResource** तालिका को इस्तेमाल करता है.</span><span class="sxs-lookup"><span data-stu-id="9228a-106">Specifically, this removes the resource capacity roll-up synchronization process and uses the **ResProjectResource** table to speed up the resource lookup.</span></span> <span data-ttu-id="9228a-107">ध्यान दें कि **ResRollup** तालिका अब इस्तेमाल नहीं की जाएगी.</span><span class="sxs-lookup"><span data-stu-id="9228a-107">Note that the **ResRollup** table will no longer be used.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9228a-108">यदि संसाधन क्षमता रोल-अप सिंक्रनाइज़ेशन प्रक्रिया या **ResProjectResource** तालिका पर निर्भरता है, तो इस फ़ीचर को इस्तेमाल न करें.</span><span class="sxs-lookup"><span data-stu-id="9228a-108">If there is a dependency on either the resource capacity roll-up synchronization process or the **ResProjectResource** table, do not use this feature.</span></span>

## <a name="enable-resource-scheduling-performance-enhancement"></a><span data-ttu-id="9228a-109">संसाधन शेड्यूलिंग प्रदर्शन वृद्धि सक्षम करें</span><span class="sxs-lookup"><span data-stu-id="9228a-109">Enable resource scheduling performance enhancement</span></span>
<span data-ttu-id="9228a-110">संसाधन शेड्यूलिंग प्रदर्शन वृद्धि को सक्षम करने के लिए, निम्न चरण पूरे करें.</span><span class="sxs-lookup"><span data-stu-id="9228a-110">To enable resource scheduling performance enhancement, complete the following steps.</span></span>

1. <span data-ttu-id="9228a-111">**फ़ीचर प्रबंधन** > **सभी**, पर जाएं और फ़ीचर सूची में, **संसाधन शेड्यूलिंग प्रदर्शन वृद्धि फ़ीचर सक्षम करें** ढूंढें.</span><span class="sxs-lookup"><span data-stu-id="9228a-111">Go to **Feature management** > **All**, and in the feature list, locate **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="9228a-112">**अभी सक्षम करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9228a-112">Select **Enable now**.</span></span>

> [!NOTE]
> <span data-ttu-id="9228a-113">यदि आपको सूची में फ़ीचर नहीं मिलता है, तो सूची को रीफ्रेश करने के लिए **अद्यतन के लिए जांचें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9228a-113">If you can't find the feature in the list, select **Check for updates** to refresh the list.</span></span>

3. <span data-ttu-id="9228a-114">अपना ब्राउज़र रीफ्रेश करें और फिर **परियोजना प्रबंधन और लेखांकन** > **आवधिक** > **परियोजना संसाधन** > **सभी कंपनियों में संसाधन कैलेंडर क्षमता को सिंक्रनाइज़ करें** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="9228a-114">Refresh your browser, and then go to **Project management and accounting** > **Periodic** > **Project resources** > **Synchronize resource calendars capacity across all companies**.</span></span>
4. <span data-ttu-id="9228a-115">पिछले डेटा को हटाने के लिए **मौजूदा क्षमता रिकॉर्ड हटाएं** को **हां** पर सेट करें.</span><span class="sxs-lookup"><span data-stu-id="9228a-115">Set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="9228a-116">यदि आप वृद्धि संबंधी डेटा उत्पन्न करना चाहते हैं, तो इसे **नहीं** पर सेट करें.</span><span class="sxs-lookup"><span data-stu-id="9228a-116">If you want generate incremental data, set it to **No**.</span></span>
5. <span data-ttu-id="9228a-117">**अवधि कोड** फ़ील्ड में, वह अवधि चुनें, जिसका डेटा उत्पन्न किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="9228a-117">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="9228a-118">यदि आप अवधि कोड चुनते हैं, तो प्रारंभ और अंतिम तिथि बताने की ज़रूरत नहीं है.</span><span class="sxs-lookup"><span data-stu-id="9228a-118">If you select a period code, a start and end date do not need to be defined.</span></span>
6. <span data-ttu-id="9228a-119">यदि आप **अवधि कोड** फ़ील्ड रिक्त छोड़ते हैं, तो डेटा उत्पन्न करने के लिए विशिष्ट प्रारंभ और समाप्ति तिथि चुनें.</span><span class="sxs-lookup"><span data-stu-id="9228a-119">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
7. <span data-ttu-id="9228a-120">**ठीक** चुनें।</span><span class="sxs-lookup"><span data-stu-id="9228a-120">Select **OK**.</span></span>

 > [!NOTE]
 > <span data-ttu-id="9228a-121">यह आपके परिवेश में सभी कंपनियों में **ResCalendarCapacity** तालिका में सामान्य डेटा वितरित करेगा, इसलिए बैच के कार्य को केवल एक कानूनी निकाय में चलाने की ज़रूरत है.</span><span class="sxs-lookup"><span data-stu-id="9228a-121">This will distribute general data to the **ResCalendarCapacity** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="9228a-122">संबंधित बैच के माध्यम से संसाधन क्षमता की गणना करने के लिए इस बैच के कार्य में डेटा की ज़रूरत है.</span><span class="sxs-lookup"><span data-stu-id="9228a-122">The data in this batch job is needed to calculate resource capacity through the associated calendar.</span></span>

8. <span data-ttu-id="9228a-123">**परियोजना प्रबंधन और लेखांकन** > **आवधिक** > **परियोजना संसाधन** > **सभी कंपनियों के परियोजना संसाधनों में पॉपुलेट करें** पर जाएं और फिर **ठीक है** चुनें.</span><span class="sxs-lookup"><span data-stu-id="9228a-123">Go to **Project management and accounting** > **Periodic** > **Project resources** > **Populate project resources across all companies** and then select **OK**.</span></span> <span data-ttu-id="9228a-124">यह **ResProjectResource**, **ResCalendarDateTimeRange** और **ResEffectiveDateTimeRange** तालिकाओं में सामान्य डेटा के लिए डेटा अपग्रेड स्क्रिप्ट है.</span><span class="sxs-lookup"><span data-stu-id="9228a-124">This is the data upgrade script for general data in the **ResProjectResource**, **ResCalendarDateTimeRange**, and **ResEffectiveDateTimeRange** tables.</span></span> <span data-ttu-id="9228a-125">**PSAPRojSchedRole.RootActivity** फ़ील्ड के लिए मान भी अद्यतन किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="9228a-125">Values for the **PSAPRojSchedRole.RootActivity** field are also updated.</span></span> <span data-ttu-id="9228a-126">यदि यह नहीं चलाया जाता है, तो संसाधन शेड्यूलिंग कार्रवाई निष्पादित करने का प्रयास करने पर आपको चेतावनी मिलेगी.</span><span class="sxs-lookup"><span data-stu-id="9228a-126">If this is not run, you will receive a warning when you try to execute resource scheduling operations.</span></span>
 
## <a name="turn-off-resource-scheduling-performance-enhancement"></a><span data-ttu-id="9228a-127">संसाधन शेड्यूलिंग प्रदर्शन वृद्धि बंद करें</span><span class="sxs-lookup"><span data-stu-id="9228a-127">Turn off resource scheduling performance enhancement</span></span>

1. <span data-ttu-id="9228a-128">**फ़ीचर प्रबंधन** > **सभी** पर जाएं और **परियोजना संसाधन शेड्यूलिंग प्रदर्शन वृद्धि फ़ीचर सक्षम करें** ढूंढें.</span><span class="sxs-lookup"><span data-stu-id="9228a-128">Go to **Feature management** > **All**  and search for **Enable project resource scheduling performance enhancement feature**.</span></span>
2. <span data-ttu-id="9228a-129">फ़ीचर चुनें और फिर **अक्षम करें** बटन चुनें.</span><span class="sxs-lookup"><span data-stu-id="9228a-129">Select the feature, and then select the **Disable** button.</span></span>
3. <span data-ttu-id="9228a-130">अपने ब्राउज़र को रिफ्रेश करें.</span><span class="sxs-lookup"><span data-stu-id="9228a-130">Refresh your browser.</span></span>
4. <span data-ttu-id="9228a-131">**परियोजना प्रबंधन और लेखा** > **आवधिक** > **क्षमता सिंक्रनाइनज़ेशन** > **संसाधन क्षमता रोल-अप सिंक्रनाइज़ करें** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="9228a-131">Go to **Project management and accounting** > **Periodic** > **Capacity synchronization** > **Synchronize resource capacity roll-ups**.</span></span>
5. <span data-ttu-id="9228a-132">पिछला डेटा हटाने के लिए **क्षमता रोल-अप सिंक्रॉनाइनज़ेश** पृष्ठ पर, **मौजूद क्षमता रिकॉर्ड हटाएं** को **हां** पर सेट करें.</span><span class="sxs-lookup"><span data-stu-id="9228a-132">On the **Capacity roll-up synchronization** page, set **Remove existing capacity records** to **Yes** to remove previous data.</span></span> <span data-ttu-id="9228a-133">अगर आप वृद्धि संबंधी डेटा उत्पन्न करना चाहते हैं, तो इसे **नहीं** पर सेट करें.</span><span class="sxs-lookup"><span data-stu-id="9228a-133">If you want to generate incremental data, set it to **No**.</span></span>
6. <span data-ttu-id="9228a-134">**अवधि कोड** फ़ील्ड में, वह अवधि चुनें, जिसका डेटा उत्पन्न किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="9228a-134">In the **Period code** field, select the period in which data should be generated.</span></span> <span data-ttu-id="9228a-135">यदि आप अवधि कोड चुनते हैं, तो प्रारंभ और अंतिम तिथि बताने की ज़रूरत नहीं है.</span><span class="sxs-lookup"><span data-stu-id="9228a-135">If you select a period code, a start and end date do not need to be defined.</span></span>
7. <span data-ttu-id="9228a-136">यदि आप **अवधि कोड** फ़ील्ड रिक्त छोड़ते हैं, तो डेटा उत्पन्न करने के लिए विशिष्ट प्रारंभ और समाप्ति तिथि चुनें.</span><span class="sxs-lookup"><span data-stu-id="9228a-136">If you leave the **Period code** field blank, select specific start and end dates to generate data.</span></span>
8. <span data-ttu-id="9228a-137">**ठीक** चुनें।</span><span class="sxs-lookup"><span data-stu-id="9228a-137">Select **OK**.</span></span>

> [!NOTE]
> <span data-ttu-id="9228a-138">यह आपके परिवेश में सभी कंपनियों के लिए **ResRollup** तालिका में सामान्य डेटा वितरित करेगा ताकि बैच का कार्य को केवल एक कानूनी निकाय में चलाने की ज़रूरत हो.</span><span class="sxs-lookup"><span data-stu-id="9228a-138">This will distribute general data to the **ResRollup** table across all companies in your environment, so the batch job only needs to be run in one legal entity.</span></span> <span data-ttu-id="9228a-139">यह बैच कार्य **संसाधन उपलब्धता** दृश्यों के लिए ज़रूरी है.</span><span class="sxs-lookup"><span data-stu-id="9228a-139">This batch job is needed for all **Resource Availability** views.</span></span> <span data-ttu-id="9228a-140">यदि यह बैच कार्य नहीं चलाया जाता है, तो **ResRollup** डेटा फ़्लाई पर उत्पन्न होगा, जिसमें समय लग सकता है.</span><span class="sxs-lookup"><span data-stu-id="9228a-140">If this batch job is not run, the **ResRollup** data will be generated on the fly, which can take time.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]