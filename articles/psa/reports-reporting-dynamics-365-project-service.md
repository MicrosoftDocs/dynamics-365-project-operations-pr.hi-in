---
title: होम पेज रिपोर्टिंग
description: यह विषय Dynamics 365 Project Service Automation में रिपोर्टिंग के बारे में जानकारी प्रदान करता है।
author: ruhercul
manager: kfend
ms.service: project-operations
ms.custom:
- dyn365-projectservice
ms.date: 03/01/2019
ms.topic: article
ms.author: ruhercul
audience: Admin
search.audienceType:
- admin
- customizer
- enduser
search.app:
- D365CE
- D365PS
- ProjectOperations
ms.openlocfilehash: e1a645b157c56066e56b22ea8cf0324fbc1ddd2c
ms.sourcegitcommit: 4cf1dc1561b92fca4175f0b3813133c5e63ce8e6
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/28/2020
ms.locfileid: "4120320"
---
# <a name="reporting-home-page"></a><span data-ttu-id="5f5e0-103">होम पेज रिपोर्टिंग</span><span class="sxs-lookup"><span data-stu-id="5f5e0-103">Reporting home page</span></span>

[!INCLUDE[cc-applies-to-psa-app-3.x](../includes/cc-applies-to-psa-app-3x.md)]

<span data-ttu-id="5f5e0-104">Microsoft Dynamics 365 Project Service Automation से प्रोजेक्ट-आधारित संस्थानों अपने व्यवसाय के संचालन को कुशलतापूर्वक प्रबंधित कर सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="5f5e0-104">Microsoft Dynamics 365 Project Service Automation lets project-based organizations efficiently manage the operations of their business.</span></span> <span data-ttu-id="5f5e0-105">किसी भी प्रोजेक्ट पर, टीम के सदस्यों को अवसर का प्रबंधन करना चाहिए, काम को उद्धृत करना और उसकी योजना बनानी चाहिए, प्रोजेक्ट को संसाधित करना, योजना के अनुसार कार्य का प्रबंधन, काम के लिए बिल बनाना चाहिए और फिर प्रोजेक्ट को पूरा करने के लिए काम करना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="5f5e0-105">On any project, team members must manage the opportunity, quote and plan the work, resource the projects, manage the work according to the plan, bill for the work, and then do the work to complete the project.</span></span> <span data-ttu-id="5f5e0-106">संचालन की रिपोर्ट करने की क्षमता संस्थान की स्थिति को निर्धारित करने और किसी भी आवश्यक सुधारात्मक कार्रवाई की बुनियाद है।</span><span class="sxs-lookup"><span data-stu-id="5f5e0-106">The ability to report on operations is key to determining the health of the organization and taking any corrective action that's required.</span></span> <span data-ttu-id="5f5e0-107">PSA अपनी सभी रिपोर्टिंग के लिए Microsoft Dynamics 365 रिपोर्टिंग विधियों और तकनीकों का उपयोग करता है।</span><span class="sxs-lookup"><span data-stu-id="5f5e0-107">PSA uses Microsoft Dynamics 365 reporting methods and technologies for all its reporting.</span></span> <span data-ttu-id="5f5e0-108">रिपोर्टिंग के विकल्पों के बारे में अधिक जानकारी के लिए, देखें [Dynamics 365 Customer Engagement (on-premises), वर्ज़न 9 के लिए रिपोर्ट लेखन मार्गदर्शिका](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/reporting-analytics-with-dynamics-365).</span><span class="sxs-lookup"><span data-stu-id="5f5e0-108">For more information about the options for reporting, see the [Report writing guide for Dynamics 365 Customer Engagement (on-premises), version 9](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/reporting-analytics-with-dynamics-365).</span></span>

## <a name="report-wizard"></a><span data-ttu-id="5f5e0-109">रिपोर्ट विज़ार्ड</span><span class="sxs-lookup"><span data-stu-id="5f5e0-109">Report Wizard</span></span>

<span data-ttu-id="5f5e0-110">गैर-डेवलपर्स रिपोर्ट विज़ार्ड से सरल रिपोर्ट बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="5f5e0-110">The Report Wizard lets non-developers create simple reports.</span></span> <span data-ttu-id="5f5e0-111">कि एप्लिकेशन एक मौजूदा प्लेटफ़ॉर्म पर बनाया गया है, यह अनुभव उस अनुभव के समान है जो [रिपोर्ट विज़ार्ड का उपयोग करके रिपोर्ट बनाएं या संपादित करें](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/basics/create-edit-copy-report-wizard) में प्रलेखित किया गया है।</span><span class="sxs-lookup"><span data-stu-id="5f5e0-111">Because the app is built on an existing platform, the experience is the same as the experience that is documented in [Create or edit a report using the Report Wizard](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/basics/create-edit-copy-report-wizard).</span></span> <span data-ttu-id="5f5e0-112">हालाँकि, आप Project Service Automation-विशिष्ट इकाइयों का उपयोग करेंगे।</span><span class="sxs-lookup"><span data-stu-id="5f5e0-112">However, you will use the Project Service Automation-specific entities.</span></span>

## <a name="custom-sql-server-reporting-services-reports"></a><span data-ttu-id="5f5e0-113">कस्टम SQL सर्वर रिपोर्टिंग सेवा रिपोर्ट</span><span class="sxs-lookup"><span data-stu-id="5f5e0-113">Custom SQL Server Reporting Services reports</span></span>

<span data-ttu-id="5f5e0-114">यदि आपके व्यवसाय को एक विशिष्ट रिपोर्ट की आवश्यकता है जो रिपोर्ट विज़ार्ड का उपयोग करके नहीं बनाई जा सकती है, तो आप एक कस्टम रिपोर्ट बना सकते हैं।</span><span class="sxs-lookup"><span data-stu-id="5f5e0-114">If your business requires a specific report that can't be created by using the Report Wizard, you can create a custom report.</span></span> <span data-ttu-id="5f5e0-115">आपके पास उपयुक्त Microsoft SQL Server Data Tools उपकरण और रिपोर्ट संलेखन एक्सटेंशन के साथ Microsoft Visual Studio संस्थापित होना चाहिए।</span><span class="sxs-lookup"><span data-stu-id="5f5e0-115">You must have Microsoft Visual Studio installed, together with the appropriate Microsoft SQL Server Data Tools and Report Authoring Extensions.</span></span> <span data-ttu-id="5f5e0-116">उपकरण और संस्करणों के बारे में अधिक जानकारी के लिए, [SQL Server Data Tools का उपयोग करते हुए रिपोर्ट लेखन परिस्थिति](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/report-writing-environment-using-sql-server-data-tools) देखें।</span><span class="sxs-lookup"><span data-stu-id="5f5e0-116">For more information about tools and versions, see [Report writing environment using SQL Server Data Tools](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/report-writing-environment-using-sql-server-data-tools).</span></span> <span data-ttu-id="5f5e0-117">कस्टम रिपोर्ट बनाने के तरीके के बारे में जानकारी के लिए, [SQL Server Data Tools का उपयोग करके एक नई रिपोर्ट बनाएं](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/create-a-new-report-using-sql-server-data-tools) देखें।</span><span class="sxs-lookup"><span data-stu-id="5f5e0-117">For information about how to create a custom report, see [Create a new report using SQL Server Data Tools](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/analytics/create-a-new-report-using-sql-server-data-tools).</span></span>

## <a name="power-bi-insights-apps"></a><span data-ttu-id="5f5e0-118">Power BI एप्स का निरीक्षण करता है।</span><span class="sxs-lookup"><span data-stu-id="5f5e0-118">Power BI insights apps</span></span>

<span data-ttu-id="5f5e0-119">Microsoft Power BI और Dynamics 365 मिल कर निरीक्षण ऐप्स के रूप में आपको अपने डेटा के साथ काम करने का एक शक्तिशाली तरीका देते हैं।</span><span class="sxs-lookup"><span data-stu-id="5f5e0-119">Together, Microsoft Power BI and Dynamics 365 give you a powerful way to work with your data, in the form of insights apps.</span></span> <span data-ttu-id="5f5e0-120">इनसाइट्स ऐप की उपलब्धता के बारे में जानकारी के लिए देखें, [Power BI इनसाइट्स ऐप पेज](https://powerbi.microsoft.com/power-bi-insights-apps/)।</span><span class="sxs-lookup"><span data-stu-id="5f5e0-120">For information about the availability of insights apps, see the [Power BI insights apps page](https://powerbi.microsoft.com/power-bi-insights-apps/).</span></span>


## <a name="additional-resources"></a><span data-ttu-id="5f5e0-121">अतिरिक्त संसाधन</span><span class="sxs-lookup"><span data-stu-id="5f5e0-121">Additional resources</span></span>
<span data-ttu-id="5f5e0-122">PSA में रिपोर्टिंग के बारे में अधिक जानकारी के लिए, निम्नलिखित विषय देखें:</span><span class="sxs-lookup"><span data-stu-id="5f5e0-122">For more information about reporting in PSA, see the following topics:</span></span>

- [<span data-ttu-id="5f5e0-123">Project Service डेटा मॉडल के साथ काम करना</span><span class="sxs-lookup"><span data-stu-id="5f5e0-123">Working with the Project Service data model</span></span>](reports-working-project-service-data-model.md)
- [<span data-ttu-id="5f5e0-124">डैशबोर्ड</span><span class="sxs-lookup"><span data-stu-id="5f5e0-124">Dashboards</span></span>](reports-dashboards.md)

