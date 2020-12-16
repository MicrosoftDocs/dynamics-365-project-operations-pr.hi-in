---
title: नए मूल्य निर्धारण आयामों के साथ प्लग-इन एट्रिब्यूट अद्यतन करना
description: इस विषय में मूल्य निर्धारण आयामों के लिए प्लग-इन एट्रिब्यूट को अद्यतन करने के बारे में जानकारी प्रदान की गई है.
author: rumant
manager: Annbe
ms.date: 11/18/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 9b0cf48318d0b9e94c4be0d3775b54e83832c1b7
ms.sourcegitcommit: 573be7e36604ace82b35e439cfa748aa7c587415
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/25/2020
ms.locfileid: "4643220"
---
# <a name="update-plug-in-attributes-with-new-pricing-dimensions"></a><span data-ttu-id="8629d-103">नए मूल्य निर्धारण आयामों के साथ प्लग-इन एट्रिब्यूट अद्यतन करें</span><span class="sxs-lookup"><span data-stu-id="8629d-103">Update plug-in attributes with new pricing dimensions</span></span>

<span data-ttu-id="8629d-104">इस विषय में मूल्य निर्धारण आयामों के लिए प्लग-इन एट्रिब्यूट को अद्यतन करने के बारे में जानकारी प्रदान की गई है.</span><span class="sxs-lookup"><span data-stu-id="8629d-104">This topic provides information about how to update plug-in attributes for pricing dimensions.</span></span>

> [!NOTE]
> <span data-ttu-id="8629d-105">यह विषय केवल कोट और Dynamics 365 Project Operations में अनुबंध सुविधाओं पर लागू होता है.</span><span class="sxs-lookup"><span data-stu-id="8629d-105">This topic is only applicable to the quote and contract features in Dynamics 365 Project Operations.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8629d-106">पूर्वावश्यकताएँ</span><span class="sxs-lookup"><span data-stu-id="8629d-106">Prerequisites</span></span>
<span data-ttu-id="8629d-107">इस विषय के चरणों को पूरा करने से पहले, आपको निम्नलिखित विषयों में प्रक्रियाएँ पूरी करनी होंगी:</span><span class="sxs-lookup"><span data-stu-id="8629d-107">Before you complete the steps in this topic, you must have completed the procedures in the following topics:</span></span>

  - [<span data-ttu-id="8629d-108">कस्टम फ़ील्ड और निकाय बनाएँ</span><span class="sxs-lookup"><span data-stu-id="8629d-108">Create custom fields and entities</span></span>](create-custom-fields-entities-pricing-dimensions.md) 
  - [<span data-ttu-id="8629d-109">कस्टम फ़ील्ड को मूल्य सेटअप और लेन-देन वाली निकाय में जोड़ें </span><span class="sxs-lookup"><span data-stu-id="8629d-109">Add custom fields to price setup and transactional entities</span></span>](add-custom-fields-price-setup-transactional-entities.md)
  - <span data-ttu-id="8629d-110">[मूल्य निर्धारण आयामों के रूप में कस्टम फ़ील्ड सेटअप करें](set-up-custom-fields-pricing-dimensions.md).</span><span class="sxs-lookup"><span data-stu-id="8629d-110">[Set up custom fields as pricing dimensions](set-up-custom-fields-pricing-dimensions.md).</span></span> 
  
<span data-ttu-id="8629d-111">यदि आपने वे प्रक्रियाएं पूरी नहीं की हैं, तो उन्हें पूरा करें और उसके बाद इस विषय पर वापस लौटें.</span><span class="sxs-lookup"><span data-stu-id="8629d-111">If you haven't completed those procedures, complete them and then return to this topic.</span></span>

## <a name="register-a-plug-in"></a><span data-ttu-id="8629d-112">एक प्लग-इन पंजीकृत करें</span><span class="sxs-lookup"><span data-stu-id="8629d-112">Register a plug-in</span></span>
<span data-ttu-id="8629d-113">जब परियोजना कोट पंक्ति के लिए **कोट पंक्ति** पृष्ठ पर कोट पंक्ति विवरण बनाया जाता है, तो सिस्टम दो अनुमान पंक्तियाँ बनाता है.</span><span class="sxs-lookup"><span data-stu-id="8629d-113">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines.</span></span> <span data-ttu-id="8629d-114">एक पंक्ति अनुमान की लागत पक्ष होती है और दूसरी पंक्ति विक्रय पक्ष होती है.</span><span class="sxs-lookup"><span data-stu-id="8629d-114">One line is for the cost side of the estimate and the other line is for sales the side.</span></span> <span data-ttu-id="8629d-115">यही बात परियोजना कॉन्ट्रेक्ट लाइनों पर लागू होती है।</span><span class="sxs-lookup"><span data-stu-id="8629d-115">This is the same  for project contract lines.</span></span>

<span data-ttu-id="8629d-116">जब आप लागत पक्ष की मात्रा या फ़ील्ड में परिवर्तन करते हैं, तो यह परिवर्तन विक्रय पक्ष में भी किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="8629d-116">When you make a change to the quantity or a field on the cost side, that change is also made on the sales side.</span></span> <span data-ttu-id="8629d-117">यह संभव है, क्योंकि Quotelinedetail और contractline विवरण निकायों पर PreOperation प्लग-इन लागत पक्ष के विशिष्ट एट्रिब्यूट को लेनदेन के विक्रय पक्ष से कनेक्ट करता है.</span><span class="sxs-lookup"><span data-stu-id="8629d-117">This is possible because the PreOperation plug-ins on Quotelinedetail and contractline detail entities connect specific attributes on the cost side to the sales side of the transaction.</span></span> <span data-ttu-id="8629d-118">यदि आप चाहते हैं कि विक्रय पक्ष पर मूल्य निर्धारण आयाम मानों में किए गए परिवर्तन लागत पक्ष पर भी किए जाएँ, तो मूल्य निर्धारण आयाम में परिवर्तन करने के बाद निम्नलिखित प्लग-इन को फिर से पंजीकृत किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="8629d-118">If you need changes made to the pricing dimension values on the sales side to also be made on the cost side, the following plug-ins must be re-registered after making changes to a pricing dimension.</span></span>

<span data-ttu-id="8629d-119">ये अद्यतन और पुनः पंजीकृत किए जाने वाला प्लग-इन हैं:</span><span class="sxs-lookup"><span data-stu-id="8629d-119">These are the plug-ins to update and re-register:</span></span>

- <span data-ttu-id="8629d-120">PreOperationContractLineDetailUpdate - **अद्यतन msdyn_orderlinetransaction**</span><span class="sxs-lookup"><span data-stu-id="8629d-120">PreOperationContractLineDetailUpdate - **Update msdyn_orderlinetransaction**</span></span>
- <span data-ttu-id="8629d-121">PreOperationQuoteLineDetailUpdate - **अद्यतन msdyn_quotelinetransaction**</span><span class="sxs-lookup"><span data-stu-id="8629d-121">PreOperationQuoteLineDetailUpdate - **Updates msdyn_quotelinetransaction**</span></span>

<span data-ttu-id="8629d-122">प्लग-इन को अद्यतन और पुनः पंजीकृत करने के लिए निम्नलिखित चरणों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="8629d-122">Complete the following steps to update and re-register the plug-ins.</span></span>

1. <span data-ttu-id="8629d-123">**PluginRegistrationTool** को खोलें और उसे अपने Project Operations Dataverse परिवेश से कनेक्ट करें.</span><span class="sxs-lookup"><span data-stu-id="8629d-123">Open **PluginRegistrationTool** and connect to your Project Operations Dataverse environment.</span></span>
2. <span data-ttu-id="8629d-124">**खोजें** चुनें और अद्यतन किए जाने वाले प्लग-इन के पहले कुछ अक्षर लिखें.</span><span class="sxs-lookup"><span data-stu-id="8629d-124">Select **Search**, and type in the first few letters of the plug-in to be updated.</span></span>
3. <span data-ttu-id="8629d-125">प्लग-इन मिलने के बाद, उसका चयन करें और उसके बाद **मुख्य प्रपत्र का चयन करें** को चुनें.</span><span class="sxs-lookup"><span data-stu-id="8629d-125">After the plug-in is found, select it, and then select **Select on Main Form**.</span></span>
4. <span data-ttu-id="8629d-126">**अद्यतन msdyn_orderlinetransaction** चरण चुनें, राइट-क्लिक करें और उसके बाद **अद्यतन करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="8629d-126">Select the **Update msdyn_orderlinetransaction** step, right-click, and then select **Update**.</span></span>
5. <span data-ttu-id="8629d-127">**अद्यतन** संवाद पृष्ठ में फ़िल्टरिंग एट्रिब्यूट में एलिप्सिस (**...**) चुनें.</span><span class="sxs-lookup"><span data-stu-id="8629d-127">In the **Update** dialog page, select the ellipsis (**...**) in the filtering attributes.</span></span>
6. <span data-ttu-id="8629d-128">फ़िल्टरिंग एट्रिब्यूट विंडो खुलती है और निकाय और मूल्य निर्धारण आयामों में सभी एट्रिब्यूट की एक सूची प्रदान करती है.</span><span class="sxs-lookup"><span data-stu-id="8629d-128">The filtering attributes window opens and provides a list of all attributes in the entity and the pricing dimensions.</span></span> <span data-ttu-id="8629d-129">मूल्य निर्धारण आयाम एट्रिब्यूट के लिए चेक बॉक्स का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="8629d-129">Select the check boxes for the pricing dimension attributes.</span></span>
7. <span data-ttu-id="8629d-130">पृष्ठ को बंद करने के लिए **ठीक** चुनें और उसके बाद **अद्यतन चरण** चुनें.</span><span class="sxs-lookup"><span data-stu-id="8629d-130">Select **OK** to close the page, and then select **Update Step**.</span></span>
8. <span data-ttu-id="8629d-131">दूसरे प्लग-इन के लिए चरण 2-7 को दोहराएं, **PreOperationQuoteLineDetail**.</span><span class="sxs-lookup"><span data-stu-id="8629d-131">Repeat steps 2-7 for the second plug-in, **PreOperationQuoteLineDetail**.</span></span> <span data-ttu-id="8629d-132">इस प्लग-इन के लिए, आपको **msdyn_quotelinetransaction का अद्यतन** चरण अद्यतन करना होगा.</span><span class="sxs-lookup"><span data-stu-id="8629d-132">For this plug-in, you need to update the **Update of msdyn_quotelinetransaction** step.</span></span>
9. <span data-ttu-id="8629d-133">**PluginRegistrationTool** बंद करें.</span><span class="sxs-lookup"><span data-stu-id="8629d-133">Close **PluginRegistrationTool**.</span></span>
