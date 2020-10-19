---
title: डेमो सेटअप और कॉन्फ़िगरेशन डेटा लागू करें
description: यह विषय Project Operations के लिए डेमो सेटअप और कॉन्फ़िगरेशन डेटा लागू करने के तरीके के बारे में जानकारी प्रदान करता है.
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 42e02f393e89d20b2a462645f519a3792bee8f2f
ms.sourcegitcommit: b9d8bf00239815f31686e9b28998ac684fd2fca4
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/02/2020
ms.locfileid: "3948897"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations-lite-deployment---deal-to-proforma-invoicing"></a><span data-ttu-id="f5a6b-103">Project Operations लाइट नियोजन के लिए डेमो सेटअप और कॉन्फ़िगरेशन डेटा लागू करें - प्रोफार्मा इंवॉयसिंग करने के लिए समझौता</span><span class="sxs-lookup"><span data-stu-id="f5a6b-103">Apply demo setup and configuration data for Project Operations lite deployment - deal to proforma invoicing</span></span>

<span data-ttu-id="f5a6b-104">_\*\*लाइट परिनियोजन - प्रोफ़ॉर्मा इनवॉइस करने के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="f5a6b-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

1. <span data-ttu-id="f5a6b-105">[मास्टर डेटा पैकेज](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip) डाउनलोड करें.</span><span class="sxs-lookup"><span data-stu-id="f5a6b-105">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="f5a6b-106">फ़ोल्डर *ProjOpsDemoDataSetupAndMaster - Integrated CMT* पर नेविगेट करें और निष्पादित फ़ाइल, *DataMigrationUtility* को चलाएं.</span><span class="sxs-lookup"><span data-stu-id="f5a6b-106">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="f5a6b-107">Common Data Service कॉन्फ़िगरेशन माइग्रेशन (CMT) विज़ार्ड के पेज 1 पर, **डेटा आयात करें** चुनें और फिर **जारी रखें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f5a6b-107">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![कॉन्फ़िगरेशन माइग्रेशन](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="f5a6b-109">CMT विज़ार्ड के पृष्ठ 2 पर **Office 365** के रूप में **परिनियोजन प्रकार**।</span><span class="sxs-lookup"><span data-stu-id="f5a6b-109">On Page 2 of the CMT Wizard, select **Office 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="f5a6b-110">**उपलब्ध संगठनों की सूची प्रदर्शित करें** और **उन्नत दिखाएं** चेक बॉक्स चुनें।</span><span class="sxs-lookup"><span data-stu-id="f5a6b-110">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="f5a6b-111">अपने किरायेदार के क्षेत्र का चयन करें, अपनी साख दर्ज करें, और फिर **लॉग-इन** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f5a6b-111">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

![साइन इन का कॉन्फ़िगरेशन करें](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="f5a6b-113">पृष्ठ 3 पर, किरायेदार पर संगठनों की सूची से, चुनें कि आप किस संगठन में डेमो डेटा आयात करना चाहते/चाहती हैं और फिर **लॉग-इन** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f5a6b-113">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="f5a6b-114">पृष्ठ 4 पर, जिप फाइल का चयन करें, अनपैक्ड फोल्डर से *MasterAndSetupData*, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span><span class="sxs-lookup"><span data-stu-id="f5a6b-114">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

![ज़िप फ़ाइल](./media/3ZipFile.png)

![किसी फ़ाइल का चयन करें](./media/4SelectAFile.png)

9. <span data-ttu-id="f5a6b-117">ज़िप फ़ाइल चुनने के बाद **डेटा आयात करें**चुनें।</span><span class="sxs-lookup"><span data-stu-id="f5a6b-117">After the zip file is selected, select **Import Data**.</span></span>

![डेटा आयात करें](./media/5ImportData.png)

10. <span data-ttu-id="f5a6b-119">आपके नेटवर्क की स्पीड के आधार पर आयात लगभग दो-दस मिनट तक चलेगा।</span><span class="sxs-lookup"><span data-stu-id="f5a6b-119">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="f5a6b-120">इसके पूरा होने के बाद, CMT विजार्ड से बाहर निकलें.</span><span class="sxs-lookup"><span data-stu-id="f5a6b-120">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="f5a6b-121">डेटा के लिए अपने संगठन की निम्नलिखित 20 निकायों में जांच करें:</span><span class="sxs-lookup"><span data-stu-id="f5a6b-121">Check your organization for data in the following 20 entities:</span></span>

- <span data-ttu-id="f5a6b-122">मुद्रा</span><span class="sxs-lookup"><span data-stu-id="f5a6b-122">Currency</span></span>
- <span data-ttu-id="f5a6b-123">संगठनात्मक इकाई</span><span class="sxs-lookup"><span data-stu-id="f5a6b-123">Organizational Unit</span></span>
- <span data-ttu-id="f5a6b-124">संपर्क</span><span class="sxs-lookup"><span data-stu-id="f5a6b-124">Contact</span></span>
- <span data-ttu-id="f5a6b-125">कर समूह</span><span class="sxs-lookup"><span data-stu-id="f5a6b-125">Tax Group</span></span>
- <span data-ttu-id="f5a6b-126">ग्राहक समूह</span><span class="sxs-lookup"><span data-stu-id="f5a6b-126">Customer Group</span></span>
- <span data-ttu-id="f5a6b-127">इकाई</span><span class="sxs-lookup"><span data-stu-id="f5a6b-127">Unit</span></span>
- <span data-ttu-id="f5a6b-128">इकाई समूह</span><span class="sxs-lookup"><span data-stu-id="f5a6b-128">Unit Group</span></span>
- <span data-ttu-id="f5a6b-129">मूल्य सूची</span><span class="sxs-lookup"><span data-stu-id="f5a6b-129">Price List</span></span>
- <span data-ttu-id="f5a6b-130">परियोजना पैरामीटर मूल्य सूची</span><span class="sxs-lookup"><span data-stu-id="f5a6b-130">Project Parameter Price List</span></span>
- <span data-ttu-id="f5a6b-131">इनवॉइस आवृत्ति</span><span class="sxs-lookup"><span data-stu-id="f5a6b-131">Invoice Frequency</span></span>
- <span data-ttu-id="f5a6b-132">इनवॉइस आवृत्ति विवरण</span><span class="sxs-lookup"><span data-stu-id="f5a6b-132">Invoice Frequency Detail</span></span>
- <span data-ttu-id="f5a6b-133">बुक करने योग्य संसाधन श्रेणी</span><span class="sxs-lookup"><span data-stu-id="f5a6b-133">Bookable Resource Category</span></span>
- <span data-ttu-id="f5a6b-134">लेनदेन श्रेणी</span><span class="sxs-lookup"><span data-stu-id="f5a6b-134">Transaction Category</span></span>
- <span data-ttu-id="f5a6b-135">व्यय श्रेणी</span><span class="sxs-lookup"><span data-stu-id="f5a6b-135">Expense Category</span></span>
- <span data-ttu-id="f5a6b-136">भूमिका मू्ल्य</span><span class="sxs-lookup"><span data-stu-id="f5a6b-136">Role Price</span></span>
- <span data-ttu-id="f5a6b-137">लेनदेन श्रेणी मूल्य</span><span class="sxs-lookup"><span data-stu-id="f5a6b-137">Transaction Category Price</span></span>
- <span data-ttu-id="f5a6b-138">विशेषता</span><span class="sxs-lookup"><span data-stu-id="f5a6b-138">Characteristic</span></span>
- <span data-ttu-id="f5a6b-139">बुक करने योग्य संसाधन</span><span class="sxs-lookup"><span data-stu-id="f5a6b-139">Bookable Resource</span></span>
- <span data-ttu-id="f5a6b-140">बुक करने योग्य संसाधन श्रेणी Assn</span><span class="sxs-lookup"><span data-stu-id="f5a6b-140">Bookable resource category Assn</span></span>
- <span data-ttu-id="f5a6b-141">बुक करने योग्य संसाधन विशेषता</span><span class="sxs-lookup"><span data-stu-id="f5a6b-141">Bookable Resource Characteristic</span></span>

![पूरा आयात](./media/6CompleteImport.png)
