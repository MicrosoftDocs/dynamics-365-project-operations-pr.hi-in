---
title: इनवॉयस को सही किया
description: यह विषय इनवॉयस को सही करने संबंधी सूचना प्रदान करता है.
author: rumant
manager: AnnBe
ms.date: 09/18/2020
ms.topic: article
ms.prod: ''
ms.service: project-operations
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: suvaidya
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: 1ebfec053a59bbadd261d4333f6737cf16292e81
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4122390"
---
# <a name="corrected-invoices"></a><span data-ttu-id="5f418-103">इनवॉयस को सही किया</span><span class="sxs-lookup"><span data-stu-id="5f418-103">Corrected invoices</span></span>

<span data-ttu-id="5f418-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="5f418-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="5f418-105">निश्चित इनवॉयस को एडिट (सुधार) किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="5f418-105">Confirmed invoices can be edited.</span></span> <span data-ttu-id="5f418-106">जब आप पुष्टि की गई इनवॉइस को संपादित करते हैं, तो सही इनवॉइस का ड्राफ्ट बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="5f418-106">When you edit a confirmed invoice, a draft of the corrected invoice is created.</span></span> <span data-ttu-id="5f418-107">चूंकि धारणा यह है कि आप मूल इनवॉइस से सभी लेनदेन और मात्राओं को पूर्णतया बदलना चाहते हैं, सही इनवॉइस में मूल इनवॉइस के सभी लेनदेन शामिल हैं, और इस पर सभी मात्राएं शून्य (0) हैं.</span><span class="sxs-lookup"><span data-stu-id="5f418-107">Because the assumption is that you want to reverse all the transactions and quantities from the original invoice, the corrected invoice includes all the transactions from the original invoice, and all the quantities on it are zero (0).</span></span>

<span data-ttu-id="5f418-108">जब किसी लेनदेन में किसी सुधार की ज़रूरत नहीं होती है तो आप उन्हें सुधार किए गए ड्राफ़्ट सुझावित इनवॉइस से हटा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="5f418-108">When transactions don't require correction, you can remove them from the draft corrective invoice.</span></span> <span data-ttu-id="5f418-109">केवल एक आंशिक मात्रा को पूर्णतया बदलें या वापस करने के लिए, आप लाइन विस्तार पर मात्रा फ़ील्ड में बदलाव कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="5f418-109">To reverse or return only a partial quantity, you can edit the Quantity field on the line detail.</span></span> <span data-ttu-id="5f418-110">यदि आप बीजक लाइन विवरण को खोलते हैं, तो आप मूल बीजक की मात्रा को देख सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="5f418-110">If you open the invoice line detail, you can see the original invoice quantity.</span></span> <span data-ttu-id="5f418-111">इसके बाद आप चालू बीजक मात्रा को एडिट कर सकते हैं ताकि यह मूल बीजक की मात्रा से कम या अधिक हो।</span><span class="sxs-lookup"><span data-stu-id="5f418-111">You can then edit the current invoice quantity so that it's less than or more than the original invoice quantity.</span></span>

<span data-ttu-id="5f418-112">जब आप सुधारित बीजक को संपुष्ट करते हैं तो मूल रूप से बिल की गई वास्तविक बिक्री उलट जाती है और नई बिल की गई वास्तविक बिक्री तैयार की जाती है।</span><span class="sxs-lookup"><span data-stu-id="5f418-112">When you confirm a corrective invoice, the original billed sales actual is reversed, and a new billed sales actual is created.</span></span> <span data-ttu-id="5f418-113">यदि मात्रा को कम किया जाता है तो अंतर के कारण नई बिल न की गई वास्तविक बिक्री भी तैयार कर ली जाती है।</span><span class="sxs-lookup"><span data-stu-id="5f418-113">If the quantity was reduced, the difference will cause a new unbilled sales actual to be created too.</span></span> <span data-ttu-id="5f418-114">उदाहरण के लिए, यदि बिल की गई मूल विक्रय आठ घंटों के लिए थी और सुधारित बीजक लाइन विवरण की घटी मात्रा छ: घंटों के लिए है, तो PSA बिल किए गए मूल विक्रय लाइन को उलट देता है और दो नए वास्तविक बिल तैयार हो जाते हैं:</span><span class="sxs-lookup"><span data-stu-id="5f418-114">For example, if the original billed sale was for eight hours, and the corrected invoice line detail has a reduced quantity of six hours, the original billed sales line is revered and two new actuals are created:</span></span>

- <span data-ttu-id="5f418-115">छ: घंटों के लिए बिल की गई वास्तविक बिक्री।</span><span class="sxs-lookup"><span data-stu-id="5f418-115">A billed sales actual for six hours.</span></span>
- <span data-ttu-id="5f418-116">शेष दो घंटों के लिए बिल न की गई वास्तविक बिक्री।</span><span class="sxs-lookup"><span data-stu-id="5f418-116">An unbilled sales actual for the remaining two hours.</span></span> <span data-ttu-id="5f418-117">इस लेनदेन को बाद में बिल किया जा सकता है या ग्राहक के साथ हुई बातचीत पर निर्भर करते हुए, प्रभार के लिए नहीं दर्शाया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="5f418-117">This transaction can either be billed later or marked as non-chargeable, depending on the negotiations with the customer.</span></span>
