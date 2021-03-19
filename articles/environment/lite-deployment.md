---
title: Project Operations परिनियोजित करें - लाइट
description: यह विषय Project Operations लाइट नियोजन स्थापित करने के तरीके के बारे में जानकारी प्रदान करता है - प्रोफार्मा इuवॉयसिंग करने के लिए समझौता.
author: stsporen
manager: Annbe
ms.date: 10/02/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 0af8067fc0673890a317ac6f4e62d74b7f4eebca
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5290091"
---
# <a name="deploy-project-operations---lite"></a><span data-ttu-id="03507-103">Project Operations परिनियोजित करें - लाइट</span><span class="sxs-lookup"><span data-stu-id="03507-103">Deploy Project Operations - lite</span></span>

<span data-ttu-id="03507-104">_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_</span><span class="sxs-lookup"><span data-stu-id="03507-104">_**Applies To:** Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="03507-105">Project Operations कई नियोजन मॉडल का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="03507-105">Project Operations supports multiple deployment models.</span></span> <span data-ttu-id="03507-106">सबसे अच्छा नियोजन मॉडल निर्धारित करने के लिए, देखें [नियोजन के प्रकार](determine-deployment-type.md).</span><span class="sxs-lookup"><span data-stu-id="03507-106">To determine the best deployment model, see [Deployment types](determine-deployment-type.md).</span></span>


> [!IMPORTANT]
> <span data-ttu-id="03507-107">यह नियोजन, लाइट नियोजन - प्रोफार्मा इंवॉयसिंग करने के लिए समझौता, एक **Common Data Service Project Operations की नियोजन** में परिणाम है.</span><span class="sxs-lookup"><span data-stu-id="03507-107">This deployment, Lite deployment – deal to proforma invoicing, results in a **Common Data Service-only deployment of Project Operations**.</span></span>

- [<span data-ttu-id="03507-108">एक नए CDS परिवेश में Project Operations इंस्टॉल करें</span><span class="sxs-lookup"><span data-stu-id="03507-108">Install Project Operations into a new CDS environment</span></span>](#new)
- [<span data-ttu-id="03507-109">एक मौजूदा CDS परिवेश में इंस्टॉल करें</span><span class="sxs-lookup"><span data-stu-id="03507-109">Install into an existing CDS environment</span></span>](#existing)



## <a name="install-project-operations-to-a-new-cds-environment"></a><a name="new"></a><span data-ttu-id="03507-110">एक नए CDS परिवेश के लिए Project Operations इंस्टॉल करें</span><span class="sxs-lookup"><span data-stu-id="03507-110">Install Project Operations to a new CDS environment</span></span>

1. <span data-ttu-id="03507-111">एक Project Operations लाइसेंस के साथ [ग्लोबल या Power Platform एडमिनिस्ट्रेटर](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) के रूप में, [पावर प्लेटफॉर्म व्यवस्थापक केंद्रर](https://admin.powerplatform.com) में एक नया CDS परिवेश बनाएं .</span><span class="sxs-lookup"><span data-stu-id="03507-111">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, create a new CDS environment in the [PowerPlatform admin center](https://admin.powerplatform.com).</span></span> <span data-ttu-id="03507-112">सुनिश्चित करें कि **CDS डेटाबेस** और **Dynamics 365 अनुप्रयोग** सक्षम हैं.</span><span class="sxs-lookup"><span data-stu-id="03507-112">Make sure that **CDS database** and **Dynamics 365 Apps** are enabled.</span></span> <span data-ttu-id="03507-113">अधिक जानकारी के लिए, देखें [Power Platform एडमिन सेंटर में परिवेश बनाएं और प्रबंधित करें](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span><span class="sxs-lookup"><span data-stu-id="03507-113">For more information, see [Create and manage environments in the Power Platform admin center](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-in-the-power-platform-admin-center).</span></span>
2. <span data-ttu-id="03507-114">Dynamics 365 ऐप की परिनियोजन सूची से **Microsoft Dynamics 365 Project Operations** चुनें.</span><span class="sxs-lookup"><span data-stu-id="03507-114">Select **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span>


## <a name="install-project-operations-to-an-existing-cds-environment"></a><a name="existing"></a><span data-ttu-id="03507-115">एक मौजूदा CDS परिवेश में Project Operations इंस्टॉल करें</span><span class="sxs-lookup"><span data-stu-id="03507-115">Install Project Operations to an existing CDS environment</span></span>

1. <span data-ttu-id="03507-116">[ग्लोबल या Power Platform एडमिनिस्ट्रेटर](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) के रूप में एक Project Operations लाइसेंस के साथ, [पावर प्लेटफॉर्म व्यवस्थापक केंद्र](https://admin.powerplatform.com) में परिवेश का पता लगाएं, जहां आप Project Operations इंस्टॉल करना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="03507-116">As the [Global or Power Platform Administrator](https://docs.microsoft.com/power-platform/admin/global-service-administrators-can-administer-without-license) with a Project Operations license, locate the environment in the [PowerPlatform admin center](https://admin.powerplatform.com) where you want to install Project Operations.</span></span>
2. <span data-ttu-id="03507-117">Dynamics 365 ऐप की परिनियोजन सूची से **Microsoft Dynamics 365 Project Operations** स्थापित करें.</span><span class="sxs-lookup"><span data-stu-id="03507-117">Install **Microsoft Dynamics 365 Project Operations** from the deployment list of Dynamics 365 apps.</span></span> <span data-ttu-id="03507-118">अधिक जानकारी के लिए, [Dynamics 365 अनुप्रयोग प्रबंधित करें](https://docs.microsoft.com/power-platform/admin/manage-apps) देखें.</span><span class="sxs-lookup"><span data-stu-id="03507-118">For more information, see [Manage Dynamics 365 apps](https://docs.microsoft.com/power-platform/admin/manage-apps).</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]