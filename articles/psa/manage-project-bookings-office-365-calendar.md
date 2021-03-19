---
title: अपने Office 365 कैलेंडर में प्रोजेक्ट और बुकिंग को व्यवस्थित करना
description: अपने Office 365 कैलेंडर में प्रोजेक्ट और बुकिंग को कैसे व्यवस्थित करें
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 8/03/2018
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: 1df4864ca8dbf6948ca88a7c82a6c0a676e3bd53
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5275045"
---
# <a name="manage-projects-and-bookings-in-your-calendar-project-service"></a><span data-ttu-id="68891-103">अपने कैलेंडर में प्रोजेक्ट और बुकिंग को व्यवस्थित करना (Project Service)</span><span class="sxs-lookup"><span data-stu-id="68891-103">Manage projects and bookings in your calendar (Project Service)</span></span>

> [!Note]
> <span data-ttu-id="68891-104">मूल्यह्रास किया गया – इस विशेषता का मूल्यह्रास किया गया और अब उपलब्ध नहीं है।</span><span class="sxs-lookup"><span data-stu-id="68891-104">DEPRECATED: This feature has been deprecated and is no longer available.</span></span>

[!include [banner](../includes/psa-now-project-operations.md)]

[!INCLUDE[cc-applies-to-psa-app-1x-2x](../includes/cc-applies-to-psa-app-1x-2x.md)]

[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] 

<span data-ttu-id="68891-105">[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] कैलेंडर का उपयोग करके व्यक्तिगत अपॉइंटमेंट, परियोजना-कार्य बुकिंग और field service कार्य ऑर्डर असाइनमेंट देखें.</span><span class="sxs-lookup"><span data-stu-id="68891-105">View personal appointments, project-work bookings, and field service work order assignments using the [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar.</span></span>  
  
 <span data-ttu-id="68891-106">जब सब कुछ एक ही स्थान पर हो, तो आपके दिन को प्रबंधित करना आसान बन जाता है.</span><span class="sxs-lookup"><span data-stu-id="68891-106">With everything in one place, it’s easy to manage your day.</span></span> <span data-ttu-id="68891-107">आपकी मीटिंग, अपॉइंटमेंट, बुकिंग और कार्य सभी आपके [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] कैलेंडर में उपलब्ध हैं.</span><span class="sxs-lookup"><span data-stu-id="68891-107">Your meetings, appointments, bookings, and tasks are all available in your [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar.</span></span>  
  
 <span data-ttu-id="68891-108">यदि आप [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)] उपयोग कर रहे हैं, तो आप Project Service समय प्रविष्टि दृश्य में अपनी व्यक्तिगत अपॉइंटमेंट्स भी दर्ज कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="68891-108">If you’re using [!INCLUDE[pn_project_service_auto](../includes/pn-project-service-auto.md)], you can also enter your personal appointments in the Project Service time entry view.</span></span> <span data-ttu-id="68891-109">यह परियोजना और संसाधन प्रबंधकों को परियोजनाओं के लिए आपकी उपलब्धता की जानकारी देता है.</span><span class="sxs-lookup"><span data-stu-id="68891-109">This lets project and resource managers know your availability for projects.</span></span> <span data-ttu-id="68891-110">यह आपके समय की बचत भी करता है क्योंकि आपको दो बार अपनी व्यक्तिगत अपॉइंटमेंट्स के बारे में जानकारी दर्ज नहीं करनी पड़ती.</span><span class="sxs-lookup"><span data-stu-id="68891-110">It also saves you time, because you don’t have to enter info about your personal appointments twice.</span></span> <span data-ttu-id="68891-111">आप बस अपने कैलेंडर से Project Service समय प्रविष्टि दृश्य में अपनी व्यक्तिगत अपॉइंटमेंट्स को आयात कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="68891-111">You can simply import your personal appointments from your calendar to Project Service time entry view.</span></span>  
  
 <span data-ttu-id="68891-112">आपका कैलेंडर आज से लेकर आने वाले चार सप्ताहों तक परियोजना और कार्य ऑर्डर बुकिंग्स को सिंक्रनाइज़ करेगा.</span><span class="sxs-lookup"><span data-stu-id="68891-112">Your calendar will sync project and work order bookings from today to upcoming four weeks.</span></span> <span data-ttu-id="68891-113">यह सेटिंग बदली नहीं जा सकती.</span><span class="sxs-lookup"><span data-stu-id="68891-113">This setting can’t be changed.</span></span>  
  
 <span data-ttu-id="68891-114">सिंक्रनाइज़ करना केवल PSA से आपके [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] कैलेंडर तक एक तरफ़ा समर्थित है,.</span><span class="sxs-lookup"><span data-stu-id="68891-114">Syncing is only supported one way, from PSA to your [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar.</span></span> <span data-ttu-id="68891-115">आप रिवर्स ऑर्डर में सिंक कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="68891-115">You can sync in the reverse order.</span></span> 
  
 <span data-ttu-id="68891-116">अपने [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] कैलेंडर का उपयोग करने का तरीका जानने के लिए, [व्‍यवसाय के लिए वेब पर Outlook में कैलेंडर देखें](https://support.office.com/article/Calendar-in-Outlook-on-the-web-for-business-5219c457-d1fe-4c2f-9032-1a816b88e936).</span><span class="sxs-lookup"><span data-stu-id="68891-116">To learn how to use your [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar, see [Calendar in Outlook on the web for business](https://support.office.com/article/Calendar-in-Outlook-on-the-web-for-business-5219c457-d1fe-4c2f-9032-1a816b88e936).</span></span>  
  
## <a name="setup"></a><span data-ttu-id="68891-117">सेटअप</span><span class="sxs-lookup"><span data-stu-id="68891-117">Setup</span></span>  
 <span data-ttu-id="68891-118">इससे पहले कि आप अपने [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] कैलेंडर में अपनी बुकिंग देख सकें और उन्हें प्रबंधित कर सकें, आपको कुछ चीज़ें सेट अप करने की आवश्यकता होगी.</span><span class="sxs-lookup"><span data-stu-id="68891-118">Before you can see and manage your bookings on your [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar, you need to set a few things up.</span></span>  
  
- <span data-ttu-id="68891-119">आपको [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] ग्‍लोबल व्यवस्थापक या सिस्टम व्यवस्थापक क्रेडेंशियल्स की आवश्यकता होगी.</span><span class="sxs-lookup"><span data-stu-id="68891-119">You will need to have [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] Global Administrator or System Administrator credentials.</span></span>  
  
- <span data-ttu-id="68891-120">आपके व्यवस्थापक को ईमेल सर्वर प्रोफ़ाइल कॉन्फ़िगर करना होगा और प्रत्येक उपयोगकर्ता को उसके मेलबॉक्स को कॉन्फ़िगर करने की आवश्यकता होगी.</span><span class="sxs-lookup"><span data-stu-id="68891-120">Your Admin will need to configure the email server profile and each user will need to configure their mailbox.</span></span> [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] <span data-ttu-id="68891-121">[सर्वर-साइड सिंक्रनाइज़ेशन का उपयोग करके ईमेल संसाधन सेट अप करें](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/admin/set-up-server-side-synchronization-of-email-appointments-contacts-and-tasks)</span><span class="sxs-lookup"><span data-stu-id="68891-121">[Set up email processing through server-side synchronization](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/admin/set-up-server-side-synchronization-of-email-appointments-contacts-and-tasks)</span></span>  
  
## <a name="turn-on-synchronization-for-your-organization-admin-task"></a><span data-ttu-id="68891-122">अपने संगठन के लिए सिंक्रनाइज़ेशन चालू करें (व्यवस्थापन कार्य)</span><span class="sxs-lookup"><span data-stu-id="68891-122">Turn on synchronization for your organization (admin task)</span></span>  
  
1.  <span data-ttu-id="68891-123">मुख्य मेनू से, **सेटिंग्‍स** > **व्यवस्थापन** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="68891-123">From the main menu, click **Settings** > **Administration**.</span></span>  
  
2.  <span data-ttu-id="68891-124">**सिस्टम सेटिंग** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="68891-124">Click **System Settings**.</span></span>  
  
3.  <span data-ttu-id="68891-125">**सिंक्रनाइज़ेशन** टैब पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="68891-125">Click the **Synchronization** tab.</span></span>  
  
4.  <span data-ttu-id="68891-126">**चुनें कि क्या संसाधन बुकिंग का निम्न के साथ सिंक्रनाइज़ेशन सक्षम करना है** के अंतर्गत, **Outlook के साथ संसाधन बुकिंग को सिंक्रनाइज़ करें** को चेक करें.</span><span class="sxs-lookup"><span data-stu-id="68891-126">Under **Select whether to enable syncing of resource booking with**, check the **Synchronize resource booking with Outlook**.</span></span>  
  
## <a name="turn-on-synchronization-for-your-user-profile-user-task"></a><span data-ttu-id="68891-127">आपके उपयोगकर्ता प्रोफ़ाइल के लिए सिंक्रनाइज़ेशन चालू करें (उपयोगकर्ता कार्य)</span><span class="sxs-lookup"><span data-stu-id="68891-127">Turn on synchronization for your user profile (user task)</span></span>  
  
1.  <span data-ttu-id="68891-128">स्क्रीन के ऊपरी-दाएँ कोने में **सेटिंग्स** बटन पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="68891-128">Click the **Settings** button in the upper-right corner of the screen.</span></span>  
  
2.  <span data-ttu-id="68891-129">**विकल्प** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="68891-129">Click **Options**.</span></span>  
  
3.  <span data-ttu-id="68891-130">**सिंक्रनाइज़ेशन** टैब पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="68891-130">Click the **Synchronization** tab.</span></span>  
  
4.  <span data-ttu-id="68891-131">**Outlook के साथ संसाधन बुकिंग सिंक्रनाइज़ेशन** के अंतर्गत, **Outlook के साथ संसाधन बुकिंग सिंक्रनाइज़ेशन** को चेक करें.</span><span class="sxs-lookup"><span data-stu-id="68891-131">Under **Resource booking sync with Outlook**, check the **Synchronization resource booking with Outlook**.</span></span>  
  
## <a name="import-your-personal-appointments-user-task"></a><span data-ttu-id="68891-132">अपनी व्यक्तिगत अपॉइंटमेंट्स आयात करें (उपयोगकर्ता कार्य)</span><span class="sxs-lookup"><span data-stu-id="68891-132">Import your personal appointments (user task)</span></span>  
 <span data-ttu-id="68891-133">आप अपने कैलेंडर से Project Service Automation समय प्रविष्टि दृश्य में अपनी व्यक्तिगत अपॉइंटमेंट्स को आयात कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="68891-133">You can import your personal appointments from your calendar to Project Service Automation time entry view.</span></span>  
  
1. <span data-ttu-id="68891-134">[!INCLUDE[pn_office_365](../includes/pn-office-365.md)] कैलेंडर खोलें और **डेटा आयात करें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="68891-134">Open [!INCLUDE[pn_office_365](../includes/pn-office-365.md)] calendar and click **Import Data**.</span></span>  
  
2. <span data-ttu-id="68891-135">फ़िल्टर स्क्रीन पर, **Exchange से अपॉइंटमेंट्स** का चयन करें और फिर **लागू करें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="68891-135">On the Filters screen, select **Appointments from Exchange** and then click **Apply**.</span></span>  
  
3. <span data-ttu-id="68891-136">सिस्टम वर्तमान सप्ताह से सुझाई गई प्रविष्टियों के रूप में अपॉइंटमेंट्स को समय प्रविष्टि दृश्य में खींचेगा.</span><span class="sxs-lookup"><span data-stu-id="68891-136">The system will pull appointments into time entry view as suggested entries from the current week.</span></span> <span data-ttu-id="68891-137">किसी अन्य सप्ताह के लिए प्रविष्टियाँ जोड़ने हेतु, **पिछला** या **अगला** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="68891-137">To add entries for another week, click **Previous** or **Next**.</span></span>  
  
4. <span data-ttu-id="68891-138">उस अपॉइंटमेंट का चयन करें जिसे आप Project Service Automation समय प्रविष्टि दृश्य में जोड़ना चाहते हैं.</span><span class="sxs-lookup"><span data-stu-id="68891-138">Select the appointment that you want to add to Project Service Automation time entry view.</span></span>  
  
5. <span data-ttu-id="68891-139">**समय प्रविष्टि** पॉपअप बॉक्स में, अपॉइंटमेंट को Project Service Automation समय प्रविष्टि दृश्य में परिवर्तित करने के लिए उपयुक्त विकल्पों का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="68891-139">On the **Time Entry** popup box, select the appropriate options to convert the appointment to a Project Service Automation time entry view.</span></span>  
  
6. <span data-ttu-id="68891-140">**सहेजें** पर क्लिक करें.</span><span class="sxs-lookup"><span data-stu-id="68891-140">Click **Save**.</span></span>  
  
### <a name="see-also"></a><span data-ttu-id="68891-141">यह भी देखें</span><span class="sxs-lookup"><span data-stu-id="68891-141">See Also</span></span>  
 [<span data-ttu-id="68891-142">समय, व्यय और सहयोग मार्गदर्शिका</span><span class="sxs-lookup"><span data-stu-id="68891-142">Time, Expense, and Collaboration Guide</span></span>](../psa/time-expense-collaboration-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]