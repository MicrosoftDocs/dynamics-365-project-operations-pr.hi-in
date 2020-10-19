---
title: कोट्स बंद करें
description: यह विषय परियोजना संचालन में एक कोट को बंद करने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: cc3b2cdeb1ac46b7d927c1f96e94e9154d3eebf8
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896193"
---
# <a name="close-quotes"></a><span data-ttu-id="2a05d-103">कोट्स बंद करें</span><span class="sxs-lookup"><span data-stu-id="2a05d-103">Close quotes</span></span> 

<span data-ttu-id="2a05d-104">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="2a05d-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="2a05d-105">एक परियोजना कोट को जीता या गंवाया के रूप में बंद किया जा सकता.</span><span class="sxs-lookup"><span data-stu-id="2a05d-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="2a05d-106">Microsoft Dynamics 365 परियोजना संचालन में कोट पर सक्रिय और संशोधित संचालन समर्थित नहीं है, इसलिए एक ड्राफ्ट कोट को बंद किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="2a05d-106">The Activate and Revise operations on quotes is not supported in Microsoft Dynamics 365 Project Operations, so a draft quote can be closed.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="2a05d-107">कोट को जीत लिया के रूप में बंद करें</span><span class="sxs-lookup"><span data-stu-id="2a05d-107">Close a quote as Won</span></span>

<span data-ttu-id="2a05d-108">एक परियोजना कोट को जीता के रूप में बंद करना कोट को बंद स्थिति के साथ बंद कर देगा और स्थिति कारण जीत लिया पर सेट हो जाएगा.</span><span class="sxs-lookup"><span data-stu-id="2a05d-108">Closing a project quote as Won will close the quote with the status set to Closed and the status reason set to Won.</span></span> <span data-ttu-id="2a05d-109">कोट को बंद करने से परियोजना कोट केवल पढ़ने योग्य बनता है और एक ड्राफ्ट परियोजना अनुबंध बनता है जिसमें कोट की जानकारी होती है.</span><span class="sxs-lookup"><span data-stu-id="2a05d-109">Closing the quote makes the project quote read-only and creates a draft project contract that contains the quote information.</span></span> <span data-ttu-id="2a05d-110">क्योंकि एक बंद कोट को फिर से खोला नहीं जा सकता है, बदलाव किए जाने से पहले एक पुष्टिकरण संवाद दिखता है, क्योंकि एक बंद कोट को फिर से नहीं खोला जा सकता है और बदलाव अपरिवर्तनीय हैं.</span><span class="sxs-lookup"><span data-stu-id="2a05d-110">Because a closed quote can't be reopened, a confirmation dialog There is a confirmation dialog before the changes are done since a closed quote cannot be re-opened and the changes are irreversible.</span></span>

<span data-ttu-id="2a05d-111">यदि कोट एक अवसर से जुड़ा है, तो अवसर पर किसी भी अन्य परियोजना के कोट अपने आप गंवाए के रूप में बंद हो जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="2a05d-111">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="2a05d-112">एक कोट को जीत लिया के रूप में बंद करने का वित्तीय प्रभाव</span><span class="sxs-lookup"><span data-stu-id="2a05d-112">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="2a05d-113">यदि किसी परियोजना पर दर्ज समय के लिए कोई वास्तविक है, जबकि यह अभी भी एक ड्राफ्ट कोट से जुड़ा हुआ है, तो केवल समय या व्यय की लागत दर्ज की जाती है।</span><span class="sxs-lookup"><span data-stu-id="2a05d-113">If there have been any actuals for time recorded on a project while it is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="2a05d-114">एक कोट को जीता के रूप में बंद करने के बाद, एप्लिकेशन पुरानी लागत वास्तविक को उलट कर और नई लागत वास्तविक को फिर से बनाने के द्वारा लागतों को रिफैक्टर करेगा।</span><span class="sxs-lookup"><span data-stu-id="2a05d-114">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="2a05d-115">एप्लिकेशन संबंधित परियोजना अनुबंध लाइन की बिलिंग विधि के आधार पर इन लागत वास्तविक को संसाधित करेगा।</span><span class="sxs-lookup"><span data-stu-id="2a05d-115">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="2a05d-116">यदि लागत वास्तविक समय और सामग्री अनुबंध लाइन का संदर्भ देती है, तो कोट बंद हो जाने पर और परियोजना अनुबंध बनने पर सिस्टम स्वचालित रूप से संबंधित गैर-बिल की बिक्री वास्तविक बनाएगा।</span><span class="sxs-lookup"><span data-stu-id="2a05d-116">If the cost actuals reference a time and material contract line, the system will automatically create corresponding unbilled sales actuals for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="2a05d-117">यदि लागत वास्तविक एक निश्चित मूल्य अनुबंध लाइन का संदर्भ देती है, तो परियोजना अनुबंध ग्राहकों के लिए विभाजित बिलिंग नियमों के आधार पर एप्लिकेशन लागत वास्तविक को पुन: प्रोसेस करना बंद कर देगा।</span><span class="sxs-lookup"><span data-stu-id="2a05d-117">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals based on the split billing rules for the project contract customers.</span></span>

## <a name="closing-a-quote-as-lost"></a><span data-ttu-id="2a05d-118">एक कोट को गंवाया के रूप में बंद:</span><span class="sxs-lookup"><span data-stu-id="2a05d-118">Closing a quote as lost:</span></span>

<span data-ttu-id="2a05d-119">एक परियोजना कोट को गंवाए के रूप में बंद करना स्थिति बंद और स्थिति का कारण गंवाया के रूप में निर्धारित करेगा.</span><span class="sxs-lookup"><span data-stu-id="2a05d-119">Closing a project quote as Lost will set the status to Closed and status reason to Lost.</span></span> <span data-ttu-id="2a05d-120">कोट बंद करने से परियोजना कोट केवल पढ़ने योग्य बन जाती है.</span><span class="sxs-lookup"><span data-stu-id="2a05d-120">Closing the quote makes the project quote read-only.</span></span> <span data-ttu-id="2a05d-121">क्योंकि एक बंद कोट को फिर से खोला नहीं जा सकता है और इससे पहले कि आप किसी कोट को बंद करें, एक पुष्टिकरण संवाद आपके बदलावों की पुष्टि करेगा।</span><span class="sxs-lookup"><span data-stu-id="2a05d-121">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="2a05d-122">यदि परियोजना कोट जो गंवाया के रूप में बंद हो गया है, उसकी किसी भी लाइन पर संदर्भित परियोजना है, तो उस परियोजना को बंद के रूप में भी चिह्नित किया जाता है और उस दिन से किसी भी संसाधन बुकिंग को रद्द कर दिया जाता है।</span><span class="sxs-lookup"><span data-stu-id="2a05d-122">If the project quote that is closed as Lost has a project referenced on any of its lines, that project is also marked as Closed and any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="2a05d-123">परियोजना संचालन में, एक कोट को जीता या गंवाया के रूप में बंद करने से अवसर की स्थिति प्रभावित नहीं होगी, जो तब तक खुली रहेगी जब तक कि इसे मैनुअल रूप से बंद न किया जाए।</span><span class="sxs-lookup"><span data-stu-id="2a05d-123">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>
