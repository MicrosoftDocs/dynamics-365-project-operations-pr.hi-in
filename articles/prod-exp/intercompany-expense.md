---
title: इंटरकंपनी व्यय
description: इस विषय में जानकारी प्रदान की गई है कि उस कानूनी निकाय के लिए, जिसके लिए कार्य निष्पादित किया गया था, कर्मचारी के व्यय असाइन करने के लिए अंतरकंपनी व्ययों का कैसे उपयोग करें.
author: ShylaThompson
manager: AnnBe
ms.date: 05/20/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvParameters
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: d908a1c062f5b7f01cf340dcd6f7f24714a992bf
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5271535"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="b21fe-103">इंटरकंपनी व्यय</span><span class="sxs-lookup"><span data-stu-id="b21fe-103">Intercompany expenses</span></span>

<span data-ttu-id="b21fe-104">एक श्रमिक जो एक संगठन में एक कानूनी निकाय द्वारा नियोजित है, एक ही संगठन में दूसरे कानूनी निकाय के लिए काम कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="b21fe-104">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="b21fe-105">आप उस कानूनी निकाय के लिए, जिसके लिए कार्य निष्पादित किया गया था, कर्मचारी के व्यय असाइन करने के लिए अंतरकंपनी व्ययों का उपयोग कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="b21fe-105">You can use intercompany expenses to assign the worker’s expenses to the legal entity for which the  work was performed.</span></span> <span data-ttu-id="b21fe-106">श्रमिक को नियोजित करने वाली कानूनी निकाय को ऋण कानूनी निकाय कहा जाता है.</span><span class="sxs-lookup"><span data-stu-id="b21fe-106">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="b21fe-107">जिस कानूनी निकाय के लिए श्रमिक ख़र्च करता है उसे उधार लेने वाली कानूनी निकाय कहा जाता है.</span><span class="sxs-lookup"><span data-stu-id="b21fe-107">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="b21fe-108">इससे पहले कि कोई कर्मचारी अंतरकंपनी व्यय को बनाए और सबमिट करें, आपको अंतरकंपनी व्यय पंक्तियाँ सक्षम करनी होंगी.</span><span class="sxs-lookup"><span data-stu-id="b21fe-108">Before a worker can create and submit intercompany expenses, you must enable intercompany expense lines.</span></span> <span data-ttu-id="b21fe-109">ऋण कानूनी निकाय में, **व्यय प्रबंधन पैरामीटर** पृष्ठ पर, **अंतरकंपनी व्यय पंक्तियों की अनुमति दें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="b21fe-109">In the loaning legal entity, on the **Expense management parameters** page, select **Allow intercompany expense lines**.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="b21fe-110">इंटरकंपनी ख़र्चों के लिए कर पोस्टिंग</span><span class="sxs-lookup"><span data-stu-id="b21fe-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="b21fe-111">अपनी व्यय रिपोर्ट में बॉरोइंग (गंतव्य) कानूनी निकाय के बजाय ऋण (स्रोत) कानूनी निकाय से संबद्ध कर समूहों का उपयोग करने से पहले, आपको सामान्य लेजर विक्रय कर सेटअप में कार्यक्षमता सक्षम करनी होगी.</span><span class="sxs-lookup"><span data-stu-id="b21fe-111">Before you can use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you must enable the functionality in the General ledger sales tax setup.</span></span> <span data-ttu-id="b21fe-112">जब **अंतरकंपनी कर पोस्टिंग के लिए कानूनी निकाय** पैरामीटर **स्रोत** पर सेट होता है और **विक्रय कर कराधान नियम लागू करें** **नहीं** पर सेट होता है, तो ऋण कानूनी निकाय के लिए कर संयोजन का उपयोग किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="b21fe-112">When the **Legal entity for intercompany tax posting** parameter is set to **Source** and **Apply sales tax taxation rules** is set to **No**, the tax combination for the loaning legal entity is used.</span></span> <span data-ttu-id="b21fe-113">जब वही मापदंड **गंतव्य** के लिए सेट किया जाता है, तो उधार लेने वाली कानूनी निकाय के लिए कर संयोजन का उपयोग किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="b21fe-113">When the same parameter is set to **Destination**, the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="b21fe-114">संयुक्त राज्य अमेरिका में कानूनी निकायों के लिए, जब मापदंड **स्रोत** के लिए सेट किया जाता है, तो **स्वीकार्य बिक्री कर** फ़ील्ड को नए **लेजर पोस्टिंग समूह** पृष्ठ पर भी कॉन्फ़िगर किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="b21fe-114">For legal entities in the United States, when the parameter is set to **Source**, the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="b21fe-115">लेखांकन इंजन कर-संबंधित लेखांकन प्रविष्टि के लिए इस फ़ील्ड से जानकारी का उपयोग करेगा.</span><span class="sxs-lookup"><span data-stu-id="b21fe-115">The accounting engine will use the information from this field for tax-related accounting entry.</span></span>   
<span data-ttu-id="b21fe-116">परियोजना के साथ या बिना पोस्ट किए गए ख़र्च लाइनों के लिए व्यवहार संगत है.</span><span class="sxs-lookup"><span data-stu-id="b21fe-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  


[!INCLUDE[footer-include](../includes/footer-banner.md)]