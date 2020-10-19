---
title: उत्पाद-आधारित कोटेशन लाइनों के लिए प्रति माह, प्रति-उपयोगकर्ता जैसी जटिल इकाइयों का प्रबंधन करना
description: यह विषय उत्पाद-आधारित कोटेशन लाइनों के लिए जटिल इकाइयों के प्रबंधन के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/06/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 741230e69302138cce8f7379f520f7178e1c80af
ms.sourcegitcommit: fd8ea1779db2bb39a428f459ae3293c4fd785572
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/06/2020
ms.locfileid: "3965801"
---
# <a name="managing-complex-units-such-as-per-user-per-month-for-product-based-quote-lines"></a><span data-ttu-id="b844c-103">उत्पाद-आधारित कोटेशन लाइनों के लिए प्रति माह, प्रति-उपयोगकर्ता जैसी जटिल इकाइयों का प्रबंधन करना</span><span class="sxs-lookup"><span data-stu-id="b844c-103">Managing complex units such as per-user, per-month for product-based quote lines</span></span>

<span data-ttu-id="b844c-104">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="b844c-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="b844c-105">Dynamics 365 Project Operations सदस्यता-आधारित उत्पादों की Sales का समर्थन करने के लिए मात्रा कारकों का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="b844c-105">Dynamics 365 Project Operations uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="b844c-106">सदस्यता-आधारित उत्पादों के लिए उद्धरण पर या प्रोजेक्ट अनुबंध पंक्ति पर मात्रा, उपयोगकर्ता महीनों की संख्या के रूप में व्यक्त की जाती है।</span><span class="sxs-lookup"><span data-stu-id="b844c-106">For subscription-based products, the quantity on the quote or project contract line is expressed as the number of user-months.</span></span>

<span data-ttu-id="b844c-107">आमतौर पर, सदस्यता सॉफ़्टवेयर की कीमत कैटलॉग में प्रति माह प्रति उपयोगकर्ता मूल्य के रूप में संग्रहीत की जाती है।</span><span class="sxs-lookup"><span data-stu-id="b844c-107">Usually, the price of subscription software is stored in the catalog as the price per user per month.</span></span> <span data-ttu-id="b844c-108">बिक्री प्रक्रिया के दौरान, उद्धरण पद्धति पर मूल्य आमतौर पर प्रति-उपयोगकर्ता, प्रति माह मूल्य होता है, जिस पर IT बिक्री एजेंट मोलभाव और छूट देता था।</span><span class="sxs-lookup"><span data-stu-id="b844c-108">During the sales process, the price on the quote line is usually the per-user, per-month price that was negotiated and discounted by the IT sales agent.</span></span> <span data-ttu-id="b844c-109">प्रत्येक सौदे में उपयोगकर्ताओं की एक अलग संख्या और सदस्यता महीनों की एक अलग संख्या होती है।</span><span class="sxs-lookup"><span data-stu-id="b844c-109">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="b844c-110">कोटेशन लाइन की गणना करने के लिए उपयोग की जाने वाली मात्रा उपयोगकर्ताओं की संख्या और सदस्यता महीनों की संख्या का एक गुणनफल है.</span><span class="sxs-lookup"><span data-stu-id="b844c-110">The quantity used to compute the quote line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="b844c-111">इस प्रकार की Sales का समर्थन करने के लिए, Project Operations ने मात्रा कारकों की अवधारणा प्रस्तुत की.</span><span class="sxs-lookup"><span data-stu-id="b844c-111">To support this type of sale, Project Operations introduced the concept of quantity factors.</span></span> <span data-ttu-id="b844c-112">Dynamics 365 में, मात्रा कारक उत्पाद की विशेषताओं पर निर्भर करते हैं।</span><span class="sxs-lookup"><span data-stu-id="b844c-112">Quantity factors rely on the product attributes in Dynamics 365.</span></span> <span data-ttu-id="b844c-113">जब आप किसी उत्पाद के लिए विशिष्ट गुणों को कॉन्फ़िगर करते हैं, तो Project Operations आपको मात्रा कारकों के रूप में एक सबसेट, या सभी गुणों की निशानदेही करने देता है.</span><span class="sxs-lookup"><span data-stu-id="b844c-113">When you configure specific properties for a product, Project Operations lets you flag a subset, or all of the properties, as quantity factors.</span></span>

<span data-ttu-id="b844c-114">Project Operations पुष्टि करता है कि केवल संख्यात्मक गुण या उत्पाद गुण जिनके पास संख्यात्मक डेटा का प्रकार होता है, उनकी मात्रा कारकों के रूप में निशानदेही की जाती है.</span><span class="sxs-lookup"><span data-stu-id="b844c-114">Project Operations validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="b844c-115">जब आप एक कोटेशन लाइन में मात्रा कारकों के साथ उत्पाद को जोड़ते हैं, तो **मात्रा** फ़ील्ड केवल पढ़ने योग्य बन जाता है.</span><span class="sxs-lookup"><span data-stu-id="b844c-115">When you add a product with quantity factors to a quote line, the **Quantity** field becomes read-only.</span></span> <span data-ttu-id="b844c-116">उत्पाद गुणों के लिए मानों को, जो मात्रा कारक होते हैं, डालने के बाद , Project Operations कोटेशन लाइन की मात्रा की गणना करता है.</span><span class="sxs-lookup"><span data-stu-id="b844c-116">After you enter values for product properties that are quantity factors, Project Operations calculates the quantity of the quote line.</span></span>

<span data-ttu-id="b844c-117">उदाहरण के लिए, Dynamics 365 Sales में निम्न गुण हो सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="b844c-117">For example, Dynamics 365 Sales might have the following properties:</span></span>

- <span data-ttu-id="b844c-118">**उपयोगकर्ता संख्या**: उपयोगकर्ताओं की संख्या</span><span class="sxs-lookup"><span data-stu-id="b844c-118">**No of users**: The number of users</span></span>
- <span data-ttu-id="b844c-119">**महीनों की संख्या**: सदस्यता महीनों की संख्या</span><span class="sxs-lookup"><span data-stu-id="b844c-119">**No of Months**: The number of subscription months</span></span>
- <span data-ttu-id="b844c-120">**उत्पाद SKU**</span><span class="sxs-lookup"><span data-stu-id="b844c-120">**Product SKU**</span></span>

<span data-ttu-id="b844c-121">आप उत्पाद लाइन के गुणों को संपादित करके **उपयोगकर्ताओं की संख्या** और **महीनों की संख्या** गुणों की मात्रा कारकों के रूप में निशानदेही कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="b844c-121">You can flag the **No of Users** and **No of Months** properties as quantity factors by editing the properties of the product line.</span></span>

<span data-ttu-id="b844c-122">उत्पाद गुणों से मात्रा कारकों को बनाने के लिए, इन चरणों का पालन करें:</span><span class="sxs-lookup"><span data-stu-id="b844c-122">To create Quantity factors from Product properties, follow these steps:</span></span>

1. <span data-ttu-id="b844c-123">Project Operations के बाएँ नेविगेशन फलक पर, **विक्रय** > **उत्पाद** पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="b844c-123">On the Project Operations left navigation pane, go to **Sales** > **Products**.</span></span>
2. <span data-ttu-id="b844c-124">उस उत्पाद को खोलें जिसके लिए आपको मात्रा कारकों को कॉन्फ़िगर करने की जरूरत है.</span><span class="sxs-lookup"><span data-stu-id="b844c-124">Open the product for which you need to configure quantity factors.</span></span> <span data-ttu-id="b844c-125">सुनिश्चित करें कि उत्पाद में पहले से ही कॉन्फ़िगर किए गए गुण हैं.</span><span class="sxs-lookup"><span data-stu-id="b844c-125">Make sure the product has properties already configured.</span></span>
3. <span data-ttu-id="b844c-126">उत्पाद के लिए **परियोजना जानकारी** पृष्ठ पर, **मात्रा कारक** टैब का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="b844c-126">On the **Project Information** page for the Product, select the **Quantity Factors** tab.</span></span>
4. <span data-ttu-id="b844c-127">सबग्रिड में, **+ नई फील्ड गणना** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="b844c-127">In the subgrid, select **+ New field computation**.</span></span>
5. <span data-ttu-id="b844c-128">मात्रा कारक का नाम दर्ज करें और उस गुण मान का चयन करें जो फ़ील्ड गणना से मानचित्रण करता है.</span><span class="sxs-lookup"><span data-stu-id="b844c-128">Enter the name of the Quantity factor and select the property value that maps to the field computation.</span></span>
6. <span data-ttu-id="b844c-129">प्रपत्र को सहेजें और बंद करें.</span><span class="sxs-lookup"><span data-stu-id="b844c-129">Save and close the form.</span></span> <span data-ttu-id="b844c-130">उत्पाद-आधारित कोटेशन लाइन के लिए मात्रा की गणना हेतु उपयोग करने के लिए सभी गुणों के लिए इन चरणों को दोहराएं.</span><span class="sxs-lookup"><span data-stu-id="b844c-130">Repeat these steps for all properties to use for computing the quantity for the product-based quote line.</span></span>

<span data-ttu-id="b844c-131">जब आप किसी उत्पाद के लिए उत्पाद-आधारित कोटेशन लाइन बनाते हैं, तो कोट लाइन की मात्रा लॉक हो जाएगी.</span><span class="sxs-lookup"><span data-stu-id="b844c-131">When you create a product-based quote line for a product, the quantity of the quote line will be locked.</span></span> <span data-ttu-id="b844c-132">मात्रा की गणना गुण मानों के गुणनफल के रूप में की जाएगी जिसे आप उस कोटेशन लाइन के लिए डालते हैं.</span><span class="sxs-lookup"><span data-stu-id="b844c-132">The quantity will be computed as a product of the property values that you input for that quote line.</span></span>
