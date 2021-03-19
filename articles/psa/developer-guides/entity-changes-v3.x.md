---
title: एंटिटी, नियंत्रण, और उपयोगकर्ता इंटरफ़ेस परिवर्तन (Project Service Automation 3.x)
description: यह विषय Microsoft Dynamics Project Service Automation 3.x के लिए समाधान परिवर्तन का वर्णन करता है।
author: makk
manager: kfend
ms.custom:
- dyn365-projectservice
ms.date: 03/15/2019
ms.topic: article
ms.service: business-applications
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.openlocfilehash: fa80f459260f30360e78a1e7bcc00706dbc0b5a4
ms.sourcegitcommit: fa32b1893286f20271fa4ec4be8fc68bd135f53c
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 02/15/2021
ms.locfileid: "5284900"
---
# <a name="entity-control-and-user-interface-changes-project-service-automation-3x"></a>एंटिटी, नियंत्रण, और उपयोगकर्ता इंटरफ़ेस परिवर्तन (Project Service Automation 3.x)

[!include [banner](../../includes/psa-now-project-operations.md)]


Microsoft Dynamics Project Service Automation (PSA) 3.x की रिलीज़ के साथ, इकाइयों, नियंत्रणों, दृश्य और उपयोगकर्ता इंटरफ़ेस में कई बदलाव किए गए हैं। यह विषय इन महत्वपूर्ण परिवर्तनों के बारे में जानकारी प्रदान करता है।

## <a name="parent-child-relationships-for-sales-document-sales-document-line-sales-document-line-detail-entities"></a>बिक्री दस्तावेज, बिक्री दस्तावेज लाइन, बिक्री दस्तावेज लाइन विवरण इकाइयों के लिए पेरेंट-चाइल्ड संबंध
संस्करण 3.0 से पहले जारी Dynamics 365 Project Service Automation (PSA) के संस्करणों में, स्ट्रिंग फ़ील्ड के माध्यम से बिक्री दस्तावेज़, बिक्री दस्तावेज़ लाइनों, और बिक्री दस्तावेज़ लाइन विवरण इकाई के बीच के कुछ रिश्तों को संबंधित इकाई के GUID के एक स्ट्रिंग प्रतिनिधित्व के साथ लागू किया गया था। यह उन प्लेटफ़ॉर्म सीमाओं के कारण था, जिनके समाधान के लिए सर्वर और क्लाइंट पक्षों पर महत्वपूर्ण कस्टम कोड की आवश्यकता होती थी, ताकि वे संबंध विशिष्ट Dynamics CRM इकाई संबंधों के समान कार्य कर सकें और स्ट्रिंग फ़ील्ड को लुकअप फ़ील्ड की तरह बना सकें।

PSA 3.0 को विक्रय दस्तावेज़ और विक्रय दस्तावेज़ लाइन इकाइयों के बीच नए इकाई संबंधों का लाभ उठाने के लिए अपडेट किया गया है।

क्योंकि लुकअप फ़ील्ड अब इकाइयों के संदर्भों को दर्शाने के लिए उपयोग किया जा सकता है, पिछले संस्करणों में संबंधित इकाई के GUID के स्ट्रिंग मान रखने वाले फ़ील्ड की अब आवश्यकता नहीं है और इसलिए उन्हें हटा दिया गया है। कस्टम क्लाइंट और सर्वर साइड कोड जो विरासत स्ट्रिंग क्षेत्रों द्वारा परिभाषित रिश्तों को संभालता है, को भी हटा दिया गया है।

### <a name="entity-schema-changes"></a>इकाई स्कीमा बदलता है
निम्न तालिका निकाले गए स्ट्रिंग फ़ील्ड और इकाइयों के लिए नए लुकअप फ़ील्ड की प्रत्येक के लिए अलग-अलग सूची प्रदान करती है। 

 निकाय |   हटाए गए फ़ील्ड (स्ट्रिंग) | नई फ़ील्ड (लुकअप)
--- | --- | ---
इनवॉयस विवरण (इनवॉइस लाइन) |  msdyn_contractline |    msdyn_contractlineid
msdyn_actual (वास्तविक) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_contractlineinvoiceschedule (परियोजना अनुबंध पंक्ति इनवॉइस शेड्यूल) |    msdyn_contractline |    msdyn_contractlineid
msdyn_contractlinescheduleofvalue (परियोजना अनुबंध पंक्ति माइलस्टोन) |   msdyn_contractline |    msdyn_contractlineid
msdyn_fact (तथ्य) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_invoicelinetransaction (इनवॉइस लाइन विवरण) | msdyn_invoiceline <br> msdyn_salescontractline | msdyn_invoicelineid <br> msdyn_salescontractlineid
msdyn_journalline (जर्नल लाइन) |  msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlineresourcecategory (परियोजना अनुबंध पंक्ति संसाधन श्रेणी) | msdyn_salescontractline |   msdyn_contractlineid
msdyn_orderlinetransaction (परियोजना अनुबंध पंक्ति विवरण) | msdyn_salescontractline |   msdyn_salescontractlineid
msdyn_orderlinetransactioncategory (परियोजना अनुबंध पंक्ति लेनदेन श्रेणी) |   msdyn_contractline |    msdyn_contractlineid
msdyn_orderlinetransactionclassification (प्रोजेक्ट अनुबंध पंक्ति लेनदेन वर्गीकरण) |   msdyn_contractline |    msdyn_contractlineid
msdyn_quotelineinvoiceschedule (कोट पंक्ति इनवॉइस शेड्यूल) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelineresourcecategory (कोट पंक्ति संसाधन श्रेणी) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinescheduleofvalue (कोट लाइन माइलस्टोन) | msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransaction (कोट लाइन विवरण) |    msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactioncategory (कोट पंक्ति लेनदेन श्रेणी) |  msdyn_quoteline |   msdyn_quotelineid
msdyn_quotelinetransactionclassification (कोट पंक्ति लेनदेन वर्गीकरण) |  msdyn_quoteline |   msdyn_quotelineid
SalesOrderDetail (ऑर्डर पंक्ति) | msdyn_quotelineid | msdyn_quoteline 

### <a name="deprecated-custom-views-and-controls"></a>कस्टम दृश्य और नियंत्रण हटाए गए
निम्नलिखित कस्टम दृश्य और नियंत्रण और उनके संबंधित आर्टिफ़ैक्ट को हटा दिया गया है।

- प्रभार्यता का दृश्य।
- कोट लाइन के लिए **प्रोजेक्ट सूचना** पेज पर कोट लाइन विवरण दिखाने का कस्टम ग्रिड नियंत्रण।
- बिक्री ऑर्डर लाइन के लिए **प्रोजेक्ट जानकारी** पेज पर प्रोजेक्ट अनुबंध लाइन विवरण दिखाने के लिए कस्टम ग्रिड नियंत्रण।

> [!NOTE]
> हटाए गए संसाधनों की पूरी सूची के लिए, [Project Service Automation v3.x में हटाए गए वेब संसाधन](../developer-guides/web-resources-deprecated-v3.x.md) देखें

## <a name="unified-client-interface-app-module"></a>एकीकृत ग्राहक इंटरफ़ेस ऐप मॉड्यूल
यूनिफाइड क्लाइंट इंटरफेस (UCI) ऐप मॉड्यूल की शुरुआत के साथ, PSA साइट मैप प्रविष्टियों को सिस्टम से हटा दिया गया है।  
अवसर, कोट, ऑर्डर, इनवॉइस के लिए फार्म स्विचिंग से संबंधित कार्यक्षमता को हटा दिया गया है, क्योंकि अब इसकी आवश्यकता नहीं है क्योंकि UCI ऐप मॉड्यूल में केवल PSA संस्करणों के फॉर्म शामिल हैं।  

निम्नलिखित वेब संसाधनों को हटा दिया गया है:

- msdyn_\SalesDocument\SalesDocumentFormLoader.js
- msdyn_\SalesDocument\PSSalesDocumentCustomFormIds.js

> [!NOTE]
> हटाए गए संसाधनों की पूरी सूची के लिए, [Project Service Automation v3.x में हटाए गए वेब संसाधन](../developer-guides/web-resources-deprecated-v3.x.md) देखें।




[!INCLUDE[footer-include](../../includes/footer-banner.md)]