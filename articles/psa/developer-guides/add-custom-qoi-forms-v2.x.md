---
title: नए कस्टम निकाय फ़ॉर्म जोड़ें (Project Service Automation 2.x)
description: यह विषय Dynamics 365 Project Service Automation 2.x में अवसरों, उद्धरणों, आदेशों या चालानों के लिए कस्टम निकाय फॉर्म को जोड़ने के बारे में जानकारी प्रदान करता है.
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
ms.openlocfilehash: 400d817ee7cbae6f6da95db4286ad6c4d6ff349a
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6007998"
---
# <a name="add-new-custom-entity-forms-project-service-automation-2x"></a><span data-ttu-id="7a904-103">नए कस्टम निकाय फ़ॉर्म जोड़ें (Project Service Automation 2.x)</span><span class="sxs-lookup"><span data-stu-id="7a904-103">Add new custom entity forms (Project Service Automation 2.x)</span></span>

[!include [banner](../../includes/psa-now-project-operations.md)]

## <a name="type-field"></a><span data-ttu-id="7a904-104">फील्ड टाइप करें</span><span class="sxs-lookup"><span data-stu-id="7a904-104">Type field</span></span> 

<span data-ttu-id="7a904-105">Dynamics 365 Project Service Automation **आइटम-आधारित** और **सेवा-आधारित** संस्करणों से इन संस्थाओं के **कार्य-आधारित** संस्करणों को अलग करने के लिए अवसर, कोट, आदेश और चालान संस्थाओं के **प्रकार** (**msdyn\_ordertype**) फ़ील्ड पर निर्भर करता है.</span><span class="sxs-lookup"><span data-stu-id="7a904-105">Dynamics 365 Project Service Automation relies on the **Type** (**msdyn\_ordertype**) field of the Opportunity, Quote, Order, and Invoice entities to distinguish **work-based** versions of these entities from **item-based** and **service-based** versions.</span></span> <span data-ttu-id="7a904-106">इन संस्थाओं के कार्य-आधारित संस्करण PSA द्वारा नियंत्रित किए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="7a904-106">Work-based versions of these entities are handled by PSA.</span></span> <span data-ttu-id="7a904-107">ग्राहक पक्ष पर बहुत सारे व्यापारिक तर्क और समाधान का सर्वर पक्ष **टाइप** फ़ील्ड पर निर्भर करता है.</span><span class="sxs-lookup"><span data-stu-id="7a904-107">Lots of business logic on the client side and server side of the solution depends on the **Type** field.</span></span> <span data-ttu-id="7a904-108">इसलिए, यह महत्वपूर्ण है कि जब निकाय बनाई जाती हैं, तो फ़ील्ड को एक सही मान के साथ आरंभ किया जाए.</span><span class="sxs-lookup"><span data-stu-id="7a904-108">Therefore, it's important that the field be initialized with a correct value when the entities are created.</span></span> <span data-ttu-id="7a904-109">गलत मान गलत व्यवहारों का कारण बन सकता है, और कुछ व्यावसायिक तर्क सही तरीके से नहीं चल पाएंगे.</span><span class="sxs-lookup"><span data-stu-id="7a904-109">An incorrect value can cause incorrect behaviors, and some business logic might not run correctly.</span></span>

## <a name="automatic-form-switching"></a><span data-ttu-id="7a904-110">स्वचालित रूप से फॉर्म स्विच करना</span><span class="sxs-lookup"><span data-stu-id="7a904-110">Automatic form switching</span></span>

<span data-ttu-id="7a904-111">बिक्री निकाय के रिकॉर्ड के गलत आरंभ और संपादन के कारण संभावित डेटा दुराचरण और अप्रत्याशित व्यवहारों से बचने के लिए, PSA में अब (लीक से हटकर) आउट-ऑफ-बॉक्स रूपों में स्वचालित रूप से स्विचन करने के लिए तर्क शामिल हैं.</span><span class="sxs-lookup"><span data-stu-id="7a904-111">To avoid potential data corruption and unexpected behaviors that are caused by incorrect initialization and editing of the sales entity records, PSA now includes logic for automatic form switching in out-of-box forms.</span></span> <span data-ttu-id="7a904-112">यह तर्क उपयोगकर्ताओं को कार्य-आधारित संस्करण या किसी अन्य प्रकार के अवसर, उद्धरण, आदेश या चालान निकाय के साथ काम करने के सही तरीके की ओर ले जाता है.</span><span class="sxs-lookup"><span data-stu-id="7a904-112">This logic takes users to the correct form for working with the work-based version or any other type of Opportunity, Quote, Order, or Invoice entity.</span></span> <span data-ttu-id="7a904-113">जब कोई उपयोगकर्ता किसी अवसर, उद्धरण, आदेश, या चालान निकाय के कार्य-आधारित संस्करण को खोलता है, तो फ़ॉर्म को **परियोजना सूचना** पर भेज दिया (स्विच कर दिया) जाता है.</span><span class="sxs-lookup"><span data-stu-id="7a904-113">When a user opens the work-based version of an Opportunity, Quote, Order, or Invoice entity, the form is switched to **Project Information**.</span></span>

<span data-ttu-id="7a904-114">स्वचालित रूप स्विचिंग तर्क **फॉर्म आईडी** मान और **msdyn\_** ऑर्डर प्रकार फ़ील्ड के बीच चिह्नांकन पर निर्भर करता है.</span><span class="sxs-lookup"><span data-stu-id="7a904-114">The automatic form switching logic relies on the mapping between the **formId** value and the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="7a904-115">उस चिह्नांकन में सभी आउट-ऑफ-बॉक्स (लीक से हटकर) फॉर्म जोड़े गए हैं.</span><span class="sxs-lookup"><span data-stu-id="7a904-115">All out-of-box forms have been added to that mapping.</span></span> <span data-ttu-id="7a904-116">तथापि, कस्टम फॉर्म को मैन्युअल (हाथ से) रूप से यह निर्दिष्ट करने के लिए जोड़ा जाना चाहिए कि उनका किस निकाय को संभालने का प्रयोजन है.</span><span class="sxs-lookup"><span data-stu-id="7a904-116">However, custom forms must be manually added to indicate which version of the entity they are intended to handle.</span></span> <span data-ttu-id="7a904-117">यह **msdyn\_ordertype** फ़ील्ड पर आधारित है.</span><span class="sxs-lookup"><span data-stu-id="7a904-117">This is based on the **msdyn\_ordertype** field.</span></span> <span data-ttu-id="7a904-118">यदि फ़ॉर्म स्विचिंग चिह्नांकन में अनुपलब्ध है, तर्क आउट-ऑफ-द-बॉक्स फॉर्म में बदल जाएगा, जो कि निकाय के **msdyn\_ordertype** फ़ील्ड में सहेजे गए मान पर आधारित है.</span><span class="sxs-lookup"><span data-stu-id="7a904-118">If the form switching is missing from the mapping, logic will switch to the out-of-box form, based on the value that is saved in the **msdyn\_ordertype** field of the entity.</span></span>

## <a name="add-custom-forms-and-turn-on-the-form-switching-logic"></a><span data-ttu-id="7a904-119">कस्टम फ़ॉर्म जोड़ें और तर्क स्विच करने वाले फ़ॉर्म को चालू करें</span><span class="sxs-lookup"><span data-stu-id="7a904-119">Add custom forms and turn on the form switching logic</span></span>

<span data-ttu-id="7a904-120">निम्नलिखित उदाहरण दर्शाते हैं कि कस्टम फ़ॉर्म कैसे जोड़ा जाता है, **मेरी परियोजना जानकारी**, ताकि यह कार्य-आधारित अवसरों के साथ काम करे.</span><span class="sxs-lookup"><span data-stu-id="7a904-120">The following example shows how to add a custom form, **My Project Information**, so that it works with work-based opportunities.</span></span> <span data-ttu-id="7a904-121">इसी प्रक्रिया का उपयोग कस्टम फ़ॉर्म को जोड़ने के लिए किया जाता है, ताकि वे उद्धरण, आदेश और चालान के साथ काम करें.</span><span class="sxs-lookup"><span data-stu-id="7a904-121">The same process is used to add custom forms so that they work with quotes, orders, and invoices.</span></span>

<span data-ttu-id="7a904-122">**परियोजना जानकारी** फ़ॉर्म का एक कस्टम संस्करण बनाने के लिए इन चरणों का पालन करें.</span><span class="sxs-lookup"><span data-stu-id="7a904-122">Follow these steps to create a custom version of the **Project Information** form.</span></span>

1. <span data-ttu-id="7a904-123">अवसर निकाय में, **परियोजना जानकारी** फ़ॉर्म खोलें, और **मेरी परियोजना जानकारी** नाम के तहत एक कॉपी सहेजें.</span><span class="sxs-lookup"><span data-stu-id="7a904-123">In the Opportunity entity, open the **Project Information** form, and save a copy under the name **My Project Information**.</span></span>
2. <span data-ttu-id="7a904-124">नए फॉर्म खोलें, और फिर, प्रॉपर्टीज़ में, सुनिश्चित करें कि **परियोजना जानकारी** फॉर्म से फॉर्म आरंभीकरण स्क्रिप्ट मौजूद हैं.</span><span class="sxs-lookup"><span data-stu-id="7a904-124">Open the new form, and then, in the properties, make sure that the form initialization scripts from the **Project Information** form are present.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="7a904-125">स्क्रिप्ट को न हटाएं.</span><span class="sxs-lookup"><span data-stu-id="7a904-125">Don't remove the scripts.</span></span> <span data-ttu-id="7a904-126">अन्यथा, कुछ डेटा को गलत तरीके से आरंभ किया जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="7a904-126">Otherwise, some data might be initialized incorrectly.</span></span>

3. <span data-ttu-id="7a904-127">सत्यापित करें कि **प्रकार** (**msdyn\_ordertype**) फ़ील्ड फ़ॉर्म में मौजूद है.</span><span class="sxs-lookup"><span data-stu-id="7a904-127">Verify that the **Type** (**msdyn\_ordertype**) field is present in the form.</span></span> 

    > [!IMPORTANT]
    > <span data-ttu-id="7a904-128">इस फ़ील्ड को न हटाएं.</span><span class="sxs-lookup"><span data-stu-id="7a904-128">Don't remove this field.</span></span> <span data-ttu-id="7a904-129">अन्यथा, स्क्रिप्ट का आरंभीकरण विफल हो जाएगा.</span><span class="sxs-lookup"><span data-stu-id="7a904-129">Otherwise, the initialization scripts will fail.</span></span>

4. <span data-ttu-id="7a904-130">नए फॉर्म का **formId** मान ज्ञात करें.</span><span class="sxs-lookup"><span data-stu-id="7a904-130">Find the **formId** value of the new form.</span></span> <span data-ttu-id="7a904-131">आप इस चरण को दो तरीकों से पूरा कर सकते हैं:</span><span class="sxs-lookup"><span data-stu-id="7a904-131">You can complete this step in two ways:</span></span>

    - <span data-ttu-id="7a904-132">अप्रबंधित समाधान के हिस्से के रूप में **मेरी परियोजना जानकारी** एक्सपोर्ट करें, और फिर एक्सपोर्ट किए गए समाधान के customization.xml फ़ाइल में **formId** मूल्य देखें.</span><span class="sxs-lookup"><span data-stu-id="7a904-132">Export the **My Project Information** form as part of an unmanaged solution, and then look up the **formId** value in the customization.xml file of the exported solution.</span></span>
    - <span data-ttu-id="7a904-133">फॉर्म एडिटर में **मेरी परियोजना जानकारी** फ़ॉर्म खोलें, और फिर URL में **fromId** पैरामीटर के बगल में वैश्विक रूप से विशिष्ट पहचानकर्ता (GUID) खोजें, जैसा कि निम्नलिखित चित्रण में दिखाया गया है.</span><span class="sxs-lookup"><span data-stu-id="7a904-133">Open the **My Project Information** form in the form editor, and then look for the globally unique identifier (GUID) next to the **fromId** parameter in the URL, as shown in the following illustration.</span></span>

    ![URL में नए फॉर्म का formId मूल्य](media/how-to-add-custom-forms-in-v2.0.png)

5. <span data-ttu-id="7a904-135">msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js वेब संसाधन को संपादित करके **msdyn\_ordertype** **formId** मान के लिए चिह्नांकन बनाएं.</span><span class="sxs-lookup"><span data-stu-id="7a904-135">Create an **msdyn\_ordertype** mapping for the **formId** value by editing the msdyn\_/SalesDocument/PSSalesDocumentCustomFormIds.js web resource.</span></span> <span data-ttu-id="7a904-136">संसाधन से कोड को हटाएं, और इसे अनुगामी कोड से बदलें.</span><span class="sxs-lookup"><span data-stu-id="7a904-136">Remove the code from the resource, and replace it with the following code.</span></span>

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

6. <span data-ttu-id="7a904-137">सहेजें और फिर अनुकूलन प्रकाशित करें.</span><span class="sxs-lookup"><span data-stu-id="7a904-137">Save and then publish the customizations.</span></span>


[!INCLUDE[footer-include](../../includes/footer-banner.md)]