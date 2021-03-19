---
title: संसाधन हेतु अनुरोध सबमिट करना
description: इस टॉपिक में किसी परियोजना हेतु संसाधन के लिए अनुरोध सब्मिट करने के बारे में जानकारी प्रदान की गई है।
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 12/1/2018
ms.topic: article
author: JohnPBurrows
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 8976ca2360be8676350178059615c59995544a71
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5282245"
---
# <a name="submitting-a-resource-request"></a><span data-ttu-id="a180b-103">संसाधन हेतु अनुरोध सबमिट करना</span><span class="sxs-lookup"><span data-stu-id="a180b-103">Submitting a resource request</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="a180b-104">आप किसी संसाधन के लिए उत्पन्न आवश्यकता को संसाधन हेतु अनुरोध के रूप में सब्मिट कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="a180b-104">You can submit a generated resource requirement as a resource request.</span></span> <span data-ttu-id="a180b-105">इसके बाद इस अनुरोध को पूर्ति के लिए किसी संसाधन प्रबंधक को भेजा जाता है।</span><span class="sxs-lookup"><span data-stu-id="a180b-105">The request is then sent to a resource manager for fulfillment.</span></span>

1. <span data-ttu-id="a180b-106">Project Service Automation (PSA) में **प्रोजेक्ट** पृष्ठ पर बुक करने-योग्य संसाधन देखने के लिए **टीम** टैब पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="a180b-106">In Project Service Automation (PSA), on the **Projects** page, click the **Team** tab to view a list bookable resources.</span></span> 
2. <span data-ttu-id="a180b-107">इस सूची से संसाधन की आवश्यकता वाले जेनेरिक संसाधन का चयन करें और फिर **अनुरोध सब्मिट करें** पर क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="a180b-107">Select the generic resource that has a resource requirement from the list and then click **Submit Request**.</span></span>

![संसाधन हेतु अनुरोध सबमिट करना](media/RM-how-to-18.png)

<span data-ttu-id="a180b-109">जेनेरिक टीम के सदस्य के अनुरोध की स्थिति परिवर्तित होकर **सब्मिटेड** हो जाएगी।</span><span class="sxs-lookup"><span data-stu-id="a180b-109">The request status of the generic team member will change to **Submitted**.</span></span>

<span data-ttu-id="a180b-110">यदि संसाधन प्रबंधक किसी नामित संसाधन की बुकिंग कर अनुरोध की पूर्ति करता है तो संसाधन प्रबंधक द्वारा अनुरोध की पूर्ति किए जाने के बाद जेनेरिक संसाधन को बदल कर नामित संसाधन रखा जाएगा।</span><span class="sxs-lookup"><span data-stu-id="a180b-110">After the request is fulfilled by the resource manager, the generic resource will be replaced by a named resource if the resource manager fulfills the request with the booking of a named resource.</span></span> <span data-ttu-id="a180b-111">अन्यथा जेनेरिक संसाधन टीम में ही रहेगा और यदि संसाधन प्रबंधक ने किसी नामित संसाधन का प्रस्ताव दिया है तो अनुरोध की स्थिति परिवर्तित होकर **समीक्षा वांछित है** हो जाएगी।</span><span class="sxs-lookup"><span data-stu-id="a180b-111">Otherwise, the generic resource will remain on the team and the request status will change to **Needs Review**, if the resource manager has proposed a named resource.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]