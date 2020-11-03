---
title: नए मूल्य निर्धारण आयामों को शामिल करने के लिए प्लग-इन विशेषताओं को अपडेट करें
description: इस टॉपिक में प्राइस-निर्धारण आयामों के लिए प्लग-इन विशेषताओं को अपडेट करने के बारे में जानकारी प्रदान की गयी है।
author: Rumant
manager: kfend
ms.custom: ''
ms.date: 11/19/2018
ms.topic: article
ms.service: dynamics-365-customerservice
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: f215555dd7b29444e00499c0e731624e51057250
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077783"
---
# <a name="update-plug-in-attributes-to-include-new-pricing-dimensions"></a><span data-ttu-id="93460-103">नए मूल्य निर्धारण आयामों को शामिल करने के लिए प्लग-इन विशेषताओं को अपडेट करें</span><span class="sxs-lookup"><span data-stu-id="93460-103">Update plug-in attributes to include new pricing dimensions</span></span>

> [!NOTE]
> <span data-ttu-id="93460-104">यदि आप Project Service Automation (PSA) कोटिंग और कॉन्ट्रैक्टिंग सुविधाओं का उपयोग नहीं कर रहे हैं, तो आप यह टॉपिक छोड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="93460-104">If you are not using the Project Service Automation (PSA) Quoting and Contracting features, you can skip this topic.</span></span>

<span data-ttu-id="93460-105">इस टॉपिक में यह माना गया है कि आपने टॉपिक की प्रक्रियाएँ पूरी कर ली हैं [कस्टम फील्ड और इकाइयाँ बनाएँ](create-custom-fields-entities.md), [प्राइस सेटअप और लेनदेन वाली इकाइयों के लिए कस्टम फ़ील्ड शामिल करें](field-references.md), और [प्राइस निर्धारण आयामों को कस्टम फ़ील्ड के तौर पर सेट करें](set-up-pricing-dimensions.md)।</span><span class="sxs-lookup"><span data-stu-id="93460-105">This topic assumes that you have completed the procedures in the topics, [Create custom fields and entities](create-custom-fields-entities.md), [Add custom fields to price setup and transactional entities](field-references.md), and [Set up custom fields as pricing dimensions](set-up-pricing-dimensions.md).</span></span> <span data-ttu-id="93460-106">यदि आपने वे प्रक्रियाएं पूरी नहीं की हैं तो वापस जाकर उन्हें पूरा करें और फिर इस टॉपिक पर वापस लौटें।</span><span class="sxs-lookup"><span data-stu-id="93460-106">If you haven't completed those procedures, go back and complete them and then return to this topic.</span></span>

<span data-ttu-id="93460-107">जब किसी परियोजना क्वोट लाइन के लिए **क्वोट लाइन** पृष्ठ पर क्वोट लाइन विवरण बनाया जाता है तो बैकग्राउंड में सिस्टम अनुमान की दो लाइनें बनाता है - एक लाइन अनुमान के लागत पक्ष के लिए और एक लाइन बिक्री पक्ष के लिए।</span><span class="sxs-lookup"><span data-stu-id="93460-107">When a quote line detail is created on the **Quote Line** page for a project quote line, the system creates two estimate lines in the background -- one line for the cost side of the estimate and one for sales side.</span></span> <span data-ttu-id="93460-108">यही बात परियोजना कॉन्ट्रेक्ट लाइनों पर लागू होती है।</span><span class="sxs-lookup"><span data-stu-id="93460-108">This is the same  for project contract lines.</span></span>

<span data-ttu-id="93460-109">जब आप लागत पक्ष की मात्रा या फील्ड में परिवर्तन करते हैं तो यह परिवर्तन बिक्री पक्ष में भी पहुंच जाता है।</span><span class="sxs-lookup"><span data-stu-id="93460-109">When you make a change to the quantity or a field on the cost side, that change is propagated to the sales side.</span></span> <span data-ttu-id="93460-110">ऐसा निम्न प्लग-इन के कारण संभव हो पाता है, जिन्हें प्राइस निर्धारण आयामों में बदलाव के बाद री -रजिस्टर किया जाना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="93460-110">This is possible because of the following plug-ins that must be re-registered after a change to pricing dimensions.</span></span>

- <span data-ttu-id="93460-111">PreOperationContractLineDetailUpdate - Updates **msdyn_orderlinetransaction** ।</span><span class="sxs-lookup"><span data-stu-id="93460-111">PreOperationContractLineDetailUpdate - Updates **msdyn_orderlinetransaction**.</span></span>
- <span data-ttu-id="93460-112">PreOperationQuoteLineDetailUpdate - Updates **msdyn_quotelinetransaction** ।</span><span class="sxs-lookup"><span data-stu-id="93460-112">PreOperationQuoteLineDetailUpdate - Updates **msdyn_quotelinetransaction**.</span></span>

<span data-ttu-id="93460-113">निम्न चरणों में प्लग-इन को री- रजिस्टर करने की प्रक्रिया बताई गई है।</span><span class="sxs-lookup"><span data-stu-id="93460-113">The following steps walk you through the process of registering the plug-ins.</span></span>

1. <span data-ttu-id="93460-114">**PluginRegistrationTool** खोलें और अपने ऑनलाइन उदाहरण से कनेक्ट करें।</span><span class="sxs-lookup"><span data-stu-id="93460-114">Open the **PluginRegistrationTool** and connect to your online instance.</span></span>
2. <span data-ttu-id="93460-115">**खोजें** पर क्लिक करें और अपडेट किए जाने वाला प्लग-इन खोजें।</span><span class="sxs-lookup"><span data-stu-id="93460-115">Click **Search** and search for the plug-in to be updated.</span></span>

 ![खोज से जुड़े वृक्ष का स्क्रीनशॉट](media/PRT-1.png)

3. <span data-ttu-id="93460-117">प्लग-इन मिलने के बाद इसका चयन करें और फिर **मेन फ़ॉर्म का चयन करें** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="93460-117">After the plug-in is found, select it and then click **Select on Main Form**.</span></span>

4. <span data-ttu-id="93460-118">अपडेट किए जाने वाले प्लग-इन के चरण का चयन करें, राइट-क्लिक करें और फिर **अपडेट** का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="93460-118">Select the step of the plug-in to be updated, right-click, and then select **Update**.</span></span>

 ![प्लग-इन का स्क्रीनशॉट अपडेट किया जाना है](media/PRT-2.png)
 
5. <span data-ttu-id="93460-120">अपडेट विंडो में फ़िल्टरिंग विशेषताओं में एलिप्सिस ( **...** ) पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="93460-120">In the update window, click the ellipsis ( **...** ) in the filtering attributes.</span></span>

 ![मौजूदा चरण कॉन्फ़िगरेशन से जुड़ी जानकारी अपडेट करें का स्क्रीनशॉट](media/PRT-3.png)
 
6. <span data-ttu-id="93460-122">प्राइस निर्धारण विशेषता चेक बॉक्स का चयन करें।</span><span class="sxs-lookup"><span data-stu-id="93460-122">Select the pricing attribute check boxes.</span></span>

 ![प्राइस-निर्धारण विशेषताओं के लिए चेकबॉक्स का चयन दिखाता हुआ स्क्रीनशॉट](media/PRT-4.png)

7. <span data-ttu-id="93460-124">पृष्ठ को बंद करने के लिए **ओके** पर क्लिक करें और फिर **अपडेट का चरण** का चुनाव करें।</span><span class="sxs-lookup"><span data-stu-id="93460-124">Click **OK** to close the page and then select **Update Step**.</span></span>

 ![“अपडेट का चरण" बटन दिखाता हुआ स्क्रीनशॉट](media/PRT-5.png)
 
8. <span data-ttu-id="93460-126">इस प्रक्रिया को दूसरे प्लग-इन  **PreOperationQuoteLineDetail - Update of msdyn_quotelinetransaction** के लिए दोहराएं।</span><span class="sxs-lookup"><span data-stu-id="93460-126">Repeat this process for the second plug-in, **PreOperationQuoteLineDetail - Update of msdyn_quotelinetransaction**.</span></span>

9. <span data-ttu-id="93460-127">प्लग-इन रजिस्ट्रेशन टूल को बंद करें।</span><span class="sxs-lookup"><span data-stu-id="93460-127">Close the plug-in registration tool.</span></span>

