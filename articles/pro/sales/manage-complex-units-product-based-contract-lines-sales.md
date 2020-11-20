---
title: उत्पाद-आधारित अनुबंध पंक्तियों के लिए जटिल इकाइयाँ प्रबंधित करें - लाइट
description: यह विषय सदस्यता-आधारित उत्पादों की बिक्री का समर्थन करने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/28/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: a58a13c8186f36e6031fe3c6f3c3a57ea920ac9e
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/30/2020
ms.locfileid: "4177378"
---
# <a name="manage-complex-units-for-product-based-contract-lines---lite"></a><span data-ttu-id="1891b-103">उत्पाद-आधारित अनुबंध पंक्तियों के लिए जटिल इकाइयाँ प्रबंधित करें - लाइट</span><span class="sxs-lookup"><span data-stu-id="1891b-103">Manage complex units for product-based contract lines - lite</span></span>

<span data-ttu-id="1891b-104">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="1891b-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1891b-105">Dynamics 365 Project Operations सदस्यता-आधारित उत्पादों की Sales का समर्थन करने के लिए मात्रा कारकों का उपयोग करता है.</span><span class="sxs-lookup"><span data-stu-id="1891b-105">Dynamics 365 Project Operations uses quantity factors to support the sale of subscription-based products.</span></span> <span data-ttu-id="1891b-106">सदस्यता-आधारित उत्पादों के लिए, अनुबंध पर या परियोजना अनुबंध पंक्ति पर मात्रा, उपयोगकर्ता महीनों की संख्या के रूप में व्यक्त की जाती है.</span><span class="sxs-lookup"><span data-stu-id="1891b-106">For subscription-based products, the quantity on the contract or project contract line is expressed as the number of user-months.</span></span>

<span data-ttu-id="1891b-107">सदस्यता सॉफ़्टवेयर का मूल्य कैटलॉग में प्रति माह प्रति उपयोगकर्ता मूल्य के रूप में संग्रहित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="1891b-107">The price of subscription software is stored in the catalog as the price per-user, per-month.</span></span> <span data-ttu-id="1891b-108">विक्रय प्रक्रिया के दौरान, अनुबंध पंक्ति पर मूल्य आमतौर पर प्रति-उपयोगकर्ता, प्रति माह मूल्य होता है, जिस पर IT बिक्री एजेंट मोलभाव और छूट देता था.</span><span class="sxs-lookup"><span data-stu-id="1891b-108">During the sales process, the price on the contract line is usually the per-user, per-month price that was negotiated and discounted by the sales agent.</span></span> <span data-ttu-id="1891b-109">प्रत्येक सौदे में उपयोगकर्ताओं की एक अलग संख्या और सदस्यता महीनों की एक अलग संख्या होती है।</span><span class="sxs-lookup"><span data-stu-id="1891b-109">Each deal has a different number of users and a different number of subscription months.</span></span> <span data-ttu-id="1891b-110">अनुबंध पंक्ति की मात्रा की गणना करने के लिए उपयोग की जाने वाली मात्रा, उपयोगकर्ताओं की संख्या और सदस्यता महीनों की संख्या की गुणा होती है.</span><span class="sxs-lookup"><span data-stu-id="1891b-110">The quantity used to calculate the amount of the contract line is a product of the number of users and the number of subscription months.</span></span>

<span data-ttu-id="1891b-111">इस प्रकार के विक्रय का समर्थन करने के लिए, Project Operations *मात्रा कारकों* की अवधारणा का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="1891b-111">To support this type of sale, Project Operations supports the concept of *quantity factors*.</span></span> <span data-ttu-id="1891b-112">मात्रा घटक उत्पाद की विशेषताओं पर निर्भर करते हैं.</span><span class="sxs-lookup"><span data-stu-id="1891b-112">Quantity factors rely on product attributes.</span></span> <span data-ttu-id="1891b-113">जब आप किसी उत्पाद के लिए विशिष्ट गुणों को कॉन्फ़िगर करते हैं, तो आपको उन विशेषताओं के उपसमूह को या सभी विशेषताओं को मात्रा कारकों के रूप में चिह्नित करने देता है.</span><span class="sxs-lookup"><span data-stu-id="1891b-113">When you configure specific properties for a product, you can flag a subset of those properties, or all the properties, as quantity factors.</span></span>

<span data-ttu-id="1891b-114">Project Operations पुष्टि करता है कि केवल संख्यात्मक गुण या उत्पाद गुण जिनके पास संख्यात्मक डेटा का प्रकार होता है, उनकी मात्रा कारकों के रूप में निशानदेही की जाती है.</span><span class="sxs-lookup"><span data-stu-id="1891b-114">Project Operations validates that only numeric properties or product properties that have a numeric data type are flagged as quantity factors.</span></span> <span data-ttu-id="1891b-115">जब कॉन्फ़िगर किए गए मात्रा कारकों वाला उत्पाद अनुबंध पंक्ति में जोड़ा जाता है, तो **मात्रा** फ़ील्ड केवल पढ़ने के लिए हो जाती है.</span><span class="sxs-lookup"><span data-stu-id="1891b-115">When a product with configured quantity factors is added to a contract line, the **Quantity** field  becomes read-only.</span></span> <span data-ttu-id="1891b-116">जब आप उन उत्पाद गुणों के लिए मान दर्ज करते हैं, जो मात्रा कारक होते हैं, तो Project Operations अनुबंध पंक्ति की मात्रा की गणना करता है.</span><span class="sxs-lookup"><span data-stu-id="1891b-116">After you enter values for product properties that are quantity factors, Project Operations calculates the quantity of the contract line.</span></span>

<span data-ttu-id="1891b-117">उदाहरण के लिए, Dynamics 365 Sales में निम्न गुण हो सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="1891b-117">For example, Dynamics 365 Sales might have the following properties:</span></span>

- <span data-ttu-id="1891b-118">**उपयोगकर्ता संख्या**: उपयोगकर्ताओं की संख्या.</span><span class="sxs-lookup"><span data-stu-id="1891b-118">**No of users**: The number of users.</span></span>
- <span data-ttu-id="1891b-119">**महीनों की संख्या**: सदस्यता महीनों की संख्या.</span><span class="sxs-lookup"><span data-stu-id="1891b-119">**No of Months**: The number of subscription months.</span></span>
- <span data-ttu-id="1891b-120">**उत्पाद SKU**: उत्पाद के लिए स्टॉक कीपिंग यूनिट (SKU).</span><span class="sxs-lookup"><span data-stu-id="1891b-120">**Product SKU**: The stock keeping unit (SKU) for the product.</span></span>

<span data-ttu-id="1891b-121">उत्पाद पद्धति की विशेषताओं को संपादित करके **उपयोगकर्ताओं की संख्या** और **महीनों की संख्या** को मात्रा कारकों के रूप में चिह्नित किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="1891b-121">The **No of Users** and **No of Months** properties can be flagged as quantity factors by editing the properties of the product line.</span></span>

<span data-ttu-id="1891b-122">उत्पाद गुणों से मात्रा कारक बनाने के लिए, निम्न चरणों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="1891b-122">To create quantity factors from product properties, complete the following steps.</span></span>

1. <span data-ttu-id="1891b-123">**Project Operations** पर, **विक्रय-उत्पाद** चुनें.</span><span class="sxs-lookup"><span data-stu-id="1891b-123">On the **Project Operations**, select **Sales-Products**.</span></span>
2. <span data-ttu-id="1891b-124">वह उत्पाद खोलें, जिसके लिए आपको मात्रा कारक सेट करने की आवश्यकता है.</span><span class="sxs-lookup"><span data-stu-id="1891b-124">Open the product for which you need to set up quantity factors.</span></span> <span data-ttu-id="1891b-125">सुनिश्चित करें कि उत्पाद में पहले से ही गुण सेट अप हैं.</span><span class="sxs-lookup"><span data-stu-id="1891b-125">Make sure that the product has properties already set up.</span></span>
3. <span data-ttu-id="1891b-126">**परियोजना जानकारी** पृष्ठ पर, **मात्रा कारक** टैब चुनें.</span><span class="sxs-lookup"><span data-stu-id="1891b-126">On the **Project Information** page, select the **Quantity Factors** tab.</span></span>
4. <span data-ttu-id="1891b-127">सबग्रिड में, **+ नई फील्ड गणना** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="1891b-127">In the subgrid, select **+ New field computation**.</span></span>
5. <span data-ttu-id="1891b-128">**मात्रा कारक** का नाम दर्ज करें और उस गुण मान का चयन करें, जो फ़ील्ड गणना पर मैप होता है.</span><span class="sxs-lookup"><span data-stu-id="1891b-128">Enter the name of the **Quantity Factor** and select the property value that maps to the field computation.</span></span>
6. <span data-ttu-id="1891b-129">प्रपत्र को सहेजें और बंद करें.</span><span class="sxs-lookup"><span data-stu-id="1891b-129">Save and close the form.</span></span>
7. <span data-ttu-id="1891b-130">सभी गुणों के लिए चरण 2-6 दोहराएं, जो एक साथ उत्पाद-आधारित अनुबंध पंक्ति के लिए मात्रा बनाएंगे.</span><span class="sxs-lookup"><span data-stu-id="1891b-130">Repeat steps 2-6 for all the properties that together will make up the quantity for the product-based contract line.</span></span>

<span data-ttu-id="1891b-131">मात्रा कारक सेट अप होने पर, जब उपयोगकर्ता इस उत्पाद के लिए एक अनुबंध पंक्ति बनाता है, तो अनुबंध पंक्ति की मात्रा लॉक हो जाती है.</span><span class="sxs-lookup"><span data-stu-id="1891b-131">With quantity factors set up, when the user creates a contract line for this product, the quantity of the contract line is locked.</span></span> <span data-ttu-id="1891b-132">उसके बाद मात्रा की गणना उस अनुबंध पंक्ति के लिए गुण मान के उत्पाद के रूप में की जाती है.</span><span class="sxs-lookup"><span data-stu-id="1891b-132">The quantity is then calculated as a product of the property values for that contract line.</span></span>
