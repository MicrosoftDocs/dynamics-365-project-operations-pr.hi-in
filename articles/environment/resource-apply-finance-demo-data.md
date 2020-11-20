---
title: किसी Finance क्लाउड-होस्टेड परिवेश में डेमो डेटा लागू करें
description: यह विषय बताता है कि परियोजना संचालन से डेमो डेटा को Dynamics 365 Finance क्लाउड द्वारा होस्ट किए गए परिवेश में कैसे लागू किया जाए।
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: a7cdbd2847ce45972aadd0d1a2d4f26270727ad9
ms.sourcegitcommit: d33ef0ae39f90fe3b0f6b4524f483e8052057361
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/03/2020
ms.locfileid: "4365240"
---
# <a name="apply-demo-data-to-a-finance-cloud-hosted-environment"></a><span data-ttu-id="65166-103">किसी Finance क्लाउड-होस्टेड परिवेश में डेमो डेटा लागू करें</span><span class="sxs-lookup"><span data-stu-id="65166-103">Apply demo data to a Finance Cloud-hosted environment</span></span>

<span data-ttu-id="65166-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="65166-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

> [!IMPORTANT]
> <span data-ttu-id="65166-105">यह विषय केवल Microsoft Dynamics 365 Finance वर्जन 10.0.13 पर लागू है और इसपर केवल क्लाउड होस्टेड परिवेश में ही काम किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="65166-105">This topic is only applicable only Microsoft Dynamics 365 Finance version 10.0.13 and can be performed only on a Cloud-hosted environment.</span></span> <span data-ttu-id="65166-106">इससे **पहले** कि आप परिवेश के लिए गुणवत्ता अपडेट लागू करें, इस विषय में चरणों को पूरा करें।</span><span class="sxs-lookup"><span data-stu-id="65166-106">Complete the steps in this topic **BEFORE** you apply quality updates to the environment.</span></span>

1. <span data-ttu-id="65166-107">अपनी LCS परियोजना में, **परिवेश विवरण** पृष्ठ खोलें।</span><span class="sxs-lookup"><span data-stu-id="65166-107">In your LCS project, open the **Environment details** page.</span></span> <span data-ttu-id="65166-108">ध्यान दें कि इसमें रिमोट डेस्कटॉप प्रोटोकॉल (RDP) का उपयोग करके परिवेश से जुड़ने के लिए आवश्यक विवरण शामिल हैं।</span><span class="sxs-lookup"><span data-stu-id="65166-108">Notice that it includes the details needed to connect to the environment by using Remote Desktop Protocol (RDP).</span></span>

![परिवेश विवरण](./media/1EnvironmentDetails.png)

<span data-ttu-id="65166-110">हाइलाइट किए गए क्रेडेंशियल्स का पहला सेट स्थानीय खाता क्रेडेंशियल्स हैं और इसमें रिमोट डेस्कटॉप कनेक्शन के लिए हाइपरलिंक शामिल है।</span><span class="sxs-lookup"><span data-stu-id="65166-110">The first set of highlighted credentials are the local account credentials and contain a hyperlink to the remote desktop connection.</span></span> <span data-ttu-id="65166-111">क्रेडेंशियल में परिवेश व्यवस्थापक उपयोगकर्ता नाम और पासवर्ड शामिल हैं।</span><span class="sxs-lookup"><span data-stu-id="65166-111">The credentials include the environment admin username and password.</span></span> <span data-ttu-id="65166-112">क्रेडेंशियल के दूसरे सेट का उपयोग इस परिवेश में SQL सर्वर पर लॉग इन करने के लिए किया जाता है।</span><span class="sxs-lookup"><span data-stu-id="65166-112">The second set of credentials are used to log in to SQL Server in this environment.</span></span>

2. <span data-ttu-id="65166-113">**स्थानीय खाते**, में हाइपरलिंक द्वारा परिवेश का रिमोट, और प्रमाणित करने के लिए **स्थानीय खाता क्रेडेंशियल्स** का उपयोग करें।</span><span class="sxs-lookup"><span data-stu-id="65166-113">Remote to the environment by the hyperlink in **Local Accounts**, and use the **Local Account credentials** to authenticate.</span></span>
3. <span data-ttu-id="65166-114">**इंटर्नेट सूचना सेवाएं** > **एप्लीकेशन पूल** > **AOSService** पर जाएं और सेवा बंद करें।</span><span class="sxs-lookup"><span data-stu-id="65166-114">Go to **Internet Information Services** > **Application Pools** > **AOSService** and stop the service.</span></span> <span data-ttu-id="65166-115">आप इस बिंदु पर सेवा रोक रहे हैं, ताकि आप SQL डेटाबेस को बदलना जारी रख सकें।</span><span class="sxs-lookup"><span data-stu-id="65166-115">You are stopping the service at this point so that you can continue to replace the SQL database.</span></span>

![AOS बंद करें](./media/2StopAOS.png)

4. <span data-ttu-id="65166-117">**सेवाओं** पर जाएं और निम्नलिखित दो आइटम बंद करें:</span><span class="sxs-lookup"><span data-stu-id="65166-117">Go to **Services** and stop the following two items:</span></span>

- <span data-ttu-id="65166-118">Microsoft Dynamics 365 Unified Operations: बैच प्रबंधन सेवा</span><span class="sxs-lookup"><span data-stu-id="65166-118">Microsoft Dynamics 365 Unified Operations: Batch Management Service</span></span>
- <span data-ttu-id="65166-119">Microsoft Dynamics 365 Unified Operations: डेटा आयात निर्यात फ़्रेमवर्क</span><span class="sxs-lookup"><span data-stu-id="65166-119">Microsoft Dynamics 365 Unified Operations: Data Import Export Framework</span></span>

![सेवाएं बंद करें](./media/3StopServices.png)

5. <span data-ttu-id="65166-121">Microsoft SQL Server Management Studio खोलें।</span><span class="sxs-lookup"><span data-stu-id="65166-121">Open Microsoft SQL Server Management Studio.</span></span> <span data-ttu-id="65166-122">SQL सर्वर क्रेडेंशियल के साथ लॉग इन करें और LCS **परिवेश विवरण** पृष्ठ से axdbadmin उपयोगकर्ता और पासवर्ड का उपयोग करें।</span><span class="sxs-lookup"><span data-stu-id="65166-122">Log in with SQL server credentials and use the axdbadmin user and password from the LCS **Environments details** page.</span></span>

![SQL Server मैनेजमेंट स्टूडियो](./media/4SSMS.png)

6. <span data-ttu-id="65166-124">ऑब्जेक्ट एक्सप्लोरर में, **डेटाबेस** और **AXDB** का पता लगाएं.</span><span class="sxs-lookup"><span data-stu-id="65166-124">In Object Explorer, **Databases** and locate **AXDB**.</span></span> <span data-ttu-id="65166-125">आप डेटाबेस को एक नए डेटाबेस के साथ बदल देंगे, जो [डाउनलोड सेंटर](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip).</span><span class="sxs-lookup"><span data-stu-id="65166-125">You will replace database with a new database that is located in the [Download Center](https://download.microsoft.com/download/1/a/3/1a314bd2-b082-4a87-abdc-1ba26c92b63d/ProjOpsDemoDataFOGARelease.zip).</span></span> 
7. <span data-ttu-id="65166-126">ज़िप फ़ाइल को उस VM में कॉपी करें जिसमें आप रिमोट कर रहे हैं और ज़िप सामग्री निकालें.</span><span class="sxs-lookup"><span data-stu-id="65166-126">Copy the zip file to the VM you are remoted into and extract zip contents.</span></span>
8. <span data-ttu-id="65166-127">SQL Server Management Studio में, **AxDB** पर राइट-क्लिक करें, और उसके बाद **कार्य** > **पुनर्स्थापित करें** > **डेटाबेस** चुनें.</span><span class="sxs-lookup"><span data-stu-id="65166-127">In SQL Server Management Studio, right-click **AxDB**, and then select **Tasks** > **Restore** > **Database**.</span></span>

![डेटाबेस पुनर्स्थापित करें](./media/5RestoreDatabase.png)

9. <span data-ttu-id="65166-129">**स्रोत डिवाइस** चुनें और आपके द्वारा कॉपी की गई ज़िप से निकाली गए फ़ाइल पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="65166-129">Select **Source Device** and navigate to the file extracted from zip you copied.</span></span>

![स्रोत डिवाइस](./media/6SourceDevice.png)

10. <span data-ttu-id="65166-131">**विकल्प**, चुनें, और फिर **मौजूदा डेटाबेस को अधिलेखित करें** और **गंतव्य डेटाबेस के लिए मौजूदा कनेक्शन बंद करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="65166-131">Select **Options**, and then select **Overwrite the existing database** and **Close existing connections to destination database**.</span></span> 
11. <span data-ttu-id="65166-132">**ठीक** चुनें।</span><span class="sxs-lookup"><span data-stu-id="65166-132">Select **OK**.</span></span>

![सेटिंग्स पुनर्स्थापित करें](./media/7RestoreSetting.png)

<span data-ttu-id="65166-134">आपको पुष्टि मिलेगी कि AXDB पुनर्स्थापना सफल रही।</span><span class="sxs-lookup"><span data-stu-id="65166-134">You will receive confirmation that the AXDB restore was successful.</span></span> <span data-ttu-id="65166-135">यह पुष्टि प्राप्त करने के बाद, आप SQL Services Management Studio बंद कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="65166-135">After you receive this confirmation, you can close SQL Services Management Studio.</span></span>

12. <span data-ttu-id="65166-136">**इंटरनेट सूचना सेवा** > **एप्लिकेशन पूल** > **AOSService** पर जाएं और AOSService शुरू करें।</span><span class="sxs-lookup"><span data-stu-id="65166-136">Go back to **Internet Information Services** > **Application Pools** > **AOSService** and start the AOSService.</span></span>
13. <span data-ttu-id="65166-137">**सेवाओं** पर जाएं और उन दो सेवाओं को शुरू करें जिन्हें आपने पहले बंद कर दिया था।</span><span class="sxs-lookup"><span data-stu-id="65166-137">Go to **Services** and start the two services you stopped earlier.</span></span>

14. <span data-ttu-id="65166-138">इस VM पर AdminUserProvisioning टूल का पता लगाएं।</span><span class="sxs-lookup"><span data-stu-id="65166-138">Locate the AdminUserProvisioning tool on this VM.</span></span> <span data-ttu-id="65166-139">K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe में देखें।</span><span class="sxs-lookup"><span data-stu-id="65166-139">Look under, K:\AosService\PackagesLocalDirectory\bin\AdminUserProvisioning.exe.</span></span>
15. <span data-ttu-id="65166-140">**ईमेल पता** फ़ील्ड में अपने उपयोगकर्ता पते का उपयोग करके .ext फ़ाइल चलाएं।</span><span class="sxs-lookup"><span data-stu-id="65166-140">Run the .ext file using your user address in the **Email Address** field.</span></span> 
16. <span data-ttu-id="65166-141">**सबमिट करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="65166-141">Select **Submit**.</span></span>

![व्यवस्थापक उपयोगकर्ता प्रोविजनिंग](./media/8AdminUserProvisioning.png)

<span data-ttu-id="65166-143">इसे पूरा करने में कुछ मिनट लगते हैं।</span><span class="sxs-lookup"><span data-stu-id="65166-143">This takes a couple of minutes to complete.</span></span> <span data-ttu-id="65166-144">आपको एक पुष्टिकरण संदेश प्राप्त होना चाहिए कि व्यवस्थापक उपयोगकर्ता सफलतापूर्वक अपडेट किया गया था।</span><span class="sxs-lookup"><span data-stu-id="65166-144">You should receive a confirmation message that the Admin user was successfully updated.</span></span>

17. <span data-ttu-id="65166-145">अंत में, कमांड प्रॉम्प्ट को व्यवस्थापक के रूप में चलाएं और iis रीसेट करें</span><span class="sxs-lookup"><span data-stu-id="65166-145">Lastly, run Command Prompt as Administrator and perform iisreset</span></span>

![IIS रीसेट करें](./media/9IISReset.png)

18. <span data-ttu-id="65166-147">रिमोट डेस्कटॉप सत्र बंद करें और LCS **परिवेश विवरण** पृष्ठ का उपयोग करके परिवेश में लॉग इन करें ताकि यह पुष्टि की जा सके कि यह उम्मीद के अनुसार काम कर रहा है।</span><span class="sxs-lookup"><span data-stu-id="65166-147">Close the remote desktop session and use the LCS **Environment details** page to log in to the environment to confirm it is working as expected.</span></span>

![Finance and Operations](./media/10FinanceAndOperations.png)
