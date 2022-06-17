---
title: नए कस्टम निकाय फ़ॉर्म जोड़ें (Project Service Automation 2.x)
description: यह लेख अवसरों, उद्धरणों, आदेशों या इनवॉइस के लिए कस्टम निकाय प्रपत्र जोड़ने के तरीके के बारे में जानकारी प्रदान करता है Dynamics 365 Project Service Automation 2. x
author: makk
ms.custom:
- dyn365-projectservice
ms.date: 3/14/2019
ms.topic: article
ms.author: makk
audience: admin
search.audienceType:
- admin
- customizer
search.app:
- D365PS
- ProjectOperations
ms.reviewer: johnmichalak
ms.openlocfilehash: b7e5cbefd9d9705e0bafcb2551e1ce56457a187e
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922730"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a>नए कस्टम निकाय फ़ॉर्म जोड़ें (Project Service Automation 2.x)

[!include [banner](../../includes/psa-now-project-operations.md)]

## <a name="type-field"></a>फील्ड टाइप करें 

Dynamics 365 Project Service Automation **आइटम-आधारित** और **सेवा-आधारित** संस्करणों से इन संस्थाओं के **कार्य-आधारित** संस्करणों को अलग करने के लिए अवसर, कोट, आदेश और चालान संस्थाओं के **प्रकार** (**msdyn\_ordertype**) फ़ील्ड पर निर्भर करता है. इन संस्थाओं के कार्य-आधारित संस्करण PSA द्वारा नियंत्रित किए जाते हैं. ग्राहक पक्ष पर बहुत सारे व्यापारिक तर्क और समाधान का सर्वर पक्ष **टाइप** फ़ील्ड पर निर्भर करता है. इसलिए, यह महत्वपूर्ण है कि जब निकाय बनाई जाती हैं, तो फ़ील्ड को एक सही मान के साथ आरंभ किया जाए. गलत मान गलत व्यवहारों का कारण बन सकता है, और कुछ व्यावसायिक तर्क सही तरीके से नहीं चल पाएंगे.

## <a name="automatic-form-switching"></a>स्वचालित रूप से फॉर्म स्विच करना

बिक्री निकाय के रिकॉर्ड के गलत आरंभ और संपादन के कारण संभावित डेटा दुराचरण और अप्रत्याशित व्यवहारों से बचने के लिए, PSA में अब (लीक से हटकर) आउट-ऑफ-बॉक्स रूपों में स्वचालित रूप से स्विचन करने के लिए तर्क शामिल हैं. यह तर्क उपयोगकर्ताओं को कार्य-आधारित संस्करण या किसी अन्य प्रकार के अवसर, उद्धरण, आदेश या चालान निकाय के साथ काम करने के सही तरीके की ओर ले जाता है. जब कोई उपयोगकर्ता किसी अवसर, उद्धरण, आदेश, या चालान निकाय के कार्य-आधारित संस्करण को खोलता है, तो फ़ॉर्म को **परियोजना सूचना** पर भेज दिया (स्विच कर दिया) जाता है.

स्वचालित रूप स्विचिंग तर्क **फॉर्म आईडी** मान और **msdyn\_** ऑर्डर प्रकार फ़ील्ड के बीच चिह्नांकन पर निर्भर करता है. उस चिह्नांकन में सभी आउट-ऑफ-बॉक्स (लीक से हटकर) फॉर्म जोड़े गए हैं. तथापि, कस्टम फॉर्म को मैन्युअल (हाथ से) रूप से यह निर्दिष्ट करने के लिए जोड़ा जाना चाहिए कि उनका किस निकाय को संभालने का प्रयोजन है. यह **msdyn\_ordertype** फ़ील्ड पर आधारित है. यदि फ़ॉर्म स्विचिंग चिह्नांकन में अनुपलब्ध है, तर्क आउट-ऑफ-द-बॉक्स फॉर्म में बदल जाएगा, जो कि निकाय के **msdyn\_ordertype** फ़ील्ड में सहेजे गए मान पर आधारित है.

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a>कस्टम फ़ॉर्म जोड़ें और तर्क स्विच करने वाले फ़ॉर्म को चालू करें

निम्नलिखित उदाहरण दर्शाते हैं कि कस्टम फ़ॉर्म कैसे जोड़ा जाता है, **मेरी परियोजना जानकारी**, ताकि यह कार्य-आधारित अवसरों के साथ काम करे. इसी प्रक्रिया का उपयोग कस्टम फ़ॉर्म को जोड़ने के लिए किया जाता है, ताकि वे उद्धरण, आदेश और चालान के साथ काम करें.

**परियोजना जानकारी** फ़ॉर्म का एक कस्टम संस्करण बनाने के लिए इन चरणों का पालन करें.

1. अवसर निकाय में, **परियोजना जानकारी** फ़ॉर्म खोलें, और **मेरी परियोजना जानकारी** नाम के तहत एक कॉपी सहेजें.
2. नए फॉर्म खोलें, और फिर, प्रॉपर्टीज़ में, सुनिश्चित करें कि **परियोजना जानकारी** फॉर्म से फॉर्म आरंभीकरण स्क्रिप्ट मौजूद हैं. 

    > [!IMPORTANT]
    > स्क्रिप्ट को न हटाएं. अन्यथा, कुछ डेटा को गलत तरीके से आरंभ किया जा सकता है.

3. सत्यापित करें कि **प्रकार** (**msdyn\_ordertype**) फ़ील्ड फ़ॉर्म में मौजूद है. 

    > [!IMPORTANT]
    > इस फ़ील्ड को न हटाएं. अन्यथा, स्क्रिप्ट का आरंभीकरण विफल हो जाएगा.

4. नए फॉर्म का **formId** मान ज्ञात करें. आप इस चरण को दो तरीकों से पूरा कर सकते हैं:

    - अप्रबंधित समाधान के हिस्से के रूप में **मेरी परियोजना जानकारी** एक्सपोर्ट करें, और फिर एक्सपोर्ट किए गए समाधान के customization.xml फ़ाइल में **formId** मूल्य देखें.
    - फॉर्म एडिटर में **मेरी परियोजना जानकारी** फ़ॉर्म खोलें, और फिर URL में **fromId** पैरामीटर के बगल में वैश्विक रूप से विशिष्ट पहचानकर्ता (GUID) खोजें, जैसा कि निम्नलिखित चित्रण में दिखाया गया है.

    ![URL में नए प्रपत्र का formId मूल्य.](media/how-to-add-custom-forms-in-v2.0.png)

5. msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js वेब संसाधन को संपादित करके **msdyn\_ordertype** **formId** मान के लिए चिह्नांकन बनाएं. संसाधन से कोड को हटाएं, और इसे अनुगामी कोड से बदलें.

    ```javascript
    define(["require", "exports"], function (require, exports) {
        "use strict";
        var SalesDocumentCustomFormIds = (function () {
            function SalesDocumentCustomFormIds() {
            }
            SalesDocumentCustomFormIds.overwriteFormIds = function (mappedFormIds) {
                /*
                ---- Notes ----
                mappedFormIds[SalesEntity][OrderType] => The array of forms IDs that support particular entity and order type
                Add or overwrite customized formId for the particular entity and order type by calling:
                    mappedFormIds[<EntityType>][<msdyn_ordertype>].push("<formId>");
                Allowed msdyn_ordertype values for reference:
                    ServiceBased: 690970002 (Field Service version of the entity)
                    WorkBased: 192350001 (PSA version of the entity)
                    ItemBased: 192350000 (Regular out of the box entity)
                Uncomment and update one of the following lines to register custom PSA form for required entity:
                */      
                //mappedFormIds[1][192350001].push("<formId>"); //Quote
                //mappedFormIds[5][192350001].push("<formId>"); //Quote Line
                //mappedFormIds[2][192350001].push("<formId>"); //Sales Order
                //mappedFormIds[6][192350001].push("<formId>"); //Sales Order Line
                // In this example we have added new form for Opportunity
                mappedFormIds[0][192350001].push("192EE537-DCC4-45D3-B7AF-EA694B9113D2"); //Opportunity
                //mappedFormIds[4][192350001].push("<formId>"); //Opportunity Line
            };
            return SalesDocumentCustomFormIds;
        }());
        exports.default = SalesDocumentCustomFormIds;
    });
    ```

6. सहेजें और फिर अनुकूलन प्रकाशित करें.


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
