---
title: अनुमोदन सेट
description: यह विषय अनुमोदन सेट, अनुरोधों और उन कार्यों के सबसेट के बारे में जानकारी प्रदान करता है.
author: stsporen
manager: tfehr
ms.date: 05/28/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: ac73313420029ece740d0bdb9c21c7abaa9defc6
ms.sourcegitcommit: fc96c6eb9a2094f9fa3d1ae39646730ef9d558ba
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/28/2021
ms.locfileid: "6116873"
---
# <a name="approval-sets"></a><span data-ttu-id="55907-103">अनुमोदन सेट</span><span class="sxs-lookup"><span data-stu-id="55907-103">Approval sets</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="55907-104">अनुमोदन समूह अनुमोदन अनुरोधों को संचालन के छोटे उपसमूहों में एक साथ सेट करता है.</span><span class="sxs-lookup"><span data-stu-id="55907-104">Approval sets group approval requests together into smaller subsets of operations.</span></span> <span data-ttu-id="55907-105">यह समूहीकरण प्रोजेक्ट के अनुसार अनुमोदनों को संसाधित करने और फिर दोबारा प्रयास करने और अनुक्रमण की अनुमति देता है.</span><span class="sxs-lookup"><span data-stu-id="55907-105">This grouping allows approvals to be processed in order by Project and allows for retrying and sequencing.</span></span> <span data-ttu-id="55907-106">समूहीकरण बड़ी मात्रा में अनुमोदनों के लिए अनुमोदन संसाधित करने की विश्वसनीयता और पता लगाने की क्षमता में सुधार करता है.</span><span class="sxs-lookup"><span data-stu-id="55907-106">Grouping improves the reliability and traceability of approval processing for large volumes of approvals.</span></span>

<span data-ttu-id="55907-107">अनुमोदन सेट उनके संबंधित रिकॉर्ड की समग्र संसाधित होने की स्थिति दिखाते हैं.</span><span class="sxs-lookup"><span data-stu-id="55907-107">Approval sets indicate the overall processing state of their related records.</span></span> <span data-ttu-id="55907-108">जब अनुमोदन सेट का उपयोग करके अनुमोदन रिकॉर्ड संसाधित किया जाता है, तो रिकॉर्ड **सबमिट किया गया** से **अनुमोदित किया गया** हो जाता है और स्वीकृति सेट से अनलिंक हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="55907-108">When an approval record is processed using an approval set, the record moves from **Submitted** to **Approved**, and is unlinked from the approval set.</span></span> <span data-ttu-id="55907-109">यदि कोई रिकॉर्ड अनुमोदन के लिए सबमिट किए जाने पर विफल हो जाता है, तो रिकॉर्ड **सबमिट किया गया** स्थिति में रहता है और अनुमोदन सेट को विफल के रूप में चिह्नित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="55907-109">If a record fails when it is submitted for approval, the record remains in a status of **Submitted** and the approval set is marked as failed.</span></span> <span data-ttu-id="55907-110">अनुमोदन सेट विफलता के त्रुटि संदेश को लॉग करता है.</span><span class="sxs-lookup"><span data-stu-id="55907-110">The approval set logs the error message of the failure.</span></span>

## <a name="processing-approvals-and-approval-sets"></a><span data-ttu-id="55907-111">संसाधित करने के अनुमोदन और अनुमोदन सेट</span><span class="sxs-lookup"><span data-stu-id="55907-111">Processing approvals and approval sets</span></span>
<span data-ttu-id="55907-112">संसाधित के लिए कतारबद्ध अनुमोदन **संसाधित करने के अनुमोदन** दृश्य में दिखाई देते हैं.</span><span class="sxs-lookup"><span data-stu-id="55907-112">Approvals that are queued for processing are visible in the **Processing Approvals** view.</span></span> <span data-ttu-id="55907-113">सिस्टम सभी प्रविष्टियों को कई बार असमकालिक रूप से संसाधित करने का प्रयास करता है, जिसमें पिछले प्रयास विफल होने पर अनुमोदन का फिर कोशिश करना शामिल है.</span><span class="sxs-lookup"><span data-stu-id="55907-113">The system tries to process all the entries multiple times asynchronously, including retrying an approval if previous attempts failed.</span></span>

<span data-ttu-id="55907-114">**अनुमोदन सेट लाइफ़टाइम** फ़ील्ड विफल के रूप में चिह्नित किए जाने से पहले सेट को संसाधित करने के लिए शेष प्रयासों की संख्या को रिकॉर्ड करती है.</span><span class="sxs-lookup"><span data-stu-id="55907-114">The **Approval Set Lifetime** field records the number of attempts left to process the set before it's marked as failed.</span></span>

## <a name="failed-approvals-and-approval-sets"></a><span data-ttu-id="55907-115">विफल अनुमोदन और अनुमोदन सेट</span><span class="sxs-lookup"><span data-stu-id="55907-115">Failed approvals and approval sets</span></span>
<span data-ttu-id="55907-116">**विफल अनुमोदन** दृश्य उन सभी अनुमोदनों को सूचीबद्ध करता है, जिनके लिए उपयोगकर्ता का हस्तक्षेप करना ज़रूरी होता है.</span><span class="sxs-lookup"><span data-stu-id="55907-116">The **Failed Approvals** view lists all approvals that require user intervention.</span></span> <span data-ttu-id="55907-117">विफलता के कारण की पहचान करने के लिए संबद्ध अनुमोदन सेट लॉग खोलें.</span><span class="sxs-lookup"><span data-stu-id="55907-117">Open the associated approval set logs to identify the cause of the failure.</span></span>
<span data-ttu-id="55907-118">**फिर कोशिश करें** का चयन करने से अनुमोदन सेट लाइफ़टाइम गणना में जुड़ जाता है, अनुमोदन सेट को वापस **संसाधित किया जा रहा है** की स्थिति में ले जाता है और शेष रिकॉर्ड को संसाधित करने का प्रयास करता है.</span><span class="sxs-lookup"><span data-stu-id="55907-118">Selecting **Retry** adds to the approval set lifetime count, moves the approval set back to a status of **Processing**, and attempts to process the remaining records.</span></span>

## <a name="configure-approval-sets"></a><span data-ttu-id="55907-119">अनुमोदन सेट कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="55907-119">Configure approval sets</span></span>

###  <a name="enable-the-approval-sets-feature"></a><span data-ttu-id="55907-120">अनुमोदन सेट विशेषता सक्षम करें</span><span class="sxs-lookup"><span data-stu-id="55907-120">Enable the Approval sets feature</span></span>
<span data-ttu-id="55907-121">इससे पहले कि आप अनुमोदन सेट सुविधा को सक्षम करें, सत्यापित करें कि वर्तमान में कोई अनुमोदन संसाधित नहीं किया जा रहा है.</span><span class="sxs-lookup"><span data-stu-id="55907-121">Before you enable the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="55907-122">**प्रोजेक्ट मापदंड** पेज पर जाएं और **सुविधा नियंत्रण** > **आधुनिक अनुमोदन सक्षम करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="55907-122">Go to the **Project parameters** page and select **Feature Control** > **Enable Modern Approvals**.</span></span>

### <a name="turn-off-the-approval-sets-feature"></a><span data-ttu-id="55907-123">अनुमोदन सेट सुविधा बंद करें</span><span class="sxs-lookup"><span data-stu-id="55907-123">Turn off the Approval sets feature</span></span>
<span data-ttu-id="55907-124">अनुमोदन सेट सुविधा को बंद करने से पहले, सत्यापित करें कि वर्तमान में कोई अनुमोदन संसाधित नहीं किया जा रहा है.</span><span class="sxs-lookup"><span data-stu-id="55907-124">Before you turn off the Approval sets feature, verify that there are no approvals currently being processed.</span></span>

- <span data-ttu-id="55907-125">**प्रोजेक्ट मापदंड** पेज पर जाएं और **सुविधा नियंत्रण** > **आधुनिक अनुमोदन अक्षम करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="55907-125">Go to the **Project Parameters** page and select **Feature Control** > **Disable Modern Approvals**.</span></span>

### <a name="configuring-the-asynchronous-threshold"></a><span data-ttu-id="55907-126">एसिंक्रॉनस सीमा कॉन्फ़िगर करना</span><span class="sxs-lookup"><span data-stu-id="55907-126">Configuring the asynchronous threshold</span></span> 
<span data-ttu-id="55907-127">जब अनुमोदन सेट बनाए जाते हैं, तो अनुमोदन के लिए रिकॉर्ड की चयनित संख्या निर्दिष्ट सीमा से अधिक होने पर संसाधित करना पृष्ठभूमि में चला जाता है.</span><span class="sxs-lookup"><span data-stu-id="55907-127">When approval sets are created, processing moves to the background when the selected number of records for approval exceeds the indicated threshold.</span></span> <span data-ttu-id="55907-128">जब अनुमोदन प्रक्रिया को सिंक्रॉनस रूप से या एसिंक्रॉनस रूप से चलाया जाना चाहिए, तब कॉन्फ़िगर करने के लिए **एसिन्क्रॉनस सीमा** फ़ील्ड का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="55907-128">Use the **Asynchronous Threshold** field to configure when approval processing should be run synchronously or asynchronously.</span></span>
<span data-ttu-id="55907-129">मान्य मान हैं:</span><span class="sxs-lookup"><span data-stu-id="55907-129">Valid values are:</span></span>

  - <span data-ttu-id="55907-130">शून्य: सभी अनुरोधों को एसिंक्रॉनस रूप में संसाधित करना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="55907-130">Zero: All requests should be processed asynchronously.</span></span> 
  - <span data-ttu-id="55907-131">शून्य से अधिक संख्याएं: अनुमोदनों को एसिंक्रॉनस रूप से तभी संसाधित किया जाता है, जब अनुमोदनों की सबमिट की गयी संख्या इस मान से अधिक हो जाती है.</span><span class="sxs-lookup"><span data-stu-id="55907-131">Numbers greater than zero: Approvals are processed asynchronously only when the submitted number of approvals exceeds this value.</span></span>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
