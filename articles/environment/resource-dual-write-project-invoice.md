---
title: प्रोजेक्ट चालान एकीकरण
description: यह विषय ग्राहक चालान के लिए Project Operations ड्यूल-राइट एकीकरण के बारे में जानकारी प्रदान करता है.
author: sigitac
ms.date: 04/26/2021
ms.topic: article
ms.prod: ''
ms.service: project-operations
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: 102a7cdba467a2071119c5b32d2e75e48170c783
ms.sourcegitcommit: 02f00960198cc78a5e96955a9e4390c2c6393bbf
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 04/28/2021
ms.locfileid: "5955763"
---
# <a name="project-invoice-integration"></a>प्रोजेक्ट चालान एकीकरण

यह विषय ग्राहक चालान के लिए Project Operations ड्यूल-राइट एकीकरण के बारे में जानकारी प्रदान करता है.

Project Operations में, प्रोजेक्ट मैनेजर प्रोजेक्ट बिलिंग बैकलॉग का प्रबंधन करता है और Microsoft Dataverse में ग्राहक के लिए प्रोफार्मा चालान बनाता है. इस प्रोफार्मा चालान के आधार पर, लेखा प्राप्त करने वाला क्लर्क या प्रोजेक्ट अकाउंटेंट एक कस्टमर फेसिंग चालान बनाता है. ड्यूल-राइट एकीकरण यह सुनिश्चित करता है कि प्रोफार्मा चालान विवरण Finance and Operations अनुप्रयोगों के लिए सिंक्रनाइज़ हैं. कस्टमर फेसिंग इनवॉइस पोस्ट किए जाने के बाद, सिस्टम Dataverse में संबंधित प्रोजेक्ट एक्चुअल्स को लेखांकन विवरण के साथ अद्यतन करता है. निम्नलिखित ग्राफिक इस एकीकरण का एक उच्च-स्तरीय वैचारिक अवलोकन प्रदान करता है.

   ![प्रोजेक्ट चालान एकीकरण](./media/DW5Invoicing.png)

प्रोजेक्ट मैनेजर द्वारा Dataverse में प्रोफार्मा चालान की पुष्टि करने के बाद, प्रोफार्मा चालान हेडर जानकारी ड्यूल-राइट तालिका मानचित्र, **प्रोजेक्ट चालान प्रस्ताव V2 (चालान)** का उपयोग करके Finance and Operations अनुप्रयोग के लिए सिंक्रनाइज़ होती है. यह Dataverse फाइनेंस और Finance and Operations तक एकतरफा एकीकरण है. सीधे Finance and Operations अनुप्रयोग में प्रोजेक्ट चालान प्रस्तावों को बनाना या हटाना समर्थित नहीं है.

Dataverse में इनवॉइस की पुष्टि **एक्चुअल्स** निकाय में बिलिंग से संबंधित रिकॉर्ड बनाने के लिए व्यावसायिक तर्क ट्रिगर करती है. ये रिकॉर्ड ड्यूल-राइट तालिका मानचित्र **Project Operations एकीकरण एक्चुअल्स (msdyn\_actuals)** का उपयोग करके Finance and Operations के लिए सिंक्रनाइज़ किए जाते हैं. अधिक जानकारी के लिए, [परियोजना अनुमान और वास्तविक आकड़ें](resource-dual-write-estimates-actuals.md) देखें. 

प्रोजेक्ट इनवॉइस प्रस्ताव लाइनें आवधिक प्रक्रिया **आयात फ़ॉर्म स्टैगिंग** द्वारा बनाई जाती हैं. यह प्रक्रिया **एक्चुअल्स स्टैगिंग** तालिका में बिल किए गए एक्चुल्स के विवरण पर आधारित होती है. अधिक जानकारी के लिए देखें [Manage project invoice proposals](../invoicing/format-update-project-invoice-proposals.md#create-project-invoice-proposals). 
