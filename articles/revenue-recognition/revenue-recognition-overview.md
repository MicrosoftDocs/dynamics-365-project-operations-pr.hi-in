---
title: आय पहचान ओवरव्यू
description: इस विषय में Project Operations में आय पहचान के बारे में जानकारी दी गई है.
author: sigitac
ms.date: 11/16/2020
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: f5f962572c6ec0298d2d91d33f83e4120a498a6f
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6013758"
---
# <a name="revenue-recognition-overview"></a><span data-ttu-id="70819-103">आय पहचान ओवरव्यू</span><span class="sxs-lookup"><span data-stu-id="70819-103">Revenue recognition overview</span></span>

<span data-ttu-id="70819-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="70819-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="70819-105">Dynamics 365 Project Operations में, आय पहचान सिद्धांत परियोजना या परियोजना के हिस्से के लिए चयनित बिलिंग विधि के आधार पर भिन्न होते हैं.</span><span class="sxs-lookup"><span data-stu-id="70819-105">In Dynamics 365 Project Operations, revenue recognition principles vary based on the selected billing method for a project or portion of the project.</span></span> <span data-ttu-id="70819-106">इस विषय में Project Operations में आय पहचान के बारे में जानकारी दी गई है.</span><span class="sxs-lookup"><span data-stu-id="70819-106">This topic provides information about revenue recognition in Project Operations.</span></span>

## <a name="transactions-accounted-using-time-and-material-billing-method"></a><span data-ttu-id="70819-107">समय और सामग्री बिलिंग विधि का उपयोग करके लेनदेन लेखा-जोखा</span><span class="sxs-lookup"><span data-stu-id="70819-107">Transactions accounted using time and material billing method</span></span>

- <span data-ttu-id="70819-108">लागत और आय पहचान जुड़े हुए हैं.</span><span class="sxs-lookup"><span data-stu-id="70819-108">Cost and revenue recognition are connected.</span></span> <span data-ttu-id="70819-109">लेनदेन लागत और बिल न किए गए विक्रय को [Project Operations एकीकरण जर्नल](../project-accounting/project-operations-integration-journal.md) का उपयोग करके पोस्ट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="70819-109">Transaction cost and unbilled sales are posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span>
- <span data-ttu-id="70819-110">परियोजना लागत और आय प्रोफ़ाइल निर्धारित करती हैं कि बिल न किए गए विक्रय लेनदेन को सामान्य लेज़र में पोस्ट किया गया है या नहीं.</span><span class="sxs-lookup"><span data-stu-id="70819-110">Project cost and revenue profile determine if unbilled sales transactions are posted to the general ledger.</span></span> <span data-ttu-id="70819-111">यदि **आय में वृद्धि** चयनित है, तो सिस्टम **WIP विक्रय मूल्य** का उपयोग करता है और **उपार्जित आय विक्रय मूल्य** पर पोस्टिंग के दौरान ध्यान दिया जाता है.</span><span class="sxs-lookup"><span data-stu-id="70819-111">If **Accrue revenue** is selected, the system uses the **WIP sales value** and the **Accrued revenue sales value** accounts during posting.</span></span> <span data-ttu-id="70819-112">निम्न इस तरीका का एक उदाहरण है.</span><span class="sxs-lookup"><span data-stu-id="70819-112">The following is an example of this method.</span></span>  

  | <span data-ttu-id="70819-113">लेनदेन प्रकार</span><span class="sxs-lookup"><span data-stu-id="70819-113">Transaction type</span></span> | <span data-ttu-id="70819-114">डेबिट/क्रेडिट</span><span class="sxs-lookup"><span data-stu-id="70819-114">Debit/Credit</span></span> | <span data-ttu-id="70819-115">राशि</span><span class="sxs-lookup"><span data-stu-id="70819-115">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="70819-116">WIP विक्रय मूल्य</span><span class="sxs-lookup"><span data-stu-id="70819-116">WIP Sales value</span></span> | <span data-ttu-id="70819-117">डेबिट</span><span class="sxs-lookup"><span data-stu-id="70819-117">Debit</span></span> | <span data-ttu-id="70819-118">100</span><span class="sxs-lookup"><span data-stu-id="70819-118">100</span></span> |
  | <span data-ttu-id="70819-119">उपार्जित आय विक्रय मूल्य</span><span class="sxs-lookup"><span data-stu-id="70819-119">Accrued revenue sales value</span></span> | <span data-ttu-id="70819-120">क्रेडिट</span><span class="sxs-lookup"><span data-stu-id="70819-120">Credit</span></span> | <span data-ttu-id="70819-121">100</span><span class="sxs-lookup"><span data-stu-id="70819-121">100</span></span> |

- <span data-ttu-id="70819-122">आय की पहचान इनवॉइसिंग के दौरान की जाती है.</span><span class="sxs-lookup"><span data-stu-id="70819-122">Revenue is recognized during invoicing.</span></span> <span data-ttu-id="70819-123">सिस्टम पोस्टिंग के दौरान **इनवॉइस की गई आय** खाते का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="70819-123">The system uses the **Invoiced revenue** account during posting.</span></span> <span data-ttu-id="70819-124">निम्न इस तरीका का एक उदाहरण है.</span><span class="sxs-lookup"><span data-stu-id="70819-124">The following is an example of this method.</span></span>  

  | <span data-ttu-id="70819-125">लेनदेन प्रकार</span><span class="sxs-lookup"><span data-stu-id="70819-125">Transaction type</span></span> | <span data-ttu-id="70819-126">डेबिट/क्रेडिट</span><span class="sxs-lookup"><span data-stu-id="70819-126">Debit/Credit</span></span> | <span data-ttu-id="70819-127">राशि</span><span class="sxs-lookup"><span data-stu-id="70819-127">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="70819-128">ग्राहक शेष</span><span class="sxs-lookup"><span data-stu-id="70819-128">Customer balance</span></span> | <span data-ttu-id="70819-129">डेबिट</span><span class="sxs-lookup"><span data-stu-id="70819-129">Debit</span></span> | <span data-ttu-id="70819-130">120</span><span class="sxs-lookup"><span data-stu-id="70819-130">120</span></span> |
  | <span data-ttu-id="70819-131">देययोग्य विक्रय कर</span><span class="sxs-lookup"><span data-stu-id="70819-131">Sales tax payable</span></span> | <span data-ttu-id="70819-132">क्रेडिट</span><span class="sxs-lookup"><span data-stu-id="70819-132">Credit</span></span> | <span data-ttu-id="70819-133">20</span><span class="sxs-lookup"><span data-stu-id="70819-133">20</span></span> |
  | <span data-ttu-id="70819-134">इनवॉइस की गई आय</span><span class="sxs-lookup"><span data-stu-id="70819-134">Invoiced Revenue</span></span> | <span data-ttu-id="70819-135">क्रेडिट</span><span class="sxs-lookup"><span data-stu-id="70819-135">Credit</span></span> | <span data-ttu-id="70819-136">100</span><span class="sxs-lookup"><span data-stu-id="70819-136">100</span></span> |

- <span data-ttu-id="70819-137">यदि बिल न की गई विक्रय पोस्ट किए जाने पर आय उपार्जित की गई थी, तो सिस्टम इनवॉइस करने पर उपार्जित आय को रिवर्स कर देगा.</span><span class="sxs-lookup"><span data-stu-id="70819-137">If revenue was accrued when the unbilled sales are posted, the system will reverse the accrued revenue at invoicing.</span></span>

  | <span data-ttu-id="70819-138">लेनदेन प्रकार</span><span class="sxs-lookup"><span data-stu-id="70819-138">Transaction type</span></span> | <span data-ttu-id="70819-139">डेबिट/क्रेडिट</span><span class="sxs-lookup"><span data-stu-id="70819-139">Debit/Credit</span></span> | <span data-ttu-id="70819-140">राशि</span><span class="sxs-lookup"><span data-stu-id="70819-140">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="70819-141">WIP विक्रय मूल्य</span><span class="sxs-lookup"><span data-stu-id="70819-141">WIP Sales value</span></span> | <span data-ttu-id="70819-142">क्रेडिट</span><span class="sxs-lookup"><span data-stu-id="70819-142">Credit</span></span> | <span data-ttu-id="70819-143">100</span><span class="sxs-lookup"><span data-stu-id="70819-143">100</span></span> |
  | <span data-ttu-id="70819-144">उपार्जित आय विक्रय मूल्य</span><span class="sxs-lookup"><span data-stu-id="70819-144">Accrued revenue sales value</span></span> | <span data-ttu-id="70819-145">डेबिट</span><span class="sxs-lookup"><span data-stu-id="70819-145">Debit</span></span> | <span data-ttu-id="70819-146">100</span><span class="sxs-lookup"><span data-stu-id="70819-146">100</span></span> |

## <a name="transactions-accounted-using-the-fixed-price-billing-method"></a><span data-ttu-id="70819-147">निश्चित मूल्य बिलिंग विधि का उपयोग करके लेनदेन लेखा-जोखा</span><span class="sxs-lookup"><span data-stu-id="70819-147">Transactions accounted using the fixed price billing method</span></span>

- <span data-ttu-id="70819-148">लागत और आय पहचान अलग-अलग होते हैं.</span><span class="sxs-lookup"><span data-stu-id="70819-148">Cost and revenue recognition are separate.</span></span> <span data-ttu-id="70819-149">लेनदेन लागत को [Project Operations एकीकरण जर्नल](../project-accounting/project-operations-integration-journal.md) का उपयोग करके पोस्ट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="70819-149">Transaction cost is posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="70819-150">बिल न किए गए विक्रय लेनदेन बनाए नहीं जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="70819-150">Unbilled sales transactions aren't created.</span></span>
- <span data-ttu-id="70819-151">यदि परियोजना लागत और आय प्रोफ़ाइल के **परियोजना पूर्णता गणना के लिए उपयोग किया जाने वाले सिद्धांत** को **कोई WIP नहीं** पर सेट किया गया है, तो आय को इनवॉइस करने के दौरान पहचाना जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="70819-151">Revenue can be recognized during invoicing if the project cost and revenue profile have **Principle used for project completion calculations** set to **No WIP**.</span></span> <span data-ttu-id="70819-152">केवल कम अवधि, सरल परियोजनाओं के लिए इस विधि का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="70819-152">Only use this method for short term, simple projects.</span></span>
- <span data-ttu-id="70819-153">आय को या तो **पूर्ण अनुबंध** या **प्रतिशत पूर्णता आय पहचान** विधि के साथ निश्चित मूल्य आय अनुमानों का उपयोग करके पहचाना जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="70819-153">Revenue can be recognized using fixed price revenue estimates, with either the **Completed contract** or **Percent completion revenue recognition** method.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="70819-154">अतिरिक्त संसाधन</span><span class="sxs-lookup"><span data-stu-id="70819-154">Additional resources</span></span>
[<span data-ttu-id="70819-155">बिल करने योग्य परियोजना आलेख के लिए लेखांकन कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="70819-155">Configure accounting for billable projects article</span></span>](../project-accounting/configure-accounting-billable-projects.md)

[<span data-ttu-id="70819-156">निश्चित मूल्य आय अनुमान परियोजनाएँ</span><span class="sxs-lookup"><span data-stu-id="70819-156">Fixed price revenue estimate projects</span></span>](rev-rec-percentage-completion-method.md)

[<span data-ttu-id="70819-157">आय अनुमान प्रबंधित करें</span><span class="sxs-lookup"><span data-stu-id="70819-157">Manage revenue estimates</span></span>](rev-rec-completed-contract-method.md)

[<span data-ttu-id="70819-158">पूर्णता की लागत विधि</span><span class="sxs-lookup"><span data-stu-id="70819-158">Cost to complete methods</span></span>](cost-complete-methods.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]