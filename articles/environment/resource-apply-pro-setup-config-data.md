---
title: Common Data Service में कॉन्फ़िगरेशन डेटा सेट अप करें और लागू करें
description: यह विषय परियोजना संचालन में कॉन्फ़िगरेशन डेटा सेट अप करने और लागू करने के बारे में जानकारी प्रदान करता है।
author: sigitac
manager: Annbe
ms.date: 11/04/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 1651d3b3b85d3dc581bf61976fada249bafd6b7b
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5289821"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service"></a><span data-ttu-id="14660-103">Common Data Service में कॉन्फ़िगरेशन डेटा सेट अप करें और लागू करें</span><span class="sxs-lookup"><span data-stu-id="14660-103">Set up and apply configuration data in the Common Data Service</span></span> 

<span data-ttu-id="14660-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="14660-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="14660-105">पूर्वावश्यकताएँ</span><span class="sxs-lookup"><span data-stu-id="14660-105">Prerequisites</span></span>

<span data-ttu-id="14660-106">Common Data Service (CDS) में डेटा को कॉन्फ़िगर करना शुरू करने से पहले, निम्नलिखित आवश्यकताएं पूरी की जानी चाहिए:</span><span class="sxs-lookup"><span data-stu-id="14660-106">Before you beging to configure data in the Common Data Service (CDS), the following prerequisites must be met:</span></span>

1.  <span data-ttu-id="14660-107">Project Operations के लिए एक CDS परिवेश और एक Dynamics 365 Finance परिवेश प्रोविज़न करें.</span><span class="sxs-lookup"><span data-stu-id="14660-107">Provision a CDS environment and a Dynamics 365 Finance environment for Project Operations.</span></span>
2.  <span data-ttu-id="14660-108">Dynamics 365 Finance से कानूनी निकाय की जानकारी CDS परिवेश के साथ साझा की जाती है.</span><span class="sxs-lookup"><span data-stu-id="14660-108">Legal entity information from Dynamics 365 Finance is shared to the CDS environment.</span></span> <span data-ttu-id="14660-109">इसका मतलब है कि CDS में **कंपनी** निकाय के पास कंपनी के निम्नलिखित रिकॉर्ड हैं:</span><span class="sxs-lookup"><span data-stu-id="14660-109">This means that the **Company** entity in CDS has the following company records:</span></span>
  - <span data-ttu-id="14660-110">THPM</span><span class="sxs-lookup"><span data-stu-id="14660-110">THPM</span></span>
  - <span data-ttu-id="14660-111">USPM</span><span class="sxs-lookup"><span data-stu-id="14660-111">USPM</span></span>
  - <span data-ttu-id="14660-112">GBPM</span><span class="sxs-lookup"><span data-stu-id="14660-112">GBPM</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="14660-113">सेटअप और कॉन्फ़िगरेशन डेटा स्थापित करें</span><span class="sxs-lookup"><span data-stu-id="14660-113">Install setup and configuration data</span></span>

1. <span data-ttu-id="14660-114">[सेटअप और कॉन्फ़िगरेशन डेटा पैकेज](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip)को डाउनलोड करें, अनब्लॉक करें और अनज़िप करें।</span><span class="sxs-lookup"><span data-stu-id="14660-114">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span></span>
2. <span data-ttu-id="14660-115">अनज़िप किए गए फ़ोल्डर में जाएं और एक्सीक्यूट योग्य फ़ाइल, *DataMigrationUtility* चलाएं।</span><span class="sxs-lookup"><span data-stu-id="14660-115">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="14660-116">Common Data Service कॉन्फ़िगरेशन माइग्रेशन (CMT) विज़ार्ड के पेज 1 पर, **डेटा आयात करें** चुनें और फिर **जारी रखें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="14660-116">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![कॉन्फ़िगरेशन माइग्रेशन](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="14660-118">CMT विज़ार्ड के पृष्ठ 2 पर **परिनियोजन के प्रकार** के रूप में **Microsoft 365** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="14660-118">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="14660-119">**उपलब्ध संगठनों की सूची प्रदर्शित करें** और **उन्नत दिखाएं** चेक बॉक्स चुनें।</span><span class="sxs-lookup"><span data-stu-id="14660-119">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="14660-120">अपने टेनेंट के क्षेत्र का चयन करें, अपने क्रेडेंशियल दर्ज करें और **लॉगिन** चुनें।</span><span class="sxs-lookup"><span data-stu-id="14660-120">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![साइन इन का कॉन्फ़िगरेशन करें](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="14660-122">पृष्ठ 3 पर, टेनेंट पर संगठनों की सूची से, उस संगठन को चुनें जिसे आप डेमो डेटा आयात करना चाहते हैं और **लॉगिन** चुनें।</span><span class="sxs-lookup"><span data-stu-id="14660-122">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="14660-123">पृष्ठ 4 पर, अनपैक किए गए फ़ोल्डर से ज़िप फ़ाइल, *SampleSetupAndConfigData* चुनें।</span><span class="sxs-lookup"><span data-stu-id="14660-123">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![ज़िप फ़ाइल चयन](./media/3ZipFile.png)

![किसी फ़ाइल का चयन करें](./media/4SelectAFile.png)

9. <span data-ttu-id="14660-126">ज़िप फ़ाइल चुनने के बाद **डेटा आयात करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="14660-126">After the zip file is selected, select **Import Data**.</span></span>

![डेटा आयात करें](./media/5ImportData.png)

10. <span data-ttu-id="14660-128">आपके नेटवर्क की स्पीड के आधार पर आयात लगभग दो-दस मिनट तक चलेगा।</span><span class="sxs-lookup"><span data-stu-id="14660-128">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="14660-129">आयात पूर्ण होने के बाद, CMT विज़ार्ड से बाहर निकलें।</span><span class="sxs-lookup"><span data-stu-id="14660-129">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="14660-130">डेटा के लिए अपने संगठन की निम्नलिखित 19 निकायों में जांच करें:</span><span class="sxs-lookup"><span data-stu-id="14660-130">Check your organization for data in the following 19 entities:</span></span>

  - <span data-ttu-id="14660-131">मुद्रा</span><span class="sxs-lookup"><span data-stu-id="14660-131">Currency</span></span>
  - <span data-ttu-id="14660-132">संगठनात्मक इकाई</span><span class="sxs-lookup"><span data-stu-id="14660-132">Organizational Unit</span></span>
  - <span data-ttu-id="14660-133">संपर्क</span><span class="sxs-lookup"><span data-stu-id="14660-133">Contact</span></span>
  - <span data-ttu-id="14660-134">कर समूह</span><span class="sxs-lookup"><span data-stu-id="14660-134">Tax Group</span></span>
  - <span data-ttu-id="14660-135">ग्राहक समूह</span><span class="sxs-lookup"><span data-stu-id="14660-135">Customer Group</span></span>
  - <span data-ttu-id="14660-136">इकाई</span><span class="sxs-lookup"><span data-stu-id="14660-136">Unit</span></span>
  - <span data-ttu-id="14660-137">इकाई समूह</span><span class="sxs-lookup"><span data-stu-id="14660-137">Unit Group</span></span>
  - <span data-ttu-id="14660-138">मूल्य सूची</span><span class="sxs-lookup"><span data-stu-id="14660-138">Price List</span></span>
  - <span data-ttu-id="14660-139">परियोजना पैरामीटर मूल्य सूची</span><span class="sxs-lookup"><span data-stu-id="14660-139">Project Parameter Price List</span></span>
  - <span data-ttu-id="14660-140">इनवॉइस आवृत्ति</span><span class="sxs-lookup"><span data-stu-id="14660-140">Invoice Frequency</span></span>
  - <span data-ttu-id="14660-141">बुक करने योग्य संसाधन श्रेणी</span><span class="sxs-lookup"><span data-stu-id="14660-141">Bookable Resource Category</span></span>
  - <span data-ttu-id="14660-142">लेनदेन श्रेणी</span><span class="sxs-lookup"><span data-stu-id="14660-142">Transaction Category</span></span>
  - <span data-ttu-id="14660-143">व्यय श्रेणी</span><span class="sxs-lookup"><span data-stu-id="14660-143">Expense Category</span></span>
  - <span data-ttu-id="14660-144">भूमिका मू्ल्य</span><span class="sxs-lookup"><span data-stu-id="14660-144">Role Price</span></span>
  - <span data-ttu-id="14660-145">लेनदेन श्रेणी मूल्य</span><span class="sxs-lookup"><span data-stu-id="14660-145">Transaction Category Price</span></span>
  - <span data-ttu-id="14660-146">विशेषता</span><span class="sxs-lookup"><span data-stu-id="14660-146">Characteristic</span></span>
  - <span data-ttu-id="14660-147">बुक करने योग्य संसाधन</span><span class="sxs-lookup"><span data-stu-id="14660-147">Bookable Resource</span></span>
  - <span data-ttu-id="14660-148">बुक करने योग्य संसाधन श्रेणी Assn</span><span class="sxs-lookup"><span data-stu-id="14660-148">Bookable resource category Assn</span></span>
  - <span data-ttu-id="14660-149">बुक करने योग्य संसाधन विशेषता</span><span class="sxs-lookup"><span data-stu-id="14660-149">Bookable Resource Characteristic</span></span>

![पूरा आयात](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="14660-151">परियोजना संचालन कॉन्फ़िगरेशन अपडेट करें</span><span class="sxs-lookup"><span data-stu-id="14660-151">Update Project Operations configurations</span></span>

1. <span data-ttu-id="14660-152">CE परिवेश पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="14660-152">Navigate to the CE environment.</span></span> <span data-ttu-id="14660-153">आप इसे [Power Platform एडमिन सेंटर](https://admin.powerplatform.microsoft.com/environments) खोलकर, परिवेश चुनकर और फिर **परिवेश खोलें** चुनकर पा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="14660-153">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![परिवेश खोलें](./media/7OpenEnvironment.png)

2. <span data-ttu-id="14660-155">अपने उपयोगकर्ता के लिए बुक करने योग्य संसाधन बनाने के लिए **परियोजनाओं** > **संसाधन** पर जाएं और फिर **नया** चुनें।</span><span class="sxs-lookup"><span data-stu-id="14660-155">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![बुक करने योग्य संसाधन](./media/8BookableResources.png)

3. <span data-ttu-id="14660-157">**सामान्य** टैब पर, अपने व्यवस्थापक उपयोगकर्ता को चुनें।</span><span class="sxs-lookup"><span data-stu-id="14660-157">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="14660-158">सत्यापित करें कि समय क्षेत्र उससे मेल खाता है जिसमें आप हैं।</span><span class="sxs-lookup"><span data-stu-id="14660-158">Verify that the time zone matches the one you are in.</span></span> 

![न्यू बुक करने योग्य संसाधन](./media/9NewBookableResource.png)

4. <span data-ttu-id="14660-160">**कंपनी** फ़ील्ड में, **शेड्यूलिंग** टैब पर, **USPM** कंपनी चुनें और फिर **सहेजें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="14660-160">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![शेड्यूलिंग टैब](./media/10SchedulingTab.png)

5. <span data-ttu-id="14660-162">**कार्य घंटे** टैब चुनें।</span><span class="sxs-lookup"><span data-stu-id="14660-162">Select the **Work hours** tab.</span></span>  

![कार्य घंटे](./media/11WorkHours.png)

6. <span data-ttu-id="14660-164">कैलेंडर में किसी भी मान पर डबल क्लिक करें और **संपादित करें** > **श्रृंखला में सभी घटनाएं** ।</span><span class="sxs-lookup"><span data-stu-id="14660-164">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![कार्य कैलेंडर](./media/12WorkCalendar.png)

7. <span data-ttu-id="14660-166">काम के घंटों को आठ (8) घंटे के कार्य दिवस में बदलें, सप्ताहांत को गैर-कार्य दिवस के रूप में चिह्नित करें और सुनिश्चित करें कि समय क्षेत्र आपकी जगह से मेल खाता है।</span><span class="sxs-lookup"><span data-stu-id="14660-166">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="14660-167">**सहेजें और बंद करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="14660-167">Select **Save and close**.</span></span>

![कैलेंडर को अपडेट करें](./media/13UpdateCalendar.png)

9. <span data-ttu-id="14660-169">**सेटिंग्स** > **कैलेंडर टेम्प्लेट** पर जाएं और **नया** चुनें।</span><span class="sxs-lookup"><span data-stu-id="14660-169">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![कैलेंडर टेम्पलेट्स](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="14660-171">एक नाम दर्ज करें, आपके द्वारा बनाए गए टेम्पलेट संसाधन को चुनें और फिर **सहेजें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="14660-171">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![कैलेंडर टेम्पलेट सहेजें](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="14660-173">**मापदंड** पर जाएं और रिकॉर्ड पर डबल-क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="14660-173">Go to **Parameters** and double-click the record.</span></span> 
 
 ![परियोजना पैरामीटर्स](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="14660-175">निम्नलिखित फ़ील्ड अपडेट करें:</span><span class="sxs-lookup"><span data-stu-id="14660-175">Update the following fields:</span></span>

 - <span data-ttu-id="14660-176">**डिफ़ॉल्ट कंपनी**: USPM</span><span class="sxs-lookup"><span data-stu-id="14660-176">**Default company**: USPM</span></span>
 - <span data-ttu-id="14660-177">**डिफ़ॉल्ट संगठनात्मक इकाई**: Contoso रोबोटिक्स ग्लोबल</span><span class="sxs-lookup"><span data-stu-id="14660-177">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="14660-178">**इन्वॉइस फ्रीक्वेंसी**: सातवें और आखिरी दिन</span><span class="sxs-lookup"><span data-stu-id="14660-178">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="14660-179">**कार्य घंटे टेम्पलेट**: आपके द्वारा बनाए गए टेम्पलेट में बदलें।</span><span class="sxs-lookup"><span data-stu-id="14660-179">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="14660-180">**सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="14660-180">Select **Save**.</span></span> 

![अपडेट किए गए परियोजना मापदंड](./media/17UpdatedProjectParameters.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]