---
title: LCS परियोजना में एक Azure सदस्यता जोड़ें
description: यह विषय LCS परियोजना से अपनी Azure सदस्यता को कैसे जोड़ा जाए, इसके बारे में जानकारी प्रदान करता है.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 6daa86d453ec5022cdd75dff0394c8818292406c
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6000618"
---
# <a name="add-an-azure-subscription-to-an-lcs-project"></a><span data-ttu-id="f1a28-103">LCS परियोजना में एक Azure सदस्यता जोड़ें</span><span class="sxs-lookup"><span data-stu-id="f1a28-103">Add an Azure subscription to an LCS project</span></span>

<span data-ttu-id="f1a28-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="f1a28-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="f1a28-105">क्लाउड-होस्ट किए गए परिवेश को मौजूदा Azure सदस्यता का उपयोग करके नियोजित किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="f1a28-105">Cloud-hosted environments must be deployed using an existing Azure subscription.</span></span> <span data-ttu-id="f1a28-106">यह विषय बताता है कि LCS परियोजना से अपनी मौजूदा Azure सदस्यता को कैसे जोड़ा जाए.</span><span class="sxs-lookup"><span data-stu-id="f1a28-106">This topic explains how to connect your existing Azure subscription to an LCS project.</span></span> 

## <a name="grant-admin-consent"></a><span data-ttu-id="f1a28-107">अनुदान व्यवस्थापक सहमति</span><span class="sxs-lookup"><span data-stu-id="f1a28-107">Grant admin consent</span></span>

1. <span data-ttu-id="f1a28-108">आपकी LCS परियोजना में, **परिवेश** अनुभाग में, **Microsoft Azure सेटिंग्स** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f1a28-108">In your LCS project, in the **Environments** section, select **Microsoft Azure settings**.</span></span>

![Microsoft Azure सेटिंग्स](./media/1MicrosoftAzureSettings.png)

2. <span data-ttu-id="f1a28-110">**परियोजना सेटिंग्स** पेज पर **Azure कनेक्टर्स** टैब पर, **अधिकृत करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f1a28-110">On the **Project settings** page, on the **Azure connectors** tab, select **Authorize**.</span></span> <span data-ttu-id="f1a28-111">यह परिवेश को इस परियोजना के लिए नियोजित होने की अनुमति देता है.</span><span class="sxs-lookup"><span data-stu-id="f1a28-111">This allows environments to be deployed to this project.</span></span>

![Azure कनेक्टर्स](./media/2AzureConnectors.png)

3. <span data-ttu-id="f1a28-113">व्यवस्थापक सहमति प्रदान करने के लिए फिर से **अधिकृत करें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f1a28-113">Select **Authorize** again to provide admin consent.</span></span>

![अनुदान व्यवस्थापक सहमति](./media/3GrantAdminConsent.png)

4. <span data-ttu-id="f1a28-115">अनुमति अनुरोध स्वीकार करें.</span><span class="sxs-lookup"><span data-stu-id="f1a28-115">Accept the permissions request.</span></span>

![अनुमति अनुरोध स्वीकार करें](./media/4AcceptPermissionRequest.png)

<span data-ttu-id="f1a28-117">अधिकृत करना अब पूरा हो गया है.</span><span class="sxs-lookup"><span data-stu-id="f1a28-117">The authorization is now complete.</span></span> 

![अधिकृत करना सफल हुआ](./media/5AuthorizationComplete.png)

## <a name="provide-dynamics-deployment-services-access-to-your-azure-subscription"></a><a name="provide"></a><span data-ttu-id="f1a28-119">अपने Azure सब्सक्रिप्शन को Dynamics Deployment Services की एक्सेस प्रदान करें</span><span class="sxs-lookup"><span data-stu-id="f1a28-119">Provide Dynamics Deployment Services access to your Azure subscription</span></span>

1. <span data-ttu-id="f1a28-120">[Microsoft Azure बिलिंग](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) पर जाएं और अपने सब्सक्रिप्शन का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f1a28-120">Go to [Microsoft Azure billing](https://portal.azure.com/#blade/Microsoft\_Azure\_Billing/SubscriptionsBlade) and select your subscription.</span></span> <span data-ttu-id="f1a28-121">Dynamics Deployment Services को परिवेशों को तैनात करने में सक्षम होने के लिए इस सदस्यता तक पहुँच प्राप्त करने की ज़रूरत है.</span><span class="sxs-lookup"><span data-stu-id="f1a28-121">Dynamics Deployment Services needs to access this subscription to be able to deploy environments.</span></span>

![Azure सब्सक्रिप्शन विवरण](./media/6AzureSubscription.png)

2. <span data-ttu-id="f1a28-123">नेविगेशन फ़लक में **एक्सेस नियंत्रण (IAM)** चुनें, और फिर **भूमिका असाइनमेंट जोड़ें** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f1a28-123">Select **Access control (IAM)** in the navigation pane, and then select **Add role assignment**.</span></span>
3. <span data-ttu-id="f1a28-124">स्लाइडर में दाईं तरफ, **योगदानकर्ता भूमिका**, चुनें, और दी गई सूची में **Dynamics परिनियोजन सेवाएं** खोजें और चुनें।</span><span class="sxs-lookup"><span data-stu-id="f1a28-124">In the slider on the right side, select **Contributor role**, and in the list provided, find and select **Dynamics Deployment Services**.</span></span> 
4. <span data-ttu-id="f1a28-125">**सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f1a28-125">Select **Save**.</span></span>

![सदस्यता पहुंच](./media/7SubscriptionAccess.png)

### <a name="add-a-subscription-connector-to-an-lcs-project"></a><span data-ttu-id="f1a28-127">LCS परियोजना में एक सदस्यता कनेक्टर जोड़ें</span><span class="sxs-lookup"><span data-stu-id="f1a28-127">Add a subscription connector to an LCS project</span></span>

1. <span data-ttu-id="f1a28-128">आपकी LCS परियोजना में, **Microsoft Azure सेटिंग्स** पृष्ठ पर, एक नया कनेक्टर जोड़ने के लिए **जोड़ें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="f1a28-128">In your LCS project, on the **Microsoft Azure settings** page, select **Add** to add a new connector.</span></span>
2. <span data-ttu-id="f1a28-129">अपनी Azure सदस्यता ID दर्ज करें।</span><span class="sxs-lookup"><span data-stu-id="f1a28-129">Enter your Azure subscription ID.</span></span> <span data-ttu-id="f1a28-130">आप स्क्रीन के निचले बाएं हिस्से में  **सेटिंग**  के अंतर्गत [Azure पोर्टल](https://ms.portal.azure.com/), में अपनी Azure सदस्यता ID देख सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="f1a28-130">You can find your Azure subscription ID in the [Azure portal](https://ms.portal.azure.com/), under  **Settings**  in the lower left of the screen.</span></span>
3. <span data-ttu-id="f1a28-131">**Azure संसाधन प्रबंधक का उपयोग करने के लिए कॉन्फ़िगर करें** फ़ील्ड में, **हाँ** चुनें।</span><span class="sxs-lookup"><span data-stu-id="f1a28-131">In the **Configure to use Azure Resource Manager** field, select **Yes**.</span></span>
4. <span data-ttu-id="f1a28-132">सुनिश्चित करें कि Azure की सदस्यता AAD टेनेंट डोमेन उस डोमेन-मालिक Azure सदस्यता से मेल खाती है, जिसका आप उपयोग कर रहे हैं, और **अगला** चुनें।</span><span class="sxs-lookup"><span data-stu-id="f1a28-132">Make sure Azure's Subscription AAD Tenant Domain matches the domain-owning Azure subscription that you are using, and select **Next**.</span></span>
5. <span data-ttu-id="f1a28-133">**Microsoft Azure सेटअप** स्क्रीन पर, पुष्टि करने के लिए **अगला** चुनें।</span><span class="sxs-lookup"><span data-stu-id="f1a28-133">On the **Microsoft Azure Setup** screen, select **Next** to confirm.</span></span> <span data-ttu-id="f1a28-134">यदि आप इस स्क्रीन पर कोई त्रुटि पाते हैं, तो इस विषय में अनुभाग [Azure सदस्यता को Dynamics परिनियोजन सेवाएं तक पहुंच प्रदान करें](#provide) पर लौटें और सुनिश्चित करें कि आपने सभी चरणों को पूरा कर लिया है।</span><span class="sxs-lookup"><span data-stu-id="f1a28-134">If you receive an error on this screen, return to the section [Provide Dynamics Deployment Services access to Azure subscription](#provide) in this topic and make sure you have completed all of the steps.</span></span>
6. <span data-ttu-id="f1a28-135">अपने कंप्यूटर पर किसी स्थानीय फ़ोल्डर में Azure प्रबंधन प्रमाणपत्र डाउनलोड करें.</span><span class="sxs-lookup"><span data-stu-id="f1a28-135">Download the Azure Management Certificate to a local folder on your computer.</span></span> <span data-ttu-id="f1a28-136">अपने Azure सदस्यता व्यवस्थापक को Azure प्रबंधन पोर्टल पर सदस्यता चुनकर और **सेटिंग्स** > **प्रबंधन प्रमाणपत्र** पर जाकर प्रमाणपत्र अपलोड करने के लिए कहें.</span><span class="sxs-lookup"><span data-stu-id="f1a28-136">Ask your Azure subscription administrator to upload the certificate to Azure Management Portal by selecting the subscription and going to **Settings** > **Management Certificates**.</span></span> <span data-ttu-id="f1a28-137">यह प्रमाणपत्र LCS को आपकी ओर से Azure के साथ संवाद करने में सक्षम बनाता है.</span><span class="sxs-lookup"><span data-stu-id="f1a28-137">This certificate enables LCS to communicate with Azure on your behalf.</span></span> <span data-ttu-id="f1a28-138">यदि आपके उपयोगकर्ता की सदस्यता तक पहुँच है, तो आप इस चरण को छोड़ सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="f1a28-138">You can skip this step if your user has access to the subscription.</span></span>
7. <span data-ttu-id="f1a28-139">**अगला** चुनें।</span><span class="sxs-lookup"><span data-stu-id="f1a28-139">Select  **Next**.</span></span>
8. <span data-ttu-id="f1a28-140">परिनियोजित किया जाने वाला Azure क्षेत्र चुनें और उस डेटा केंद्र को चुनें जो उस जगह के पास है जहां आप इस सिस्टम का उपयोग करने की योजना बना रहे हैं।</span><span class="sxs-lookup"><span data-stu-id="f1a28-140">Select the Azure region to deploy in and select a data center that is close to where you plan to use this system.</span></span>
9.  <span data-ttu-id="f1a28-141">**कनेक्ट** चुनें।</span><span class="sxs-lookup"><span data-stu-id="f1a28-141">Select  **Connect**.</span></span>

<span data-ttu-id="f1a28-142">आपने अपनी Azure सदस्यता को सफलतापूर्वक कनेक्ट कर लिया है।</span><span class="sxs-lookup"><span data-stu-id="f1a28-142">You have successfully connected your Azure subscription.</span></span> <span data-ttu-id="f1a28-143">अब आप Dynamics 365 Finance क्लाउड द्वारा होस्ट किए गए परिवेश परिनियोजित कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="f1a28-143">You can now deploy Dynamics 365 Finance cloud-hosted environments.</span></span>




[!INCLUDE[footer-include](../includes/footer-banner.md)]
