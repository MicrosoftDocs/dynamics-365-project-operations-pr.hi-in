---
title: आंतरिक परियोजनाओं के लिए लेखांकन कॉन्फ़िगर करें
description: यह विषय परियोजना संचालन की आंतरिक परियोजनाओं के लिए किस तरह लेखांकन प्रथाओं को तैयार किया जाए, पर जानकारी प्रदान करता है.
author: sigitac
manager: Annbe
ms.date: 10/09/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 65d05e3a6321dc32aee55c28b3eaa4bd0bae2f86
ms.sourcegitcommit: 5fd529f2308edfe9322082313e6d50146df56aca
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/06/2021
ms.locfileid: "5857980"
---
# <a name="configure-accounting-for-internal-projects"></a><span data-ttu-id="8a0c6-103">आंतरिक परियोजनाओं के लिए लेखांकन कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="8a0c6-103">Configure accounting for internal projects</span></span>

<span data-ttu-id="8a0c6-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="8a0c6-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="8a0c6-105">आंतरिक परियोजनाएं कंपनियों को गतिविधियों संबंधित लागत ट्रैक करने की अनुमति प्रदान करती हैं, जिनका बिल ग्राहक को नहीं दिया जाता.</span><span class="sxs-lookup"><span data-stu-id="8a0c6-105">Internal projects allow companies track cost related to activities that aren't being billed to a customer.</span></span> <span data-ttu-id="8a0c6-106">आंतरिक परियोजनाओं के उदाहरण, जिनमें शामिल हैं:</span><span class="sxs-lookup"><span data-stu-id="8a0c6-106">Examples of internal projects include:</span></span>

- <span data-ttu-id="8a0c6-107">किसी प्रोडक्ट को बनाना जैसे कि मोबाइल ऐप और विकास से जुड़ी लागत को ट्रैक करना.</span><span class="sxs-lookup"><span data-stu-id="8a0c6-107">Developing a product, such as a mobile app, and tracking the cost associated with the development.</span></span>
- <span data-ttu-id="8a0c6-108">बिक्री से पहले के समय और व्यय का प्रबंधन करना.</span><span class="sxs-lookup"><span data-stu-id="8a0c6-108">Managing pre-sale time and expense.</span></span> <span data-ttu-id="8a0c6-109">यदि निविदा को जीत लिया जाता है तो बिक्री से पहले की इस आंतरिक परियोजना को बाद में बिल योग्य परियोजना में परिवर्तित किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="8a0c6-109">This pre-sale internal project can be converted later to a billable project if quote is won.</span></span>

<span data-ttu-id="8a0c6-110">कोई भी परियोजना, जो Dynamics 365 Project Operations में किसी अनुबंध से संबद्ध नहीं है, उसे आंतरिक माना जाता है.</span><span class="sxs-lookup"><span data-stu-id="8a0c6-110">Any project not associated with a contract in Dynamics 365 Project Operations is treated as internal.</span></span> <span data-ttu-id="8a0c6-111">परियोजना की लागत और राजस्व प्रोफाइल का उपयोग परियोजना के लेखांकन नियमों को निर्धारित करने के लिए नहीं किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8a0c6-111">Project cost and revenue profiles aren't used to determine accounting rules for the project.</span></span> <span data-ttu-id="8a0c6-112">लाभ और घाटा/हानि सिद्धांतों का उपयोग करके आंतरिक परियोजना लागत को हमेशा पोस्ट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8a0c6-112">Internal project cost is always posted using profit and loss principles.</span></span> <span data-ttu-id="8a0c6-113">**लेजर पोस्टिंग सेटअप** पृष्ठ/पन्ने पर पोस्टिंग के लिए लेजर खातों को परिभाषित किया गया है.</span><span class="sxs-lookup"><span data-stu-id="8a0c6-113">Ledger accounts for postings are defined on the **Ledger posting setup** page.</span></span>

- <span data-ttu-id="8a0c6-114">**लागत** खाता को डेबिट करके और **पेरोल एलोकेशन** खाता को क्रेडिट करके समय के लेन-देन को पोस्ट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8a0c6-114">Time transactions are posted by debiting the **Cost** account and crediting the **Payroll allocation** account.</span></span>
- <span data-ttu-id="8a0c6-115">**लागत** खाता को डेबिट करके और **खर्च के लिए ऑफसेट खाता** को क्रेडिट करके खर्च के लेन-देन को पोस्ट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8a0c6-115">Expense transactions are posted by debiting the **Cost** account and crediting the **Offset account for expense**.</span></span>
- <span data-ttu-id="8a0c6-116">आइटम लेन-देन **लागत** खाते को डेबिट करके और **लागत - आइटम** खाते को जमा करके पोस्ट किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="8a0c6-116">Item transactions are posted by debiting the **Cost** account and crediting the **Cost - Item** account.</span></span>

<span data-ttu-id="8a0c6-117">परियोजना के लिए लेन-देन को पोस्ट करने के बाद, यदि परियोजना अनुबंध से जुड़ी परियोजना है तो सिस्टम सभी जमा लेन-देन को बदल देता है और नए बिल योग्य लेन-देन बना देता है.</span><span class="sxs-lookup"><span data-stu-id="8a0c6-117">After transactions are posted to the project, if the project is associated with a project contract, the system reverses all accumulated transactions and creates new billable transactions.</span></span> <span data-ttu-id="8a0c6-118">बिल योग्य लेनदेन संबंधित परियोजना लागत और राजस्व प्रोफ़ाइल में परिभाषित लेखांकन नियमों का पालन करते हैं।</span><span class="sxs-lookup"><span data-stu-id="8a0c6-118">The billable transactions follow the accounting rules defined in respective Project cost and revenue profile.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]
