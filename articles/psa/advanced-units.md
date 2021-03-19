---
title: इकाई समूह और इकाइयाँ
description: यह विषय इकाई समूहों और इकाइयों के बारे में जानकारी प्रदान करता है।
author: rumant
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/05/2019
ms.topic: article
ms.author: rumant
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: 45e4a95b429cd9d1f174653bd28cf567f690676d
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5291621"
---
# <a name="unit-groups-and-units"></a><span data-ttu-id="631b2-103">इकाई समूह और इकाइयाँ</span><span class="sxs-lookup"><span data-stu-id="631b2-103">Unit groups and units</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="631b2-104">इकाई समूह और इकाइयां Microsoft Dynamics 365 में मूलभूत इकाइयां हैं।</span><span class="sxs-lookup"><span data-stu-id="631b2-104">Unit groups and units are basic entities in Microsoft Dynamics 365.</span></span> <span data-ttu-id="631b2-105">एक इकाई माप की एक एकल इकाई है, और कई इकाइयों को इकाई समूहों में वर्गीकृत किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-105">A unit is a single unit of measure, and multiple units can be grouped into unit groups.</span></span> <span data-ttu-id="631b2-106">एक इकाई समूह को कभी-कभी Dynamics 365 उपयोगकर्ता इंटरफ़ेस (UI) में एक इकाई शेड्यूल के रूप में संदर्भित किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-106">A unit group is sometimes referred to as a unit schedule in the Dynamics 365 user interface (UI).</span></span> 

<span data-ttu-id="631b2-107">यहां इकाइयों और इकाई समूहों के कुछ उदाहरण दिए गए हैं:</span><span class="sxs-lookup"><span data-stu-id="631b2-107">Here are some examples of units and unit groups:</span></span>
 
- <span data-ttu-id="631b2-108">**इकाई समूह**: दूरी</span><span class="sxs-lookup"><span data-stu-id="631b2-108">**Unit group**: Distance</span></span> 
    - <span data-ttu-id="631b2-109">**इकाइयां**: मील, किलोमीटर और इसी तरह।</span><span class="sxs-lookup"><span data-stu-id="631b2-109">**Units**: Mile, Kilometer, and so on.</span></span>
- <span data-ttu-id="631b2-110">**इकाई समूह**: समय</span><span class="sxs-lookup"><span data-stu-id="631b2-110">**Unit group**: Time</span></span>
    - <span data-ttu-id="631b2-111">**इकाइयां**: घंटा, दिन, सप्ताह और इसी तरह।</span><span class="sxs-lookup"><span data-stu-id="631b2-111">**Units**: Hour, day, week, and so on.</span></span> 

<span data-ttu-id="631b2-112">जब आप एक इकाई समूह में कई इकाइयां स्थापित करते हैं, तो आपको पहले समूह के लिए डिफ़ॉल्ट इकाई या प्राथमिक इकाई के रूप में स्थापित की गई इकाई को निर्दिष्ट करके उनके बीच एक रूपांतरण कारक भी स्थापित करना होगा।</span><span class="sxs-lookup"><span data-stu-id="631b2-112">When you set up multiple units in a unit group, you must also set up a conversion factor between them by designating the first unit that you set up as the default or primary unit for the unit group.</span></span> 

<span data-ttu-id="631b2-113">उदाहरण के लिए, **समय** इकाई समूह में, यदि आप पहली इकाई के रूप में **घंटा** सेट करते हैं, तो सिस्टम **घंटे** को डिफ़ॉल्ट इकाई के रूप में नामित करता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-113">For example, in a **Time** unit group, if you set up **Hour** as the first unit, the system designates **Hour** as the default unit.</span></span> <span data-ttu-id="631b2-114">यदि आपके द्वारा सेट की गई अगली इकाई **दिन** है, तो आपको **दिन** से **घंटे** के लिए एक रूपांतरण कारक स्थापित करना होगा।</span><span class="sxs-lookup"><span data-stu-id="631b2-114">If the next unit that you set up is **Day**, you must set up a conversion factor for **Day** to **Hour**.</span></span> <span data-ttu-id="631b2-115">यदि आप **सप्ताह** को तीसरी इकाई के रूप में जोड़ते हैं, तो आपको **सप्ताह** के लिए **दिन** या **घंटे** के रूप में रूपांतरण कारक स्थापित करना होगा।</span><span class="sxs-lookup"><span data-stu-id="631b2-115">If you then add **Week** as a third unit, you must set up a conversion factor for **Week** in terms of **Day** or **Hour**.</span></span> 

<span data-ttu-id="631b2-116">निम्न तस्वीर **दिन** इकाई के लिए एक उदाहरण सेटअप दिखाती है, जहां **मात्रा** फ़ील्ड एक दिन में होने वाले घंटों की संख्या को दर्शाता है, और **सप्ताह**, जहां **मात्रा** फ़ील्ड उन दिनों की संख्या दिखाता है जो एक सप्ताह में होते हैं।</span><span class="sxs-lookup"><span data-stu-id="631b2-116">The following image shows an example setup for the **Day** unit, where the **Quantity** field shows the number of hours that are in a day, and **Week**, where the **Quantity** field show the number of days that are in a week.</span></span>

> ![इकाई समूह: सूचना पृष्ठ](media/advanced-2.png)

## <a name="using-units-and-unit-groups"></a><span data-ttu-id="631b2-118">इकाइयों और यूनिट समूहों का उपयोग करना</span><span class="sxs-lookup"><span data-stu-id="631b2-118">Using units and unit groups</span></span>

<span data-ttu-id="631b2-119">Dynamics 365 Project Service Automation इकाइयों और यूनिट समूहों का उपयोग खर्च और समय दोनों के लिए अनुमान और प्रविष्टियों को प्रोसेस करने के लिए करता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-119">Dynamics 365 Project Service Automation uses units and unit groups to process estimates and entries for both expenses and time.</span></span> 

<span data-ttu-id="631b2-120">खर्चों के लिए, प्रत्येक व्यय श्रेणी में एक डिफ़ॉल्ट इकाई समूह और इकाई होती है।</span><span class="sxs-lookup"><span data-stu-id="631b2-120">For expenses, each expense category has a default unit group and unit.</span></span> <span data-ttu-id="631b2-121">इन मूल्यों को मूल्य श्रेणियों के लिए मूल्य सूची प्रविष्टियों पर डिफ़ॉल्ट मान के रूप में दर्ज किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-121">These values are entered as default values on price list entries for expense categories.</span></span> 

<span data-ttu-id="631b2-122">उदाहरण के लिए, आपके पास एक खर्च श्रेणी है जिसका नाम **माइलेज** है।</span><span class="sxs-lookup"><span data-stu-id="631b2-122">For example, you have an expense category that is named **Mileage**.</span></span> <span data-ttu-id="631b2-123">इसका एक इकाई समूह है जिसका नाम **दूरी** और एक डिफॉल्ट इकाई है जिसका नाम **मील** है।</span><span class="sxs-lookup"><span data-stu-id="631b2-123">It has a unit group that is named **Distance** and a default unit that is named **Mile**.</span></span> <span data-ttu-id="631b2-124">यदि आप **दूरी** इकाई ग्रुप सेट करते हैं, ताकि इसकी दो इकाइयां (**मील** और **किलोमीटर**) हों, तो आप **माइलेज** श्रेणी के लिए दो मूल्य एक मूल्य सूची पर सेट कर सकते हैं: मूल्य प्रति मील और मूल्य प्रति किलोमीटर।</span><span class="sxs-lookup"><span data-stu-id="631b2-124">If you set up the **Distance** unit group so that it has two units (**Mile** and **Kilometer**), you can set two prices for the **Mileage** category on one price list: price per mile and price per kilometer.</span></span>

| <span data-ttu-id="631b2-125">खर्च की श्रेणी</span><span class="sxs-lookup"><span data-stu-id="631b2-125">Expense category</span></span>  | <span data-ttu-id="631b2-126">इकाई समूह</span><span class="sxs-lookup"><span data-stu-id="631b2-126">Unit group</span></span>  | <span data-ttu-id="631b2-127">इकाई</span><span class="sxs-lookup"><span data-stu-id="631b2-127">Unit</span></span>      | <span data-ttu-id="631b2-128">मूल्य निर्धारण विधि</span><span class="sxs-lookup"><span data-stu-id="631b2-128">Pricing method</span></span>  | <span data-ttu-id="631b2-129">मूल्य प्रति इकाई</span><span class="sxs-lookup"><span data-stu-id="631b2-129">Price per unit</span></span>  |
|-------------------|---------------|-----------|-------------------|-------------------|
| <span data-ttu-id="631b2-130">माइलेज़</span><span class="sxs-lookup"><span data-stu-id="631b2-130">Mileage</span></span>           | <span data-ttu-id="631b2-131">दूरी</span><span class="sxs-lookup"><span data-stu-id="631b2-131">Distance</span></span>      | <span data-ttu-id="631b2-132">मील</span><span class="sxs-lookup"><span data-stu-id="631b2-132">Mile</span></span>      | <span data-ttu-id="631b2-133">मूल्य प्रति इकाई</span><span class="sxs-lookup"><span data-stu-id="631b2-133">Price per unit</span></span>    | <span data-ttu-id="631b2-134">10 USD</span><span class="sxs-lookup"><span data-stu-id="631b2-134">10 USD</span></span>            |
| <span data-ttu-id="631b2-135">माइलेज़</span><span class="sxs-lookup"><span data-stu-id="631b2-135">Mileage</span></span>           | <span data-ttu-id="631b2-136">दूरी</span><span class="sxs-lookup"><span data-stu-id="631b2-136">Distance</span></span>      | <span data-ttu-id="631b2-137">किलोमीटर</span><span class="sxs-lookup"><span data-stu-id="631b2-137">Kilometer</span></span> | <span data-ttu-id="631b2-138">मूल्य प्रति इकाई</span><span class="sxs-lookup"><span data-stu-id="631b2-138">Price per unit</span></span>    |  <span data-ttu-id="631b2-139">6 USD</span><span class="sxs-lookup"><span data-stu-id="631b2-139">6 USD</span></span>            |

<span data-ttu-id="631b2-140">जब आप किसी प्रोजेक्ट पर खर्च दर्ज करते हैं, तो सिस्टम कीमत पर श्रेणी और इकाई के संयोजन के माध्यम से मूल्य निर्धारित करता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-140">When you enter an expense on a project, the system determines the price through the combination of the category and the unit on the expense.</span></span> 

| <span data-ttu-id="631b2-141">खर्च का विवरण</span><span class="sxs-lookup"><span data-stu-id="631b2-141">Expense description</span></span>        | <span data-ttu-id="631b2-142">खर्च की श्रेणी</span><span class="sxs-lookup"><span data-stu-id="631b2-142">Expense category</span></span>  | <span data-ttu-id="631b2-143">इकाई</span><span class="sxs-lookup"><span data-stu-id="631b2-143">Unit</span></span>  | <span data-ttu-id="631b2-144">मात्रा</span><span class="sxs-lookup"><span data-stu-id="631b2-144">Quantity</span></span>  | <span data-ttu-id="631b2-145">इकाई मूल्य</span><span class="sxs-lookup"><span data-stu-id="631b2-145">Unit price</span></span>   |
|----------------------------|---------------------|-------|-----------|----------------|
| <span data-ttu-id="631b2-146">ग्राहक स्थान पर ड्राइव करें</span><span class="sxs-lookup"><span data-stu-id="631b2-146">Drive to client location</span></span> | <span data-ttu-id="631b2-147">माइलेज़</span><span class="sxs-lookup"><span data-stu-id="631b2-147">Mileage</span></span>             | <span data-ttu-id="631b2-148">मील</span><span class="sxs-lookup"><span data-stu-id="631b2-148">Mile</span></span>  | <span data-ttu-id="631b2-149">10</span><span class="sxs-lookup"><span data-stu-id="631b2-149">10</span></span>        | <span data-ttu-id="631b2-150">10 USD</span><span class="sxs-lookup"><span data-stu-id="631b2-150">10 USD</span></span>         |

<span data-ttu-id="631b2-151">समय के लिए, प्रत्येक मूल्य सूची हेडर में **डिफॉल्ट समय इकाई** फ़ील्ड होता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-151">For time, each price list header has a **Default Time Unit** field.</span></span> <span data-ttu-id="631b2-152">जब आप मूल्य सूची हेडर बनाते हैं तो मान सेट हो जाता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-152">The value is set when you create the price list header.</span></span> <span data-ttu-id="631b2-153">इस इकाई का उपयोग उस मूल्य सूची पर सभी भूमिका-आधारित मूल्य निर्धारित करने के लिए किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-153">This unit is then used to set all role-based prices on that price list.</span></span>

<span data-ttu-id="631b2-154">**कोटेशन पर समय** फ़ील्ड के लिए अनुमानित लाइनों को समय की किसी भी इकाई में व्यक्त किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-154">Estimate lines for the **Time on Quote** field can be expressed in any unit of time.</span></span> <span data-ttu-id="631b2-155">हालांकि, प्रोजेक्ट के लिए अनुमान लाइनें और प्रोजेक्ट के लिए समय प्रविष्टियां केवल समय की इकाई **घंटे** का उपयोग कर सकती हैं।</span><span class="sxs-lookup"><span data-stu-id="631b2-155">However, estimate lines on projects and time entries for projects can use only the **Hour** unit of time.</span></span> <span data-ttu-id="631b2-156">यदि समय प्रविष्टि या अनुमान लाइन पर इकाई उस भूमिका के लिए मूल्य सूची लाइन पर इकाई से मेल नहीं खाती है, तो सिस्टम मूल्य को उन इकाइयों में परिवर्तित करता है जो प्रोजेक्ट अनुमान या प्रोजेक्ट वास्तविक लेन-देन में परिभाषित हैं।</span><span class="sxs-lookup"><span data-stu-id="631b2-156">If the unit on the time entry or estimate line doesn't match the unit on the price list line for that role, the system converts the price to the units that are defined in the project estimate or the project actual transaction.</span></span>

<span data-ttu-id="631b2-157">निम्न उदाहरण दिखाता है कि PSA इकाई समूह, इकाइयों और रूपांतरण कारकों का उपयोग कैसे करता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-157">The following example shows how PSA uses the unit group, units, and conversion factors.</span></span>
- <span data-ttu-id="631b2-158">इकाइयां</span><span class="sxs-lookup"><span data-stu-id="631b2-158">Units</span></span>

   - <span data-ttu-id="631b2-159">**इकाई समूह**: समय</span><span class="sxs-lookup"><span data-stu-id="631b2-159">**Unit group**: Time</span></span> 
   - <span data-ttu-id="631b2-160">**इकाइयां**: घंटा</span><span class="sxs-lookup"><span data-stu-id="631b2-160">**Units**: Hour</span></span> 
    
    - <span data-ttu-id="631b2-161">**दिन** - रूपांतरण कारक: 8 घंटे</span><span class="sxs-lookup"><span data-stu-id="631b2-161">**Day** - Conversion factor: 8 hours</span></span>       
    - <span data-ttu-id="631b2-162">**सप्ताह** - रूपांतरण कारक: 40 घंटे</span><span class="sxs-lookup"><span data-stu-id="631b2-162">**Week** - Conversion factor: 40 hours</span></span>  
        
- <span data-ttu-id="631b2-163">प्रोजेक्ट A पर मूल्य सूची सेटअप:</span><span class="sxs-lookup"><span data-stu-id="631b2-163">Price list setup on Project A:</span></span>

    - <span data-ttu-id="631b2-164">**नाम**: यूके बिक्री मूल्य 2016</span><span class="sxs-lookup"><span data-stu-id="631b2-164">**Name**: UK sales prices 2016</span></span> 
    - <span data-ttu-id="631b2-165">**डिफ़ॉल्ट समय इकाई**: दिन</span><span class="sxs-lookup"><span data-stu-id="631b2-165">**Default time unit**: Day</span></span> 
    - <span data-ttu-id="631b2-166">**मुद्रा**: GBP</span><span class="sxs-lookup"><span data-stu-id="631b2-166">**Currency**: GBP</span></span>

| <span data-ttu-id="631b2-167">भूमिका</span><span class="sxs-lookup"><span data-stu-id="631b2-167">Role</span></span>      | <span data-ttu-id="631b2-168">इकाई समूह</span><span class="sxs-lookup"><span data-stu-id="631b2-168">Unit group</span></span> | <span data-ttu-id="631b2-169">इकाई</span><span class="sxs-lookup"><span data-stu-id="631b2-169">Unit</span></span> | <span data-ttu-id="631b2-170">संगठनात्मक इकाई</span><span class="sxs-lookup"><span data-stu-id="631b2-170">Organizational unit</span></span> | <span data-ttu-id="631b2-171">मूल्य</span><span class="sxs-lookup"><span data-stu-id="631b2-171">Price</span></span>   |
|-----------|------------|------|---------------------|---------|
| <span data-ttu-id="631b2-172">डेवलपर</span><span class="sxs-lookup"><span data-stu-id="631b2-172">Developer</span></span> | <span data-ttu-id="631b2-173">Time</span><span class="sxs-lookup"><span data-stu-id="631b2-173">Time</span></span>       | <span data-ttu-id="631b2-174">Day</span><span class="sxs-lookup"><span data-stu-id="631b2-174">Day</span></span>  | <span data-ttu-id="631b2-175">Contoso UK</span><span class="sxs-lookup"><span data-stu-id="631b2-175">Contoso UK</span></span>          | <span data-ttu-id="631b2-176">800 GBP</span><span class="sxs-lookup"><span data-stu-id="631b2-176">800 GBP</span></span> |

### <a name="time-entry"></a><span data-ttu-id="631b2-177">समय प्रविष्टि</span><span class="sxs-lookup"><span data-stu-id="631b2-177">Time entry</span></span>

<span data-ttu-id="631b2-178">निम्न तालिका PSA द्वारा तीन घंटे की प्रोजेक्ट के लिए बनाई गई बिक्री-साइड लेन-देन को दर्शाती है।</span><span class="sxs-lookup"><span data-stu-id="631b2-178">The following table shows the resulting sales-side transaction created by PSA for a three hour project.</span></span>


| <span data-ttu-id="631b2-179">परियोजना</span><span class="sxs-lookup"><span data-stu-id="631b2-179">Project</span></span>   | <span data-ttu-id="631b2-180">कार्य</span><span class="sxs-lookup"><span data-stu-id="631b2-180">Task</span></span>    | <span data-ttu-id="631b2-181">भूमिका</span><span class="sxs-lookup"><span data-stu-id="631b2-181">Role</span></span>      | <span data-ttu-id="631b2-182">मात्रा</span><span class="sxs-lookup"><span data-stu-id="631b2-182">Quantity</span></span> | <span data-ttu-id="631b2-183">इकाई</span><span class="sxs-lookup"><span data-stu-id="631b2-183">Unit</span></span>  | <span data-ttu-id="631b2-184">इकाई मूल्य</span><span class="sxs-lookup"><span data-stu-id="631b2-184">Unit price</span></span> | <span data-ttu-id="631b2-185">बिल न की गई बिक्री राशि</span><span class="sxs-lookup"><span data-stu-id="631b2-185">Unbilled sales amount</span></span> |
|-----------|---------|-----------|----------|-------|------------|-----------------------|
| <span data-ttu-id="631b2-186">प्रोजेक्ट A</span><span class="sxs-lookup"><span data-stu-id="631b2-186">Project A</span></span> | <span data-ttu-id="631b2-187">डिज़ाइन करें</span><span class="sxs-lookup"><span data-stu-id="631b2-187">Design</span></span>  | <span data-ttu-id="631b2-188">डेवलपर</span><span class="sxs-lookup"><span data-stu-id="631b2-188">Developer</span></span> | <span data-ttu-id="631b2-189">3</span><span class="sxs-lookup"><span data-stu-id="631b2-189">3</span></span>        | <span data-ttu-id="631b2-190">Hour</span><span class="sxs-lookup"><span data-stu-id="631b2-190">Hour</span></span>  | <span data-ttu-id="631b2-191">100 GBP</span><span class="sxs-lookup"><span data-stu-id="631b2-191">100 GBP</span></span>    | <span data-ttu-id="631b2-192">300 GBP</span><span class="sxs-lookup"><span data-stu-id="631b2-192">300 GBP</span></span>               |

## <a name="time-unit-faq"></a><span data-ttu-id="631b2-193">समय इकाई अक्सर पूछे जाने वाले प्रश्न</span><span class="sxs-lookup"><span data-stu-id="631b2-193">Time unit FAQ</span></span>

### <a name="does-psa-convert-to-different-units-in-the-case-of-expenses"></a><span data-ttu-id="631b2-194">क्या PSA खर्चों के मामले में विभिन्न इकाइयों में परिवर्तित हो जाता है?</span><span class="sxs-lookup"><span data-stu-id="631b2-194">Does PSA convert to different units in the case of expenses?</span></span>
<span data-ttu-id="631b2-195">नहीं.</span><span class="sxs-lookup"><span data-stu-id="631b2-195">No.</span></span> <span data-ttu-id="631b2-196">इकाई रूपांतरण केवल समय के लिए काम करता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-196">Unit conversion works only for time.</span></span> <span data-ttu-id="631b2-197">खर्चों के लिए, यदि सिस्टम खर्च श्रेणी और इकाई के संयोजन के लिए मूल्य नहीं पा सकता है, तो कीमत डिफ़ॉल्ट रूप से 0.00 पर सेट होती है।</span><span class="sxs-lookup"><span data-stu-id="631b2-197">For expenses, if the system can't find a price for the combination of the expense category and unit, the price is set to 0.00 by default.</span></span>

### <a name="why-does-psa-convert-time-units"></a><span data-ttu-id="631b2-198">PSA समय इकाइयों को क्यों परिवर्तित करता है?</span><span class="sxs-lookup"><span data-stu-id="631b2-198">Why does PSA convert time units?</span></span>
<span data-ttu-id="631b2-199">कुछ देशों या क्षेत्रों में, कानूनी आवश्यकता है कि बिल दरों को दिनों में स्थापित किया जाए।</span><span class="sxs-lookup"><span data-stu-id="631b2-199">In some countries or regions, there is a legal requirement that bill rates be set up in days.</span></span> <span data-ttu-id="631b2-200">कोटेशन चक्र के दौरान मूल्य बातचीत और छूट प्रत्येक बिल योग्य भूमिका के लिए दिन की दरों का उपयोग करके किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-200">Price negotiation and discounting during the quote cycle is done by using day rates for each billable role.</span></span> <span data-ttu-id="631b2-201">अनुसूची अनुमान और समय प्रविष्टि घंटे में की जाती है।</span><span class="sxs-lookup"><span data-stu-id="631b2-201">Schedule estimation and time entry are done in hours.</span></span> <span data-ttu-id="631b2-202">समय इकाइयों में इस अंतर का समर्थन करने के लिए, PSA समय इकाइयों को परिवर्तित करता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-202">To support this difference in time units, PSA converts time units.</span></span>

### <a name="can-time-units-be-changed-on-project-estimates"></a><span data-ttu-id="631b2-203">क्या प्रोजेक्ट अनुमानों पर समय इकाइयों को बदला जा सकता है?</span><span class="sxs-lookup"><span data-stu-id="631b2-203">Can time units be changed on project estimates?</span></span>
<span data-ttu-id="631b2-204">नहीं.</span><span class="sxs-lookup"><span data-stu-id="631b2-204">No.</span></span> <span data-ttu-id="631b2-205">शेड्यूल अनुमान वर्तमान में घंटों तक सीमित है और इसे बदला नहीं जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-205">Schedule estimation is currently restricted to hours and can’t be changed.</span></span>

### <a name="can-units-and-unit-groups-be-edited-deleted-and-added"></a><span data-ttu-id="631b2-206">क्या इकाई और इकाई समूह संपादित, हटाए और जोड़े जा सकते हैं?</span><span class="sxs-lookup"><span data-stu-id="631b2-206">Can units and unit groups be edited, deleted, and added?</span></span>
<span data-ttu-id="631b2-207">हाँ.</span><span class="sxs-lookup"><span data-stu-id="631b2-207">Yes.</span></span> <span data-ttu-id="631b2-208">**समय** इकाई समूह और **घंटा** इकाई के अपवाद के साथ, सभी इकाइयों को हटाया या संपादित किया जा सकता है और नई इकाइयों को जोड़ा जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-208">With exception of the **Time** unit group and the **Hour** unit, all units can be deleted or edited, and new units can be added.</span></span> <span data-ttu-id="631b2-209">PSA में, **समय** इकाई समूह और **घंटा** इकाई को हटाया नहीं जा सकता।</span><span class="sxs-lookup"><span data-stu-id="631b2-209">In PSA, the **Time** unit group and the **Hour** unit can't be deleted.</span></span> <span data-ttu-id="631b2-210">हालांकि, उन्हें **नाम** फ़ील्ड के लिए अनुवादित पाठ के साथ अपडेट किया जा सकता है।</span><span class="sxs-lookup"><span data-stu-id="631b2-210">However, they can be updated with a translated text for the **Name** field.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]