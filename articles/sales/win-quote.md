---
title: कोट बंद करें
description: यह विषय परियोजना संचालन में समापन कोट चिह्नों के बारे में जानकारी प्रदान करता है।
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a2c752ba6395ed4bf025092219350dc245f7428f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5277250"
---
# <a name="close-a-quote"></a><span data-ttu-id="4f57f-103">कोट बंद करें</span><span class="sxs-lookup"><span data-stu-id="4f57f-103">Close a quote</span></span>

<span data-ttu-id="4f57f-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="4f57f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="4f57f-105">एक परियोजना कोट को जीता या गंवाया के रूप में बंद किया जा सकता.</span><span class="sxs-lookup"><span data-stu-id="4f57f-105">A project quote can be closed as Won or Lost.</span></span> <span data-ttu-id="4f57f-106">क्योंकि Microsoft Dynamics 365 Project Operations में कोट पर सक्रिय करे और संशोधन करें कार्य समर्थित नहीं है, इसलिए आप ड्राफ़्ट कोट को बंद कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="4f57f-106">Because the functions Activate and Revise are not supported on quotes in Microsoft Dynamics 365 Project Operations, you can close a draft quote.</span></span>

## <a name="close-a-quote-as-won"></a><span data-ttu-id="4f57f-107">कोट को जीत लिया के रूप में बंद करें</span><span class="sxs-lookup"><span data-stu-id="4f57f-107">Close a quote as Won</span></span>

<span data-ttu-id="4f57f-108">एक परियोजना कोट को जीत लिया के रूप में बंद करने से कोट की स्थिति **बंद** हो जाएगी और स्थिति का कारण **जीत लिया** पर निर्धारित हो जाएगा।</span><span class="sxs-lookup"><span data-stu-id="4f57f-108">Closing a project quote as Won will set the status of the quote to **Closed** and status reason to **Won**.</span></span> <span data-ttu-id="4f57f-109">कोट को बंद करना इसे केवल पढ़ने-योग्य बनाता है और सभी कोट सूचनाओं के साथ एक ड्राफ्ट परियोजना अनुबंध बनाता है।</span><span class="sxs-lookup"><span data-stu-id="4f57f-109">Closing the quotes makes it read-only and creates a draft project contract with all the quote information.</span></span> <span data-ttu-id="4f57f-110">क्योंकि एक बंद कोट को फिर से खोला नहीं जा सकता, इससे पहले कि आप एक कोट को बंद करें, एक पुष्टिकरण संवाद आपके बदलावों की पुष्टि करेगा।</span><span class="sxs-lookup"><span data-stu-id="4f57f-110">Because a closed quote can't be reopened, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="4f57f-111">परियोजना कोट से निर्मित परियोजना अनुबंध भी परियोजना प्रबंधन और परियोजना संचालन के लेखांकन मॉड्यूल में उपलब्ध कराया जाता है।</span><span class="sxs-lookup"><span data-stu-id="4f57f-111">The project contract created from a project quote is also made available in the Project management and accounting module of Project Operations.</span></span> <span data-ttu-id="4f57f-112">यदि किसी परियोजना अनुबंध को उसकी किसी भी लाइन पर परियोजना के लिए मैप नहीं किया जाता है, तो यह परियोजना अनुबंध निष्क्रिय परियोजना अनुबंध के रूप में उपलब्ध कराया जाता है और जैसे ही कोई परियोजना अपनी कम से कम एक अनुबंध लाइन पर मैप की जाती है, तो यह सक्रिय हो जाती है।</span><span class="sxs-lookup"><span data-stu-id="4f57f-112">If a project contract is not mapped to a project on any of its lines, this project contract is made available as an inactive project contract and becomes active as soon as a project is mapped to at least one of its contract lines.</span></span>

<span data-ttu-id="4f57f-113">यदि कोट एक अवसर से जुड़ा है, तो अवसर पर किसी भी अन्य परियोजना के कोट अपने आप गंवाए के रूप में बंद हो जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="4f57f-113">If the quote is attached to an opportunity, any other project quotes on the opportunity are automatically closed as Lost.</span></span>

### <a name="financial-impact-of-closing-a-quote-as-won"></a><span data-ttu-id="4f57f-114">एक कोट को जीत लिया के रूप में बंद करने का वित्तीय प्रभाव</span><span class="sxs-lookup"><span data-stu-id="4f57f-114">Financial impact of closing a quote as Won</span></span>

<span data-ttu-id="4f57f-115">यदि किसी परियोजना पर दर्ज समय के लिए कोई वास्तविक है, जबकि यह अभी भी एक ड्राफ्ट कोट से जुड़ा हुआ है, तो केवल समय या व्यय की लागत दर्ज की जाती है।</span><span class="sxs-lookup"><span data-stu-id="4f57f-115">If there have been any actuals for time recorded on a project while it is still attached to a draft quote, only the cost of the time or expense is recorded.</span></span> <span data-ttu-id="4f57f-116">एक कोट को जीता के रूप में बंद करने के बाद, एप्लिकेशन पुरानी लागत वास्तविक को उलट कर और नई लागत वास्तविक को फिर से बनाने के द्वारा लागतों को रिफैक्टर करेगा।</span><span class="sxs-lookup"><span data-stu-id="4f57f-116">After a quote is closed as Won, the application will refactor the costs by reversing the older cost actuals and re-creating new cost actuals.</span></span> <span data-ttu-id="4f57f-117">एप्लिकेशन संबंधित परियोजना अनुबंध लाइन की बिलिंग विधि के आधार पर इन लागत वास्तविक को संसाधित करेगा।</span><span class="sxs-lookup"><span data-stu-id="4f57f-117">The application will process these cost actuals based on the Billing method of the associated project contract line.</span></span> <span data-ttu-id="4f57f-118">यदि लागत वास्तविक समय और सामग्री अनुबंध लाइन का संदर्भ देती है, तो कोट बंद हो जाने पर और परियोजना अनुबंध बनने पर सिस्टम स्वचालित रूप से संबंधित गैर-बिल की बिक्री वास्तविक बनाएगा।</span><span class="sxs-lookup"><span data-stu-id="4f57f-118">If the cost actuals reference a time and material contract line, the system will automatically create corresponding unbilled sales actuals for when the quote is closed and the project contract is created.</span></span> <span data-ttu-id="4f57f-119">यदि लागत वास्तविक एक निश्चित मूल्य अनुबंध लाइन का संदर्भ देती है, तो परियोजना अनुबंध ग्राहकों के लिए विभाजित बिलिंग नियमों के आधार पर एप्लिकेशन लागत वास्तविक को पुन: प्रोसेस करना बंद कर देगा।</span><span class="sxs-lookup"><span data-stu-id="4f57f-119">If the cost actuals reference a fixed price contract line, the application will stop reprocessing the cost actuals based on the split billing rules for the project contract customers.</span></span>

<span data-ttu-id="4f57f-120">परियोजना प्रबंधन और लेखा मॉड्यूल में सभी पुन: प्रोसेस किए गए वास्तविक परियोजना लेखा परीक्षक की समीक्षा, अपडेट, और सामान्य खाता बही में पोस्ट करने के लिए उपलब्ध हैं।</span><span class="sxs-lookup"><span data-stu-id="4f57f-120">All reprocessed actuals are available in the Project management and accounting module for the Project accountant to review, update, and post to the General ledger.</span></span> 

## <a name="close-a-quote-as-lost"></a><span data-ttu-id="4f57f-121">एक कोट को गंवाए के रूप में बंद करें</span><span class="sxs-lookup"><span data-stu-id="4f57f-121">Close a quote as Lost</span></span>

<span data-ttu-id="4f57f-122">एक परियोजना कोट को गंवाए के रूप में बंद करना स्थिति **बंद** और स्थिति का कारण **गंवाया** के रूप में निर्धारित करेगा।</span><span class="sxs-lookup"><span data-stu-id="4f57f-122">Closing a project quote as Lost will set the status to **Closed** and status reason to **Lost**.</span></span> <span data-ttu-id="4f57f-123">कोट बंद करने से यह केवल पढ़ने योग्य बन जाता है।</span><span class="sxs-lookup"><span data-stu-id="4f57f-123">Closing the quote makes it read-only.</span></span> <span data-ttu-id="4f57f-124">क्योंकि एक बंद कोट को फिर से खोला नहीं जा सकता है और इससे पहले कि आप किसी कोट को बंद करें, एक पुष्टिकरण संवाद आपके बदलावों की पुष्टि करेगा।</span><span class="sxs-lookup"><span data-stu-id="4f57f-124">Because a closed quote can't be reopened and, before you close a quote, a confirmation dialog will confirm your changes.</span></span>

<span data-ttu-id="4f57f-125">यदि परियोजना कोट जो गंवाया के रूप में बंद हो गया है, उसकी किसी भी लाइन पर संदर्भित परियोजना है, तो उस परियोजना को बंद के रूप में भी चिह्नित किया जाता है और उस दिन से किसी भी संसाधन बुकिंग को रद्द कर दिया जाता है।</span><span class="sxs-lookup"><span data-stu-id="4f57f-125">If the project quote that is closed as Lost has a project referenced on any of its lines, that project is also marked as Closed and any resource bookings from that day forward are canceled.</span></span>

> [!NOTE]
> <span data-ttu-id="4f57f-126">परियोजना संचालन में, एक कोट को जीता या गंवाया के रूप में बंद करने से अवसर की स्थिति प्रभावित नहीं होगी, जो तब तक खुली रहेगी जब तक कि इसे मैनुअल रूप से बंद न किया जाए।</span><span class="sxs-lookup"><span data-stu-id="4f57f-126">In Project Operations, closing a quote as Won or Lost will not impact that status of the Opportunity, which will remain open until it is manually closed.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]