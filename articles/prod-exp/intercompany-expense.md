---
title: इंटरकंपनी व्यय
description: एक श्रमिक जो एक संगठन में एक कानूनी निकाय द्वारा नियोजित है, एक ही संगठन में दूसरे कानूनी निकाय के लिए काम कर सकता है. इस स्थिति में, आप इंटरकंपनी ख़र्च सुविधा का उपयोग श्रमिक के ख़र्चों को उस कानूनी निकाय से असाइन करने के लिए कर सकते हैं जिसके लिए काम किया गया था.
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
ms.openlocfilehash: 0967f23e4e1f8e0431c55d4d54554e7e90e2451c
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077851"
---
# <a name="intercompany-expenses"></a><span data-ttu-id="86bf3-104">इंटरकंपनी व्यय</span><span class="sxs-lookup"><span data-stu-id="86bf3-104">Intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="86bf3-105">एक श्रमिक जो एक संगठन में एक कानूनी निकाय द्वारा नियोजित है, एक ही संगठन में दूसरे कानूनी निकाय के लिए काम कर सकता है.</span><span class="sxs-lookup"><span data-stu-id="86bf3-105">A worker who is employed by one legal entity in an organization might perform work for another legal entity in the same organization.</span></span> <span data-ttu-id="86bf3-106">इस स्थिति में, आप इंटरकंपनी ख़र्च सुविधा का उपयोग श्रमिक के ख़र्चों को उस कानूनी निकाय से असाइन करने के लिए कर सकते हैं जिसके लिए काम किया गया था.</span><span class="sxs-lookup"><span data-stu-id="86bf3-106">In this situation, you can use the intercompany expense feature to assign the worker’s expenses to the legal entity for which the work was performed.</span></span> <span data-ttu-id="86bf3-107">श्रमिक को नियोजित करने वाली कानूनी निकाय को ऋण कानूनी निकाय कहा जाता है.</span><span class="sxs-lookup"><span data-stu-id="86bf3-107">The legal entity that employs the worker is called the loaning legal entity.</span></span> <span data-ttu-id="86bf3-108">जिस कानूनी निकाय के लिए श्रमिक ख़र्च करता है उसे उधार लेने वाली कानूनी निकाय कहा जाता है.</span><span class="sxs-lookup"><span data-stu-id="86bf3-108">The legal entity for which the worker incurs expenses is called the borrowing legal entity.</span></span> 

<span data-ttu-id="86bf3-109">इससे पहले कि एक श्रमिक एक अलग कानूनी निकाय के लिए किए गए काम के लिए ख़र्च बना और प्रस्तुत कर सकता है, ऋण कानूनी निकाय में, **ख़र्च प्रबंधन मापदंड** पृष्ठ पर, **इंटरकंपनी ख़र्च लाइनों की अनुमति दें** विकल्प का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="86bf3-109">Before a worker can create and submit expenses for work that is performed for a different legal entity, in the loaning legal entity, on the **Expense management parameters** page, select the **Allow intercompany expense lines** option.</span></span> 

## <a name="tax-posting-for-intercompany-expenses"></a><span data-ttu-id="86bf3-110">इंटरकंपनी ख़र्चों के लिए कर पोस्टिंग</span><span class="sxs-lookup"><span data-stu-id="86bf3-110">Tax posting for intercompany expenses</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="86bf3-111">यदि आप अपनी ख़र्च रिपोर्ट में उधार (गंतव्य) कानूनी निकाय के बजाय ऋण (स्रोत) कानूनी इकाई से जुड़े कर समूहों का उपयोग करना चाहते हैं, तो आपको इसे सामान्य लेजर बिक्री कर सेट अप में कॉन्फ़िगर करने की आवश्यकता होगी.</span><span class="sxs-lookup"><span data-stu-id="86bf3-111">If you want to use tax groups that are associated with the loaning (source) legal entity instead of the borrowing (destination) legal entity in your expense report, you will need to configure this in the General ledger sales tax set up.</span></span> <span data-ttu-id="86bf3-112">जब सामान्य लेजर मापदंड, **इंटरकंपनी कर पोस्टिंग के लिए कानूनी निकाय** **स्रोत** पर और **बिक्री कर कर-निर्धारण नियम लागू करें** **नही** पर सेट है, तो ऋण कानूनी निकाय के लिए कर संयोजन का उपयोग किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="86bf3-112">When the General ledger parameter, **Legal entity for intercompany tax posting** is set to **Source** and **Apply sales tax taxation rules** is set to **No** , the tax combination for the loaning legal entity will be used.</span></span> <span data-ttu-id="86bf3-113">जब वही मापदंड **गंतव्य** के लिए सेट किया जाता है, तो उधार लेने वाली कानूनी निकाय के लिए कर संयोजन का उपयोग किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="86bf3-113">When the same parameter is set to **Destination** , the tax combination for borrowing legal entity will be used.</span></span> <span data-ttu-id="86bf3-114">संयुक्त राज्य अमेरिका में कानूनी निकायों के लिए, जब मापदंड **स्रोत** के लिए सेट किया जाता है, तो **स्वीकार्य बिक्री कर** फ़ील्ड को नए **लेजर पोस्टिंग समूह** पृष्ठ पर भी कॉन्फ़िगर किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="86bf3-114">For legal entities in the United States, when the parameter is set to **Source** , the **Sales tax receivable** field must also be configured on the new **Ledger posting groups** page.</span></span> <span data-ttu-id="86bf3-115">लेखांकन इंजन कर से जुड़ी लेखांकन प्रविष्टि के लिए इस फील्ड से जानकारी का इस्तेमाल करेगा.</span><span class="sxs-lookup"><span data-stu-id="86bf3-115">The accounting engine will use the information from this field for tax related accounting entry.</span></span>   
<span data-ttu-id="86bf3-116">परियोजना के साथ या बिना पोस्ट किए गए ख़र्च लाइनों के लिए व्यवहार संगत है.</span><span class="sxs-lookup"><span data-stu-id="86bf3-116">The behavior is consistent for expense lines posted with or without a project.</span></span>  
