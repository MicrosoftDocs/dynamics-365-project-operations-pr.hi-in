---
title: पुष्टि किया गया परियोजना अनुबंध
description: यह विषय परियोजना संचालन में अनुबंध की पुष्टि कैसे करें, की जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/13/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: babce9c64098a9c87072786d914d2340251a8986
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077820"
---
# <a name="confirm-a-project-contract"></a><span data-ttu-id="8d87f-103">पुष्टि किया गया परियोजना अनुबंध</span><span class="sxs-lookup"><span data-stu-id="8d87f-103">Confirm a project contract</span></span>

<span data-ttu-id="8d87f-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="8d87f-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="8d87f-105">Dynamics 365 Project Operations में एक परियोजना अनुबंध **पुष्ट हुआ** के कारण के साथ सक्रिय, या **नहीं मिला** के कारण के साथ बंद किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="8d87f-105">A project contract in Dynamics 365 Project Operations can be active with a reason of **Confirmed** , or closed with a reason of **Lost**.</span></span> <span data-ttu-id="8d87f-106">जब आप एक परियोजना अनुबंध की पुष्टि करते हैं, तो स्टेटस **ड्राफ्ट** से **सक्रिय** में अपडेट हो जाता है और स्टेटस का कारण **पुष्ट हुआ** हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="8d87f-106">When you confirm a project contract, the status updates from **Draft** to **Active** and the status reason is **Confirmed**.</span></span> <span data-ttu-id="8d87f-107">एक सक्रिय या बंद परियोजना को न तो बदला जा सकता है और न ही दोबारा खोला जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="8d87f-107">An active or closed contract can't be edited or reopened.</span></span> 

### <a name="financial-impact-of-confirming-a-project-contract"></a><span data-ttu-id="8d87f-108">एक/किसी परियोजना अनुबंध की पुष्टि करने का आर्थिक/ वित्तीय प्रभाव</span><span class="sxs-lookup"><span data-stu-id="8d87f-108">Financial impact of confirming a project contract</span></span>

<span data-ttu-id="8d87f-109">एक/किसी परियोजना अनुबंध की पुष्टि होने के बाद, अनुप्रयोग पुरानी वास्तविक लागत को उलट कर और नई वास्तविक लागत बनाकर लागत की फिर से गणना करता है.</span><span class="sxs-lookup"><span data-stu-id="8d87f-109">After a project contract is confirmed, the application recalculates the costs by reversing the older cost actuals and creating new cost actuals.</span></span> <span data-ttu-id="8d87f-110">फिर नई वास्तविक लागत को जुड़ी हुई परियोजना अनुबंध पंक्ति की बिलिंग विधि के आधार पर संसाधित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8d87f-110">The new cost actuals are then processed based on the billing method of the associated project contract line.</span></span> <span data-ttu-id="8d87f-111">यदि वास्तविक लागत समय और सामग्री अनुबंध पंक्ति का सन्दर्भ देती है, तो अनुप्रयोग स्वतः संबंधित वास्तविक बिना बिल बिक्री को फिर से निर्मित करता है.</span><span class="sxs-lookup"><span data-stu-id="8d87f-111">If the cost actuals reference a Time and Material contract line, the application automatically re-creates corresponding unbilled sales actuals.</span></span> <span data-ttu-id="8d87f-112">यदि वास्तविक लागत एक तय कीमत अनुबंध पंक्ति का सन्दर्भ देती है, तो अनुप्रयोग वास्तविक लागत को फिर से संसाधित करना बंद कर देता है.</span><span class="sxs-lookup"><span data-stu-id="8d87f-112">If the cost actuals reference a Fixed Price contract line, the application stops reprocessing the cost actuals.</span></span>

<span data-ttu-id="8d87f-113">सीमा से अधिक नहीं, चैरिटीबिलिटी सेटअप, और वास्तविक पर मूल्य निर्धारण और लागत का मूल्यांकन किया जाता है और फिर पुष्टिकरण प्रक्रिया के भाग के रूप में अपडेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8d87f-113">Not-to-exceed limits, chargeability setup, and pricing and costing on the actuals is evaluated and then updated as part of the confirmations process.</span></span>

## <a name="close-a-project-contract-as-lost"></a><span data-ttu-id="8d87f-114">परियोजना अनुबंध को नहीं मिले के तौर पर बंद करें</span><span class="sxs-lookup"><span data-stu-id="8d87f-114">Close a project contract as lost</span></span>

<span data-ttu-id="8d87f-115">जब आप किसी परियोजना अनुबंध को नहीं मिले के रूप में बंद करते हैं, तो अनुबंध का स्टेटस **बंद** और स्टेटस का कारण **नहीं मिला** के तौर पर अपडेट हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="8d87f-115">When you close a project contract as lost, the contract status is updated to **Closed** and the status reason is **Lost**.</span></span> <span data-ttu-id="8d87f-116">यह परियोजना अनुबंध केवल पढ़ने के लिए है.</span><span class="sxs-lookup"><span data-stu-id="8d87f-116">The project contract becomes read-only.</span></span> <span data-ttu-id="8d87f-117">परिवर्तनों के पूरा होने से पहले ही एक पुष्टिकरण संवाद प्रदान किया जाएगा क्योंकि आप एक बंद परियोजना अनुबंध को फिर से नहीं खोल सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="8d87f-117">A confirmation dialog is provided before the changes are complete because you can't reopen a closed project contract.</span></span>

<span data-ttu-id="8d87f-118">यदि वह परियोजना अनुबंध जो नहीं मिला के तौर पर बंद हो गया है, उसकी तर्ज पर किसी परियोजना का संदर्भ देता है, तो उस परियोजना को भी बंद के रूप में चिह्नित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8d87f-118">If the project contract that is closed as lost references a project on its lines, that project is also marked as closed.</span></span> <span data-ttu-id="8d87f-119">उस दिन के बाद से किसी भी संसाधन बुकिंग को रद्द कर दिया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8d87f-119">Any resource bookings from that day forward are canceled.</span></span> <span data-ttu-id="8d87f-120">परियोजना अनुबंध पर वास्तविक बिना बिल बिक्री को जो पहले से इनवॉइस पर नहीं है, को उलट दिया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="8d87f-120">Any unbilled sales actuals on the project contract that aren't already on an invoice, will be reversed.</span></span>

> [!NOTE]
> <span data-ttu-id="8d87f-121">Dynamics 365 Project Operations में, नहीं मिला के रूप में परियोजना अनुबंध को बंद करने से यह संबंधित अवसर की स्थिति पर प्रभाव नहीं पड़ेगा.</span><span class="sxs-lookup"><span data-stu-id="8d87f-121">In Dynamics 365 Project Operations, closing a project contract as lost will not impact that status of the associated opportunity.</span></span> <span data-ttu-id="8d87f-122">यह अवसर खुला ही रहेगा और इसे मैन्युअल रूप से बंद करना होगा.</span><span class="sxs-lookup"><span data-stu-id="8d87f-122">The opportunity will remain open and must be manually closed.</span></span>
