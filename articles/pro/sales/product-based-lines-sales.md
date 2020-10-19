---
title: उत्पाद-आधारित अवसर पंक्तियाँ
description: यह विषय Project Operations में उत्पाद आधारित अवसर लाइन आइटम के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 17ffcf8dc94d42102115281d281d6b553cf1fa17
ms.sourcegitcommit: a2c3cd49a3b667b8b5edaa31788b4b9b1f728d78
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/28/2020
ms.locfileid: "3896238"
---
# <a name="product-based-opportunity-lines"></a><span data-ttu-id="c83a9-103">उत्पाद-आधारित अवसर पंक्तियाँ</span><span class="sxs-lookup"><span data-stu-id="c83a9-103">Product-based opportunity lines</span></span>

<span data-ttu-id="c83a9-104">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="c83a9-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="c83a9-105">उत्पाद आधारित अवसर लाइनें, अवसर पर लाइन आइटम हैं.</span><span class="sxs-lookup"><span data-stu-id="c83a9-105">Product-based opportunity lines are line items on the Opportunity.</span></span> <span data-ttu-id="c83a9-106">ये लाइनें ग्राहक को किसी अन्य मूल्य-वर्धित सेवाओं के बिना अंतिम इनवॉइस पर अलग लाइन आइटमों के रूप में डिलीवर की जाती हैं.</span><span class="sxs-lookup"><span data-stu-id="c83a9-106">These lines are delivered to the customer as distinct line items on the eventual invoice without any other value-added services.</span></span> <span data-ttu-id="c83a9-107">संबद्ध ख़र्च और खपत किसी भी संबंधित परियोजनाओं के कार्यों पर ट्रैक नहीं होता है.</span><span class="sxs-lookup"><span data-stu-id="c83a9-107">The associated spend and consumption isn't tracked on tasks of any related projects.</span></span>

<span data-ttu-id="c83a9-108">उत्पाद-आधारित लाइनें, कैटलॉग आइटम या राइट-इन उत्पाद हो सकती हैं.</span><span class="sxs-lookup"><span data-stu-id="c83a9-108">Product-based lines can be catalog items or write-in products.</span></span> <span data-ttu-id="c83a9-109">अवसर के उत्पाद-आधारित लाइनों पर अधिकांश कार्यक्षमता Dynamics 365 Sales एप्लिकेशन द्वारा प्रदान की गई कार्यक्षमता का पालन करती है.</span><span class="sxs-lookup"><span data-stu-id="c83a9-109">Most of the functionality on an Opportunity's product-based lines follows the functionality provided by the Dynamics 365 Sales application.</span></span> <span data-ttu-id="c83a9-110">उत्पाद-आधारित अवसर लाइनों के बारे में अधिक जानकारी के लिए, देखें [एक अवसर के लिए उत्पादों को जोड़ें](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span><span class="sxs-lookup"><span data-stu-id="c83a9-110">For more information about product-based opportunity lines, see [Add products to an opportunity](https://docs.microsoft.com/dynamics365/sales-enterprise/add-products-opportunity).</span></span>

<span data-ttu-id="c83a9-111">**ग्राहक बजट** उत्पाद-आधारित अवसर लाइनों के बारे में एक अवधारणा है जो परियोजना-आधारित अवसरों के लिए विशिष्ट है.</span><span class="sxs-lookup"><span data-stu-id="c83a9-111">One concept about product-based opportunity lines that is specific to project-based opportunities is **Customer Budget**.</span></span> <span data-ttu-id="c83a9-112">इस फ़ील्ड का उपयोग उस राशि को ट्रैक करने के लिए करें जो ग्राहक लाइन आइटम के लिए भुगतान करने को तैयार है.</span><span class="sxs-lookup"><span data-stu-id="c83a9-112">Use this field to track the amount the customer is willing to pay for the line item.</span></span>

<span data-ttu-id="c83a9-113">यदि अवसर सारांश की राजस्व विधि **सिस्टम द्वारा गणना** के लिए सेट है, तो अनुमानित राजस्व की गणना करने के लिए उत्पाद-आधारित और परियोजना-आधारित लाइनों में ग्राहक बजट मूल्यों को संक्षेप में प्रस्तुत किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="c83a9-113">If the revenue method of the Opportunity summary is set to **System Calculated**, the customer budget values across product- and project-based lines are summarized to calculate the estimated revenue.</span></span>
