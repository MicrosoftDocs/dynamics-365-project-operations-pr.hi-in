---
title: परियोजना संचालन के लिए Common Data Service में कॉन्फ़िगरेशन डेटा सेट अप करें और लागू करें
description: यह विषय परियोजना संचालन में कॉन्फ़िगरेशन डेटा सेट अप करने और लागू करने के बारे में जानकारी प्रदान करता है।
author: sigitac
manager: Annbe
ms.date: 10/01/2020
ms.topic: article
ms.service: dynamics-365-customerservice
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 5e72b88a4dae1eb89859fdfd55f6d5e6ee5befcd
ms.sourcegitcommit: 11a61db54119503e82faec5f99c4273e8d1247e5
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077573"
---
# <a name="set-up-and-apply-configuration-data-in-the-common-data-service-for-project-operations"></a><span data-ttu-id="77cf2-103">परियोजना संचालन के लिए Common Data Service में कॉन्फ़िगरेशन डेटा सेट अप करें और लागू करें</span><span class="sxs-lookup"><span data-stu-id="77cf2-103">Set up and apply configuration data in the Common Data Service for Project Operations</span></span>

<span data-ttu-id="77cf2-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए परियोजना संचालन_</span><span class="sxs-lookup"><span data-stu-id="77cf2-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

## <a name="install-setup-and-configuration-data"></a><span data-ttu-id="77cf2-105">सेटअप और कॉन्फ़िगरेशन डेटा स्थापित करें</span><span class="sxs-lookup"><span data-stu-id="77cf2-105">Install setup and configuration data</span></span>

1. <span data-ttu-id="77cf2-106">[सेटअप और कॉन्फ़िगरेशन डेटा पैकेज](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip)को डाउनलोड करें, अनब्लॉक करें और अनज़िप करें।</span><span class="sxs-lookup"><span data-stu-id="77cf2-106">Download, unblock, and unzip the [Setup and Configuration Data Package](https://download.microsoft.com/download/1/3/4/1349369c-6209-42b7-b3b4-5be0e67cacd8/ProjOpsSampleSetupData-%20Integrated%20UR1.zip).</span></span>
2. <span data-ttu-id="77cf2-107">अनज़िप किए गए फ़ोल्डर में जाएं और एक्सीक्यूट योग्य फ़ाइल, *DataMigrationUtility* चलाएं।</span><span class="sxs-lookup"><span data-stu-id="77cf2-107">Navigate to the unzipped folder and run the executable file, *DataMigrationUtility*.</span></span>
3. <span data-ttu-id="77cf2-108">Common Data Service कॉन्फ़िगरेशन माइग्रेशन (CMT) विज़ार्ड के पेज 1 पर, **डेटा आयात करें** चुनें और फिर **जारी रखें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="77cf2-108">On page 1 of the Common Data Service Configuration Migration (CMT) Wizard, select **Import Data** and then select **Continue**.</span></span>

![कॉन्फ़िगरेशन माइग्रेशन](./media/1ConfigurationMigration.png)

4. <span data-ttu-id="77cf2-110">CMT विज़ार्ड के पृष्ठ 2 पर **परिनियोजन के प्रकार** के रूप में **Microsoft 365** का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="77cf2-110">On Page 2 of the CMT Wizard, select **Microsoft 365** as the **Deployment Type**.</span></span>
5. <span data-ttu-id="77cf2-111">**उपलब्ध संगठनों की सूची प्रदर्शित करें** और **उन्नत दिखाएं** चेक बॉक्स चुनें।</span><span class="sxs-lookup"><span data-stu-id="77cf2-111">Select the **Display a list of available organizations** and **Show Advanced** check boxes.</span></span>
6. <span data-ttu-id="77cf2-112">अपने टेनेंट के क्षेत्र का चयन करें, अपने क्रेडेंशियल दर्ज करें और **लॉगिन** चुनें।</span><span class="sxs-lookup"><span data-stu-id="77cf2-112">Select the region of your tenant, enter your credentials, and select **Login**.</span></span>

![साइन इन का कॉन्फ़िगरेशन करें](./media/2ConfigurationSignin.png)

7. <span data-ttu-id="77cf2-114">पृष्ठ 3 पर, टेनेंट पर संगठनों की सूची से, उस संगठन को चुनें जिसे आप डेमो डेटा आयात करना चाहते हैं और **लॉगिन** चुनें।</span><span class="sxs-lookup"><span data-stu-id="77cf2-114">On page 3, from the list of organizations on the tenant, select the organization you want to import the demo data into and select **Login**.</span></span>
8. <span data-ttu-id="77cf2-115">पृष्ठ 4 पर, अनपैक किए गए फ़ोल्डर से ज़िप फ़ाइल, *SampleSetupAndConfigData* चुनें।</span><span class="sxs-lookup"><span data-stu-id="77cf2-115">On page 4, select the zip file, *SampleSetupAndConfigData* from the unpacked folder.</span></span>

![ज़िप फ़ाइल चयन](./media/3ZipFile.png)

![किसी फ़ाइल का चयन करें](./media/4SelectAFile.png)

9. <span data-ttu-id="77cf2-118">ज़िप फ़ाइल चुनने के बाद **डेटा आयात करें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="77cf2-118">After the zip file is selected, select **Import Data**.</span></span>

![डेटा आयात करें](./media/5ImportData.png)

10. <span data-ttu-id="77cf2-120">आपके नेटवर्क की स्पीड के आधार पर आयात लगभग दो-दस मिनट तक चलेगा।</span><span class="sxs-lookup"><span data-stu-id="77cf2-120">Import will run for approximately two-ten minutes depending on your network speed.</span></span> <span data-ttu-id="77cf2-121">आयात पूर्ण होने के बाद, CMT विज़ार्ड से बाहर निकलें।</span><span class="sxs-lookup"><span data-stu-id="77cf2-121">After import completes, exit the CMT Wizard.</span></span> 
11. <span data-ttu-id="77cf2-122">डेटा के लिए अपने संगठन की निम्नलिखित 19 निकायों में जांच करें:</span><span class="sxs-lookup"><span data-stu-id="77cf2-122">Check your organization for data in the following 19 entities:</span></span>

  - <span data-ttu-id="77cf2-123">मुद्रा</span><span class="sxs-lookup"><span data-stu-id="77cf2-123">Currency</span></span>
  - <span data-ttu-id="77cf2-124">संगठनात्मक इकाई</span><span class="sxs-lookup"><span data-stu-id="77cf2-124">Organizational Unit</span></span>
  - <span data-ttu-id="77cf2-125">संपर्क</span><span class="sxs-lookup"><span data-stu-id="77cf2-125">Contact</span></span>
  - <span data-ttu-id="77cf2-126">कर समूह</span><span class="sxs-lookup"><span data-stu-id="77cf2-126">Tax Group</span></span>
  - <span data-ttu-id="77cf2-127">ग्राहक समूह</span><span class="sxs-lookup"><span data-stu-id="77cf2-127">Customer Group</span></span>
  - <span data-ttu-id="77cf2-128">इकाई</span><span class="sxs-lookup"><span data-stu-id="77cf2-128">Unit</span></span>
  - <span data-ttu-id="77cf2-129">इकाई समूह</span><span class="sxs-lookup"><span data-stu-id="77cf2-129">Unit Group</span></span>
  - <span data-ttu-id="77cf2-130">मूल्य सूची</span><span class="sxs-lookup"><span data-stu-id="77cf2-130">Price List</span></span>
  - <span data-ttu-id="77cf2-131">परियोजना पैरामीटर मूल्य सूची</span><span class="sxs-lookup"><span data-stu-id="77cf2-131">Project Parameter Price List</span></span>
  - <span data-ttu-id="77cf2-132">इनवॉइस आवृत्ति</span><span class="sxs-lookup"><span data-stu-id="77cf2-132">Invoice Frequency</span></span>
  - <span data-ttu-id="77cf2-133">बुक करने योग्य संसाधन श्रेणी</span><span class="sxs-lookup"><span data-stu-id="77cf2-133">Bookable Resource Category</span></span>
  - <span data-ttu-id="77cf2-134">लेनदेन श्रेणी</span><span class="sxs-lookup"><span data-stu-id="77cf2-134">Transaction Category</span></span>
  - <span data-ttu-id="77cf2-135">व्यय श्रेणी</span><span class="sxs-lookup"><span data-stu-id="77cf2-135">Expense Category</span></span>
  - <span data-ttu-id="77cf2-136">भूमिका मू्ल्य</span><span class="sxs-lookup"><span data-stu-id="77cf2-136">Role Price</span></span>
  - <span data-ttu-id="77cf2-137">लेनदेन श्रेणी मूल्य</span><span class="sxs-lookup"><span data-stu-id="77cf2-137">Transaction Category Price</span></span>
  - <span data-ttu-id="77cf2-138">विशेषता</span><span class="sxs-lookup"><span data-stu-id="77cf2-138">Characteristic</span></span>
  - <span data-ttu-id="77cf2-139">बुक करने योग्य संसाधन</span><span class="sxs-lookup"><span data-stu-id="77cf2-139">Bookable Resource</span></span>
  - <span data-ttu-id="77cf2-140">बुक करने योग्य संसाधन श्रेणी Assn</span><span class="sxs-lookup"><span data-stu-id="77cf2-140">Bookable resource category Assn</span></span>
  - <span data-ttu-id="77cf2-141">बुक करने योग्य संसाधन विशेषता</span><span class="sxs-lookup"><span data-stu-id="77cf2-141">Bookable Resource Characteristic</span></span>

![पूरा आयात](./media/6CompleteImport.png)

## <a name="update-project-operations-configurations"></a><span data-ttu-id="77cf2-143">परियोजना संचालन कॉन्फ़िगरेशन अपडेट करें</span><span class="sxs-lookup"><span data-stu-id="77cf2-143">Update Project Operations configurations</span></span>

1. <span data-ttu-id="77cf2-144">CE परिवेश पर जाएं।</span><span class="sxs-lookup"><span data-stu-id="77cf2-144">Navigate to the CE environment.</span></span> <span data-ttu-id="77cf2-145">आप इसे [Power Platform एडमिन सेंटर](https://admin.powerplatform.microsoft.com/environments) खोलकर, परिवेश चुनकर और फिर **परिवेश खोलें** चुनकर पा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="77cf2-145">You can find it by opening the [Power Platform Admin Center](https://admin.powerplatform.microsoft.com/environments), selecting the environment, and then selecting **Open Environment**.</span></span> 

![परिवेश खोलें](./media/7OpenEnvironment.png)

2. <span data-ttu-id="77cf2-147">अपने उपयोगकर्ता के लिए बुक करने योग्य संसाधन बनाने के लिए **परियोजनाओं** > **संसाधन** पर जाएं और फिर **नया** चुनें।</span><span class="sxs-lookup"><span data-stu-id="77cf2-147">Go to **Projects** > **Resources** and then select **New** to create a bookable resource for your user.</span></span>

![बुक करने योग्य संसाधन](./media/8BookableResources.png)

3. <span data-ttu-id="77cf2-149">**सामान्य** टैब पर, अपने व्यवस्थापक उपयोगकर्ता को चुनें।</span><span class="sxs-lookup"><span data-stu-id="77cf2-149">On the **General** tab, select your admin user.</span></span> <span data-ttu-id="77cf2-150">सत्यापित करें कि समय क्षेत्र उससे मेल खाता है जिसमें आप हैं।</span><span class="sxs-lookup"><span data-stu-id="77cf2-150">Verify that the time zone matches the one you are in.</span></span> 

![न्यू बुक करने योग्य संसाधन](./media/9NewBookableResource.png)

4. <span data-ttu-id="77cf2-152">**कंपनी** फ़ील्ड में, **शेड्यूलिंग** टैब पर, **USPM** कंपनी चुनें और फिर **सहेजें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="77cf2-152">On the **Scheduling** tab, in the **Company** field, pick the **USPM** company, and then select **Save**.</span></span> 

![शेड्यूलिंग टैब](./media/10SchedulingTab.png)

5. <span data-ttu-id="77cf2-154">**कार्य घंटे** टैब चुनें।</span><span class="sxs-lookup"><span data-stu-id="77cf2-154">Select the **Work hours** tab.</span></span>  

![कार्य घंटे](./media/11WorkHours.png)

6. <span data-ttu-id="77cf2-156">कैलेंडर में किसी भी मान पर डबल क्लिक करें और **संपादित करें** > **श्रृंखला में सभी घटनाएं** ।</span><span class="sxs-lookup"><span data-stu-id="77cf2-156">Double-click on any value in the calendar and select **Edit** > **All events in the series**.</span></span> 

![कार्य कैलेंडर](./media/12WorkCalendar.png)

7. <span data-ttu-id="77cf2-158">काम के घंटों को आठ (8) घंटे के कार्य दिवस में बदलें, सप्ताहांत को गैर-कार्य दिवस के रूप में चिह्नित करें और सुनिश्चित करें कि समय क्षेत्र आपकी जगह से मेल खाता है।</span><span class="sxs-lookup"><span data-stu-id="77cf2-158">Change work hours to an eight (8) hour work day, mark weekends as non-work days, and make sure time zone matches yours.</span></span> 
8. <span data-ttu-id="77cf2-159">**सहेजें और बंद करें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="77cf2-159">Select **Save and close**.</span></span>

![कैलेंडर को अपडेट करें](./media/13UpdateCalendar.png)

9. <span data-ttu-id="77cf2-161">**सेटिंग्स** > **कैलेंडर टेम्प्लेट** पर जाएं और **नया** चुनें।</span><span class="sxs-lookup"><span data-stu-id="77cf2-161">Go to **Settings** > **Calendar templates** and select **New**.</span></span>
 
 ![कैलेंडर टेम्पलेट्स](./media/14CalendarTemplates.png)
 
 10. <span data-ttu-id="77cf2-163">एक नाम दर्ज करें, आपके द्वारा बनाए गए टेम्पलेट संसाधन को चुनें और फिर **सहेजें** चुनें।</span><span class="sxs-lookup"><span data-stu-id="77cf2-163">Enter a name, select the template resource you created, and then select **Save**.</span></span> 
 
 ![कैलेंडर टेम्पलेट सहेजें](./media/15SaveCalendarTemplate.png)
 
 11. <span data-ttu-id="77cf2-165">**मापदंड** पर जाएं और रिकॉर्ड पर डबल-क्लिक करें।</span><span class="sxs-lookup"><span data-stu-id="77cf2-165">Go to **Parameters** and double-click the record.</span></span> 
 
 ![परियोजना पैरामीटर्स](./media/16ProjectParameters.png)
 
12. <span data-ttu-id="77cf2-167">निम्नलिखित फ़ील्ड अपडेट करें:</span><span class="sxs-lookup"><span data-stu-id="77cf2-167">Update the following fields:</span></span>

 - <span data-ttu-id="77cf2-168">**डिफ़ॉल्ट कंपनी** : USPM</span><span class="sxs-lookup"><span data-stu-id="77cf2-168">**Default company** : USPM</span></span>
 - <span data-ttu-id="77cf2-169">**डिफ़ॉल्ट संगठनात्मक इकाई** : Contoso रोबोटिक्स ग्लोबल</span><span class="sxs-lookup"><span data-stu-id="77cf2-169">**Default Organizational Unit** : Contoso Robotics Global</span></span>
 - <span data-ttu-id="77cf2-170">**इन्वॉइस फ्रीक्वेंसी** : सातवें और आखिरी दिन</span><span class="sxs-lookup"><span data-stu-id="77cf2-170">**Invoice Frequency** : Seventh and Last day</span></span>
 - <span data-ttu-id="77cf2-171">**कार्य घंटे टेम्पलेट** : आपके द्वारा बनाए गए टेम्पलेट में बदलें।</span><span class="sxs-lookup"><span data-stu-id="77cf2-171">**Work hour template** : Change to the template you created.</span></span>

13. <span data-ttu-id="77cf2-172">**सहेजें** चुनें.</span><span class="sxs-lookup"><span data-stu-id="77cf2-172">Select **Save**.</span></span> 

![अपडेट किए गए परियोजना मापदंड](./media/17UpdatedProjectParameters.png)
