---
title: डेमो सेटअप और कॉन्फ़िगरेशन डेटा लागू करें - लाइट
description: यह विषय Project Operations के लिए डेमो सेटअप और कॉन्फ़िगरेशन डेटा लागू करने के तरीके के बारे में जानकारी प्रदान करता है.
author: sigitac
manager: Annbe
ms.date: 01/27/2021
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 762b0cf317d442565a033f56033a53a5b5cc435c
ms.sourcegitcommit: b4298ca4729643c1040ef35dde8c67f829461ce7
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 01/29/2021
ms.locfileid: "5089121"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a><span data-ttu-id="09306-103">Project Operations के लिए डेमो सेटअप और कॉन्फ़िगरेशन डेटा लागू करें - लाइट</span><span class="sxs-lookup"><span data-stu-id="09306-103">Apply demo setup and configuration data for Project Operations - lite</span></span> 

<span data-ttu-id="09306-104">_\*\*लाइट परिनियोजन - प्रोफ़ॉर्मा इनवॉइस करने के लिए डील_</span><span class="sxs-lookup"><span data-stu-id="09306-104">_\*\*Lite deployment - deal to proforma invoicing_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="09306-105">पूर्वावश्यकताएँ</span><span class="sxs-lookup"><span data-stu-id="09306-105">Prerequisites</span></span>

<span data-ttu-id="09306-106">कॉन्फ़िगरेशन शुरू करने से पहले, आपके पास Dynamics 365 Project Operations के लिए एक Common Data Service (CDS) परिवेश प्रोविज़न किया गया होना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="09306-106">Before you begin the configuration, you must have a Common Data Service (CDS) environment provisioned for Dynamics 365 Project Operations.</span></span>


## <a name="instructions"></a><span data-ttu-id="09306-107">निर्देश</span><span class="sxs-lookup"><span data-stu-id="09306-107">Instructions</span></span>

1. <span data-ttu-id="09306-108">[मास्टर डेटा पैकेज](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip) डाउनलोड करें.</span><span class="sxs-lookup"><span data-stu-id="09306-108">Download the [Master Data Package](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData%20-%20CE%20only%20CMT.zip).</span></span> 
2. <span data-ttu-id="09306-109">फ़ोल्डर *ProjOpsDemoDataSetupAndMaster - Integrated CMT* पर नेविगेट करें और निष्पादित फ़ाइल, *DataMigrationUtility* को चलाएं.</span><span class="sxs-lookup"><span data-stu-id="09306-109">Navigate to the folder *ProjOpsDemoDataSetupAndMaster - Integrated CMT* and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="09306-110">Common Data Service कॉन्फ़िगरेशन माइग्रेशन (CMT) विज़ार्ड के पेज 1 पर, **डेटा आयात करें** चुनें और फिर **जारी रखें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="09306-110">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

    ![कॉन्फ़िगरेशन माइग्रेशन](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="09306-112">CMT विज़ार्ड के पृष्ठ 2 पर **परिनियोजन के प्रकार** के रूप में **Microsoft 365** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="09306-112">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="09306-113">**उपलब्ध संगठनों की सूची प्रदर्शित करें** और **उन्नत दिखाएं** चेक बॉक्स चुनें।</span><span class="sxs-lookup"><span data-stu-id="09306-113">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="09306-114">अपने किरायेदार के क्षेत्र का चयन करें, अपनी साख दर्ज करें, और फिर **लॉग-इन** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="09306-114">Select the region of your tenant, enter your credentials, and then select **Login**.</span></span>

   ![साइन इन का कॉन्फ़िगरेशन करें](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="09306-116">पृष्ठ 3 पर, किरायेदार पर संगठनों की सूची से, चुनें कि आप किस संगठन में डेमो डेटा आयात करना चाहते/चाहती हैं और फिर **लॉग-इन** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="09306-116">On page 3, from the list of Organizations on the Tenant, select which organization you want to import the demo data into and then select **Login**.</span></span>
8. <span data-ttu-id="09306-117">पृष्ठ 4 पर, जिप फाइल का चयन करें, अनपैक्ड फोल्डर से *MasterAndSetupData*, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span><span class="sxs-lookup"><span data-stu-id="09306-117">On page 4, select the zip file, *MasterAndSetupData* from the unpacked folder, *ProjOpsDemoDataSetupAndMaster - Integrated CMT*.</span></span>

   ![ज़िप फ़ाइल](./media/3ZipFile.png)

   ![किसी फ़ाइल का चयन करें](./media/4SelectAFile.png)

9. <span data-ttu-id="09306-120">ज़िप फ़ाइल चुनने के बाद **डेटा आयात करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="09306-120">After the zip file is selected, select **Import Data**.</span></span>

   ![डेटा आयात करें](./media/5ImportData.png)

10. <span data-ttu-id="09306-122">आपके नेटवर्क की स्पीड के आधार पर आयात लगभग दो-दस मिनट तक चलेगा।</span><span class="sxs-lookup"><span data-stu-id="09306-122">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="09306-123">इसके पूरा होने के बाद, CMT विजार्ड से बाहर निकलें.</span><span class="sxs-lookup"><span data-stu-id="09306-123">After it completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="09306-124">डेटा के लिए अपने संगठन की निम्नलिखित 20 निकायों में जांच करें:</span><span class="sxs-lookup"><span data-stu-id="09306-124">Check your organization for data in the following 20 entities:</span></span>

    -   <span data-ttu-id="09306-125">मुद्रा</span><span class="sxs-lookup"><span data-stu-id="09306-125">Currency</span></span>
    -   <span data-ttu-id="09306-126">खाता</span><span class="sxs-lookup"><span data-stu-id="09306-126">Account</span></span>
    -   <span data-ttu-id="09306-127">संगठनात्मक इकाई</span><span class="sxs-lookup"><span data-stu-id="09306-127">Organizational Unit</span></span>
    -   <span data-ttu-id="09306-128">संपर्क</span><span class="sxs-lookup"><span data-stu-id="09306-128">Contact</span></span>
    -   <span data-ttu-id="09306-129">इकाई</span><span class="sxs-lookup"><span data-stu-id="09306-129">Unit</span></span>
    -   <span data-ttu-id="09306-130">इकाई समूह</span><span class="sxs-lookup"><span data-stu-id="09306-130">Unit Group</span></span>
    -   <span data-ttu-id="09306-131">मूल्य सूची</span><span class="sxs-lookup"><span data-stu-id="09306-131">Price List</span></span>
    -   <span data-ttu-id="09306-132">परियोजना पैरामीटर मूल्य सूची</span><span class="sxs-lookup"><span data-stu-id="09306-132">Project Parameter Price List</span></span> 
    -   <span data-ttu-id="09306-133">इनवॉइस आवृत्ति</span><span class="sxs-lookup"><span data-stu-id="09306-133">Invoice Frequency</span></span>
    -   <span data-ttu-id="09306-134">बुक करने योग्य संसाधन श्रेणी</span><span class="sxs-lookup"><span data-stu-id="09306-134">Bookable Resource Category</span></span>
    -   <span data-ttu-id="09306-135">लेनदेन श्रेणी</span><span class="sxs-lookup"><span data-stu-id="09306-135">Transaction Category</span></span>
    -   <span data-ttu-id="09306-136">व्यय श्रेणी</span><span class="sxs-lookup"><span data-stu-id="09306-136">Expense Category</span></span>
    -   <span data-ttu-id="09306-137">भूमिका मू्ल्य</span><span class="sxs-lookup"><span data-stu-id="09306-137">Role Price</span></span>
    -   <span data-ttu-id="09306-138">लेनदेन श्रेणी मूल्य</span><span class="sxs-lookup"><span data-stu-id="09306-138">Transaction Category Price</span></span>
    -   <span data-ttu-id="09306-139">विशेषता</span><span class="sxs-lookup"><span data-stu-id="09306-139">Characteristic</span></span>
    -   <span data-ttu-id="09306-140">बुक करने योग्य संसाधन</span><span class="sxs-lookup"><span data-stu-id="09306-140">Bookable Resource</span></span>
    -   <span data-ttu-id="09306-141">बुक करने योग्य संसाधन श्रेणी Assn</span><span class="sxs-lookup"><span data-stu-id="09306-141">Bookable resource category Assn</span></span>
    -   <span data-ttu-id="09306-142">बुक करने योग्य संसाधन विशेषता</span><span class="sxs-lookup"><span data-stu-id="09306-142">Bookable Resource Characteristic</span></span>

    ![पूरा आयात](./media/6CompleteImport.png)
