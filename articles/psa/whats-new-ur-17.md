---
title: Project Service Automation के अपडेट रिलीज़ 17, V3 में नया क्या है और उसमें क्या परिवर्तन हुआ है
description: यह विषय Project Service Automation अपडेट रिलीज़ 17, V3 में उपलब्ध सुविधाओं और सुधारों को सूचीबद्ध करता है.
author: ruhercul
manager: kfend
ms.service: dynamics-365-customerservice
ms.custom: dyn365-projectservice
ms.date: 03/06/2020
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
ms.openlocfilehash: 7ba685568692dafe117de42a71bb14d391cd7cc4
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077656"
---
# <a name="project-service-automation-update-release-17-v3"></a>Project Service Automation V3 अद्यतन रिलीज़ 17, V3

हमें Dynamics 365 के लिए Project Service Automation अनुप्रयोग हेतु नवीनतम अपडेट की घोषणा करते हुए खुशी हो रही है. इस रिलीज़ में गुणवत्ता, प्रदर्शन और उपयोगिता में कुछ महत्वपूर्ण सुधार शामिल हैं.  यह रिलीज़ Dynamics 365 9.x के साथ संगत में है. इस रिलीज़ को अपडेट करने के लिए, Dynamics 365 online के लिए व्यवस्थापन केंद्र पर जाएँ और अपडेट को स्थापित करने के लिए समाधान पृष्ठ पर जाएँ. अधिक जानकारी के लिए, देखें [पसंदीदा समाधान को स्थापित, अपडेट या हटाएँ](https://docs.microsoft.com/power-platform/admin/install-remove-preferred-solution).

यह टॉपिक PSA V3, अपडेट रिलीज़ 17 के लिए नई या बदली गई सुविधाओं और सुधारों को सूचीबद्ध करता है. इस संस्करण की बिल्ड संख्या V3.10.6.34 है और यह आमतौर पर मार्च 2020 के स्वयं-अपडेट के माध्यम से उपलब्ध है.


## <a name="update-release-17"></a>अपडेट रिलीज़ 17

### <a name="bug-fixes"></a>बग समाधान

**सामान्‍य**

- निश्चित: टीम के सदस्य लाइसेंस लागू करने के लिए Project Service Automation अपडेट करें (Project Resource Hub में टीम के सदस्य सेवा प्लान मेटाडेटा 3.x शामिल होगा)
 
**समय और व्यय**

- निश्चित: गैर-शून्य मूल्य से शून्य (0) के लिए व्यय अनुमान बदलना संभव नहीं है. बदलाव को नजरअंदाज किया जाता है.

**परियोजना प्रबंधन**

- निश्चित: टीम के सदस्य के पद नाम पर शून्य मानों के लिए एक चेक जोड़ा गया है.
- निश्चित: **msdyn_resourceassignment** निकाय पर **msdyn_userresourceid** फ़ील्ड को रोका गया.
- निश्चित: 2.x से 3.x पर अपग्रेड करें अब कार्य असाइनमेंट पर रिक्त प्रयास आकृति को संभालता है.

**Sales**

- निश्चित: **Invoice.PreValidateInvoiceUpdate** अब रिकॉर्ड मालिकों को फिर से ठीक करने के परिदृश्य को संभालता है.
- निश्चित: जब लेन-देन वर्ग **समय** , **UnitGroup** सहित सभी प्रविष्टियों के लिए गैर-संपादन योग्य है, **QuoteLineDetails** , **JournalLine** , **InvoiceLineDetail** , और **ContractLineDetails**. हालाँकि, **इकाई** केवल **JournalLine** और **InvoiceLineDetails** के लिए गैर-संपादन योग्य है.


