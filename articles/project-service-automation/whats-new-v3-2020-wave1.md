---
title: Project Service Automation वर्ज़न 3.x wave 1 2020 में क्या क्या नया है या बदल गया है
description: यह टॉपिक Project Service Automation वर्ज़न 3 wave 1 2020 में क्या नया है और क्या बदला है, इसके बारे में जानकारी प्रदान करता है.
manager: kfend
ms.service: business-applications
ms.custom:
- dyn365-projectservice
ms.date: 01/24/2020
ms.topic: article
ms.prod: ''
ms.technology: Dynamics 365 Project Service Automation 3.x wave 1 2020
author: stsporen
ms.assetid: 48b408c1-11e7-4005-abac-8fd7c0b064b1
ms.author: stsporen
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
ms.openlocfilehash: 478080c0570b71188c9f1e12b18b5aadc13903e5
ms.sourcegitcommit: 8c786230ef2a497280885b827162561776e2eb00
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 03/24/2020
ms.locfileid: "3752011"
---
# <a name="whats-new-or-changed-in-project-service-automation-version-3-wave-1-2020"></a><span data-ttu-id="7bc49-103">Project Service Automation वर्ज़न 3 wave 1 2020 में क्या क्या नया है या बदल गया है</span><span class="sxs-lookup"><span data-stu-id="7bc49-103">What's new or changed in Project Service Automation version 3 wave 1 2020</span></span>
<span data-ttu-id="7bc49-104">यह टॉपिक Project Service Automation (PSA) वर्ज़न 3.x wave 1 2020 की नवीनतम रिलीज़ के लिए आगे बढ़ने पर मुख्य अपडेट विचारों पर प्रकाश डालता है.</span><span class="sxs-lookup"><span data-stu-id="7bc49-104">The topic highlights key upgrade considerations when moving to the latest release of Project Service Automation (PSA) version 3.x wave 1 2020.</span></span>

## <a name="time-entry"></a><span data-ttu-id="7bc49-105">समय प्रविष्टि</span><span class="sxs-lookup"><span data-stu-id="7bc49-105">Time entry</span></span>
<span data-ttu-id="7bc49-106">समय प्रविष्टि अनुभव को अधिक ग्राहक परिदृश्यों में समय प्रविष्टि के विस्तार की क्षमता प्रदान करने के लिए बढ़ाया गया है.</span><span class="sxs-lookup"><span data-stu-id="7bc49-106">The time entry experience has been extended to deliver capabilities for extending time entry into more customer scenarios.</span></span> <span data-ttu-id="7bc49-107">इसमें प्रविष्टि प्रकार जोड़ने की क्षमता शामिल है, जो अब फील्ड स्कीमा नाम के आधार पर विशिष्ट व्यवहार को चलाते हैं **समय प्रविष्टि सेटिंग**, **समय स्रोत** के रूप में प्रदर्शित.</span><span class="sxs-lookup"><span data-stu-id="7bc49-107">This includes the capability to add entry types, which now drive specific behavior based on the field schema name **Time Entry Settings**, displayed as **Time Source**.</span></span>

### <a name="upgrade-consideration"></a><span data-ttu-id="7bc49-108">नवीनीकरण विचार</span><span class="sxs-lookup"><span data-stu-id="7bc49-108">Upgrade consideration</span></span>
<span data-ttu-id="7bc49-109">इस कार्यक्षमता का समर्थन करने के लिए, PSA के भीतर की भूमिकाओं को नए विशेषाधिकार शामिल करने के लिए अपडेट किया गया है.</span><span class="sxs-lookup"><span data-stu-id="7bc49-109">To support this functionality, the roles within PSA have been updated to include new privileges.</span></span> <span data-ttu-id="7bc49-110">ये विशेषाधिकार नई इकाई, **समय प्रविष्टि सेटिंग** तक पहुँच प्रदान करते हैं.</span><span class="sxs-lookup"><span data-stu-id="7bc49-110">These privileges grant read access to the new entity, **Time Entry Settings**.</span></span>

<span data-ttu-id="7bc49-111">जिन उपयोगकर्ताओं को समय को रिकॉर्ड करने की क्षमता की आवश्यकता होती है, उन्हें मौजूदा भूमिकाओं के साथ-साथ उपयोगकर्ता भूमिका **समय प्रविष्टि उपयोगकर्ता** दी जानी चाहिए.</span><span class="sxs-lookup"><span data-stu-id="7bc49-111">Users who require the ability to log time should be granted the user role **Time Entry User** in addition to existing roles.</span></span> <span data-ttu-id="7bc49-112">इस भूमिका में नई कार्यक्षमता शामिल है और यह सुनिश्चित करती है कि समय प्रविष्टि काम करना जारी रखेगी.</span><span class="sxs-lookup"><span data-stu-id="7bc49-112">This role includes the new functionality and ensures that time entry will continue to work.</span></span>

### <a name="currently-extended-time-entry-changes"></a><span data-ttu-id="7bc49-113">वर्तमान में विस्तारित समय प्रविष्टि परिवर्तन</span><span class="sxs-lookup"><span data-stu-id="7bc49-113">Currently extended time entry changes</span></span>
<span data-ttu-id="7bc49-114">समय प्रविष्टि के वर्तमान उपयोगकर्ताओं पर प्रभाव को कम करने के लिए, यह भूमिका परिवर्तन समय प्रविष्टि का उपयोग जारी रखने के लिए आवश्यक एकमात्र कोर आवश्यकता है.</span><span class="sxs-lookup"><span data-stu-id="7bc49-114">To minimize the impact to current users of time entry, this role change is the only core requirement necessary to continue utilizing time entry.</span></span> <span data-ttu-id="7bc49-115">यदि आपने कस्टम दृश्य या अलग समय प्रविष्टि अनुभव बनाए हैं, तो आपको **समय प्रविष्टि सेटिंग** फील्ड को सही PSA मान पीआर सेट करना होगा.</span><span class="sxs-lookup"><span data-stu-id="7bc49-115">If you have created custom views or separate time entry experiences, you must set the **Time Entry Setting** fields to the correct PSA value.</span></span>
