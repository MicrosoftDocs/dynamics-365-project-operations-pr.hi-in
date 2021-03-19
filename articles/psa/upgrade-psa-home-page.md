---
title: होम पृष्ठ को अपग्रेड करें
description: इस टॉपिक में इस बात से संबंधित जानकारी दी गयी है कि Dynamics 365 Project Service Automation में नई और बदली हुई विशेषताओं के बारे में महत्वपूर्ण जानकारी कहाँ से मिल सकती है और अपग्रेड कर नवीनतम संस्करण पाने की प्रोसेस क्या है.
manager: kfend
ms.prod: ''
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 05/30/2019
ms.topic: article
author: rumant
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
ms.openlocfilehash: 838eecb1229ea20106c7d5487dc37a81e8df501b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5281705"
---
# <a name="upgrade-home-page"></a><span data-ttu-id="9d38b-103">होम पृष्ठ को अपग्रेड करें</span><span class="sxs-lookup"><span data-stu-id="9d38b-103">Upgrade home page</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

## <a name="upgrade-from-psa-version-2x-or-1x-to-version-3x"></a><span data-ttu-id="9d38b-104">PSA संस्करण 2.x या 1.x से संस्करण 3.x में नवीनीकरण करें</span><span class="sxs-lookup"><span data-stu-id="9d38b-104">Upgrade from PSA version 2.x or 1.x to version 3.x</span></span>

### <a name="new-instances"></a><span data-ttu-id="9d38b-105">नए आवृत्तियाँ</span><span class="sxs-lookup"><span data-stu-id="9d38b-105">New instances</span></span>

<span data-ttu-id="9d38b-106">17 मई, 2019 को जब एक नए इंस्टांस की प्रोविजनिंग के दौरान Project Service Automation का चयन किया जाता है तो वर्ज़न 3.x डिफ़ॉल्ट रूप से इंस्टाल हो जाता है.</span><span class="sxs-lookup"><span data-stu-id="9d38b-106">As of May 17, 2019, when Project Service Automation is selected during the provisioning of a new instance, version 3.x is installed by default.</span></span>

### <a name="existing-instances"></a><span data-ttu-id="9d38b-107">मौजूदा आवृत्तियाँ</span><span class="sxs-lookup"><span data-stu-id="9d38b-107">Existing instances</span></span>

<span data-ttu-id="9d38b-108">पहले, जिन ग्राहकों के पास PSA संस्करण 2.x की कोई आवृत्ति थी और संस्करण 3.x में नवीनीकरण करने की आवश्यकता थी, जो PSA का एकीकृत क्लाइंट इंटरफेस-आधारित (UCI) संस्करण है, को Microsoft समर्थन से संपर्क कर अपनी आवृत्ति का विवरण देना होता था, ताकि समर्थन संस्करण 3.x में नवीनीकृत करने के लिए आवृत्ति को सक्षम कर सके.</span><span class="sxs-lookup"><span data-stu-id="9d38b-108">Previously, customers who have an instance of PSA version 2.x and needed to upgrade to version 3.x, which is the Unified client interface-based (UCI) version of PSA, had to contact Microsoft Support and provide the details of their instance so that support could enable the instance for upgrade to version 3.x.</span></span> <span data-ttu-id="9d38b-109">1 मार्च, 2020 तक, जिन ग्राहकों के पास PSA संस्करण 2.x की आवृत्ति थी और जिन्हें संस्करण 3.x में नवीनीकरण करने की आवश्यकता थी, वे Microsoft समर्थन से संपर्क किए बिना अपनी आवृत्तियों को सीधे व्यवस्थापक पोर्टल से नवीनीकृत कर पाएंगे.</span><span class="sxs-lookup"><span data-stu-id="9d38b-109">As of March 1, 2020, customers who have an instance of PSA version 2.x and need to upgrade to version 3.x, will able to upgrade their instances directly from the Admin portal without having to contact Microsoft Support.</span></span>  

> [!NOTE]
> <span data-ttu-id="9d38b-110">PSA वर्ज़न 3.x में महत्वपूर्ण परिवर्तन शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="9d38b-110">PSA version 3.x includes significant changes.</span></span> <span data-ttu-id="9d38b-111">इसे यूज़र को बेहतर अनुभव प्रदान करने के लिए यूनिफाइड इंटरफेस फ्रेमवर्क पर बनाया गया है.</span><span class="sxs-lookup"><span data-stu-id="9d38b-111">It has been built on the Unified Interface framework to help provide an improved user experience.</span></span> <span data-ttu-id="9d38b-112">री-डिज़ाइन्ड ऐप सुसंगत, एक-सा यूज़र इंटरफ़ेस (UI) डिलिवर करता है और किसी भी स्क्रीन आकार या डिवाइस पर सर्वोत्तम रूप से देखने के डिज़ाइन सिद्धांतों पर आधारित है.</span><span class="sxs-lookup"><span data-stu-id="9d38b-112">The redesigned app delivers a consistent, uniform user interface (UI), and it follows responsive design principles for optimal viewing on any screen size or device.</span></span> <span data-ttu-id="9d38b-113">सारे ऍप्लिकेशन में अन्य परिवर्तन भी किये गए हैं.</span><span class="sxs-lookup"><span data-stu-id="9d38b-113">There have been other changes throughout the application.</span></span> <span data-ttu-id="9d38b-114">जिन कुछ क्षेत्रों को बदला गया है, उनमें मूल्य निर्धारण, बुकिंग और संसाधनों को एसाइन करना, समय, व्यय और अनुमोदन शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="9d38b-114">Some of the areas that have been changed include pricing, booking and assigning resources, time, expenses, and approvals.</span></span>

<span data-ttu-id="9d38b-115">आपके अपग्रेड शुरू करने से पहले हम आपको निम्न कार्यों को पूरा करने की सिफारिश करेंगे:</span><span class="sxs-lookup"><span data-stu-id="9d38b-115">Before you begin the upgrade process, we recommend that you complete the following tasks:</span></span>

- <span data-ttu-id="9d38b-116">सत्यापित करें कि Dynamics 365 Field Service और Project Service Automation, दोनों ही पहचाने गए इंस्टांस पर इंस्टाल्ड हैं या नहीं.</span><span class="sxs-lookup"><span data-stu-id="9d38b-116">Verify whether both Dynamics 365 Field Service and Project Service Automation are installed on the identified instance.</span></span> <span data-ttu-id="9d38b-117">यदि दोनों समाधान इंस्टाल्ड हैं तो आपको इंस्टांस का नियमित उपयोग फिर से शुरू करने से पहले दोनों को अपग्रेड करने के बारे में सोचना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="9d38b-117">If both solutions are installed, you should plan to upgrade both before you resume regular use of the instance.</span></span>
- <span data-ttu-id="9d38b-118">निम्न टॉपिक की सावधानीपूर्वक समीक्षा करें.</span><span class="sxs-lookup"><span data-stu-id="9d38b-118">Carefully review the following topics.</span></span> <span data-ttu-id="9d38b-119">विभिन्न वर्ज़न में परिवर्तनों के बारे में जागरूकता और समझ पाने से आपको अपग्रेड प्रोसेस में मदद मिलेगी.</span><span class="sxs-lookup"><span data-stu-id="9d38b-119">Awareness and understanding of the changes between versions will help you with the upgrade process.</span></span> <span data-ttu-id="9d38b-120">इन टॉपिक में PSA में हुए बड़े बदलावों के बारे में जानकारी के अलावा अपग्रेड कर वर्ज़न 3.x पाने के संबंध में विचार और सिफारिशें भी दी गई हैं.</span><span class="sxs-lookup"><span data-stu-id="9d38b-120">These topics provide information about the major changes in PSA, together with considerations and recommendations for planning your upgrade to version 3.x.</span></span>

    - [<span data-ttu-id="9d38b-121">Project Service Automation वर्ज़न 3 में क्या क्या नया है या बदल गया है</span><span class="sxs-lookup"><span data-stu-id="9d38b-121">What's new or changed in Project Service Automation version 3</span></span>](whats-new-changed-v3.md)
    - [<span data-ttu-id="9d38b-122">अपग्रेड से जुड़ा विचार - Project Service Automation वर्ज़न 2.x या 1.x से वर्ज़न 3</span><span class="sxs-lookup"><span data-stu-id="9d38b-122">Upgrade considerations - Project Service Automation version 2.x or 1.x to version 3</span></span>](upgrade-v3.md)

- <span data-ttu-id="9d38b-123">अपने प्रोडक्शन इंस्टांस को अपग्रेड करने से पहले अपने कार्यान्वयन में हुए परिवर्तनों का मूल्यांकन करने के लिए अपने सैंडबॉक्स इंस्टांस को अपग्रेड करें.</span><span class="sxs-lookup"><span data-stu-id="9d38b-123">Upgrade your sandbox instance to evaluate the changes in your implementation before you upgrade your production instance.</span></span>

<span data-ttu-id="9d38b-124">पहले बताए गए टॉपिक की समीक्षा करने के बाद जब आप अपग्रेड कर PSA वर्ज़न संस्करण 3.x या UCI- आधारित वर्ज़न पर जाने को तैयार हैं तो एडमिन सेंटर से अपग्रेड उपलब्ध कराने के लिए Microsoft सपोर्ट को अपना अनुरोध सबमिट करें.</span><span class="sxs-lookup"><span data-stu-id="9d38b-124">After you've reviewed the topics that were mentioned earlier and are ready to upgrade to PSA version 3.x or the UCI-based version, submit a request to Microsoft support to make the upgrade available from Admin center.</span></span> <span data-ttu-id="9d38b-125">अपने अनुरोध में अपने इंस्टांस का विवरण दें.</span><span class="sxs-lookup"><span data-stu-id="9d38b-125">In your request, provide the details of your instance.</span></span>

## <a name="older-versions-of-psa-psa-version-2x-in-a-newly-created-instance"></a><span data-ttu-id="9d38b-126">नए बने इंस्टांस में PSA (PSA वर्ज़न 2.x) के पुराने वर्ज़न</span><span class="sxs-lookup"><span data-stu-id="9d38b-126">Older versions of PSA (PSA version 2.x) in a newly created instance</span></span>

<span data-ttu-id="9d38b-127">17 मई, 2019 को सभी नए इंस्टांस में डिफ़ॉल्ट क्लाइंट के तौर पर UCI होगा.</span><span class="sxs-lookup"><span data-stu-id="9d38b-127">As of May 17, 2019, all new instances will have UCI as the default client.</span></span> <span data-ttu-id="9d38b-128">इस परिवर्तन के साथ एलाइनमेंट के लिए PSA वर्ज़न 3.x और Field Service वर्ज़न 8.x डिफ़ॉल्ट रूप से प्रोविज़न किया जाएगा, क्योंकि ये वर्ज़न UCI क्लाइंट के साथ काम करने के लिए बनाये गए हैं.</span><span class="sxs-lookup"><span data-stu-id="9d38b-128">For alignment with this change, PSA version 3.x and Field Service version 8.x will be provisioned by default, because these versions are designed to work with the UCI client.</span></span>

<span data-ttu-id="9d38b-129">1 मार्च 2020 से, Dynamics PSA के ग्राहक अब PSA के पुराने संस्करणों के साथ एक नया परिवेश नहीं बना पाएंगे, उदाहरण के लिए PSA संस्करण 2.x या इससे कम.</span><span class="sxs-lookup"><span data-stu-id="9d38b-129">Starting March 1, 2020, customers of Dynamics PSA will no longer be able to create a new environment with older versions of PSA, for example PSA version 2.x or lower.</span></span> <span data-ttu-id="9d38b-130">किसी भी नए वातावरण को केवल PSA का संस्करण 3.x प्राप्त करना होगा.</span><span class="sxs-lookup"><span data-stu-id="9d38b-130">Any new environment will be to get only version 3.x of PSA.</span></span>

> [!NOTE]
> <span data-ttu-id="9d38b-131">Field Service और PSA ऍप्लिकेशन के पुराने वर्ज़न का उपयोग करते समय सर्वोत्तम अनुभव पाने के लिए **सिस्टम सेटिंग्स** पृष्ठ पर जाएं और **केवल नया यूनिफ़ाइड इंटरफ़ेस उपयोग करें (सलाह दी जाती है)** फ़ील्ड के लिए **नहीं** का चयन चूंकि ये वर्ज़न UCI में सही ढंग से लोड करने के लिए नहीं बने हैं.</span><span class="sxs-lookup"><span data-stu-id="9d38b-131">For the best experience when you use older versions of the Field Service and PSA applications, go to the **System settings** page and for the field, **Use the new Unified Interface only (recommended)** field, select **No** as these versions aren't designed to be correctly loaded in UCI.</span></span> <span data-ttu-id="9d38b-132">UCI को बंद करने के बाद आप पुराने वेब क्लाइंट का उपयोग कर Field Service और PSA के इन वर्ज़न को खोलकर चला सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="9d38b-132">After you have turned off UCI, you can open and run these versions of Field Service and PSA by using the old web client.</span></span> 


[!INCLUDE[footer-include](../includes/footer-banner.md)]