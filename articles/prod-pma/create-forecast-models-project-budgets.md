---
title: प्रोजेक्ट बजट के लिए पूर्वानुमान मॉडल बनाएं
description: यह विषय शेष बजट के लिए पूर्वानुमान मॉडल बनाने का तरीका बताता है.
author: Yowelle
manager: AnnBe
ms.date: 04/24/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 7
ms.search.validFrom: 2019-01-15
ms.openlocfilehash: 5a3b9d3c154a85b50536a67ae0eb45d9b4f25f15
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271040"
---
# <a name="create-forecast-models-for-project-budgets"></a><span data-ttu-id="b0b74-103">प्रोजेक्ट बजट के लिए पूर्वानुमान मॉडल बनाएं</span><span class="sxs-lookup"><span data-stu-id="b0b74-103">Create forecast models for project budgets</span></span> 

[!include [banner](../includes/banner.md)]

<span data-ttu-id="b0b74-104">यह विषय शेष बजट के लिए पूर्वानुमान मॉडल बनाने का तरीका बताता है.</span><span class="sxs-lookup"><span data-stu-id="b0b74-104">This topic describes how to create a forecast model for remaining budgets.</span></span> <span data-ttu-id="b0b74-105">एक प्रोजेक्ट जो बजट नियंत्रण के अधीन है, दो प्रकार के बजट का उपयोग करती है: मूल और शेष.</span><span class="sxs-lookup"><span data-stu-id="b0b74-105">A project that is subject to budget control uses two types of budgets: original and remaining.</span></span> <span data-ttu-id="b0b74-106">जब आप कोई प्रोजेक्ट बजट बनाते हैं, तो आपको मूल और शेष बजट का पूर्वानुमान मॉडल निर्दिष्ट करना होगा जो **पूर्वानुमान मॉडल** पृष्ठ में बनाए गए थे.</span><span class="sxs-lookup"><span data-stu-id="b0b74-106">When you create a project budget, you must specify the original and remaining budget forecast models that were created in the **Forecast models** page.</span></span> <span data-ttu-id="b0b74-107">जब आप प्रोजेक्ट बजट करते हैं तो निर्दिष्ट मॉडलों के आधार पर प्रोजेक्ट बजट बनाए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="b0b74-107">Project budgets based on the specified models are created when you commit the project budget.</span></span>

> [!NOTE]
> <span data-ttu-id="b0b74-108">बजट नियंत्रण के लिए उपयोग किये जाने वाला पूर्वानुमान मॉडल में उपमॉडल नहीं हो सकता है या उपमॉडल के रूप में उपयोग नहीं हो सकता है.</span><span class="sxs-lookup"><span data-stu-id="b0b74-108">A forecast model that is used for budget control can’t have a submodel or be used as a submodel.</span></span>

1. <span data-ttu-id="b0b74-109">**प्रोजेक्ट प्रबंधन और लेखांकन** > **सेटअप** > **पूर्वानुमान**  > **पूर्वानुमान मॉडल** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="b0b74-109">Select **Project management and accounting** > **Setup** > **Forecasts**  > **Forecast models**.</span></span>
2. <span data-ttu-id="b0b74-110">एक नया पूर्वानुमान मॉडल बनाने के लिए **नया** चुनें, और फिर नए मॉडल के लिए एक मॉडल ID नंबर और नाम दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="b0b74-110">Select **New** to create a new forecast model, and then enter a model ID number and name for the new model.</span></span> 
3. <span data-ttu-id="b0b74-111">पूर्वानुमान मॉडल के लिए पूर्वानुमान लाइनों में किसी भी परिवर्तन को रोकने के लिए **बंद हुआ** विकल्प को **हा** पर सेट करें.</span><span class="sxs-lookup"><span data-stu-id="b0b74-111">Set the **Stopped** option to **Yes** to prevent any changes to the forecast lines for the forecast model.</span></span> 
4. <span data-ttu-id="b0b74-112">यदि मॉडल के साथ जुड़ी हुई पूर्वानुमान लाइनें सामान्य खाता बही में नकदी प्रवाह पूर्वानुमान उत्पन्न करती हैं, तो सेट करें **नकदी प्रवाह पूर्वानुमान में शामिल करें** सेवा **हाँ.**</span><span class="sxs-lookup"><span data-stu-id="b0b74-112">If the forecast lines that the model is associated with should generate cash flow forecasts in the general ledger, set **Include in Cash flow forecasts** to **Yes.**</span></span> 
5. <span data-ttu-id="b0b74-113">इनवॉइस की तिथि के रूप में प्रोजेक्ट की तिथि का उपयोग करने के लिए, **इनवॉइस तिथि का पूर्वानुमान** को **हाँ** पर सेट करें.</span><span class="sxs-lookup"><span data-stu-id="b0b74-113">To use the project date as the invoice date, set **Forecast Invoice date** to **Yes**.</span></span> 
6. <span data-ttu-id="b0b74-114">**बजट के प्रकार** फ़ील्ड में, निम्नलिखित मॉडल के प्रकारों में से एक का चयन करें:</span><span class="sxs-lookup"><span data-stu-id="b0b74-114">In the **Budget type** field, select one of the following model types:</span></span>

   - <span data-ttu-id="b0b74-115">**मूल बजट**: प्रारंभिक बजट बनाने और अनुमोदित होने पर तय की गई मूल बजट राशि का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="b0b74-115">**Original budget**: Use the original budget amounts that are committed when the initial budget is created and approved.</span></span>
   - <span data-ttu-id="b0b74-116">**शेष बजट**: प्रोजेक्ट की सक्रियता के दौरान शेष बजट राशि का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="b0b74-116">**Remaining budget**: Use the remaining budget amounts during the life of the project.</span></span> <span data-ttu-id="b0b74-117">इस पूर्वानुमान मॉडल में शेष राशि वास्तविक लेनदेन से कम हो जाती है और बजट के संशोधनों से बढ़ जाती है या कम हो जाती है.</span><span class="sxs-lookup"><span data-stu-id="b0b74-117">The balances in this forecast model are reduced by actual transactions and increased or decreased by budget revisions.</span></span>
   - <span data-ttu-id="b0b74-118">**कैरी-फॉरवर्ड**: प्रोजेक्ट के लिए कैरी-फॉरवर्ड बजट राशि का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="b0b74-118">**Carry-forward**: Use the carry-forward budget amounts for the project.</span></span> <span data-ttu-id="b0b74-119">कैरी-फॉरवर्ड एक वैकल्पिक प्रक्रिया है जिसे उपयोग ना हुए बजट राशि को एक वित्तीय वर्ष से दूसरे में स्थानांतरित करने के लिए चलाया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b0b74-119">Carry-forward is an optional process that can be run to transfer unused budget amounts from one fiscal year to another.</span></span>

7. <span data-ttu-id="b0b74-120">आवश्यकतानुसार निम्नलिखित विकल्प निर्धारित करें:</span><span class="sxs-lookup"><span data-stu-id="b0b74-120">Set the following options as required:</span></span>

   - <span data-ttu-id="b0b74-121">इनवॉइस तिथि के रूप में प्रोजेक्ट की तिथि का उपयोग करने के लिए **इनवॉइस तिथि का पूर्वानुमान** सक्षम करें.</span><span class="sxs-lookup"><span data-stu-id="b0b74-121">Enable **Forecast invoice date** to use the project date as the invoice date.</span></span>
   - <span data-ttu-id="b0b74-122">कार्य प्रगति पर (WIP) के आधार पर पूर्वानुमान लगाने के लिए **WIP के साथ पूर्वानुमान** सक्षम करें, और फिर WIP के प्रकार का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="b0b74-122">Enable **Forecast with WIP** to forecast based on work in progress (WIP), and then select the type of WIP.</span></span> 
   - <span data-ttu-id="b0b74-123">आप **कोई नहीं** के रूप में डिफ़ॉल्ट **बजट के प्रकार** रख सकते हैं या एक नया प्रकार दर्ज कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="b0b74-123">You can keep the default **Budget type** as **None** or enter a new type.</span></span> <span data-ttu-id="b0b74-124">आपके द्वारा रिकॉर्ड बदलने के बाद बजट का प्रकार बदला नहीं जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="b0b74-124">The budget type can't be changed after you change a record.</span></span>     
    > [!NOTE]
    > <span data-ttu-id="b0b74-125">यदि आप डिफ़ॉल्ट बजट का प्रकार बदलते हैं, तो अन्य सभी विकल्प अपडेट के लिए अनुपलब्ध हो जाएंगे, और आप इस पूर्वानुमान मॉडल का पुन: उपयोग नहीं कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="b0b74-125">If you change the default budget type, all other options will become unavailable for updates, and you can't reuse this forecast model.</span></span> 
   


 



[!INCLUDE[footer-include](../includes/footer-banner.md)]