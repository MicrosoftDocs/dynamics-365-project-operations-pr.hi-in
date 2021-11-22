---
title: Dynamics 365 Project Operations की स्थापना रद्द करें
description: यह विषय Dynamics 365 Project Operations में स्थापना रद्द कैसे करते हैं, के बारे में जानकारी प्रदान करता है.
author: stsporen
ms.date: 11/09/2021
ms.topic: article
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b87c9324b1c95c10ef1e18b0fbf4572bdbe76827
ms.sourcegitcommit: b8b7a59eee7d93638446e93726d270316e45ab3d
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 11/10/2021
ms.locfileid: "7783645"
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
    | 9 | FieldServiceCommon                                 | Dynamics 365 Finance या Dynamics 365 Supply Chain Management के साथ दोहरे लेखन के लिए आवश्यक है.   |
    | 10 | msdyn_AssetCommon                                  | Dynamics 365 Finance या Dynamics 365 Supply Chain Management के साथ दोहरे लेखन के लिए आवश्यक है.   |
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