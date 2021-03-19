---
title: आय पहचान ओवरव्यू
description: इस विषय में Project Operations में आय पहचान के बारे में जानकारी दी गई है.
author: sigitac
manager: Annbe
ms.date: 11/16/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5e77a0442f634a50f8099fadec42ff400fee0e81
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5278870"
---
# <a name="revenue-recognition-overview"></a><span data-ttu-id="3b5e2-103">आय पहचान ओवरव्यू</span><span class="sxs-lookup"><span data-stu-id="3b5e2-103">Revenue recognition overview</span></span>

<span data-ttu-id="3b5e2-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="3b5e2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="3b5e2-105">Dynamics 365 Project Operations में, आय पहचान सिद्धांत परियोजना या परियोजना के हिस्से के लिए चयनित बिलिंग विधि के आधार पर भिन्न होते हैं.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-105">In Dynamics 365 Project Operations, revenue recognition principles vary based on the selected billing method for a project or portion of the project.</span></span> <span data-ttu-id="3b5e2-106">इस विषय में Project Operations में आय पहचान के बारे में जानकारी दी गई है.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-106">This topic provides information about revenue recognition in Project Operations.</span></span>

## <a name="transactions-accounted-using-time-and-material-billing-method"></a><span data-ttu-id="3b5e2-107">समय और सामग्री बिलिंग विधि का उपयोग करके लेनदेन लेखा-जोखा</span><span class="sxs-lookup"><span data-stu-id="3b5e2-107">Transactions accounted using time and material billing method</span></span>

- <span data-ttu-id="3b5e2-108">लागत और आय पहचान जुड़े हुए हैं.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-108">Cost and revenue recognition are connected.</span></span> <span data-ttu-id="3b5e2-109">लेनदेन लागत और बिल न किए गए विक्रय को [Project Operations एकीकरण जर्नल](../project-accounting/project-operations-integration-journal.md) का उपयोग करके पोस्ट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-109">Transaction cost and unbilled sales are posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span>
- <span data-ttu-id="3b5e2-110">परियोजना लागत और आय प्रोफ़ाइल निर्धारित करती हैं कि बिल न किए गए विक्रय लेनदेन को सामान्य लेज़र में पोस्ट किया गया है या नहीं.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-110">Project cost and revenue profile determine if unbilled sales transactions are posted to the general ledger.</span></span> <span data-ttu-id="3b5e2-111">यदि **आय में वृद्धि** चयनित है, तो सिस्टम **WIP विक्रय मूल्य** का उपयोग करता है और **उपार्जित आय विक्रय मूल्य** पर पोस्टिंग के दौरान ध्यान दिया जाता है.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-111">If **Accrue revenue** is selected, the system uses the **WIP sales value** and the **Accrued revenue sales value** accounts during posting.</span></span> <span data-ttu-id="3b5e2-112">निम्न इस तरीका का एक उदाहरण है.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-112">The following is an example of this method.</span></span>  

  | <span data-ttu-id="3b5e2-113">लेनदेन प्रकार</span><span class="sxs-lookup"><span data-stu-id="3b5e2-113">Transaction type</span></span> | <span data-ttu-id="3b5e2-114">डेबिट/क्रेडिट</span><span class="sxs-lookup"><span data-stu-id="3b5e2-114">Debit/Credit</span></span> | <span data-ttu-id="3b5e2-115">राशि</span><span class="sxs-lookup"><span data-stu-id="3b5e2-115">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="3b5e2-116">WIP विक्रय मूल्य</span><span class="sxs-lookup"><span data-stu-id="3b5e2-116">WIP Sales value</span></span> | <span data-ttu-id="3b5e2-117">डेबिट</span><span class="sxs-lookup"><span data-stu-id="3b5e2-117">Debit</span></span> | <span data-ttu-id="3b5e2-118">100</span><span class="sxs-lookup"><span data-stu-id="3b5e2-118">100</span></span> |
  | <span data-ttu-id="3b5e2-119">उपार्जित आय विक्रय मूल्य</span><span class="sxs-lookup"><span data-stu-id="3b5e2-119">Accrued revenue sales value</span></span> | <span data-ttu-id="3b5e2-120">क्रेडिट</span><span class="sxs-lookup"><span data-stu-id="3b5e2-120">Credit</span></span> | <span data-ttu-id="3b5e2-121">100</span><span class="sxs-lookup"><span data-stu-id="3b5e2-121">100</span></span> |

- <span data-ttu-id="3b5e2-122">आय की पहचान इनवॉइसिंग के दौरान की जाती है.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-122">Revenue is recognized during invoicing.</span></span> <span data-ttu-id="3b5e2-123">सिस्टम पोस्टिंग के दौरान **इनवॉइस की गई आय** खाते का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-123">The system uses the **Invoiced revenue** account during posting.</span></span> <span data-ttu-id="3b5e2-124">निम्न इस तरीका का एक उदाहरण है.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-124">The following is an example of this method.</span></span>  

  | <span data-ttu-id="3b5e2-125">लेनदेन प्रकार</span><span class="sxs-lookup"><span data-stu-id="3b5e2-125">Transaction type</span></span> | <span data-ttu-id="3b5e2-126">डेबिट/क्रेडिट</span><span class="sxs-lookup"><span data-stu-id="3b5e2-126">Debit/Credit</span></span> | <span data-ttu-id="3b5e2-127">राशि</span><span class="sxs-lookup"><span data-stu-id="3b5e2-127">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="3b5e2-128">ग्राहक शेष</span><span class="sxs-lookup"><span data-stu-id="3b5e2-128">Customer balance</span></span> | <span data-ttu-id="3b5e2-129">डेबिट</span><span class="sxs-lookup"><span data-stu-id="3b5e2-129">Debit</span></span> | <span data-ttu-id="3b5e2-130">120</span><span class="sxs-lookup"><span data-stu-id="3b5e2-130">120</span></span> |
  | <span data-ttu-id="3b5e2-131">देययोग्य विक्रय कर</span><span class="sxs-lookup"><span data-stu-id="3b5e2-131">Sales tax payable</span></span> | <span data-ttu-id="3b5e2-132">क्रेडिट</span><span class="sxs-lookup"><span data-stu-id="3b5e2-132">Credit</span></span> | <span data-ttu-id="3b5e2-133">20</span><span class="sxs-lookup"><span data-stu-id="3b5e2-133">20</span></span> |
  | <span data-ttu-id="3b5e2-134">इनवॉइस की गई आय</span><span class="sxs-lookup"><span data-stu-id="3b5e2-134">Invoiced Revenue</span></span> | <span data-ttu-id="3b5e2-135">क्रेडिट</span><span class="sxs-lookup"><span data-stu-id="3b5e2-135">Credit</span></span> | <span data-ttu-id="3b5e2-136">100</span><span class="sxs-lookup"><span data-stu-id="3b5e2-136">100</span></span> |

- <span data-ttu-id="3b5e2-137">यदि बिल न की गई विक्रय पोस्ट किए जाने पर आय उपार्जित की गई थी, तो सिस्टम इनवॉइस करने पर उपार्जित आय को रिवर्स कर देगा.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-137">If revenue was accrued when the unbilled sales are posted, the system will reverse the accrued revenue at invoicing.</span></span>

  | <span data-ttu-id="3b5e2-138">लेनदेन प्रकार</span><span class="sxs-lookup"><span data-stu-id="3b5e2-138">Transaction type</span></span> | <span data-ttu-id="3b5e2-139">डेबिट/क्रेडिट</span><span class="sxs-lookup"><span data-stu-id="3b5e2-139">Debit/Credit</span></span> | <span data-ttu-id="3b5e2-140">राशि</span><span class="sxs-lookup"><span data-stu-id="3b5e2-140">Amount</span></span> |
  | --- | --- | --- |
  | <span data-ttu-id="3b5e2-141">WIP विक्रय मूल्य</span><span class="sxs-lookup"><span data-stu-id="3b5e2-141">WIP Sales value</span></span> | <span data-ttu-id="3b5e2-142">क्रेडिट</span><span class="sxs-lookup"><span data-stu-id="3b5e2-142">Credit</span></span> | <span data-ttu-id="3b5e2-143">100</span><span class="sxs-lookup"><span data-stu-id="3b5e2-143">100</span></span> |
  | <span data-ttu-id="3b5e2-144">उपार्जित आय विक्रय मूल्य</span><span class="sxs-lookup"><span data-stu-id="3b5e2-144">Accrued revenue sales value</span></span> | <span data-ttu-id="3b5e2-145">डेबिट</span><span class="sxs-lookup"><span data-stu-id="3b5e2-145">Debit</span></span> | <span data-ttu-id="3b5e2-146">100</span><span class="sxs-lookup"><span data-stu-id="3b5e2-146">100</span></span> |

## <a name="transactions-accounted-using-the-fixed-price-billing-method"></a><span data-ttu-id="3b5e2-147">निश्चित मूल्य बिलिंग विधि का उपयोग करके लेनदेन लेखा-जोखा</span><span class="sxs-lookup"><span data-stu-id="3b5e2-147">Transactions accounted using the fixed price billing method</span></span>

- <span data-ttu-id="3b5e2-148">लागत और आय पहचान अलग-अलग होते हैं.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-148">Cost and revenue recognition are separate.</span></span> <span data-ttu-id="3b5e2-149">लेनदेन लागत को [Project Operations एकीकरण जर्नल](../project-accounting/project-operations-integration-journal.md) का उपयोग करके पोस्ट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-149">Transaction cost is posted using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="3b5e2-150">बिल न किए गए विक्रय लेनदेन बनाए नहीं जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-150">Unbilled sales transactions aren't created.</span></span>
- <span data-ttu-id="3b5e2-151">यदि परियोजना लागत और आय प्रोफ़ाइल के **परियोजना पूर्णता गणना के लिए उपयोग किया जाने वाले सिद्धांत** को **कोई WIP नहीं** पर सेट किया गया है, तो आय को इनवॉइस करने के दौरान पहचाना जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-151">Revenue can be recognized during invoicing if the project cost and revenue profile have **Principle used for project completion calculations** set to **No WIP**.</span></span> <span data-ttu-id="3b5e2-152">केवल कम अवधि, सरल परियोजनाओं के लिए इस विधि का उपयोग करें.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-152">Only use this method for short term, simple projects.</span></span>
- <span data-ttu-id="3b5e2-153">आय को या तो **पूर्ण अनुबंध** या **प्रतिशत पूर्णता आय पहचान** विधि के साथ निश्चित मूल्य आय अनुमानों का उपयोग करके पहचाना जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="3b5e2-153">Revenue can be recognized using fixed price revenue estimates, with either the **Completed contract** or **Percent completion revenue recognition** method.</span></span>

## <a name="additional-resources"></a><span data-ttu-id="3b5e2-154">अतिरिक्त संसाधन</span><span class="sxs-lookup"><span data-stu-id="3b5e2-154">Additional resources</span></span>
[<span data-ttu-id="3b5e2-155">बिल करने योग्य परियोजना आलेख के लिए लेखांकन कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="3b5e2-155">Configure accounting for billable projects article</span></span>](../project-accounting/configure-accounting-billable-projects.md)

[<span data-ttu-id="3b5e2-156">निश्चित मूल्य आय अनुमान परियोजनाएँ</span><span class="sxs-lookup"><span data-stu-id="3b5e2-156">Fixed price revenue estimate projects</span></span>](rev-rec-percentage-completion-method.md)

[<span data-ttu-id="3b5e2-157">आय अनुमान प्रबंधित करें</span><span class="sxs-lookup"><span data-stu-id="3b5e2-157">Manage revenue estimates</span></span>](rev-rec-completed-contract-method.md)

[<span data-ttu-id="3b5e2-158">पूर्णता की लागत विधि</span><span class="sxs-lookup"><span data-stu-id="3b5e2-158">Cost to complete methods</span></span>](cost-complete-methods.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]