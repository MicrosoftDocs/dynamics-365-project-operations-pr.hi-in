---
title: कोई संसाधन अनुरोध सबमिट करें
description: आप किसी संसाधन के लिए उत्पन्न आवश्यकता को संसाधन हेतु अनुरोध के रूप में सब्मिट कर सकते हैं। इसके बाद इस अनुरोध को पूर्ति के लिए किसी संसाधन प्रबंधक को भेजा जाता है।
author: ruhercul
manager: Annbe
ms.date: 10/04/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: ruhercul
ms.openlocfilehash: 94cf0f0d88e9be2522936b45122ed0037434d4f3
ms.sourcegitcommit: 2cf93d8bf0be5b61a739195a41334c34d910e9ba
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/05/2020
ms.locfileid: "3961712"
---
# <a name="submit-a-resource-request"></a><span data-ttu-id="e4c23-104">कोई संसाधन अनुरोध सबमिट करें</span><span class="sxs-lookup"><span data-stu-id="e4c23-104">Submit a resource request</span></span>

<span data-ttu-id="e4c23-105">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="e4c23-105">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="e4c23-106">आप किसी संसाधन के लिए उत्पन्न आवश्यकता को संसाधन हेतु अनुरोध के रूप में सब्मिट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="e4c23-106">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="e4c23-107">इसके बाद इस अनुरोध को पूर्ति के लिए किसी संसाधन प्रबंधक को भेजा जाता है।</span><span class="sxs-lookup"><span data-stu-id="e4c23-107">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="e4c23-108">Dynamics 365 Project Operations में, **प्रोजेक्ट** पृष्ठ पर, बुक करने-योग्य संसाधन सूची देखने के लिए **टीम** टैब पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="e4c23-108">In Dynamics 365 Project Operations, on the **Projects** page, select the **Team** tab to view a list of bookable resources.</span></span> 
2. <span data-ttu-id="e4c23-109">इस सूची से संसाधन की आवश्यकता वाले जेनेरिक संसाधन का चयन करें, और फिर **अनुरोध सब्मिट करें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="e4c23-109">Select the generic resource that has a resource requirement from the list, and then click **Submit Request**.</span></span>

<span data-ttu-id="e4c23-110">जेनेरिक टीम के सदस्य के अनुरोध की स्थिति परिवर्तित होकर **सब्मिटेड** हो जाएगी।</span><span class="sxs-lookup"><span data-stu-id="e4c23-110">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="e4c23-111">अनुरोध पूरा होने के बाद, यदि संसाधन प्रबंधक एक नामित संसाधन बुक करके अनुरोध को पूरा करता है तो सामान्य संसाधन को एक नामित संसाधन से बदल दिया जाता है।</span><span class="sxs-lookup"><span data-stu-id="e4c23-111">After the request is fulfilled, the generic resource is replaced by a named resource if the resource manager fulfills the request by booking a named resource.</span></span> <span data-ttu-id="e4c23-112">अन्यथा, यदि संसाधन प्रबंधक एक नामित संसाधन का प्रस्ताव करता है, तो जेनेरिक संसाधन टीम पर रहता है और अनुरोध स्थिति **समीक्षा की ज़रूरत है**में बदल जाएगी।</span><span class="sxs-lookup"><span data-stu-id="e4c23-112">Otherwise, if the resource manager proposes a named resource, the generic resource remains on the team and the request status will change to **Needs Review**.</span></span>
