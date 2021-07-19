---
title: संसाधन/गैर-स्टॉक किए गए परिदृश्य के लिए परियोजना संचालन पूर्वावलोकन सदस्यता के लिए साइन अप करें
description: यह विषय संसाधन/गैर-स्टॉक किए गए परिदृश्यों के लिए परियोजना संचालन की सदस्यता और परिनियोजित कैसे करना है, की जानकारी देता है।
author: sigitac
ms.date: 07/02/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: da93fcf23ee3f255812842e31cb22b5d39daa963
ms.sourcegitcommit: 52b26950bb3b1596ad81aa4ff91745ee9615d1b0
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 07/02/2021
ms.locfileid: "6334829"
---
# <a name="sign-up-for-project-operations-preview-subscriptions-for-resource-non-stocked-scenarios"></a><span data-ttu-id="d0955-103">संसाधन/गैर-स्टॉक किए गए परिदृश्य के लिए परियोजना संचालन पूर्वावलोकन सदस्यता के लिए साइन अप करें</span><span class="sxs-lookup"><span data-stu-id="d0955-103">Sign up for Project Operations preview subscriptions for resource/ non-stocked scenarios</span></span>

<span data-ttu-id="d0955-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations_</span><span class="sxs-lookup"><span data-stu-id="d0955-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

<span data-ttu-id="d0955-105">यह विषय बताता है कि ट्रायल प्रस्ताव की सदस्यता कैसे लें और संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations परिवेश को कैसे परिनियोजित करें.</span><span class="sxs-lookup"><span data-stu-id="d0955-105">This topic explains how to subscribe to the trial offer and deploy Project Operations environment for resource/non-stocked based scenarios.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0955-106">पूर्वावश्यकताएँ</span><span class="sxs-lookup"><span data-stu-id="d0955-106">Prerequisites</span></span>
- <span data-ttu-id="d0955-107">पूर्वावलोकन नियोजित करने वाले उपयोगकर्ता के पास Azure टेनेंट वैश्विक प्रशासक अधिकार होना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="d0955-107">The user who deploys the preview must have Azure tenant global administrator rights.</span></span> <span data-ttu-id="d0955-108">आप पहले ऑफ़र रिडीम के दौरान टेनेंट बना सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="d0955-108">You can create a tenant during the first offer redemption.</span></span> 
- <span data-ttu-id="d0955-109">वित्त परिवेश में परिनियोजन के लिए एक मान्य Azure सदस्यता की आवश्यकता होती है जिसे परिवेश के अनुसार बिल किया जाएगा।</span><span class="sxs-lookup"><span data-stu-id="d0955-109">Deploying a Finance environment requires a valid Azure subscription that will be billed per environment.</span></span> <span data-ttu-id="d0955-110">आप अपने संगठनों की मौजूदा सदस्यता का उपयोग कर सकते हैं या शुरू करने के लिए एक [Azure परीक्षण](https://azure.microsoft.com/en-us/free/) का उपयोग कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="d0955-110">You can use your organizations existing subscription or use an [Azure trial](https://azure.microsoft.com/en-us/free/) to get started.</span></span> <span data-ttu-id="d0955-111">CDS परिवेश को सीमित 30 दिन की अवधि के लिए मुफ्त प्रदान किया जाएगा।</span><span class="sxs-lookup"><span data-stu-id="d0955-111">The CDS environment will be provided free for a limited 30 day period.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d0955-112">एक संगठन में केवल एक व्यक्ति, टेनेंट व्यवस्थापक को इस कार्य को करने की आवश्यकता है।</span><span class="sxs-lookup"><span data-stu-id="d0955-112">Only one person, the tenant administrator, in an organization needs to perform this task.</span></span> <span data-ttu-id="d0955-113">यदि आप इस रिलीज़ के सदस्य नहीं हैं, तो तब तक इंतजार करें जब तक कि आपके संगठन द्वारा साइन अप नहीं किया जाता है और आपको अपना उपयोगकर्ता क्रेडेंशियल प्राप्त न हो जाए।</span><span class="sxs-lookup"><span data-stu-id="d0955-113">If you aren't the subscriber to this release, wait until your organization has been signed up and you've received your user credentials.</span></span>
> 
> <span data-ttu-id="d0955-114">ट्रायल टैनेंट में एकल उपयोग के लिए हैं.</span><span class="sxs-lookup"><span data-stu-id="d0955-114">Trials are single use in the tenant.</span></span> <span data-ttu-id="d0955-115">आप केवल एक बार ट्रायल चला सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="d0955-115">You can only run a trial one time.</span></span> <span data-ttu-id="d0955-116">हम सुझाव देते हैं कि आप ट्रायल उद्देश्य के लिए नया टैनेंट बनाएं.</span><span class="sxs-lookup"><span data-stu-id="d0955-116">We recommend that you create a new tenant for the purpose of the trial.</span></span>


### <a name="dynamics-365-project-operations-ce---preview-trial"></a><span data-ttu-id="d0955-117">Dynamics 365 Project Operations(CE) - पूर्वावलोकन परीक्षण</span><span class="sxs-lookup"><span data-stu-id="d0955-117">Dynamics 365 Project Operations (CE) - Preview Trial</span></span> 

<span data-ttu-id="d0955-118">शुरू करने से पहले, सुनिश्चित करें कि आप टेनेंट में उपयोगकर्ता वर्क अकाउंट के साथ ब्राउज़र में लॉग इन कर रहे हैं जहां आप Project Operations का पूर्वावलोकन चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="d0955-118">Before you begin, make sure you are logged in to a browser with the user work account in the tenant where you want the Project Operations preview.</span></span>

1. <span data-ttu-id="d0955-119">पहला ऑफ़र कोड, **Dynamics 365 Project Operations** यहाँ [Project Operations परीक्षण](https://aka.ms/try-po) रिडीम करें.</span><span class="sxs-lookup"><span data-stu-id="d0955-119">Redeem the first offer code, **Dynamics 365 Project Operations** here [Project Operations Trial](https://aka.ms/try-po).</span></span>
2. <span data-ttu-id="d0955-120">ऑर्डर की पुष्टि करें.</span><span class="sxs-lookup"><span data-stu-id="d0955-120">Confirm your order.</span></span>

  <span data-ttu-id="d0955-121">आप देखेंगे अनुमोदन प्रस्ताव सफलतापूर्वक चुका दिया गया है.</span><span class="sxs-lookup"><span data-stu-id="d0955-121">You will see confirmation offer was successfully redeemed.</span></span>

### <a name="dynamics-365-finance-preview-trial"></a><span data-ttu-id="d0955-122">Dynamics 365 Finance पूर्वावलोकन परीक्षण</span><span class="sxs-lookup"><span data-stu-id="d0955-122">Dynamics 365 Finance preview trial</span></span>

<span data-ttu-id="d0955-123">[वित्त पूर्वावलोकन परीक्षण के लिए Dynamics 365](https://aka.ms/trypoche) पर जाएँ और ऑफ़र के साथ पिछले अनुभाग के चरणों को दोहराएं, क्लाउड होस्टेड परिवेश के लिए साइन अप करें.</span><span class="sxs-lookup"><span data-stu-id="d0955-123">Go to [Dynamics 365 for Finance Preview Trial](https://aka.ms/trypoche) and repeat the steps from the previous section with the offer, Sign up for the Cloud Hosted Environment.</span></span>  

## <a name="assign-licenses"></a><span data-ttu-id="d0955-124">लाइसेंस असाइन करें</span><span class="sxs-lookup"><span data-stu-id="d0955-124">Assign licenses</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d0955-125">निम्नलिखित चरणों को पूरा करने के लिए आपको अपने संगठन के Microsoft 365 पोर्टल तक प्रशासनिक पहुंच की आवश्यकता होगी.</span><span class="sxs-lookup"><span data-stu-id="d0955-125">You will need administrative access to your organization's Microsoft 365 Portal to complete the following steps.</span></span>

1. <span data-ttu-id="d0955-126">अपने उपयोगकर्ताओं को लाइसेंस आवंटित करने के लिए [Microsoft 365 व्यवस्थापक केंद्र](https://portal.office.com/) पर जाएं.</span><span class="sxs-lookup"><span data-stu-id="d0955-126">Go to [Microsoft 365 admin center](https://portal.office.com/) to assign the licenses to your users.</span></span>

2. <span data-ttu-id="d0955-127">**सक्रिय उपयोगकर्ता** पृष्ठ पर उन उपयोगकर्ताओं का चयन करें, जिन्हें आप लाइसेंस देना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="d0955-127">On the **Active users** page, select the users that you want to assign a license to.</span></span>

3. <span data-ttu-id="d0955-128">सत्यापित करें कि **Dynamics 365 Project Operations** लाइसेंस को चुना गया है और **परिवर्तनों को सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="d0955-128">Verify that the **Dynamics 365 Project Operations** license has been selected and select **Save changes**.</span></span>

> [!NOTE]
> <span data-ttu-id="d0955-129">वित्त परीक्षण प्रस्ताव को उपयोगकर्ता को सौंपने की आवश्यकता नहीं है।</span><span class="sxs-lookup"><span data-stu-id="d0955-129">The Finance trial offer does not need to be assigned to a user.</span></span>

## <a name="start-a-new-project-in-lcs"></a><span data-ttu-id="d0955-130">LCS में एक नई परियोजना प्रारंभ करें</span><span class="sxs-lookup"><span data-stu-id="d0955-130">Start a new project in LCS</span></span>

<span data-ttu-id="d0955-131">विषय LCS में एक नई परियोजना शुरू करें, [LCS में एक नई परियोजना शुरू करें](create-lcs-project.md)</span><span class="sxs-lookup"><span data-stu-id="d0955-131">Create a new LCS project as described in the topic, [Start a new project in LCS](create-lcs-project.md)</span></span>

## <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="d0955-132">LCS परियोजना में एक Azure सदस्यता जोड़ें</span><span class="sxs-lookup"><span data-stu-id="d0955-132">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="d0955-133">इस कार्य को पूरा करने के लिए, विषय LCS परियोजना में एक Azure सदस्यता जोड़ें [LCS प्रोजेक्ट के लिए एक Azure सदस्यता जोड़ें](resource-add-azure-subscription-lcs-project.md) ।</span><span class="sxs-lookup"><span data-stu-id="d0955-133">To complete this task, follow the steps in the topic, [Add an Azure subscription to LCS project](resource-add-azure-subscription-lcs-project.md).</span></span>

## <a name="deploy-finance-demo-environment-with-project-operations-for-resourcenon-stocked-scenarios"></a><span data-ttu-id="d0955-134">संसाधन/गैर-स्टॉक किए गए परिदृश्यों के लिए परियोजना संचालन के साथ वित्त डेमो परिवेश नियोजित करें</span><span class="sxs-lookup"><span data-stu-id="d0955-134">Deploy Finance demo environment with Project Operations for resource/non-stocked scenarios</span></span>

<span data-ttu-id="d0955-135">परिनियोजन को पूरा करने के लिए, विषय, [नए परिवेश का प्रावधान करें](resource-provision-new-environment.md) में मार्गदर्शन का पालन करें।</span><span class="sxs-lookup"><span data-stu-id="d0955-135">Follow the guidance in the topic, [Provision a new environment](resource-provision-new-environment.md) to complete the deployment.</span></span> <span data-ttu-id="d0955-136">पूर्वावलोकन के लिए [डेमो परिवेश](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) परिनियोजन प्रकार का उपयोग करें।</span><span class="sxs-lookup"><span data-stu-id="d0955-136">Use the [demo environment](/dynamics365/fin-ops-core/dev-itpro/deployment/deploy-demo-environment) deployment type for preview.</span></span> 

## <a name="install-cds-setup-and-configuration-data"></a><span data-ttu-id="d0955-137">CDS सेटअप और कॉन्फ़िगरेशन डेटा स्थापित करें</span><span class="sxs-lookup"><span data-stu-id="d0955-137">Install CDS setup and configuration data</span></span>

<span data-ttu-id="d0955-138">CDS सेटअप और कॉन्फ़िगरेशन डेटा स्थापित करें जैसा कि विषय, [सामान्य डेटा सेवा में कॉन्फ़िगरेशन डेटा सेट अप और लागू करें Common Data Service](resource-apply-pro-setup-config-data.md)में वर्णित है।</span><span class="sxs-lookup"><span data-stu-id="d0955-138">Install CDS setup and configuration data as described in the topic, [Set up and apply configuration data in the Common Data Service](resource-apply-pro-setup-config-data.md).</span></span>
<span data-ttu-id="d0955-139">इस चरण को तभी पूरा करें, जब वित्त डेमो परिवेश परिनियोजित हो और डेमो डेटा तैयार हो.</span><span class="sxs-lookup"><span data-stu-id="d0955-139">Complete this step only after Finance demo environment is deployed and demo data is ready.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
