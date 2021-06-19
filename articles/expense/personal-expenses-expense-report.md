---
title: व्यय रिपोर्ट पर व्यक्तिगत व्यय के साथ कार्य करें
description: इस विषय में व्यावसायिक उद्देश्यों के लिए यात्रा करते समय कर्मचारियों द्वारा खर्च किए गए व्यक्तिगत व्यय के साथ काम करने के तरीके के बारे में जानकारी दी गई है.
author: suvaidya
ms.date: 05/11/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: suvaidya
ms.openlocfilehash: ae25eca08089d224f1e17e95eeb571054de8a5c0
ms.sourcegitcommit: fd6e9ff78392c7bac35591d9130c00d2750438ae
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/12/2021
ms.locfileid: "6025686"
---
# <a name="work-with-personal-expenses-on-an-expense-report"></a><span data-ttu-id="1af5c-103">व्यय रिपोर्ट पर व्यक्तिगत व्यय के साथ कार्य करें</span><span class="sxs-lookup"><span data-stu-id="1af5c-103">Work with personal expenses on an expense report</span></span>

<span data-ttu-id="1af5c-104">_**पर लागू होता है:** साधन / गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations, Lite परिनियोजन - प्रोफार्मा इनवॉइसिंग के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="1af5c-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios, Lite deployment - deal to proforma invoicing_</span></span>

<span data-ttu-id="1af5c-105">व्यावसायिक यात्रा के दौरान, कोई कर्मचारी अपने कॉर्पोरेट क्रेडिट कार्ड से व्यक्तिगत व्यय कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="1af5c-105">During business travel, an employee might charge personal expenses to their corporate credit card.</span></span> <span data-ttu-id="1af5c-106">यदि व्यक्तिगत व्यय को हैंडल करने के लिए प्रक्रिया को परिभाषित नहीं किया गया है, तो कर्मचारी द्वारा अपनी आइटम के अनुसार व्यय रिपोर्ट सबमिट करने पर व्यय रिपोर्ट अनुमोदन प्रक्रिया बाधित हो सकती है.</span><span class="sxs-lookup"><span data-stu-id="1af5c-106">If a process hasn't been defined for handling personal expenses, the expense report approval process might be disrupted when an employee submits their itemized expense report.</span></span>

<span data-ttu-id="1af5c-107">ऐसे दो तरीके हैं जिनका उपयोग आप कर्मचारी के व्यक्तिगत व्यय को संभालने के लिए कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="1af5c-107">There are two methods you can use to work with an employee's personal expenses:</span></span>

  - <span data-ttu-id="1af5c-108">**कर्मचारी द्वारा भुगतान किया गया**: आपका संगठन कॉर्पोरेट क्रेडिट कार्ड के लिए बिल पर दिखाई देने वाले व्यक्तिगत व्ययों का भुगतान नहीं करता है.</span><span class="sxs-lookup"><span data-stu-id="1af5c-108">**Paid by employee**: Your organization doesn't pay personal expenses that appear on the bill for the corporate credit card.</span></span> <span data-ttu-id="1af5c-109">इसके बजाय, कर्मचारी क्रेडिट कार्ड विक्रेता को व्ययों के लिए सीधे भुगतान करता है.</span><span class="sxs-lookup"><span data-stu-id="1af5c-109">Instead, the employee pays the credit card vendor directly for the expenses.</span></span> 
  - <span data-ttu-id="1af5c-110">**कंपनी द्वारा भुगतान किया गया**: आपका संगठन कॉर्पोरेट क्रेडिट कार्ड के लिए पूर्ण बिल का भुगतान करता है, और उसके बाद व्यक्तिगत व्यय के लिए कर्मचारी के खाते को डेबिट करता है.</span><span class="sxs-lookup"><span data-stu-id="1af5c-110">**Paid by company**: Your organization pays the full bill for the corporate credit card, and then debits the worker's account for the personal expenses.</span></span>

<span data-ttu-id="1af5c-111">आप उस विधि का चयन कर सकते हैं जिसका उपयोग आपका संगठन **ख़र्च प्रबंधन मापदंड** पृष्ठ पर करता है.</span><span class="sxs-lookup"><span data-stu-id="1af5c-111">You can select the method that your organization uses on the **Expense management parameters** page.</span></span>


## <a name="enable-split-expense-function-when-personal-amount-field-has-value-defined"></a><span data-ttu-id="1af5c-112">व्यक्तिगत धनराशि फ़ील्ड में मान निर्धारित होने पर विभाजित व्यय फ़ंक्शन सक्षम करें</span><span class="sxs-lookup"><span data-stu-id="1af5c-112">Enable split expense function when personal amount field has value defined</span></span>

<span data-ttu-id="1af5c-113">सुविधा, **व्यक्तिगत राशि फ़ील्ड में मान निर्धारित होने पर विभाजित व्यय फ़ंक्शन सक्षम करें** केवल उन व्यय रिपोर्टों पर लागू होती है, जिन्हें पंक्ति-स्तरीय कार्यप्रवाह का उपयोग करके अनुमोदित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="1af5c-113">The feature, **Enable split expense function when personal amount field has value defined** only applies to expense reports that are approved using a line-level workflow.</span></span> <span data-ttu-id="1af5c-114">रिपोर्ट को **व्यय रिपोर्ट संसाधित करें** > **मुझे सौंपी गईं व्यय रिपोर्ट** > **व्यय रिपोर्ट खोलें** पर जाकर अनुमोदित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="1af5c-114">Reports are approved by going to **Process expense reports** > **Expense reports assigned to me** > **Open expense report**.</span></span> 

<span data-ttu-id="1af5c-115">इस सुविधा को सक्षम करने के लिए, **कार्यस्थान** > **विशेषता प्रबंधन** पर जाएं, **व्यक्तिगत राशि फ़ील्ड में मान निर्धारित होने पर विभाजित व्यय फ़ंक्शन सक्षम करें** चुनें और फिर **अभी सक्षम करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="1af5c-115">To enable this feature, go to **Workspaces** > **Feature Management**, select **Enable split expense function when personal amount field has value defined**, and then select **Enable now**.</span></span> 

<span data-ttu-id="1af5c-116">जब सुविधा सक्षम होती है, रिपोर्ट सबमिट करने पर इस कार्यात्मकता का उपयोग करने वाली व्यय पंक्तियां, दो पंक्तियां उत्पन्न करती हैं.</span><span class="sxs-lookup"><span data-stu-id="1af5c-116">When the feature is enabled, expense lines that use this functionality generate two lines when the report is submitted.</span></span> <span data-ttu-id="1af5c-117">दो पंक्तियां उत्पन्न की जाती हैं, जिससे अनुमोदक प्रत्येक पंक्ति को अलग से अनुमोदित कर सके.</span><span class="sxs-lookup"><span data-stu-id="1af5c-117">Two lines are generated so that the approver can approve each line separately.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
