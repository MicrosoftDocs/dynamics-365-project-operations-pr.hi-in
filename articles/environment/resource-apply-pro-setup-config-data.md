---
title: Common Data Service में कॉन्फ़िगरेशन डेटा सेट अप करें और लागू करें
description: यह विषय परियोजना संचालन में कॉन्फ़िगरेशन डेटा सेट अप करने और लागू करने के बारे में जानकारी प्रदान करता है।
author: sigitac
ms.date: 05/10/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 2ea00df6112fb69b61f1889463424fdfee79aec9
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6001293"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service"></a><span data-ttu-id="f5aee-103">Common Data Service में कॉन्फ़िगरेशन डेटा सेट अप करें और लागू करें</span><span class="sxs-lookup"><span data-stu-id="f5aee-103">Set up and apply configuration data in the Common Data Service</span></span> 

<span data-ttu-id="f5aee-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations_</span><span class="sxs-lookup"><span data-stu-id="f5aee-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

[!include [rename-banner](~/includes/cc-data-platform-banner.md)]

## <a name="prerequisites"></a><span data-ttu-id="f5aee-105">पूर्वावश्यकताएँ</span><span class="sxs-lookup"><span data-stu-id="f5aee-105">Prerequisites</span></span>

<span data-ttu-id="f5aee-106">इससे पहले कि आप Common Data Service (CDS) में डेटा कॉन्फ़िगर करना शुरू करें, निम्नलिखित शर्तें पूरी होनी चाहिए:</span><span class="sxs-lookup"><span data-stu-id="f5aee-106">Before you begin to configure data in the Common Data Service (CDS), the following prerequisites must be met:</span></span>

1.  <span data-ttu-id="f5aee-107">Project Operations के लिए एक CDS परिवेश और एक Dynamics 365 Finance परिवेश प्रोविज़न करें.</span><span class="sxs-lookup"><span data-stu-id="f5aee-107">Provision a CDS environment and a Dynamics 365 Finance environment for Project Operations.</span></span>
2.  <span data-ttu-id="f5aee-108">Dynamics 365 Finance से कानूनी निकाय की जानकारी CDS परिवेश के साथ साझा की जाती है.</span><span class="sxs-lookup"><span data-stu-id="f5aee-108">Legal entity information from Dynamics 365 Finance is shared to the CDS environment.</span></span> <span data-ttu-id="f5aee-109">इसका मतलब है कि CDS में **कंपनी** निकाय के पास कंपनी के निम्नलिखित रिकॉर्ड हैं:</span><span class="sxs-lookup"><span data-stu-id="f5aee-109">This means that the **Company** entity in CDS has the following company records:</span></span>
  - <span data-ttu-id="f5aee-110">THPM</span><span class="sxs-lookup"><span data-stu-id="f5aee-110">THPM</span></span>
  - <span data-ttu-id="f5aee-111">USPM</span><span class="sxs-lookup"><span data-stu-id="f5aee-111">USPM</span></span>
  - <span data-ttu-id="f5aee-112">GBPM</span><span class="sxs-lookup"><span data-stu-id="f5aee-112">GBPM</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="f5aee-113">सेटअप और कॉन्फ़िगरेशन डेटा स्थापित करें</span><span class="sxs-lookup"><span data-stu-id="f5aee-113">Install setup and configuration data</span></span>

1. <span data-ttu-id="f5aee-114">[सेटअप और कॉन्फ़िगरेशन डेटा पैकेज](https://download.microsoft.com/download/e/2/d/e2da6c98-d5dd-450c-aabe-fd6bf2ba374b/ProjOpsSampleSetupData-%20Integrated%20Latest.zip)को डाउनलोड करें, अनब्लॉक करें और अनज़िप करें।</span><span class="sxs-lookup"><span data-stu-id="f5aee-114">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/e/2/d/e2da6c98-d5dd-450c-aabe-fd6bf2ba374b/ProjOpsSampleSetupData-%20Integrated%20Latest.zip).</span></span>
2. <span data-ttu-id="f5aee-115">अनज़िप किए गए फ़ोल्डर में जाएं और एक्सीक्यूट योग्य फ़ाइल, *DataMigrationUtility* चलाएं।</span><span class="sxs-lookup"><span data-stu-id="f5aee-115">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="f5aee-116">Common Data Service कॉन्फ़िगरेशन माइग्रेशन (CMT) विज़ार्ड के पेज 1 पर, **डेटा आयात करें** चुनें और फिर **जारी रखें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f5aee-116">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![कॉन्फ़िगरेशन माइग्रेशन](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="f5aee-118">CMT विज़ार्ड के पृष्ठ 2 पर **परिनियोजन के प्रकार** के रूप में **Microsoft 365** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="f5aee-118">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="f5aee-119">**उपलब्ध संगठनों की सूची प्रदर्शित करें** और **उन्नत दिखाएं** चेक बॉक्स चुनें।</span><span class="sxs-lookup"><span data-stu-id="f5aee-119">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="f5aee-120">अपने टेनेंट के क्षेत्र का चयन करें, अपने क्रेडेंशियल दर्ज करें और **लॉगिन** चुनें।</span><span class="sxs-lookup"><span data-stu-id="f5aee-120">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![साइन इन का कॉन्फ़िगरेशन करें](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="f5aee-122">पृष्ठ 3 पर, टेनेंट पर संगठनों की सूची से, उस संगठन को चुनें जिसे आप डेमो डेटा आयात करना चाहते हैं और **लॉगिन** चुनें।</span><span class="sxs-lookup"><span data-stu-id="f5aee-122">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="f5aee-123">पृष्ठ 4 पर, अनपैक किए गए फ़ोल्डर से ज़िप फ़ाइल, *SampleSetupAndConfigData* चुनें।</span><span class="sxs-lookup"><span data-stu-id="f5aee-123">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![ज़िप फ़ाइल चयन](./media/3ZipFile.png)

![किसी फ़ाइल का चयन करें](./media/4SelectAFile.png)

9. <span data-ttu-id="f5aee-126">ज़िप फ़ाइल चुनने के बाद **डेटा आयात करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="f5aee-126">After the zip file is selected, select **Import Data**.</span></span>

![डेटा आयात करें](./media/5ImportData.png)

10. <span data-ttu-id="f5aee-128">आपके नेटवर्क की स्पीड के आधार पर आयात लगभग दो-दस मिनट तक चलेगा।</span><span class="sxs-lookup"><span data-stu-id="f5aee-128">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="f5aee-129">आयात पूर्ण होने के बाद, CMT विज़ार्ड से बाहर निकलें।</span><span class="sxs-lookup"><span data-stu-id="f5aee-129">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="f5aee-130">डेटा के लिए अपने संगठन की निम्नलिखित 26 निकायों में जांच करें:</span><span class="sxs-lookup"><span data-stu-id="f5aee-130">Check your organization for data in the following 26 entities:</span></span>

  - <span data-ttu-id="f5aee-131">मुद्रा</span><span class="sxs-lookup"><span data-stu-id="f5aee-131">Currency</span></span>
  - <span data-ttu-id="f5aee-132">खातों का चार्ट</span><span class="sxs-lookup"><span data-stu-id="f5aee-132">Chart of Accounts</span></span>
  - <span data-ttu-id="f5aee-133">वित्त कैलेंडर</span><span class="sxs-lookup"><span data-stu-id="f5aee-133">Fiscal Calendar</span></span>
  - <span data-ttu-id="f5aee-134">मुद्रा विनिमय दर प्रकार</span><span class="sxs-lookup"><span data-stu-id="f5aee-134">Currency Exchange Rate Types</span></span>
  - <span data-ttu-id="f5aee-135">भुगतान दिन</span><span class="sxs-lookup"><span data-stu-id="f5aee-135">Payment Day</span></span>
  - <span data-ttu-id="f5aee-136">भुगतान शेड्यूल</span><span class="sxs-lookup"><span data-stu-id="f5aee-136">Payment Schedule</span></span>
  - <span data-ttu-id="f5aee-137">भुगतान अवधि</span><span class="sxs-lookup"><span data-stu-id="f5aee-137">Payment Term</span></span>
  - <span data-ttu-id="f5aee-138">संगठनात्मक इकाई</span><span class="sxs-lookup"><span data-stu-id="f5aee-138">Organizational Unit</span></span>
  - <span data-ttu-id="f5aee-139">संपर्क</span><span class="sxs-lookup"><span data-stu-id="f5aee-139">Contact</span></span>
  - <span data-ttu-id="f5aee-140">कर समूह</span><span class="sxs-lookup"><span data-stu-id="f5aee-140">Tax Group</span></span>
  - <span data-ttu-id="f5aee-141">ग्राहक समूह</span><span class="sxs-lookup"><span data-stu-id="f5aee-141">Customer Group</span></span>
  - <span data-ttu-id="f5aee-142">विक्रेता समूह</span><span class="sxs-lookup"><span data-stu-id="f5aee-142">Vendor Group</span></span>
  - <span data-ttu-id="f5aee-143">इकाई</span><span class="sxs-lookup"><span data-stu-id="f5aee-143">Unit</span></span>
  - <span data-ttu-id="f5aee-144">इकाई समूह</span><span class="sxs-lookup"><span data-stu-id="f5aee-144">Unit Group</span></span>
  - <span data-ttu-id="f5aee-145">मूल्य सूची</span><span class="sxs-lookup"><span data-stu-id="f5aee-145">Price List</span></span>
  - <span data-ttu-id="f5aee-146">परियोजना पैरामीटर मूल्य सूची</span><span class="sxs-lookup"><span data-stu-id="f5aee-146">Project Parameter Price List</span></span>
  - <span data-ttu-id="f5aee-147">इनवॉइस आवृत्ति</span><span class="sxs-lookup"><span data-stu-id="f5aee-147">Invoice Frequency</span></span>
  - <span data-ttu-id="f5aee-148">बुक करने योग्य संसाधन श्रेणी</span><span class="sxs-lookup"><span data-stu-id="f5aee-148">Bookable Resource Category</span></span>
  - <span data-ttu-id="f5aee-149">लेनदेन श्रेणी</span><span class="sxs-lookup"><span data-stu-id="f5aee-149">Transaction Category</span></span>
  - <span data-ttu-id="f5aee-150">व्यय श्रेणी</span><span class="sxs-lookup"><span data-stu-id="f5aee-150">Expense Category</span></span>
  - <span data-ttu-id="f5aee-151">भूमिका मू्ल्य</span><span class="sxs-lookup"><span data-stu-id="f5aee-151">Role Price</span></span>
  - <span data-ttu-id="f5aee-152">लेनदेन श्रेणी मूल्य</span><span class="sxs-lookup"><span data-stu-id="f5aee-152">Transaction Category Price</span></span>
  - <span data-ttu-id="f5aee-153">विशेषता</span><span class="sxs-lookup"><span data-stu-id="f5aee-153">Characteristic</span></span>
  - <span data-ttu-id="f5aee-154">बुक करने योग्य संसाधन</span><span class="sxs-lookup"><span data-stu-id="f5aee-154">Bookable Resource</span></span>
  - <span data-ttu-id="f5aee-155">बुक करने योग्य संसाधन श्रेणी Assn</span><span class="sxs-lookup"><span data-stu-id="f5aee-155">Bookable resource category Assn</span></span>
  - <span data-ttu-id="f5aee-156">बुक करने योग्य संसाधन विशेषता</span><span class="sxs-lookup"><span data-stu-id="f5aee-156">Bookable Resource Characteristic</span></span>

![पूरा आयात](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="f5aee-158">परियोजना संचालन कॉन्फ़िगरेशन अपडेट करें</span><span class="sxs-lookup"><span data-stu-id="f5aee-158">Update Project Operations configurations</span></span>

1. <span data-ttu-id="f5aee-159">CE परिवेश पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="f5aee-159">Navigate to the CE environment.</span></span> <span data-ttu-id="f5aee-160">आप इसे [Power Platform एडमिन सेंटर](https://admin.powerplatform.microsoft.com/environments) खोलकर, परिवेश चुनकर और फिर **परिवेश खोलें** चुनकर पा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="f5aee-160">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![परिवेश खोलें](./media/7OpenEnvironment.png)

2. <span data-ttu-id="f5aee-162">अपने उपयोगकर्ता के लिए बुक करने योग्य संसाधन बनाने के लिए **परियोजनाओं** > **संसाधन** पर जाएं और फिर **नया** चुनें।</span><span class="sxs-lookup"><span data-stu-id="f5aee-162">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![बुक करने योग्य संसाधन](./media/8BookableResources.png)

3. <span data-ttu-id="f5aee-164">**सामान्य** टैब पर, अपने व्यवस्थापक उपयोगकर्ता को चुनें।</span><span class="sxs-lookup"><span data-stu-id="f5aee-164">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="f5aee-165">सत्यापित करें कि समय क्षेत्र उससे मेल खाता है जिसमें आप हैं।</span><span class="sxs-lookup"><span data-stu-id="f5aee-165">Verify that the time zone matches the one you are in.</span></span> 

![न्यू बुक करने योग्य संसाधन](./media/9NewBookableResource.png)

4. <span data-ttu-id="f5aee-167">**कंपनी** फ़ील्ड में, **शेड्यूलिंग** टैब पर, **USPM** कंपनी चुनें और फिर **सहेजें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="f5aee-167">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![शेड्यूलिंग टैब](./media/10SchedulingTab.png)

5. <span data-ttu-id="f5aee-169">**कार्य घंटे** टैब चुनें।</span><span class="sxs-lookup"><span data-stu-id="f5aee-169">Select the **Work hours** tab.</span></span>  

![कार्य घंटे](./media/11WorkHours.png)

6. <span data-ttu-id="f5aee-171">कैलेंडर में किसी भी मान पर डबल क्लिक करें और **संपादित करें** > **श्रृंखला में सभी घटनाएं** ।</span><span class="sxs-lookup"><span data-stu-id="f5aee-171">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![कार्य कैलेंडर](./media/12WorkCalendar.png)

7. <span data-ttu-id="f5aee-173">काम के घंटों को आठ (8) घंटे के कार्य दिवस में बदलें, सप्ताहांत को गैर-कार्य दिवस के रूप में चिह्नित करें और सुनिश्चित करें कि समय क्षेत्र आपकी जगह से मेल खाता है।</span><span class="sxs-lookup"><span data-stu-id="f5aee-173">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="f5aee-174">**सहेजें और बंद करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f5aee-174">Select **Save and close**.</span></span>

![कैलेंडर को अपडेट करें](./media/13UpdateCalendar.png)

9. <span data-ttu-id="f5aee-176">**सेटिंग्स** > **कैलेंडर टेम्प्लेट** पर जाएं और **नया** चुनें।</span><span class="sxs-lookup"><span data-stu-id="f5aee-176">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![कैलेंडर टेम्पलेट्स](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="f5aee-178">एक नाम दर्ज करें, आपके द्वारा बनाए गए टेम्पलेट संसाधन को चुनें और फिर **सहेजें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="f5aee-178">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![कैलेंडर टेम्पलेट सहेजें](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="f5aee-180">**मापदंड** पर जाएं और रिकॉर्ड पर डबल-क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="f5aee-180">Go to **Parameters** and double-click the record.</span></span> 
 
 ![परियोजना पैरामीटर्स](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="f5aee-182">निम्नलिखित फ़ील्ड अपडेट करें:</span><span class="sxs-lookup"><span data-stu-id="f5aee-182">Update the following fields:</span></span>

 - <span data-ttu-id="f5aee-183">**डिफ़ॉल्ट कंपनी**: USPM</span><span class="sxs-lookup"><span data-stu-id="f5aee-183">**Default company**: USPM</span></span>
 - <span data-ttu-id="f5aee-184">**डिफ़ॉल्ट संगठनात्मक इकाई**: Contoso रोबोटिक्स ग्लोबल</span><span class="sxs-lookup"><span data-stu-id="f5aee-184">**Default Organizational Unit**: Contoso Robotics Global</span></span>
 - <span data-ttu-id="f5aee-185">**इन्वॉइस फ्रीक्वेंसी**: सातवें और आखिरी दिन</span><span class="sxs-lookup"><span data-stu-id="f5aee-185">**Invoice Frequency**: Seventh and Last day</span></span>
 - <span data-ttu-id="f5aee-186">**कार्य घंटे टेम्पलेट**: आपके द्वारा बनाए गए टेम्पलेट में बदलें।</span><span class="sxs-lookup"><span data-stu-id="f5aee-186">**Work hour template**: Change to the template you created.</span></span>

13. <span data-ttu-id="f5aee-187">**सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="f5aee-187">Select **Save**.</span></span> 

![अपडेट किए गए परियोजना मापदंड](./media/17UpdatedProjectParameters.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
