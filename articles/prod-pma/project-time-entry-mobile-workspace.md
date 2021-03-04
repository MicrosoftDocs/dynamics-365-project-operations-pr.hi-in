---
title: प्रोजेक्ट टाइम एंट्री मोबाइल कार्यस्थान
description: यह विषय परियोजना समय प्रविष्टि मोबाइल कार्यक्षेत्र के बारे में जानकारी प्रदान करता है. यह कार्यस्थान उपयोगकर्ताओं को उनके मोबाइल डिवाइस का इस्तेमाल करके किसी परियोजना का समय दर्ज करने और सहेजने देता है.
author: Yowelle
manager: AnnBe
ms.date: 12/01/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 272101
ms.assetid: 4505f021-b9bb-4b87-be24-6bf0bd88ee60
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: Version 1611
ms.search.validFrom: 2016-11-30
ms.openlocfilehash: 23a5a9f25cfdd6df74257b3500c7a035d711b5f6
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077681"
---
# <a name="project-time-entry-mobile-workspace"></a>प्रोजेक्ट टाइम एंट्री मोबाइल कार्यस्थान

[!include [banner](../includes/banner.md)]

यह विषय **परियोजना समय प्रविष्टि** मोबाइल कार्यक्षेत्र के बारे में जानकारी प्रदान करता है. यह कार्यस्थान उपयोगकर्ताओं को उनके मोबाइल डिवाइस का इस्तेमाल करके किसी परियोजना का समय दर्ज करने और सहेजने देता है.

इस मोबाइल कार्यक्षेत्र का इस्तेमाल Dynamics 365 Unified Ops मोबाइल अनुप्रयोग के साथ किया जाना है. 

## <a name="overview"></a>अवलोकन
उनके रोज के काम के हिस्से के रूप में, परियोजना संसाधन अक्सर साइट पर या यात्रा कर रहे हैं. **परियोजना समय प्रविष्टि** मोबाइल कार्यक्षेत्र उपयोगकर्ताओं को उनकी पसंद के मोबाइल डिवाइस पर किसी परियोजना के लिए उनका बिल योग्य या गैर-बिल योग्य समय दर्ज करने देता है. इसलिए, परियोजना संसाधन कभी भी और कहीं भी समय प्रविष्टियां दर्ज कर सकते हैं. वो पहले रिकॉर्ड की जा गयी समय प्रविष्टियां भी देख सकते हैं. 

खास तौर पर, **परियोजना समय प्रविष्टि** मोबाइल कार्यक्षेत्र में, उपयोगकर्ता ये कार्य कर सकते हैं:

-   किसी भी चुनी गयी तिथि के लिए, किसी विशिष्ट कार्य में प्रयुक्त घंटों की संख्या दर्ज करें.
-   समय दर्ज करने के लिए परियोजना नाम या ग्राहक से परियोजना ढूंढें.
-   आपके प्रयुक्त समय के लिए श्रेणी और गतिविधि निर्दिष्ट करें.
-   परियोजना के लिए समय को बिल योग्य या गैर-बिल योग्य के रूप में रिकॉर्ड करें.
-   विकल्पतः कोई भी बाहरी या आंतरिक टिप्पणी दर्ज करें.

## <a name="prerequisites"></a>पूर्वावश्यकताएँ
Microsoft Dynamics 365 के संस्करण के आधार पर शर्तें अलग होती हैं, जिनको आपके संगठन के लिए तैनात किया गया है.

### <a name="prerequisites-if-you-use-dynamics-365-finance"></a>शर्तें अगर आप Dynamics 365 Finance इस्तेमाल करते हैं
अगर Finance आपके संगठन के लिए तैनात किया गया है, तो सिस्टम व्यवस्थापक को **परियोजना समय प्रविष्टि** मोबाइल कार्यक्षेत्र प्रकाशित करना होगा. निर्देशों के लिए, [मोबाइल कार्यस्थान प्रकाशित करें](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/publish-mobile-workspace) देखें.

### <a name="prerequisites-if-you-use-version-1611-with-platform-update-3-or-later"></a>शर्तें अगर आप प्लेटफ़ॉर्म अपडेट 3 का वर्जन 1611 या इसके बाद के वर्जन इस्तेमाल करते हैं
यदि प्लेटफ़ॉर्म अपडेट 3 के साथ संस्करण 1611 या इसके बाद का संस्करण, आपके संगठन के लिए तैनात किया गया है, तो सिस्टम व्यवस्थापक को निम्नलिखित शर्तें पूरी करनी चाहिए. 

<table>
<thead>
<tr class="header">
<th>पूर्वावश्यकता</th>
<th>भूमिका</th>
<th>वर्णन</th>
</tr>
</thead>
<tbody>
<tr class="odd">

<td>KB 4018050 लागू करें.</td>
<td>सिस्टम व्यवस्थापक</td>
<td>KB 4018050, X++ अपडेट या मेटाडेटा हॉटफिक्स है जिसमें <strong>परियोजना समय प्रविष्टि</strong> मोबाइल कार्यस्थान है. KB 4018050 कार्यान्वित करने के लिए, आपके सिस्टम व्यवस्थापक को निम्न चरणों का पालन करना होगा.
<ol>
<li><a href="https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/migration-upgrade/download-hotfix-lcs">Microsoft Dynamics Lifecycle Services (LCS) से मेटाडेटा हॉटफिक्स डाउनलोड करें</a>.</li>
<li><a href="https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/migration-upgrade/install-metadata-hotfix-package">मेटाडेटा हॉटफ़िक्स स्थापित करें</a>.</li>
<li>लागू करने <a href="https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/create-apply-deployable-package">योग्य पैकेज बनाएं</a> जिसमें <strong>ApplicationSuite</strong> और <strong>ProjectMobile</strong> मॉडल हों और उसके बाद LCS में तैनात करने योग्य पैकेज अपलोड करें.</li>
<li><a href="https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/deployment/apply-deployable-package-system">तैनात करने योग्य पैकेज लागू करें</a>.</li>

</ol></td>
</tr>
<tr class="even">
<td><strong>परियोजना समय प्रविष्टि</strong> मोबाइल कार्यस्थान प्रकाशित करें.</td>
<td>सिस्टम व्यवस्थापक</td>
<td><a href="https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/publish-mobile-workspace">मोबाइल कार्यस्थान प्रकाशित करें</a> देखें.</td>
</tr>
</tbody>
</table>

## <a name="download-and-install-the-mobile-app"></a>मोबाइल अनुप्रयोग डाउनलोड और स्थापित करें

Finance and Operations मोबाइल अनुप्रयोग डाउनलोड और स्थापित करें:

-   [Android फ़ोन के लिए](https://go.microsoft.com/fwlink/?linkid=850662)
-   [iPhone के लिए](https://go.microsoft.com/fwlink/?linkid=850663)

## <a name="sign-in-to-the-mobile-app"></a>मोबाइल अनुप्रयोग में साइन इन करें
1.  अपनी मोबाइल डिवाइस पर अनुप्रयोग शुरू करें.
2.  अपना Dynamics 365 URL दर्ज करें.
3.  पहली बार जब आप साइन इन करते हैं, तो आपको अपने उपयोगकर्ता नाम और पासवर्ड के लिए संकेत दिया जाता है. अपने क्रेडेंशियल दर्ज करें.
4.  साइन इन करने के बाद, आपकी कंपनी के लिए उपलब्ध कार्यक्षेत्र दिखाए जाते हैं. ध्यान दें कि यदि आपका सिस्टम व्यवस्थापक बाद में नया कार्यक्षेत्र प्रकाशित करता है, तो आपको मोबाइल कार्यस्थानों की सूची को रीफ्रेश करना होगा.

[![रीफ़्रेश हेतु नीचे की ओर खींचें](./media/pull-to-refresh-list-of-workspaces-183x300.png)](./media/pull-to-refresh-list-of-workspaces.png)

## <a name="enter-time-by-using-the-project-time-entry-mobile-workspace"></a>परियोजना समय प्रविष्टि मोबाइल कार्यस्थान का इस्तेमाल करके समय दर्ज करें
1.  अपने मोबाइल डिवाइस पर, **परियोजना समय प्रविष्टि** कार्यस्थान चुनें.
2.  **समय प्रविष्टि** चुनें. वर्तमान सप्ताह के लिए कैलेंडर तिथियां दिखाई गई हैं.
3.  चुनी गयी तिथि के लिए, **कार्रवाई** &gt; **नयी प्रविष्टि** चुनें.
4.  रिकॉर्ड करने के लिए घंटों की संख्या दर्ज करें.
5.  समय प्रविष्टि के लिए परियोजना चुनें. सूची उन परियोजनाओं को दिखाती है जो ऑफ़लाइन इस्तेमाल के लिए आपके अनुप्रयोग में लोड होती हैं. डिफ़ॉल्ट रूप से, 50 आइटम लोड किए जाते हैं, लेकिन डेवलपर इस संख्या को परिवर्तित कर सकते हैं. अधिक जानकारी के लिए, [मोबाइल प्लेटफ़ॉर्म](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/mobile-app-home-page) देखें.
6.  अगर आपकी परियोजना सूची में नहीं है तो **खोजें** चुनें. नाम से खोजें या बदलकर परियोजना नाम या ग्राहक नाम से खोजें.
7.  एक श्रेणी चुनें. सूची उन श्रेणियों को दिखाती है जिन्हें ऑफ़लाइन इस्तेमाल के लिए आपके अनुप्रयोग में लोड की गयी हैं. डिफ़ॉल्ट रूप से, 50 आइटम लोड किए जाते हैं, लेकिन डेवलपर इस संख्या को परिवर्तित कर सकते हैं. अधिक जानकारी के लिए, [मोबाइल प्लेटफ़ॉर्म](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/mobile-app-home-page) देखें.
8.  अगर आपकी श्रेणी लिस्ट में नहीं है तो **खोजें** चुनें. नाम से खोजें या बदलकर श्रेणी नाम से खोजें.
9.  एक गतिविधि का चयन करें. सूची उन गतिविधियों को दिखाती है जो ऑफ़लाइन इस्तेमाल के लिए आपके अनुप्रयोग में लोड होती हैं. डिफ़ॉल्ट रूप से, 50 आइटम लोड किए जाते हैं, लेकिन डेवलपर इस संख्या को परिवर्तित कर सकते हैं. अधिक जानकारी के लिए, [मोबाइल प्लेटफ़ॉर्म](https://docs.microsoft.com/dynamics365/fin-ops-core/dev-itpro/mobile-apps/mobile-app-home-page) देखें.
10. यदि आपकी गतिविधि सूची में नहीं है, तो **खोजें** चुनें. गतिविधि संख्या से खोजें या बदलकर उद्देश्य से खोजें.

11. लाइन गुण का चयन करें.
12. वैकल्पिक: कोई भी बाहरी और आंतरिक टिप्पणी दर्ज करें.
13. **पूर्ण** चयन करें.