---
title: Dynamics 365 Project Operations की स्थापना रद्द करें
description: यह आलेख अनइंस्टॉल करने के तरीके के बारे में जानकारी प्रदान करता है।Dynamics 365 Project Operations
author: stsporen
ms.date: 11/09/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 33a505594d6db47b4f8a0c8a630a0836f424e7d5
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8911966"
---
# <a name="uninstall-dynamics-365-project-operations"></a>Dynamics 365 Project Operations की स्थापना रद्द करें 

_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक -आधारित परिदृश्यों के लिए Project Operations_

Dynamics 365 Project Operations को अनइंस्टॉल करने के लिए, आपको व्यवस्थापक की भूमिका सौंपी जानी चाहिए.

1. **सेटिंग** > **समाधान** पर जाएँ.

    ![सेटिंग पृष्ठ.](./media/uninstall-proj-ops-solutions.png)
  
2. समाधानों को ठीक उसी ऑर्डर में निकालें, जिस तरह वे निम्न तालिका में सूचीबद्ध हैं. 

    | चरण | समाधान   नाम                                    | नोट                                                                                         |
    |------|----------------------------------------------------|----------------------------------------------------------------------------------------------|
    | 1 | msdyn_ProjectServiceUpgrade_managed.cab            | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 2 | ProjectOperations_Anchor                           | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 3 | Dynamics365ProjectOperationsDualWriteEntityMaps    | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 4 | Dynamics365ProjectOperationsDualWrite              | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 5 | ProjectService                                     | कोई अतिरिक्त नोट नहीं.                                                                         |
    | 6 | ProjectServiceCore_Patch                           | कोई अतिरिक्त नोट नहीं.                                                                         |
    | 7 | ProjectServiceCore                                 | कोई अतिरिक्त नोट नहीं.                                                                         |
    | 8 | ProjectServiceDeprecatedComponents                 | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 9 | FieldServiceCommon                                 | Dynamics 365 Finance या Dynamics 365 Supply Chain Management.   |
    | 10 | msdyn_AssetCommon                                  | Dynamics 365 Finance या Dynamics 365 Supply Chain Management.   |
    | 11 | msdyn_TESA_Anchor                                  | Dynamics 365 Field Service के लिए आवश्यक है.                                                     |
    | 12" | msdyn_TESA_Patch                                   | Dynamics 365 Field Service के लिए आवश्यक है.                                                     |
    | 13 | msdyn_TESA                                         | Dynamics 365 Field Service के लिए आवश्यक है.                                                     |
    | 14 | ResourceSchedulingControls                         | Dynamics 365 Field Service के लिए आवश्यक है.                                                     |
    | 15 | MicrosoftDynamicsScheduling3_CumulativePatch       | Dynamics 365 Field Service के लिए आवश्यक है.                                                     |
    | 16 | MicrosoftDynamicsScheduling_Patch_xx               | Dynamics 365 Field Service के लिए आवश्यक है.                                                     |
    | 17 | MicrosoftDynamicsScheduling                        | Dynamics 365 Field Service के लिए आवश्यक है.                                                     |
    | 18 | Dynamics365FinanceAndOperationsAnchor              | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 19 | Dynamics365Notes                                   | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 20 | Dynamics365FinanceAndOperationsDualWriteEntityMaps | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 21 | DualWriteCore                                      | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 22 | Dynamics365AssetManagementApp                      | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 23 | Dynamics365AssetManagement                         | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 24 | Dynamics365SupplyChainExtended                     | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 25 | Dynamics365Financeविस्तारित                         | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 26 | HCMCommon                                          | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 27 | Dynamics365FinanceAndOperationsCommon              | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 28 | पक्ष                                              | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 29 | Dynamics365Company                                 | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 30 | CurrencyExchangeRates                              | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
    | 31 | AssetCommon                                        | यदि नहीं मिलता है, तो इस समाधान को छोड़ दें.                                                            |
