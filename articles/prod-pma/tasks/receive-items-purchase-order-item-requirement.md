---
title: जरूरी आइटम से क्रय ऑर्डर पर प्राप्त आइटम
description: यह विषय वर्णन करता है कि किसी जरूरी आइटम से क्रय ऑर्डर पर आइटम कैसे प्राप्त करते हैं.
author: Yowelle
manager: AnnBe
ms.date: 08/06/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjProjectsListPage, ProjTable, ProjSalesItemReq, InventItemIdLookupSimple, PurchCreateFromSalesOrder, VendAccountItemLookup, PurchTable, PurchEditLines
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: andchoi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: a5b3622458da957ed150311f6ea75d5f1444d5f1
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077867"
---
# <a name="receive-items-on-purchase-order-from-item-requirement"></a><span data-ttu-id="c57cf-103">जरूरी आइटम से क्रय ऑर्डर पर प्राप्त आइटम</span><span class="sxs-lookup"><span data-stu-id="c57cf-103">Receive items on purchase order from item requirement</span></span>

[!include [banner](../../includes/banner.md)]

<span data-ttu-id="c57cf-104">यह विषय वर्णन करता है कि किसी जरूरी आइटम से क्रय ऑर्डर पर आइटम कैसे प्राप्त करते हैं.</span><span class="sxs-lookup"><span data-stu-id="c57cf-104">This topic explains how to receive items on a purchase order from an item requirement.</span></span>

<span data-ttu-id="c57cf-105">आइटम लेनदेन के स्थान पर जरूरी आइटम का उपयोग कर, वास्तव में आइटम के इस्तेमाल होने से पहले आप डिलिवरी तय कर सकते हैं, क्रय ऑर्डर बनाएं, आइटम को व्यापार-समझौता रूपरेखा में शामिल करें, और जरूरी आइटम को उत्पादन योजना में शामिल करें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-105">By using an item requirement instead of an item transaction, you can plan for delivery just before the item is actually used, create a purchase order, include the item in the trade-agreement framework, and include the item requirement in production planning.</span></span> 

<span data-ttu-id="c57cf-106">यह कार्य USSI डेटा सेट का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="c57cf-106">This task uses the USSI data set.</span></span>

1. <span data-ttu-id="c57cf-107">नेविगेशन फलक में **मॉड्यूल > परियोजना प्रबंधन और लेखांकन > परियोजनाएं > सभी परियोजनाएं** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="c57cf-107">In the navigation pane, go to **Modules > Project management and accounting > Projects > All projects**.</span></span>
2. <span data-ttu-id="c57cf-108">इस सूची में वांछित पंक्ति में लिंक को चुनें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-108">In the list, select the link in the desired row.</span></span>
3. <span data-ttu-id="c57cf-109">क्रिया फलक पर, **योजना** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-109">On the Action Pane, select **Plan**.</span></span>
4. <span data-ttu-id="c57cf-110">**आइटम आवश्यकताएँ** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-110">Select **Item requirements**.</span></span>
5. <span data-ttu-id="c57cf-111">**नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-111">Select **New**.</span></span>
6. <span data-ttu-id="c57cf-112">नई पंक्ति में, **आइटम संख्या** फील्ड में एक मूल्य दर्ज करें या चुनें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-112">In the new row, enter or select a value in the **Item number** field.</span></span>
7. <span data-ttu-id="c57cf-113">**मात्रा** फ़ील्ड में, संख्या दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-113">In the **Quantity** field, enter a number.</span></span>
8. <span data-ttu-id="c57cf-114">**सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-114">Select **Save**.</span></span>
9. <span data-ttu-id="c57cf-115">क्रिया फलक पर, **प्रबंधन** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-115">On the Action Pane, select **Manage**.</span></span>
10. <span data-ttu-id="c57cf-116">**फ़ंक्शन** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-116">Select **Functions**.</span></span>
11. <span data-ttu-id="c57cf-117">**क्रय आदेश बनाएँ** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-117">Select **Create purchase order**.</span></span>
12. <span data-ttu-id="c57cf-118">**सभी को शामिल करें** चेक बॉक्स चुनें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-118">Select the **Include all** check box.</span></span>
13. <span data-ttu-id="c57cf-119">**वेंडर खाता** फील्ड, में मूल्य को दर्ज करें या चुनें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-119">In the **Vendor account** field, enter or select a value.</span></span>
14. <span data-ttu-id="c57cf-120">**ठीक** चुनें।</span><span class="sxs-lookup"><span data-stu-id="c57cf-120">Select **OK**.</span></span>
15. <span data-ttu-id="c57cf-121">नेविगेशन फलक में **मॉड्यूल> देनदारी लेखे> क्रय आदेश> सभी क्रय आदेश** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="c57cf-121">In the navigation pane, go to **Modules > Accounts payable > Purchase orders > All purchase orders**.</span></span>
16. <span data-ttu-id="c57cf-122">इस सूची में वांछित पंक्ति में लिंक को चुनें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-122">In the list, select the link in the desired row.</span></span>
17. <span data-ttu-id="c57cf-123">क्रिया फलक पर, **क्रय** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-123">On the Action Pane, select **Purchase**.</span></span>
18. <span data-ttu-id="c57cf-124">**पुष्टि करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-124">Select **Confirm**.</span></span>
19. <span data-ttu-id="c57cf-125">क्रिया फलक पर, **प्राप्त करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-125">On the Action Pane, select **Receive**.</span></span>
20. <span data-ttu-id="c57cf-126">**उत्पाद रसीद** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-126">Select **Product receipt**.</span></span>
21. <span data-ttu-id="c57cf-127">**उत्पाद रसीद** में, एक मूल्य टाइप करें.</span><span class="sxs-lookup"><span data-stu-id="c57cf-127">In the **Product receipt** field, type a value.</span></span>
22. <span data-ttu-id="c57cf-128">**ठीक** चुनें।</span><span class="sxs-lookup"><span data-stu-id="c57cf-128">Select **OK**.</span></span>

