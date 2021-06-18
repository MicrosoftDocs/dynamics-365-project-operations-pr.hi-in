---
title: कोई कोट बंद करें - लाइट
description: यह विषय परियोजना संचालन में एक कोट को बंद करने के बारे में जानकारी प्रदान करता है.
author: rumant
ms.date: 10/01/2020
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 75345fed57dcbdb84f2a82587c7d0c152530c72b
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5994138"
---
# <a name="close-a-quote---lite"></a><span data-ttu-id="53884-103">कोई कोट बंद करें - लाइट</span><span class="sxs-lookup"><span data-stu-id="53884-103">Close a quote - lite</span></span>

<span data-ttu-id="53884-104">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="53884-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="53884-105">एक परियोजना कोट को जीता या गंवाया के रूप में बंद किया जा सकता.</span><span class="sxs-lookup"><span data-stu-id="53884-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="53884-106">ड्राफ़्ट कोट को बंद किया जा सकता है, क्योंकि कोट पर सक्रिय और संशोधन कार्रवाई Microsoft Dynamics 365 Project Operations में समर्थित नहीं है.</span><span class="sxs-lookup"><span data-stu-id="53884-106">A draft quote can be closed because the Activate and Revise operations on quotes isn't supported in Microsoft Dynamics 365 Project Operations.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="53884-107">कोट को जीत लिया के रूप में बंद करें</span><span class="sxs-lookup"><span data-stu-id="53884-107">Close a quote as Won</span></span>

<span data-ttu-id="53884-108">जब आप किसी परियोजना कोट को जीते गए के रूप में बंद करते हैं, तो स्थिति बंद पर और स्थिति विवरण जीता गया पर सेट हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="53884-108">When you close a project quote as Won, the status is set to Closed and the status reason is Won.</span></span> <span data-ttu-id="53884-109">कोट को बंद करने से परियोजना कोट केवल पढ़ने योग्य बनता है और एक ड्राफ्ट परियोजना अनुबंध बनता है जिसमें कोट की जानकारी होती है.</span><span class="sxs-lookup"><span data-stu-id="53884-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="53884-110">क्योंकि एक बंद कोट को फिर से खोला नहीं जा सकता है, इसलिए एक पुष्टि संवाद आपके परिवर्तनों की पुष्टि करेगा.</span><span class="sxs-lookup"><span data-stu-id="53884-110">Because a closed quote can't be reopened, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="53884-111">यदि कोट एक अवसर से जुड़ा है, तो अवसर पर किसी भी अन्य परियोजना के कोट अपने आप गंवाए के रूप में बंद हो जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="53884-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="53884-112">एक कोट को जीत लिया के रूप में बंद करने का वित्तीय प्रभाव</span><span class="sxs-lookup"><span data-stu-id="53884-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="53884-113">यदि किसी परियोजना पर समय के लिए कोई वास्तविक है जबकि वह अभी भी ड्राफ़्ट कोट से संलग्न है, तो केवल समय या व्यय की लागत दर्ज की जाती है.</span><span class="sxs-lookup"><span data-stu-id="53884-113">If there are any actuals for time on a project while is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="53884-114">एक कोट को जीता के रूप में बंद करने के बाद, एप्लिकेशन पुरानी लागत वास्तविक को उलट कर और नई लागत वास्तविक को फिर से बनाने के द्वारा लागतों को रिफैक्टर करेगा।</span><span class="sxs-lookup"><span data-stu-id="53884-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="53884-115">एप्लिकेशन संबंधित परियोजना अनुबंध लाइन की बिलिंग विधि के आधार पर इन लागत वास्तविक को संसाधित करेगा।</span><span class="sxs-lookup"><span data-stu-id="53884-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="53884-116">यदि लागत वास्तविक समय और सामग्री अनुबंध पंक्ति को संदर्भ करती है, तो कोट के बंद होने और परियोजना अनुबंध के बनाए जाने पर संबंधित बिल न किए गए विक्रय वास्तविक बनाए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="53884-116">If the cost actuals reference a time and material contract line, corresponding unbilled sales actuals are created for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="53884-117">यदि लागत वास्तविक एक निश्चित मूल्य अनुबंध पंक्ति को संदर्भित करती है, तो एप्लिकेशन परियोजना अनुबंध ग्राहकों के लिए विभाजित बिलिंग नियमों के आधार पर लागत वास्तविक को पुनः संसाधित करना बंद कर देगा.</span><span class="sxs-lookup"><span data-stu-id="53884-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals that are based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="53884-118">एक कोट को गंवाया के रूप में बंद:</span><span class="sxs-lookup"><span data-stu-id="53884-118">Closing a quote as lost:</span></span>

<span data-ttu-id="53884-119">जब आप किसी परियोजना कोट को हारे गए के रूप में बंद करते हैं, तो स्थिति बंद पर और स्थिति विवरण हारे गया पर सेट हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="53884-119">When you close a project quote as Lost, the status is set to Closed and status reason is Lost.</span></span> <span data-ttu-id="53884-120">कोट बंद करने से परियोजना कोट केवल पढ़ने योग्य बन जाती है.</span><span class="sxs-lookup"><span data-stu-id="53884-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="53884-121">क्योंकि एक बंद कोट को फिर से खोला नहीं जा सकता है और इससे पहले कि आप किसी कोट को बंद करें, एक पुष्टिकरण संवाद आपके बदलावों की पुष्टि करेगा।</span><span class="sxs-lookup"><span data-stu-id="53884-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="53884-122">यदि हारे गए के रूप में बंद किया गया परियोजना कोट किसी परियोजना को उसकी किसी पंक्ति पर संदर्भित करता है, तो उस परियोजना को बंद के रूप में भी चिह्नित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="53884-122">If the project quote that is closed as Lost references a project on any of its lines, that project is also marked as Closed.</span></span> <span data-ttu-id="53884-123">उस दिन के बाद से किसी भी संसाधन बुकिंग को रद्द कर दिया जाता है.</span><span class="sxs-lookup"><span data-stu-id="53884-123">Any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="53884-124">परियोजना संचालन में, एक कोट को जीता या गंवाया के रूप में बंद करने से अवसर की स्थिति प्रभावित नहीं होगी, जो तब तक खुली रहेगी जब तक कि इसे मैनुअल रूप से बंद न किया जाए।</span><span class="sxs-lookup"><span data-stu-id="53884-124">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]