---
title: Project Service Automation के अपडेट रिलीज़ 17, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 17, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
ms.topic: article
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
ms.openlocfilehash: 12df166e1bd1b5f0e11d79dc24122fb1ed7e6e6c
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5280805"
---
# <a name="project-service-automation-update-release-17-v3"></a><span data-ttu-id="e1e1a-103">Project Service Automation V3 अद्यतन रिलीज़ 17, V3</span><span class="sxs-lookup"><span data-stu-id="e1e1a-103">Project Service Automation Update Release 17, V3</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

<span data-ttu-id="e1e1a-104">हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है.</span><span class="sxs-lookup"><span data-stu-id="e1e1a-104">We’re pleased to announce the latest update for the Project Service Automation application for Dynamics 365.</span></span> <span data-ttu-id="e1e1a-105">इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="e1e1a-105">This release includes some important improvements to quality, performance, and usability.</span></span>  <span data-ttu-id="e1e1a-106">यह रिलीज़ Dynamics 365 9.x के साथ संगत में है.</span><span class="sxs-lookup"><span data-stu-id="e1e1a-106">This release is compatible with Dynamics 365 9.x.</span></span> <span data-ttu-id="e1e1a-107">इस रिलीज़ को अपडेट करने के लिए, Dynamics 365 online के लिए व्यवस्थापन केंद्र पर जाएँ और अपडेट को स्थापित करने के लिए समाधान पृष्ठ पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="e1e1a-107">To update to this release, visit the Admin Center for Dynamics 365 online, solutions page to install the update.</span></span> <span data-ttu-id="e1e1a-108">अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span><span class="sxs-lookup"><span data-stu-id="e1e1a-108">For more information, see [Install, update, or remove a preferred solution](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).</span></span>

<span data-ttu-id="e1e1a-109">यह टॉपिक PSA V3, अपडेट रिलीज़ 17 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है.</span><span class="sxs-lookup"><span data-stu-id="e1e1a-109">This topic lists the features and fixes that are new or changed for PSA V3, Update Release 17.</span></span> <span data-ttu-id="e1e1a-110">इस संस्करण की बिल्ड संख्या V3.10.6.34 है और यह आमतौर पर मार्च 2020 के स्वयं-अपडेट के माध्यम से उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="e1e1a-110">This version has a build number of V3.10.6.34 and is generally available through a self-update in March 2020.</span></span>


## <a name="update-release-17"></a><span data-ttu-id="e1e1a-111">अपडेट रिलीज़ 17</span><span class="sxs-lookup"><span data-stu-id="e1e1a-111">Update Release 17</span></span>

### <a name="bug-fixes"></a><span data-ttu-id="e1e1a-112">बग समाधान</span><span class="sxs-lookup"><span data-stu-id="e1e1a-112">Bug fixes</span></span>

<span data-ttu-id="e1e1a-113">**सामान्‍य**</span><span class="sxs-lookup"><span data-stu-id="e1e1a-113">**General**</span></span>

- <span data-ttu-id="e1e1a-114">निश्चित: टीम के सदस्य लाइसेंस लागू करने के लिए Project Service Automation अपडेट करें (Project Resource Hub में टीम के सदस्य सेवा प्लान मेटाडेटा 3.x शामिल होगा)</span><span class="sxs-lookup"><span data-stu-id="e1e1a-114">Fixed: Update Project Service Automation to enforce Team Member licenses (Project Resource Hub will include Team Member Service plan metadata 3.x)</span></span>
 
<span data-ttu-id="e1e1a-115">**समय और व्यय**</span><span class="sxs-lookup"><span data-stu-id="e1e1a-115">**Time and Expense**</span></span>

- <span data-ttu-id="e1e1a-116">निश्चित: गैर-शून्य मूल्य से शून्य (0) के लिए व्यय अनुमान बदलना संभव नहीं है.</span><span class="sxs-lookup"><span data-stu-id="e1e1a-116">Fixed: It is not possible to change an expense estimate from a non-zero price to zero (0).</span></span> <span data-ttu-id="e1e1a-117">बदलाव को नजरअंदाज किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="e1e1a-117">The change is ignored.</span></span>

<span data-ttu-id="e1e1a-118">**परियोजना प्रबंधन**</span><span class="sxs-lookup"><span data-stu-id="e1e1a-118">**Project Management**</span></span>

- <span data-ttu-id="e1e1a-119">निश्चित: टीम के सदस्य के पद नाम पर शून्य मानों के लिए एक चेक जोड़ा गया है.</span><span class="sxs-lookup"><span data-stu-id="e1e1a-119">Fixed: A check for null values has been added on a team member's position name.</span></span>
- <span data-ttu-id="e1e1a-120">निश्चित: **msdyn_resourceassignment** निकाय पर **msdyn_userresourceid** फ़ील्ड को रोका गया.</span><span class="sxs-lookup"><span data-stu-id="e1e1a-120">Fixed: **msdyn_userresourceid** field on the **msdyn_resourceassignment** entity has been deprecated.</span></span>
- <span data-ttu-id="e1e1a-121">निश्चित: 2.x से 3.x पर अपग्रेड करें अब कार्य असाइनमेंट पर रिक्त प्रयास आकृति को संभालता है.</span><span class="sxs-lookup"><span data-stu-id="e1e1a-121">Fixed: Upgrade from 2.x to 3.x now handles empty effort contours on task assignments.</span></span>

<span data-ttu-id="e1e1a-122">**Sales**</span><span class="sxs-lookup"><span data-stu-id="e1e1a-122">**Sales**</span></span>

- <span data-ttu-id="e1e1a-123">निश्चित: **Invoice.PreValidateInvoiceUpdate** अब रिकॉर्ड मालिकों को फिर से ठीक करने के परिदृश्य को संभालता है.</span><span class="sxs-lookup"><span data-stu-id="e1e1a-123">Fixed: **Invoice.PreValidateInvoiceUpdate** now handles the scenario of reassigning record owners properly.</span></span>
- <span data-ttu-id="e1e1a-124">निश्चित: जब लेन-देन वर्ग **समय**, **UnitGroup** सहित सभी प्रविष्टियों के लिए गैर-संपादन योग्य है, **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail**, और **ContractLineDetails**.</span><span class="sxs-lookup"><span data-stu-id="e1e1a-124">Fixed: When the transaction class is **Time**, **UnitGroup** is non-editable for all entities including, **QuoteLineDetails**, **JournalLine**, **InvoiceLineDetail**, and **ContractLineDetails**.</span></span> <span data-ttu-id="e1e1a-125">हालाँकि, **इकाई** केवल **JournalLine** और **InvoiceLineDetails** के लिए गैर-संपादन योग्य है.</span><span class="sxs-lookup"><span data-stu-id="e1e1a-125">However, **Unit** is non-editable only for **JournalLine** and **InvoiceLineDetails**.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]