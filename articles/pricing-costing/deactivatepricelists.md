---
title: प्राइस लिस्टों को निष्क्रिय करें
description: यह विषय अप्रयुक्त या पुरानी प्राइस लिस्टों को निष्क्रिय या हटाने का तरीका बताता है.
author: rumant
ms.date: 03/19/2021
ms.topic: article
ms.prod: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: ''
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Professional Service industries
ms.author: rumant
ms.dyn365.ops.version: ''
ms.search.validFrom: 2020-10-01
ms.openlocfilehash: d5d6cf6b4b097c08edca5a3235ed1b438a0eae2d
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001338"
---
# <a name="deactivate-price-lists"></a><span data-ttu-id="882eb-103">मूल्य सूचियों को निष्क्रिय करें</span><span class="sxs-lookup"><span data-stu-id="882eb-103">Deactivate price lists</span></span> 

<span data-ttu-id="882eb-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="882eb-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="882eb-105">Dynamics 365 Project Operations से पुरानी या अप्रयुक्त प्राइस लिस्टों को हटाने के लिए, आपको दो चरण पूरे करने होंगे.</span><span class="sxs-lookup"><span data-stu-id="882eb-105">To remove old or unused price lists from Dynamics 365 Project Operations, there are two steps you must complete.</span></span> 

1. <span data-ttu-id="882eb-106">विशिष्ट पेजों से प्राइस लिस्ट हटाएं या मिटाएं.</span><span class="sxs-lookup"><span data-stu-id="882eb-106">Remove or delete the price list from specific pages.</span></span>
2. <span data-ttu-id="882eb-107">**प्राइस लिस्ट** पेज पर सक्रिय प्राइस लिस्टों से प्राइस लिस्ट को निष्क्रिय करें या मिटा दें.</span><span class="sxs-lookup"><span data-stu-id="882eb-107">Deactivate or delete the price list from the Active price lists on the **Price Lists** page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="882eb-108">आपको प्राइस लिस्ट को पूरी तरह से हटाने के लिए दोनों चरणों को पूरा करना होगा.</span><span class="sxs-lookup"><span data-stu-id="882eb-108">You must complete both steps to fully remove a price list.</span></span> <span data-ttu-id="882eb-109">केवल चरण 2 को करना, जो सक्रिय प्राइस लिस्टों के दृश्य से प्राइस लिस्ट को सीधे मिटाना या निष्क्रिय करना है, पर्याप्त नहीं है.</span><span class="sxs-lookup"><span data-stu-id="882eb-109">Only performing step 2, which is to directly delete or deactivate the price list from the Active Price Lists view, is not sufficient.</span></span> <span data-ttu-id="882eb-110">आपको इस प्राइस लिस्ट के संबंध को चरण 1 में उल्लिखित सभी स्थानों से भी मिटाना होगा.</span><span class="sxs-lookup"><span data-stu-id="882eb-110">You must also delete the association of this price list from all the places mentioned in step 1.</span></span>

## <a name="delete-the-price-list-from-specific-pages"></a><span data-ttu-id="882eb-111">विशिष्ट पेजों से प्राइस लिस्ट मिटाएं</span><span class="sxs-lookup"><span data-stu-id="882eb-111">Delete the price list from specific pages</span></span>
1. <span data-ttu-id="882eb-112">Project Operations से किसी प्राइस लिस्ट को मिटाने के लिए, निम्नलिखित पेजों पर जाएं:</span><span class="sxs-lookup"><span data-stu-id="882eb-112">To delete a price list from Project Operations, go to the following pages:</span></span>  

      - <span data-ttu-id="882eb-113">**परियोजना मापदंड** पेज > **प्राइस लिस्ट** टैब</span><span class="sxs-lookup"><span data-stu-id="882eb-113">**Project parameters** page > **Price Lists** tab</span></span>
      - <span data-ttu-id="882eb-114">**संगठनात्मक इकाई** पेज > **प्राइस लिस्ट** ग्रिड</span><span class="sxs-lookup"><span data-stu-id="882eb-114">**Organizational Unit** page > **Price Lists** grid</span></span>
      - <span data-ttu-id="882eb-115">**खाता** पेज > **प्रोजेक्ट मूल्य सूचियाँ** ग्रिड</span><span class="sxs-lookup"><span data-stu-id="882eb-115">**Account** page > **Project Price Lists** grid</span></span>
      - <span data-ttu-id="882eb-116">**परियोजना के लिए कोट** पेज > **परियोजना के प्राइस लिस्ट** ग्रिड: यह सभी सक्रिय परियोजना कोट पर लागू होता है.</span><span class="sxs-lookup"><span data-stu-id="882eb-116">**Project Quotes** page > **Project Price Lists** grid: This applies to all active project quotes.</span></span>
      - <span data-ttu-id="882eb-117">**परियोजना अनुबंध** पेज > **परियोजना प्राइस लिस्ट** ग्रिड: यह सभी सक्रिय परियोजना अनुबंधों पर लागू होता है.</span><span class="sxs-lookup"><span data-stu-id="882eb-117">**Project Contracts** page > **Project Price Lists** grid: This applies to all active project contracts.</span></span>

 2. <span data-ttu-id="882eb-118">प्रत्येक पेज के लिए, आपको उस प्राइस लिस्ट का चयन करना होगा जिसे आप मिटाना चाहते हैं, और फिर **मिटाएं** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="882eb-118">For each page, you need to select the price list that you want to delete, and then select **Delete**.</span></span> 
 
## <a name="delete-or-deactivate-the-price-list-from-the-price-lists-page"></a><span data-ttu-id="882eb-119">प्राइस लिस्ट पेज से प्राइस लिस्ट को मिटाएं या निष्क्रिय करें</span><span class="sxs-lookup"><span data-stu-id="882eb-119">Delete or deactivate the price list from the Price Lists page</span></span>
 
1. <span data-ttu-id="882eb-120">सक्रिय प्राइस लिस्टों से एक प्राइस लिस्ट को मिटाने के लिए, **बिक्री**  > **ग्राहक** > **प्राइस लिस्ट** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="882eb-120">To delete a price list from the active price lists, go to **Sales** > **Customers** > **Price Lists**.</span></span> 
2. <span data-ttu-id="882eb-121">उस प्राइस लिस्ट का चयन करें जिसे आप मिटाना चाहते हैं और फिर **मिटाएं** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="882eb-121">Select the price list that you want to delete and then select **Delete**.</span></span> <span data-ttu-id="882eb-122">यदि प्राइस लिस्ट किसी भी मौजूदा लेनदेन पर संदर्भित है, तो आप इसे मिटा नहीं पाएंगे.</span><span class="sxs-lookup"><span data-stu-id="882eb-122">If the price list is referenced on any existing transactions, you won't be able to delete it.</span></span> <span data-ttu-id="882eb-123">यदि ऐसा होता है, तो आप प्राइस लिस्ट को निष्क्रिय कर सकते हैं ताकि यह किसी भी दृश्य में दिखाई न दे.</span><span class="sxs-lookup"><span data-stu-id="882eb-123">If this happens, you can deactivate the price list so that it doesn't appear in any views.</span></span> 
3. <span data-ttu-id="882eb-124">प्राइस लिस्ट को निष्क्रिय करने के लिए, प्राइस लिस्ट को फिर से चुनें, और फिर **निष्क्रिय करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="882eb-124">To deactivate the price list, select the price list again, and then select **Deactivate**.</span></span>   
