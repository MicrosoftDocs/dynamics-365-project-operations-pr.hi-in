---
title: अपना परिनियोजन प्रकार निर्धारित करें
description: यह विषय आपकी कंपनी के लिए Project operations के उचित नियोजन के प्रकार को निर्धारित करने में आपकी मदद करने हेतु जानकारी प्रदान करता है.
author: stsporen
manager: Annbe
ms.date: 11/05/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: stsporen
ms.openlocfilehash: 2da6af3240d8e561d01b1fcd8d32b657dbac1588
ms.sourcegitcommit: 24528bb9c0ef8898077cb3bc672daa211c0e73aa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/04/2021
ms.locfileid: "5479566"
---
# <a name="determine-your-deployment-type"></a><span data-ttu-id="2b66c-103">अपना परिनियोजन प्रकार निर्धारित करें</span><span class="sxs-lookup"><span data-stu-id="2b66c-103">Determine your deployment type</span></span>

<span data-ttu-id="2b66c-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="2b66c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2b66c-105">लाइसेंस खरीदने के बाद, [निर्देशित स्थापना प्रवाह](https://aka.ms/provisionprojectoperations) का उपयोग करके Dynamics 365 Project Operations के सर्वश्रेष्ठ परिनियोजन मॉडल का निर्धारण करने के लिए यहाँ शुरू करें.</span><span class="sxs-lookup"><span data-stu-id="2b66c-105">After you purchase the license, start here to determine the best deployment model of Dynamics 365 Project Operations using the [Guided installation flow](https://aka.ms/provisionprojectoperations).</span></span>
> <span data-ttu-id="2b66c-106">निर्देशित इंस्टॉलेशन प्रवाह को पूरा करने के बाद, आपको अपनी इंस्टॉलेशन को पूरा करने के लिए उचित प्रबंधन पोर्टल पर निर्देशित किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="2b66c-106">After you have finshed the Guided installation flow, you will be directed to the correct management portal to complete your installation.</span></span> <span data-ttu-id="2b66c-107">इंस्टॉलेशन को पूरा करने के लिए नियोजन विवरण देखें.</span><span class="sxs-lookup"><span data-stu-id="2b66c-107">See the deployment details to complete the installation.</span></span>


## <a name="existing-customers-of-dynamics-using-dynamics-365-project-service-automation"></a><span data-ttu-id="2b66c-108">Dynamics 365 Project Service Automation उपयोग से Dynamics के मौजूदा ग्राहक</span><span class="sxs-lookup"><span data-stu-id="2b66c-108">Existing customers of Dynamics using Dynamics 365 Project Service Automation</span></span>
<span data-ttu-id="2b66c-109">Project Operations में Project Service Automation के साथ भेजी गई क्षमताएं शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="2b66c-109">Project Operations includes the capabilities that shipped with Project Service Automation.</span></span> <span data-ttu-id="2b66c-110">इन ग्राहकों के लिए 2021 रिलीज़ वेव 1 में एक अपग्रेड पथ जारी किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="2b66c-110">An upgrade path will be released for these customers in the 2021 release wave 1.</span></span>

## <a name="existing-customers-of-dynamics-365-finance-using-project-management-and-accounting"></a><span data-ttu-id="2b66c-111">परियोजना प्रबंधन और लेखांकन के उपयोग से Dynamics 365 Finance के मौजूदा ग्राहक</span><span class="sxs-lookup"><span data-stu-id="2b66c-111">Existing customers of Dynamics 365 Finance using Project management and accounting</span></span> 

<span data-ttu-id="2b66c-112">Finance के मौजूदा ग्राहक जो परियोजना प्रबंधन और लेखा कार्यक्षमता का उपयोग करते हैं, वे इसका, इसी तरह से उपयोग करना जारी रख सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="2b66c-112">Existing customers of Finance who use the Project management and accounting functionality can continue to use it as is.</span></span> <span data-ttu-id="2b66c-113">देखें [स्टॉक/उत्पादन आदेश परिदृश्यों के लिए Project Operations](#pma).</span><span class="sxs-lookup"><span data-stu-id="2b66c-113">See [Project Operations for stocked/production order scenarios](#pma).</span></span>


## <a name="deployment-regions"></a><span data-ttu-id="2b66c-114">परिनियोजन क्षेत्र</span><span class="sxs-lookup"><span data-stu-id="2b66c-114">Deployment regions</span></span>
<span data-ttu-id="2b66c-115">यह निर्धारित करने के लिए कि कौन से क्षेत्र Project Operations परिनियोजन का समर्थन करते हैं, देखें [Dynamics 365 के लिए भौगोलिक उपलब्धता और Power Platform रिपोर्ट](https://dynamics.microsoft.com/en-us/geographic-availability/).</span><span class="sxs-lookup"><span data-stu-id="2b66c-115">To determine which regions support Project Operations deployment, see [Geographical availability for Dynamics 365 and Power Platform report](https://dynamics.microsoft.com/en-us/geographic-availability/).</span></span> <span data-ttu-id="2b66c-116">**रिपोर्ट देखें** चुनें और समर्थित क्षेत्र देखने के लिए **Dynamics 365 > संचालन ऐप्स >Dynamics 365 Project Operations** का विस्तार करें.</span><span class="sxs-lookup"><span data-stu-id="2b66c-116">Select **View Report**, and expand **Dynamics 365 > Operations Apps > Dynamics 365 Project Operations** to view the supported regions.</span></span>

## <a name="deployment-types"></a><span data-ttu-id="2b66c-117">परिनियोजन प्रकार</span><span class="sxs-lookup"><span data-stu-id="2b66c-117">Deployment types</span></span>
<span data-ttu-id="2b66c-118">Project Operations आपकी आवश्यकताओं से मेल खाने के लिए कई नियोजन विकल्पों का समर्थन करता है.</span><span class="sxs-lookup"><span data-stu-id="2b66c-118">Project Operations supports multiple deployment options to match your requirements.</span></span> <span data-ttu-id="2b66c-119">चाहे आप एक नए या मौजूदा Dynamics 365 ग्राहक हों, Project Operations आपकी आवश्यकताओं का समर्थन कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="2b66c-119">Whether you're a new or existing Dynamics 365 customer, Project Operations can support your needs.</span></span>

<span data-ttu-id="2b66c-120">हमारी [नियोजन प्रश्नावली](https://aka.ms/provisionprojectoperations) आपको सही नियोजन निर्धारित करने में मदद करेगी.</span><span class="sxs-lookup"><span data-stu-id="2b66c-120">Our [Deployment questionnaire](https://aka.ms/provisionprojectoperations) will help you determine the right deployment.</span></span> <span data-ttu-id="2b66c-121">परिणाम आपको निम्नलिखित प्रतिनियुक्ति प्रकारों में से एक की ओर निर्देशित करेंगे:</span><span class="sxs-lookup"><span data-stu-id="2b66c-121">The results will guide you toward one of the following deployment types:</span></span>

- [<span data-ttu-id="2b66c-122">लाइट परिनियोजन – प्रोफ़ॉर्मा इनवॉइस करने के लिए डील</span><span class="sxs-lookup"><span data-stu-id="2b66c-122">Lite deployment – deal to proforma invoicing</span></span>](#lite)
- [<span data-ttu-id="2b66c-123">संसाधन/गैर-स्टॉक परिदृश्यों के लिए Project Operations</span><span class="sxs-lookup"><span data-stu-id="2b66c-123">Project Operations for resource/non-stocked scenarios</span></span>](#integrated)
- [<span data-ttu-id="2b66c-124">स्टॉक/उत्पादन ऑर्डर परिदृश्यों के लिए Project Operations</span><span class="sxs-lookup"><span data-stu-id="2b66c-124">Project Operations for stocked/production order scenarios</span></span>](#pma)

<span data-ttu-id="2b66c-125">Project Operations कानूनी निकाय-स्तर के कॉन्फ़िगरेशन के माध्यम से एक ही परिवेश पर स्टॉक/उत्पादन आदेश परिदृश्यों और गैर-स्टॉक/संसाधन-आधारित परिदृश्यों का समर्थन करते हैं.</span><span class="sxs-lookup"><span data-stu-id="2b66c-125">Project Operations support stocked/production order scenarios and non-stocked/resource-based scenarios on the same environment through legal entity-level configurations.</span></span> <span data-ttu-id="2b66c-126">उदाहरण के लिए, Contoso अपनी अमेरिकी विनिर्माण सुविधा (कानूनी निकाय = Contoso विनिर्माण संयुक्त राज्य अमेरिका) में स्टॉक/उत्पादन आदेश क्षमताओं का उपयोग कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="2b66c-126">For example, Contoso can use the stocked/production order capabilities in their US manufacturing facility (Legal entity = Contoso Manufacturing United States).</span></span> <span data-ttu-id="2b66c-127">Contoso यूनाइटेड किंगडम में अपने Contoso रोबोटिक्स आर्म्स सर्विसिंग सुविधा में गैर-स्टॉक/संसाधन-आधारित क्षमताओं का उपयोग कर सकता है (कानूनी निकाय = Contoso रोबोटिक्स यूनाइटेड किंगडम).</span><span class="sxs-lookup"><span data-stu-id="2b66c-127">Contoso can use the non-stocked/resource-based capabilities in their Contoso Robotics Arms servicing facility in UK (Legal entity = Contoso Robotics United Kingdom).</span></span>

### <a name="lite-deployment---deal-to-proforma-invoicing"></a><a  name="lite"></a><span data-ttu-id="2b66c-128">लाइट परिनियोजन - प्रोफ़ॉर्मा इनवॉइस करने के लिए डील</span><span class="sxs-lookup"><span data-stu-id="2b66c-128">Lite deployment - deal to proforma invoicing</span></span>

<span data-ttu-id="2b66c-129">मामूली प्रतिनियुक्ति में निम्नलिखित क्षमताएं शामिल हैं:</span><span class="sxs-lookup"><span data-stu-id="2b66c-129">The lite deployment includes the following capabilities:</span></span>

- <span data-ttu-id="2b66c-130">Dynamics 365 Sales एप्लिकेशन अनुभवों का विस्तार करने वाली परियोजनाओं के लिए विक्रय प्रक्रिया</span><span class="sxs-lookup"><span data-stu-id="2b66c-130">Sales process for projects that extends Dynamics 365 Sales application experiences</span></span>
- <span data-ttu-id="2b66c-131">वेब के लिए Microsoft Project का उपयोग करके परियोजना की योजना</span><span class="sxs-lookup"><span data-stu-id="2b66c-131">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="2b66c-132">बहु-आयामी मूल्य निर्धारण</span><span class="sxs-lookup"><span data-stu-id="2b66c-132">Multi-dimensional pricing</span></span>
- <span data-ttu-id="2b66c-133">एकीकृत संसाधन प्रबंधन</span><span class="sxs-lookup"><span data-stu-id="2b66c-133">Unified resource management</span></span>
- <span data-ttu-id="2b66c-134">समय ट्रैकिंग</span><span class="sxs-lookup"><span data-stu-id="2b66c-134">Time tracking</span></span>
- <span data-ttu-id="2b66c-135">मूल व्यय</span><span class="sxs-lookup"><span data-stu-id="2b66c-135">Basic expense</span></span>
- <span data-ttu-id="2b66c-136">प्रोफ़ॉर्मा और ग्राहक-फोसिंग इनवॉयसिंग</span><span class="sxs-lookup"><span data-stu-id="2b66c-136">Proforma and customer-facing invoicing</span></span> 

#### <a name="deployment-steps"></a><span data-ttu-id="2b66c-137">परिनियोजन चरण</span><span class="sxs-lookup"><span data-stu-id="2b66c-137">Deployment steps</span></span>
<span data-ttu-id="2b66c-138">[प्रतिनियुक्ति प्रश्नावली](https://aka.ms/provisionprojectoperations) का उपयोग करके Project Operations का सबसे अच्छा नियोजन मॉडल निर्धारित करें.</span><span class="sxs-lookup"><span data-stu-id="2b66c-138">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="2b66c-139">इस नियोजन के लिए, देखें [पूर्वावलोकन सदस्यता के लिए साइन-अप करें](lite-preview-subscription-sign-up.md) और [नए परिवेश का प्रावधान](lite-deployment.md).</span><span class="sxs-lookup"><span data-stu-id="2b66c-139">For this deployment, see [Sign-up for preview subscriptions](lite-preview-subscription-sign-up.md) and [Provision new environment](lite-deployment.md).</span></span> 


### <a name="project-operations-for-resourcenon-stocked-scenarios"></a><a name="integrated"></a><span data-ttu-id="2b66c-140">संसाधन/गैर-स्टॉक परिदृश्यों के लिए Project Operations</span><span class="sxs-lookup"><span data-stu-id="2b66c-140">Project Operations for resource/non-stocked scenarios</span></span>
<span data-ttu-id="2b66c-141">संसाधन/गैर-स्टॉक किए गए परिदृश्यों के लिए Project Operations में निम्नलिखित क्षमताएं शामिल हैं:</span><span class="sxs-lookup"><span data-stu-id="2b66c-141">The Project Operations for resource/non-stocked scenarios includes the following capabilities:</span></span>
 
- <span data-ttu-id="2b66c-142">Dynamics 365 Sales एप्लिकेशन का विस्तार करने वाली परियोजनाओं के लिए विक्रय प्रक्रिया</span><span class="sxs-lookup"><span data-stu-id="2b66c-142">Sales process for projects that extends the Dynamics 365 Sales application</span></span>
- <span data-ttu-id="2b66c-143">वेब के लिए Microsoft Project का उपयोग करके परियोजना की योजना</span><span class="sxs-lookup"><span data-stu-id="2b66c-143">Project planning using Microsoft Project for the Web</span></span>
- <span data-ttu-id="2b66c-144">बहु-आयामी मूल्य निर्धारण</span><span class="sxs-lookup"><span data-stu-id="2b66c-144">Multi-dimensional pricing</span></span>
- <span data-ttu-id="2b66c-145">एकीकृत संसाधन प्रबंधन</span><span class="sxs-lookup"><span data-stu-id="2b66c-145">Unified resource management</span></span>
- <span data-ttu-id="2b66c-146">समय ट्रैकिंग</span><span class="sxs-lookup"><span data-stu-id="2b66c-146">Time tracking</span></span>
- <span data-ttu-id="2b66c-147">मूल व्यय</span><span class="sxs-lookup"><span data-stu-id="2b66c-147">Basic expense</span></span>
- <span data-ttu-id="2b66c-148">पूरा व्यय</span><span class="sxs-lookup"><span data-stu-id="2b66c-148">Full expense</span></span>
- <span data-ttu-id="2b66c-149">OCR रसीद</span><span class="sxs-lookup"><span data-stu-id="2b66c-149">Receipt OCR</span></span>
- <span data-ttu-id="2b66c-150">प्रोफ़ॉर्मा और ग्राहक-फोसिंग इनवॉयसिंग</span><span class="sxs-lookup"><span data-stu-id="2b66c-150">Proforma and customer-facing invoicing</span></span> 
- <span data-ttu-id="2b66c-151">परियोजनाओं के लिए राजस्व मान्यता</span><span class="sxs-lookup"><span data-stu-id="2b66c-151">Revenue recognition for projects</span></span>

#### <a name="deployment-steps"></a><span data-ttu-id="2b66c-152">परिनियोजन चरण</span><span class="sxs-lookup"><span data-stu-id="2b66c-152">Deployment steps</span></span>
<span data-ttu-id="2b66c-153">[प्रतिनियुक्ति प्रश्नावली](https://aka.ms/provisionprojectoperations) का उपयोग करके Project Operations का सबसे अच्छा नियोजन मॉडल निर्धारित करें.</span><span class="sxs-lookup"><span data-stu-id="2b66c-153">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="2b66c-154">इस नियोजन के लिए, देखें [पूर्वावलोकन सदस्यता के लिए साइन-अप करें](resource-sign-up-preview-subscription.md) और [नए परिवेश का प्रावधान](resource-provision-new-environment.md).</span><span class="sxs-lookup"><span data-stu-id="2b66c-154">For this deployment, see [Sign-up for preview subscriptions](resource-sign-up-preview-subscription.md) and [Provision new environment](resource-provision-new-environment.md).</span></span> 


### <a name="project-operations-for-stockedproduction-order-scenarios"></a><a name="pma"></a><span data-ttu-id="2b66c-155">स्टॉक/उत्पादन ऑर्डर परिदृश्यों के लिए Project Operations</span><span class="sxs-lookup"><span data-stu-id="2b66c-155">Project Operations for stocked/production order scenarios</span></span>

- <span data-ttu-id="2b66c-156">WBS का उपयोग कर परियोजना की योजना बनाना</span><span class="sxs-lookup"><span data-stu-id="2b66c-156">Project planning using WBS</span></span>
- <span data-ttu-id="2b66c-157">संसाधन प्रबंधन</span><span class="sxs-lookup"><span data-stu-id="2b66c-157">Resource Management</span></span>
- <span data-ttu-id="2b66c-158">समय ट्रैकिंग</span><span class="sxs-lookup"><span data-stu-id="2b66c-158">Time Tracking</span></span>
- <span data-ttu-id="2b66c-159">पूरा व्यय</span><span class="sxs-lookup"><span data-stu-id="2b66c-159">Full Expense</span></span>
- <span data-ttu-id="2b66c-160">OCR रसीद</span><span class="sxs-lookup"><span data-stu-id="2b66c-160">Receipt OCR</span></span>
- <span data-ttu-id="2b66c-161">पूर्ण इनवॉइस करना</span><span class="sxs-lookup"><span data-stu-id="2b66c-161">Full Invoicing</span></span>
- <span data-ttu-id="2b66c-162">आमदनी मान्यता</span><span class="sxs-lookup"><span data-stu-id="2b66c-162">Revenue Recognition</span></span>
- <span data-ttu-id="2b66c-163">उत्पादन आदेश</span><span class="sxs-lookup"><span data-stu-id="2b66c-163">Production Orders</span></span>
- <span data-ttu-id="2b66c-164">सामग्री समर्थन</span><span class="sxs-lookup"><span data-stu-id="2b66c-164">Materials support</span></span>

#### <a name="deployment-steps"></a><span data-ttu-id="2b66c-165">परिनियोजन चरण</span><span class="sxs-lookup"><span data-stu-id="2b66c-165">Deployment steps</span></span>
<span data-ttu-id="2b66c-166">[प्रतिनियुक्ति प्रश्नावली](https://aka.ms/provisionprojectoperations) का उपयोग करके Project Operations का सबसे अच्छा नियोजन मॉडल निर्धारित करें.</span><span class="sxs-lookup"><span data-stu-id="2b66c-166">Determine the best deployment model of Project Operations using the [Deployment questionnaire](https://aka.ms/provisionprojectoperations).</span></span>

<span data-ttu-id="2b66c-167">इस नियोजन के लिए, देखें [पूर्वावलोकन सदस्यता के लिए साइन-अप करें](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) और [नए परिवेश का प्रावधान](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json).</span><span class="sxs-lookup"><span data-stu-id="2b66c-167">For this deployment, see [Sign-up for preview subscriptions](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/dev-tools/sign-up-preview-subscription?toc=/dynamics365/finance/toc.json) and [Provision new environment](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment?toc=/dynamics365/finance/toc.json).</span></span> 



[!INCLUDE[footer-include](../includes/footer-banner.md)]
