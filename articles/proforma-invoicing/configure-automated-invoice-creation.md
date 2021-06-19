---
title: स्वचालित इनवॉइस निर्माण कॉन्फ़िगर करें
description: यह विषय स्वचालित रूप से इनवॉइस बनाने के लिए सिस्टम को कॉन्फ़िगर करने के लिए कैसे के बारे में जानकारी देता है.
author: rumant
ms.date: 10/13/2020
ms.topic: article
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: dffa95c163f7f8d5074e02cd56d6f1ed429a7c72
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6005343"
---
# <a name="configure-automatic-invoice-creation"></a><span data-ttu-id="8fe02-103">स्वचालित इनवॉइस निर्माण कॉन्फ़िगर करें</span><span class="sxs-lookup"><span data-stu-id="8fe02-103">Configure automatic invoice creation</span></span>

<span data-ttu-id="8fe02-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="8fe02-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>


<span data-ttu-id="8fe02-105">Dynamics 365 Project Operations में स्वचालित इनवॉइस चलाने को कॉन्फ़िगर करने के लिए निम्न चरणों को पूरा करें.</span><span class="sxs-lookup"><span data-stu-id="8fe02-105">Complete the following steps to configure an automated invoice run in Dynamics 365 Project operations.</span></span>

1. <span data-ttu-id="8fe02-106">**सेटिंग्स** > **बैच जॉब** पर जाएँ.</span><span class="sxs-lookup"><span data-stu-id="8fe02-106">Go to **Settings** > **Batch jobs**.</span></span>
2. <span data-ttu-id="8fe02-107">एक बैच जॉब तैयार करें और उसे **परियोजना संचालन क्रिएट इनवॉयस** नाम दें.</span><span class="sxs-lookup"><span data-stu-id="8fe02-107">Create a batch job, and name it **Project operations create invoices**.</span></span> <span data-ttu-id="8fe02-108">बैच जॉब के नाम में "इनवॉइस बनाएं" शब्द ज़रूर शामिल होने चाहिए.</span><span class="sxs-lookup"><span data-stu-id="8fe02-108">The name of the batch job must include the words "create invoices."</span></span>
3. <span data-ttu-id="8fe02-109">**जॉब प्रकार** फील्ड में, **कुछ नहीं** चुनें.</span><span class="sxs-lookup"><span data-stu-id="8fe02-109">In the **Job Type** field, select **None**.</span></span> <span data-ttu-id="8fe02-110">**रोज़ की आवॉत्ति** और **सक्रिय है** विकल्प अपने आप **हाँ** में सेट होते हैं।</span><span class="sxs-lookup"><span data-stu-id="8fe02-110">By default, the **Frequency Daily** and **Is Active** options are set to **Yes**.</span></span>
4. <span data-ttu-id="8fe02-111">**वर्कफ्लो चलाएँ** चुनें।</span><span class="sxs-lookup"><span data-stu-id="8fe02-111">Select **Run Workflow**.</span></span> <span data-ttu-id="8fe02-112">**लुक अप रिकार्ड** डॉयलॉग बॉक्स में, आपको तीन वर्कफ्लो दिखेंगे:</span><span class="sxs-lookup"><span data-stu-id="8fe02-112">In the **Look Up Record** dialog box, you will see three workflows:</span></span>

    - <span data-ttu-id="8fe02-113">ProcessRunCaller</span><span class="sxs-lookup"><span data-stu-id="8fe02-113">ProcessRunCaller</span></span>
    - <span data-ttu-id="8fe02-114">ProcessRunner</span><span class="sxs-lookup"><span data-stu-id="8fe02-114">ProcessRunner</span></span>
    - <span data-ttu-id="8fe02-115">UpdateRoleUtilization</span><span class="sxs-lookup"><span data-stu-id="8fe02-115">UpdateRoleUtilization</span></span>

5. <span data-ttu-id="8fe02-116">**ProcessRunCaller** चुनें, फिर **Add** चुनें।</span><span class="sxs-lookup"><span data-stu-id="8fe02-116">Select **ProcessRunCaller**, and then select **Add**.</span></span>
6. <span data-ttu-id="8fe02-117">अगले डॉयलॉग बॉक्स में,**ओके** चुनें।</span><span class="sxs-lookup"><span data-stu-id="8fe02-117">In the next dialog box, select **OK**.</span></span> <span data-ttu-id="8fe02-118">**प्रोसेस** वर्कफ्लो के बाद एक **स्लीप** वर्कफ्लो आएगा।</span><span class="sxs-lookup"><span data-stu-id="8fe02-118">A **Sleep** workflow is followed by a **Process** workflow.</span></span>

  > [!NOTE]
  > <span data-ttu-id="8fe02-119">आप **ProcessRunner** को 5 चरणों में चुन सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="8fe02-119">You can also select **ProcessRunner** in step 5.</span></span> <span data-ttu-id="8fe02-120">इसके बाद, जब आप **OK** चुनते हैं, तो **स्लीप** वर्कफ्लो के बाद **प्रोसेस** वर्कफ्लो आएगा।</span><span class="sxs-lookup"><span data-stu-id="8fe02-120">Then, when you select **OK**, a **Process** workflow is followed by a **Sleep** workflow.</span></span>

<span data-ttu-id="8fe02-121">**ProcessRunCaller** और **ProcessRunner** वर्कफ्लो बीजक तैयार करेंगे।</span><span class="sxs-lookup"><span data-stu-id="8fe02-121">The **ProcessRunCaller** and **ProcessRunner** workflows create invoices.</span></span> <span data-ttu-id="8fe02-122">**ProcessRunCaller** कॉल **ProcessRunner**।</span><span class="sxs-lookup"><span data-stu-id="8fe02-122">**ProcessRunCaller** calls **ProcessRunner**.</span></span> <span data-ttu-id="8fe02-123">**ProcessRunner** वह वर्कफ्लो होता है जो वास्तव में बीजक तैयार करता है।</span><span class="sxs-lookup"><span data-stu-id="8fe02-123">**ProcessRunner** is the workflow that actually creates the invoices.</span></span> <span data-ttu-id="8fe02-124">यह बीजक तैयार करने के लिए आवश्यक सभी संविदा लाइनों से गुजरता है और उन लाइनों के लिए बीजक तैयार करता है।</span><span class="sxs-lookup"><span data-stu-id="8fe02-124">It goes through all the contract lines that invoices must be created for, and it creates invoices for those lines.</span></span> <span data-ttu-id="8fe02-125">बीजक के लिए आवश्यक संविदा लाइनें तय करने के लिए, जॉब में संविदा लाइनों के लिए बीजक चलाने की तारीखें देखी जाती हैं।</span><span class="sxs-lookup"><span data-stu-id="8fe02-125">To determine the contract lines that invoices must be created for, the job looks at invoice run dates for the contract lines.</span></span> <span data-ttu-id="8fe02-126">यदि किसी एक संविदा से संबंधित संविदा लाइनों की बीजक चलाने की तारीखें समान हैं तो दो बीजक लाइनों वाले एक बीजक में लेनदेन संयोजित कर दिए जाते हैं।</span><span class="sxs-lookup"><span data-stu-id="8fe02-126">If contract lines that belong to one contract have the same invoice run date, the transactions are combined into one invoice that has two invoice lines.</span></span> <span data-ttu-id="8fe02-127">यदि बीजक तैयार करने के लिए कोई लेनदेन न हों तो जॉब बीजक तैयार करना छोड़ देता है।</span><span class="sxs-lookup"><span data-stu-id="8fe02-127">If there are no transactions to create invoices for, the job skips invoice creation.</span></span>

<span data-ttu-id="8fe02-128">**ProcessRunner** चलने का काम पूरा होने के बाद, यह **ProcessRunCaller** को बुलाता है और अंतिम समय देता है और बंद हो जाता है।</span><span class="sxs-lookup"><span data-stu-id="8fe02-128">After **ProcessRunner** has finished running, it calls **ProcessRunCaller**, provides the end time, and is closed.</span></span> <span data-ttu-id="8fe02-129">इसके बाद **ProcessRunCaller** टाइमर शुरु करता है जो निर्दिष्ट अंतिम समय से 24 घंटों तक चलते रहता है।</span><span class="sxs-lookup"><span data-stu-id="8fe02-129">**ProcessRunCaller** then starts a timer that runs for 24 hours from the specified end time.</span></span> <span data-ttu-id="8fe02-130">टाइमर के अंत में, **ProcessRunCaller** बंद हो जाएगा।</span><span class="sxs-lookup"><span data-stu-id="8fe02-130">At the end of the timer, **ProcessRunCaller** is closed.</span></span>

<span data-ttu-id="8fe02-131">बीजक तैयार करने के लिए बैच प्रोसेस जॉब आवर्ती जॉब है।</span><span class="sxs-lookup"><span data-stu-id="8fe02-131">The batch process job for creating invoices is a recurrent job.</span></span> <span data-ttu-id="8fe02-132">यदि बैच प्रोसेस कई बार चलाया जाता है तो जॉब कई बार किया जाएगा और त्रुटियाँ होंगी।</span><span class="sxs-lookup"><span data-stu-id="8fe02-132">If this batch process is run many times, multiple instances of the job are created and cause errors.</span></span> <span data-ttu-id="8fe02-133">इसलिए, आपको केवल एक बार बैच प्रोसेस शुरु करना चाहिए और इसके बंद होने पर ही दोबारा चालू करना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="8fe02-133">Therefore, you should start the batch process only one time, and you should restart it only if it stops running.</span></span>

> [!NOTE]
> <span data-ttu-id="8fe02-134">बैच इनवॉइसिंग केवल परियोजना अनुबंध लाइनों के लिए चलती है जो इनवॉइस शेड्यूल से कॉन्फ़िगर किए गए हैं.</span><span class="sxs-lookup"><span data-stu-id="8fe02-134">Batch invoicing only runs for project contract lines that are configured by invoice schedules.</span></span> <span data-ttu-id="8fe02-135">निश्चित मूल्य बिलिंग विधि वाली अनुबंध पंक्ति में माइलस्टोन कॉन्फ़िगर होने चाहिए.</span><span class="sxs-lookup"><span data-stu-id="8fe02-135">A contract line with a fixed price billing method must have milestones configured.</span></span> <span data-ttu-id="8fe02-136">समय और सामग्री बिलिंग विधि वाली परियोजना अनुबंध पंक्ति को दिनांक-आधारित इनवॉइस शेड्यूल सेट अप की आवश्यकता होगी.</span><span class="sxs-lookup"><span data-stu-id="8fe02-136">A project contract line with a time and material billing method will need a date-based invoice schedule set up.</span></span> <span data-ttu-id="8fe02-137">यही बात परियोजना-आधारित अनुबंध पंक्ति पर लागू होती है.</span><span class="sxs-lookup"><span data-stu-id="8fe02-137">The same applies to a project-based contract line.</span></span>     


[!INCLUDE[footer-include](../includes/footer-banner.md)]