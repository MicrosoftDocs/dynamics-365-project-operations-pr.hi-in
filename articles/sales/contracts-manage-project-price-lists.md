---
title: परियोजना अनुबंधों पर परियोजना मूल्य सूचियाँ प्रबंधित करें
description: यह विषय परियोजना अनुबंधों पर परियोजना मूल्य सूचियाँ प्रबंधित करने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/27/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: 2cfac6eda64d1d8e578115bba07942a7d786328f
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5278600"
---
# <a name="manage-project-price-lists-on-project-contracts"></a><span data-ttu-id="1ca88-103">परियोजना अनुबंधों पर परियोजना मूल्य सूचियाँ प्रबंधित करें</span><span class="sxs-lookup"><span data-stu-id="1ca88-103">Manage project price lists on project contracts</span></span>

<span data-ttu-id="1ca88-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="1ca88-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1ca88-105">Dynamics 365 Project Operations में परियोजना अनुबंध किसी अनुबंध पर कई दिनांक प्रभावी विक्रय मूल्य सूचियों का समर्थन करने के लिए डिज़ाइन किया गया है.</span><span class="sxs-lookup"><span data-stu-id="1ca88-105">Project contracts in Dynamics 365 Project Operations are designed to support multiple date effective sales price lists on a contract.</span></span> <span data-ttu-id="1ca88-106">Project Operations में, **परियोजना मूल्य सूचियाँ** नामक एक नया संबद्ध निकाय मौजूद है.</span><span class="sxs-lookup"><span data-stu-id="1ca88-106">In Project Operations, there is a new associated entity called **Project Price Lists**.</span></span> <span data-ttu-id="1ca88-107">इस निकाय का परियोजना अनुबंध के साथ वन-टू-मैनी संबंध है.</span><span class="sxs-lookup"><span data-stu-id="1ca88-107">This entity has a one-to-many relationship to a project contract.</span></span>

<span data-ttu-id="1ca88-108">परियोजना मूल्य सूचियों का उपयोग किसी परियोजना पर समय और ख़र्च की लेनदेन की कीमत लगाने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="1ca88-108">Project price lists are used to price time and expense transactions on a project.</span></span> <span data-ttu-id="1ca88-109">जब किसी अनुबंध में एक या अधिक परियोजना मूल्य सूचियाँ होती हैं, तो इन मूल्य सूचियों का उपयोग समय और व्यय अनुमानों और उन परियोजनाओं पर वास्तविक का मूल्यांकन करने के लिए किया जाता है, जो अनुबंध पंक्ति के माध्यम से अनुबंध से संबद्ध हैं.</span><span class="sxs-lookup"><span data-stu-id="1ca88-109">When a contract has one or more project price lists, these price lists are used to price for time and expense estimates and actuals on projects that are associated to the contract through the contract line.</span></span>

<span data-ttu-id="1ca88-110">जब किसी परियोजना अनुबंध पर कोई परियोजना मूल्य सूची नहीं होती है, तो आपको एक चेतावनी संदेश दिखाई देगा कि परियोजना मूल्य सूचियाँ नहीं है और आपके अनुमानों, वास्तविक परियोजना कार्य और व्ययों का मूल्यांकन नहीं किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="1ca88-110">When there are no project price lists on a project contract, you will see a warning message that there are no project price lists and your estimates, actual project work, and expenses will not be priced.</span></span> <span data-ttu-id="1ca88-111">विक्रय मानों के लिए कोई मूल्य नहीं होगा.</span><span class="sxs-lookup"><span data-stu-id="1ca88-111">There will be no price for sales values.</span></span>

## <a name="associate-or-unassociate-a-project-price-list-on-a-project-contract"></a><span data-ttu-id="1ca88-112">परियोजना अनुबंध से परियोजना मूल्य सूची संबद्ध करें या असंबद्ध करें</span><span class="sxs-lookup"><span data-stu-id="1ca88-112">Associate or unassociate a project price list on a project contract</span></span>

### <a name="create-or-associate-a-specific-price-list-for-estimating-project-based-work-and-expenses"></a><span data-ttu-id="1ca88-113">परियोजना-आधारित कार्य और व्ययों के आकलन के लिए एक विशिष्ट मूल्य सूची बनाएं या संबद्ध करें</span><span class="sxs-lookup"><span data-stu-id="1ca88-113">Create or associate a specific price list for estimating project-based work and expenses</span></span>

1. <span data-ttu-id="1ca88-114">परियोजना अनुबंध पर, **परियोजना मूल्य सूचियाँ** टैब चुनें.</span><span class="sxs-lookup"><span data-stu-id="1ca88-114">On the project contract, select the **Project Price Lists** tab.</span></span>
2. <span data-ttu-id="1ca88-115">सबग्रिड में, **+ नई परियोजना मूल्य सूची जोड़ें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="1ca88-115">In the subgrid, select **+ Add New Project Price List**.</span></span>
3. <span data-ttu-id="1ca88-116">**त्वरित बनाएँ** स्लाइडर पर, एक मूल्य सूची चुनें.</span><span class="sxs-lookup"><span data-stu-id="1ca88-116">On the **Quick Create** slider, select a price list.</span></span> 

  <span data-ttu-id="1ca88-117">ड्रॉप-डाउन सूची उन सभी मूल्य सूचियों को दिखाती है, जिनका संदर्भ **विक्रय** पर सेट है, जहां मूल्य सूची की मुद्रा अनुबंध की मुद्रा से मेल खाती है.</span><span class="sxs-lookup"><span data-stu-id="1ca88-117">The drop-down list shows all price lists that have the context set to **Sales**, where the currency on the price list matches the currency on the contract.</span></span>
  
4. <span data-ttu-id="1ca88-118">परियोजना मूल्य सूची संबद्धता के लिए एक विवरण दर्ज करें, **सहेजें** चुनें और उसके बाद **त्वरित बनाएँ** स्लाइडर बंद करें.</span><span class="sxs-lookup"><span data-stu-id="1ca88-118">Enter a description for the project price list association, select **Save**, and then close the **Quick Create** slider.</span></span>

   <span data-ttu-id="1ca88-119">एक परियोजना मूल्य सूची संबंद्ध बनाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="1ca88-119">A project price list association is created.</span></span>
   
5. <span data-ttu-id="1ca88-120">परियोजना अनुबंध से एक से अधिक परियोजना मूल्य सूची संबद्ध करने के लिए चरण 1-4 दोहराएँ.</span><span class="sxs-lookup"><span data-stu-id="1ca88-120">Repeat steps 1-4 to associate more than one project price list to the project contract.</span></span> <span data-ttu-id="1ca88-121">यदि प्रत्येक संबद्ध परियोजना मूल्य सूची पर आपके पास भिन्न दिनांक प्रभाविकता है, तो केवल एकाधिक परियोजना मूल्य सूचियाँ बनाएँ.</span><span class="sxs-lookup"><span data-stu-id="1ca88-121">Only create multiple project price lists if you have different date effectivity on each of the associated project price list.</span></span>

> [!NOTE]
> <span data-ttu-id="1ca88-122">Project Operations परियोजना मूल्य सूचियों की दिनांक प्रभावकारिता को ओवरलैप करने का समर्थन नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="1ca88-122">Project Operations doesn't support overlapping the date effectivity of the project price lists.</span></span> <span data-ttu-id="1ca88-123">यदि किसी दिए गए दिनांक वाले ट्रांज़ैक्शन के लिए कई परियोजना मूल्य सूचियाँ हैं, तो उस ट्रांज़ैक्शन का मूल्य डिफ़ॉल्ट रूप से शून्य होगा.</span><span class="sxs-lookup"><span data-stu-id="1ca88-123">If there are multiple project prices lists for a transaction with a given date, the price on that transaction will be defaulted to zero.</span></span>

### <a name="remove-a-project-price-list-association"></a><span data-ttu-id="1ca88-124">परियोजना मूल्य सूची संबद्धता निकालें</span><span class="sxs-lookup"><span data-stu-id="1ca88-124">Remove a project price list association</span></span>

- <span data-ttu-id="1ca88-125">परियोजना मूल्य सूची चुनें और उसके बाद सबग्रिड पर **अनुबंध परियोजना मूल्य सूची हटाएं** चुनें.</span><span class="sxs-lookup"><span data-stu-id="1ca88-125">Select the project price list, and then select **Delete Contract Project Price List** on the subgrid.</span></span> 

  <span data-ttu-id="1ca88-126">मूल्य सूची को अनुबंध की परियोजना मूल्य सूचियों से हटा दिया जाता है.</span><span class="sxs-lookup"><span data-stu-id="1ca88-126">The price list is removed from the project price lists on the contract.</span></span> <span data-ttu-id="1ca88-127">मूल्य सूची स्वयं नहीं हटाई जाएगी.</span><span class="sxs-lookup"><span data-stu-id="1ca88-127">The price list itself will not be deleted.</span></span> <span data-ttu-id="1ca88-128">केवल अनुबंध की संबद्धता को हटा दिया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="1ca88-128">Only the association to the contract will be deleted.</span></span>

## <a name="set-up-automatic-defaulting-of-project-price-lists-on-a-contract"></a><span data-ttu-id="1ca88-129">अनुबंध पर परियोजना मूल्य सूचियों की स्वचालित डिफ़ॉल्टिंग सेट अप करें</span><span class="sxs-lookup"><span data-stu-id="1ca88-129">Set up automatic defaulting of project price lists on a contract</span></span>

<span data-ttu-id="1ca88-130">परियोजना मूल्य सूची को परियोजना अनुबंध पर डिफ़ॉल्ट सूची के रूप में स्थापित किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="1ca88-130">A project price list can be set up as the default list on a project contract.</span></span> <span data-ttu-id="1ca88-131">यह सेटअप यह सुनिश्चित करने में मदद कर सकता है कि आपके संगठन के सभी अनुबंध हमेशा उस मूल्य अवधि के लिए एक मानक मूल्य सूची के साथ शुरू होते हैं.</span><span class="sxs-lookup"><span data-stu-id="1ca88-131">This setup can help ensure that all contracts in your organization always start with a standard price list for that price period.</span></span>

### <a name="set-up-the-organizational-default-for-project-price-lists"></a><span data-ttu-id="1ca88-132">परियोजना मूल्य सूचियों के लिए संगठनात्मक डिफ़ॉल्ट सेट अप करें</span><span class="sxs-lookup"><span data-stu-id="1ca88-132">Set up the organizational default for project price lists</span></span>

1. <span data-ttu-id="1ca88-133">**सेटिंग** > **सामान्य** पर जाएँ और उसके बाद **पैरामीटर** चुनें.</span><span class="sxs-lookup"><span data-stu-id="1ca88-133">Go to **Settings** > **General**, and then select **Parameters**.</span></span>
2. <span data-ttu-id="1ca88-134">**सक्रिय पैरामीटर** सूची पृष्ठ में, रिकॉर्ड को खोलने के लिए उसे चुनें और उस पर डबल-क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="1ca88-134">In the **Active Parameters** list page, select and double-click the record to open it.</span></span> <span data-ttu-id="1ca88-135">डबल-क्लिक करते समय, सुनिश्चित करें कि आप हाइपरलिंक वाले फ़ील्ड मान पर क्लिक नहीं कर रहे हैं.</span><span class="sxs-lookup"><span data-stu-id="1ca88-135">While double–clicking, make sure that you are not clicking on a field value that is hyperlink.</span></span> 
3. <span data-ttu-id="1ca88-136">**सक्रिय पैरामीटर** पृष्ठ पर, **मूल्य सूची** टैब चुनें. सबग्रिड डिफ़ॉल्ट मूल्य सूचियों की एक सूची दिखाती है.</span><span class="sxs-lookup"><span data-stu-id="1ca88-136">On the **Active Parameters** page, select the **Price List** tab. A subgrid shows a list of default price lists.</span></span> <span data-ttu-id="1ca88-137">यह मानक लागत और विक्रय मूल्य सूचियों की एक सूची है.</span><span class="sxs-lookup"><span data-stu-id="1ca88-137">This is a list of standard cost and sales price lists.</span></span> <span data-ttu-id="1ca88-138">उस प्रत्येक मुद्रा के लिए जिसमें आप समान बेचते हैं यहाँ एक **विक्रय** मूल्य सूची संबद्ध होना सुनिश्चित करता है कि विक्रय मूल्य सूची उस किसी भी अनुबंध के लिए डिफ़ॉल्ट है, जो आप उन ग्राहकों के लिए बनाते हैं, जो इस मुद्रा में लेनदेन करते हैं.</span><span class="sxs-lookup"><span data-stu-id="1ca88-138">Having a **Sales** price list associated here for every currency that you sell in ensures that the sales price list is the default on any contract that you create for customers that transact in this currency.</span></span>

### <a name="set-up-a-customer-specific-project-price-list"></a><span data-ttu-id="1ca88-139">ग्राहक-विशिष्ट परियोजना मूल्य सूची सेट अप करें</span><span class="sxs-lookup"><span data-stu-id="1ca88-139">Set up a customer-specific project price list</span></span>

<span data-ttu-id="1ca88-140">जब अपने ग्राहकों के साथ मास्टर मूल्य निर्धारण समझौते पर बातचीत की होती है, तो आप ग्राहक-विशिष्ट परियोजना मूल्य सूचियाँ भी सेट अप कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="1ca88-140">You can also set up customer–specific project price lists when you have negotiated a master pricing agreement with your customers.</span></span>

1. <span data-ttu-id="1ca88-141">**विक्रय** > **ग्राहक** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="1ca88-141">Go to **Sales** > **Customers**.</span></span>
2. <span data-ttu-id="1ca88-142">सक्रिय खातों की सूची से, वह ग्राहक चुनें, जिसके लिए आपके पास विशेष मूल्य सूची है.</span><span class="sxs-lookup"><span data-stu-id="1ca88-142">From the list of active accounts, select the customer for whom have special price list.</span></span>
3. <span data-ttu-id="1ca88-143">ग्राहक रिकॉर्ड को खोलने के लिए उसे चुनें और उसके बाद **परियोजना मूल्य सूची** टैब चुनें. सबग्रिड इस ग्राहक के लिए परियोजना मूल्य सूचियों की एक सूची दिखाती है.</span><span class="sxs-lookup"><span data-stu-id="1ca88-143">Select the customer record to open it and then select the **Project Price Lists** tab. A subgrid shows a list of project price lists specific to this customer.</span></span> 
4. <span data-ttu-id="1ca88-144">यहाँ एक नई मूल्य सूची संबद्धता बनाएँ, ताकि इस ग्राहक के पास विशिष्ट परियोजना मूल्य सूची हो.</span><span class="sxs-lookup"><span data-stu-id="1ca88-144">Create a new price list association here to have project price list specific to this customer.</span></span>

## <a name="custom-pricing-on-a-project-contract"></a><span data-ttu-id="1ca88-145">परियोजना अनुबंध पर कस्टम मूल्य निर्धारण</span><span class="sxs-lookup"><span data-stu-id="1ca88-145">Custom pricing on a project contract</span></span>

<span data-ttu-id="1ca88-146">आपके पास संगठनात्मक और ग्राहक-विशिष्ट डिफ़ॉल्ट परियोजना मूल्य सूचियाँ होने के बाद, आपके परियोजना अनुबंध इन परियोजना मूल्य सूची संबद्धता के साथ स्वचालित रूप से बन जाएंगे.</span><span class="sxs-lookup"><span data-stu-id="1ca88-146">After you have organizational and customer-specific default project price lists, your project contracts will be created with these project price list associations automatically.</span></span> <span data-ttu-id="1ca88-147">हालाँकि, परियोजना अनुबंध की परियोजना मूल्य सूचियाँ हमेशा दिनांक और अनुबंध नाम के साथ कॉपी की जाती हैं.</span><span class="sxs-lookup"><span data-stu-id="1ca88-147">However, project price lists on a project contract are always copied with the date and contract name appended to them.</span></span> <span data-ttu-id="1ca88-148">उसके बाद खाता और परियोजना प्रबंधक इन प्रतियों पर मूल्यों का संपादन करना शुरू कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="1ca88-148">The account and project managers can then begin making edits to prices on these copies.</span></span> <span data-ttu-id="1ca88-149">ये बदले हुए मूल्य केवल इस परियोजना अनुबंध पर लागू होंगे.</span><span class="sxs-lookup"><span data-stu-id="1ca88-149">These changed prices will be applicable to this project contract only.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]