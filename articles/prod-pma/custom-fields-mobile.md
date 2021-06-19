---
title: iOS और Android पर Microsoft Dynamics 365 Project Timesheet मोबाइल अनुप्रयोग के लिए कस्टम फ़ील्ड लागू करें
description: यह विषय कस्टम फील्ड के क्रियान्वयन के लिए विस्तार के इस्तेमाल का आम पैटर्न उपलब्ध कराता है.
author: Yowelle
ms.date: 05/29/2019
ms.topic: article
ms.prod: ''
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Service industries
ms.author: andchoi
ms.dyn365.ops.version: 10.0.3
ms.search.validFrom: 2019-05-29
ms.openlocfilehash: 23b002559dcbb9118ccb2b36d70707ccb37b19ad
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "6003036"
---
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a><span data-ttu-id="785bd-103">iOS और Android पर Microsoft Dynamics 365 Project Timesheet मोबाइल अनुप्रयोग के लिए कस्टम फ़ील्ड लागू करें</span><span class="sxs-lookup"><span data-stu-id="785bd-103">Implement custom fields for the Microsoft Dynamics 365 Project Timesheet mobile app on iOS and Android</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="785bd-104">यह विषय कस्टम फील्ड के क्रियान्वयन के लिए विस्तार के इस्तेमाल का आम पैटर्न उपलब्ध कराता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-104">This topic provides common patterns for using extensions to implement custom fields.</span></span> <span data-ttu-id="785bd-105">निम्नलिखित विषय शामिल हैं:</span><span class="sxs-lookup"><span data-stu-id="785bd-105">The following topics are covered:</span></span>

- <span data-ttu-id="785bd-106">डेटा के विभिन्न प्रकार, जिसका कस्टम फील्ड फ्रेमवर्क समर्थन करता है</span><span class="sxs-lookup"><span data-stu-id="785bd-106">The various data types that the custom field framework supports</span></span>
- <span data-ttu-id="785bd-107">टाइमशीट एंट्री में रीड-ऑनली या संपादित होने लायक फील्ड को कैसे दिखाएं, और उपयोगकर्ता द्वारा उपलब्ध मूल्य को डेटाबेस में कैसे सुरक्षित रखें</span><span class="sxs-lookup"><span data-stu-id="785bd-107">How to show read-only or editable fields on timesheet entries, and save user-provided values back to the database</span></span>
- <span data-ttu-id="785bd-108">टाइमशीट हेडर में रीड-ओनली फील्ड को कैसे दिखाएं</span><span class="sxs-lookup"><span data-stu-id="785bd-108">How to show read-only fields on the timesheet header</span></span>
- <span data-ttu-id="785bd-109">फील्ड में डिफॉल्ट मूल्य दर्ज करने के लिए अन्य कस्टम बिजनस लॉजिक को कैसे एकीकृत करें और अतिरिक्त सत्यापन करें</span><span class="sxs-lookup"><span data-stu-id="785bd-109">How to integrate other custom business logic to enter default values in fields and do additional validation</span></span>

## <a name="audience"></a><span data-ttu-id="785bd-110">श्रोता</span><span class="sxs-lookup"><span data-stu-id="785bd-110">Audience</span></span>

<span data-ttu-id="785bd-111">यह विषय उन डेवलपर के लिए है जो Microsoft Dynamics 365 Project Timesheet मोबाइल एप्लिकेशन में अपने कस्टम फील्ड को एकीकृत कर रहे हैं, जो कि Apple iOS और Google Android के लिए उपलब्ध है.</span><span class="sxs-lookup"><span data-stu-id="785bd-111">This topic is intended for developers who are integrating their custom fields into the Microsoft Dynamics 365 Project Timesheet mobile application that is available for Apple iOS and Google Android.</span></span> <span data-ttu-id="785bd-112">ऐसा माना जाता है कि पाठक X++ डेवलपमेंट से प्रॉजेक्ट टाइमशीट की कार्यप्रणाली से परिचित हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-112">The assumption is that readers are familiar with X++ development and project timesheet functionality.</span></span>

## <a name="data-contract--tstimesheetcustomfield-x-class"></a><span data-ttu-id="785bd-113">डेटा अनुबंध- TSTimesheetCustomField X++ क्लास</span><span class="sxs-lookup"><span data-stu-id="785bd-113">Data contract – TSTimesheetCustomField X++ class</span></span>

<span data-ttu-id="785bd-114">**TSTimesheetCustomField** क्लास X++ डेटा अनुबंध क्लास है जो कि टाइमशीट कार्यप्रणाली के लिए कस्टम फील्ड की सूचना का प्रतिनिधित्व करता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-114">The **TSTimesheetCustomField** class is the X++ data contract class that represents information about a custom field for timesheet functionality.</span></span> <span data-ttu-id="785bd-115">कस्टम फील्ड वस्तुओं की सूची TSTimesheetDetails आंकड़ा अनुबंध और TSTimesheetEntry आंकड़ा अनुबंध दोनों में डाला जाता है, ताकि कस्टम फील्ड मोबाइल ऐप में दिख सकें.</span><span class="sxs-lookup"><span data-stu-id="785bd-115">Lists of the custom field objects are passed on both the TSTimesheetDetails data contract and the TSTimesheetEntry data contract to show custom fields in the mobile app.</span></span>

- <span data-ttu-id="785bd-116">**TSTimesheetDetails** - टाइमशीट हैडर अनुबंध.</span><span class="sxs-lookup"><span data-stu-id="785bd-116">**TSTimesheetDetails** - The timesheet header contract.</span></span>
- <span data-ttu-id="785bd-117">**TSTimesheetEntry** - टाइमशीट लेनदेन अनुबंध.</span><span class="sxs-lookup"><span data-stu-id="785bd-117">**TSTimesheetEntry** - The timesheet transaction contract.</span></span> <span data-ttu-id="785bd-118">इन वस्तुओं के समूह के पास समान परियोजना सूचना होती है और **timesheetLineRecId** मूल्य में एक पंक्ति बनाती है.</span><span class="sxs-lookup"><span data-stu-id="785bd-118">Groups of these objects that have the same project information and **timesheetLineRecId** value constitute a line.</span></span>

### <a name="fieldbasetype-types"></a><span data-ttu-id="785bd-119">fieldBaseType (प्रकार)</span><span class="sxs-lookup"><span data-stu-id="785bd-119">fieldBaseType (Types)</span></span>

<span data-ttu-id="785bd-120">**TsTimesheetCustom** वस्तु में **FieldBaseType** प्रॉपर्टी वस्तु फील्ड को निर्धारित करती जो कि अनुप्रयोग में नजर आती है.</span><span class="sxs-lookup"><span data-stu-id="785bd-120">The **FieldBaseType** property on the **TsTimesheetCustom** object determines the type of the field that appears in the app.</span></span> <span data-ttu-id="785bd-121">दिए गए **प्रकार** मूल्य, जिसका समर्थन किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-121">The following **Types** values that are supported.</span></span>

| <span data-ttu-id="785bd-122">प्रकार मान</span><span class="sxs-lookup"><span data-stu-id="785bd-122">Types value</span></span> | <span data-ttu-id="785bd-123">प्रकार</span><span class="sxs-lookup"><span data-stu-id="785bd-123">Type</span></span>              | <span data-ttu-id="785bd-124">नोट्स</span><span class="sxs-lookup"><span data-stu-id="785bd-124">Notes</span></span> |
|-------------|-------------------|-------|
| <span data-ttu-id="785bd-125">0</span><span class="sxs-lookup"><span data-stu-id="785bd-125">0</span></span>           | <span data-ttu-id="785bd-126">स्ट्रिंग (और Enum)</span><span class="sxs-lookup"><span data-stu-id="785bd-126">String (and Enum)</span></span> | <span data-ttu-id="785bd-127">फ़ील्ड टेक्स्ट फ़ील्ड के रूप में प्रकट होती है.</span><span class="sxs-lookup"><span data-stu-id="785bd-127">The field appears as a text field.</span></span> |
| <span data-ttu-id="785bd-128">1</span><span class="sxs-lookup"><span data-stu-id="785bd-128">1</span></span>           | <span data-ttu-id="785bd-129">Integer</span><span class="sxs-lookup"><span data-stu-id="785bd-129">Integer</span></span>           | <span data-ttu-id="785bd-130">मूल्य को बिना दशमलव स्थान के एक संख्या के रूप में दिखाया गया है.</span><span class="sxs-lookup"><span data-stu-id="785bd-130">The value is shown as a number without decimal places.</span></span> |
| <span data-ttu-id="785bd-131">2</span><span class="sxs-lookup"><span data-stu-id="785bd-131">2</span></span>           | <span data-ttu-id="785bd-132">वास्तविक</span><span class="sxs-lookup"><span data-stu-id="785bd-132">Real</span></span>              | <span data-ttu-id="785bd-133">मान को संख्या के रूप में दिखाया जाता है जिसमें दशमलव स्थान होता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-133">The value is shown as a number that has decimal places.</span></span><p><span data-ttu-id="785bd-134">अनुप्रयोग में वास्तविक मूल्य को एक मुद्रा के रूप में दिखाने के लिए **fieldExtenededType** प्रॉपर्टी का इस्तेमाल किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-134">To show the real value as a currency in the app, use the **fieldExtenededType** property.</span></span> <span data-ttu-id="785bd-135">आप **दशमलों की संख्या** प्रॉपर्टी का इस्तेमाल कर दिखाए जाने वाले दशमलव स्थान की संख्या तय कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-135">You can use the **numberOfDecimals** property to set the number of decimal places that are shown.</span></span></p> |
| <span data-ttu-id="785bd-136">3</span><span class="sxs-lookup"><span data-stu-id="785bd-136">3</span></span>           | <span data-ttu-id="785bd-137">दिनांक</span><span class="sxs-lookup"><span data-stu-id="785bd-137">Date</span></span>              | <span data-ttu-id="785bd-138">तारीख का फ़ॉर्मेट उपयोगकर्ता के **तारीख, समय और संख्या फ़ॉर्मेट** सेटिंग द्वारा निर्धारित किया जाता है, जिसका वर्णन **उपयोगकर्ता विकल्पों** में **भाषा व देश/क्षेत्र वरीयता** के अंदर किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-138">Date formats are determined by the user's **Date, times, and number format** setting that is specified under **Language and country/region preference** in **User options**.</span></span> |
| <span data-ttu-id="785bd-139">4</span><span class="sxs-lookup"><span data-stu-id="785bd-139">4</span></span>           | <span data-ttu-id="785bd-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="785bd-140">Boolean</span></span>           | |
| <span data-ttu-id="785bd-141">15</span><span class="sxs-lookup"><span data-stu-id="785bd-141">15</span></span>          | <span data-ttu-id="785bd-142">GUID</span><span class="sxs-lookup"><span data-stu-id="785bd-142">GUID</span></span>              | |
| <span data-ttu-id="785bd-143">16</span><span class="sxs-lookup"><span data-stu-id="785bd-143">16</span></span>          | <span data-ttu-id="785bd-144">Int64</span><span class="sxs-lookup"><span data-stu-id="785bd-144">Int64</span></span>             | |

- <span data-ttu-id="785bd-145">अगर **stringOptions** प्रॉपर्टी **TSTimesheetCustomField** विषय में उपलब्ध नहीं कराया जाता, तो उपयोगकर्ता को एक रिक्त-टेक्स्ट फील्ड उपलब्ध कराया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-145">If the **stringOptions** property isn't provided on the **TSTimesheetCustomField** object, a free-text field is provided to the user.</span></span>

    <span data-ttu-id="785bd-146">**stringLength** गुण का इस्तेमाल अधिक से अधिक स्ट्रिंग की लंबाई निर्धारित करने के लिए किया जा सकता है जो कि उपयोगकर्ता दर्ज कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-146">The **stringLength** property can be used to set the maximum string length that users can enter.</span></span>

- <span data-ttu-id="785bd-147">अगर **stringOptions** प्रॉपर्टी **TSTimesheetCustomField** विषय में उपलब्ध कराया जाता है, तो सूचीबद्ध किए गए अवयव एकमात्र मूल्य होते हैं, जो कि उपयोगकर्ता विकल्प बटन (रेडियो बटन) का उपयोग कर चुन सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-147">If the **stringOptions** property is provided on the **TSTimesheetCustomField** object, those list elements are the only values that users can select by using option buttons (radio buttons).</span></span>

    <span data-ttu-id="785bd-148">इस मामले में, स्ट्रिंग फील्ड यूजर एंट्री के उद्देश्य से असंख्य मूल्य के रूप में काम कर सकती है.</span><span class="sxs-lookup"><span data-stu-id="785bd-148">In this case, the string field can act as an enum value for the purpose of user entry.</span></span> <span data-ttu-id="785bd-149">डेटाबेस के मान को इनम के रूप में सेव करने के लिए, कमांड की श्रृंखला का उपयोग करके डेटाबेस में सेव करने से पहले मैन्युअल रूप से स्ट्रिंग मान को एनम मान पर मैप करें (उदाहरण के लिये इस विषय पर बाद में देखें "एक टाइमशीट प्रविष्टि को अनुप्रयोग से डेटाबेस में पुन: सेव करने के लिये TSTimesheetEntryService वर्ग पर कमांड की श्रृंखला का प्रयोग" अनुभाग).</span><span class="sxs-lookup"><span data-stu-id="785bd-149">To save the value to the database as an enum, manually map the string value back to the enum value before you save to the database by using chain of command (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a><span data-ttu-id="785bd-150">fieldExtendedType (TSCustomFieldExtendedType)</span><span class="sxs-lookup"><span data-stu-id="785bd-150">fieldExtendedType (TSCustomFieldExtendedType)</span></span>

<span data-ttu-id="785bd-151">आप वास्तविक मूल्य को मुद्रा के रूप में फॉर्मैट करने के लिए इस प्रॉपर्टी का उपयोग कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-151">You can use this property to format real values as currency.</span></span> <span data-ttu-id="785bd-152">यह दृष्टिकोण तब लागू होता है जब **fieldBaseType** मूल्य **वास्तविक** हो.</span><span class="sxs-lookup"><span data-stu-id="785bd-152">This approach is applicable only when the **fieldBaseType** value is **Real**.</span></span>

- <span data-ttu-id="785bd-153">**TSCustomFieldExtendedType:कोई नहीं** – में कोई फॉर्मैटिंग लागू नहीं होता.</span><span class="sxs-lookup"><span data-stu-id="785bd-153">**TSCustomFieldExtendedType:None** – No formatting is applied.</span></span>
- <span data-ttu-id="785bd-154">**TSCustomFieldExtendedType::मुद्रा** – मूल्य को मुद्रा के रूप में फॉर्मैट करता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-154">**TSCustomFieldExtendedType::Currency** – Format the value as currency.</span></span>

    <span data-ttu-id="785bd-155">जब मुद्रा फॉर्मैटिंग सक्रिय है, तब **stringValue** फील्ड का इस्तमाल मुद्रा कोड डालने में किया जा सकता है, जो कि ऐप में दिखना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="785bd-155">When currency formatting is active, the **stringValue** field can be used pass the currency code that should be shown in the app.</span></span> <span data-ttu-id="785bd-156">मान केवल पढ़ने के लिए मान है.</span><span class="sxs-lookup"><span data-stu-id="785bd-156">The value is a read-only value.</span></span>

    <span data-ttu-id="785bd-157">**वास्तविक मूल्य** फ़ील्ड में धन राशि है जिसे डेटाबेस में सहेजा जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="785bd-157">The **realValue** field contains the money amount that should be saved to the database.</span></span>

### <a name="fieldsection-tscustomfieldsection"></a><span data-ttu-id="785bd-158">fieldSection (TSCustomFieldSection)</span><span class="sxs-lookup"><span data-stu-id="785bd-158">fieldSection (TSCustomFieldSection)</span></span>

<span data-ttu-id="785bd-159">आप इस निर्दिष्ट प्रॉपर्टी का इस्तेमाल कर सकते हैं जहां कस्टम फील्ड गुण में नजर आने चाहिए.</span><span class="sxs-lookup"><span data-stu-id="785bd-159">You can use this property specify where the custom field should appear in the app.</span></span>

- <span data-ttu-id="785bd-160">**TSCustomFieldSection::हेडर** – फील्ड अनुप्रयोग में **और ब्यौरा देखें** सेक्शन में नजर आएगा.</span><span class="sxs-lookup"><span data-stu-id="785bd-160">**TSCustomFieldSection::Header** – The field will appear in the **View more details** section in the app.</span></span> <span data-ttu-id="785bd-161">ये फील्ड हमेशा रीड-ओनली रहते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-161">These fields are always read-only.</span></span>
- <span data-ttu-id="785bd-162">**TSCustomFieldSection::पंक्ति** – फील्ड टाइमशीट प्रविष्टियों में सबसे अलग सभी पंक्ति फील्ड के बाद नजर आएगा.</span><span class="sxs-lookup"><span data-stu-id="785bd-162">**TSCustomFieldSection::Line** – The field will appear after all the out-of-box line fields on timesheet entries.</span></span> <span data-ttu-id="785bd-163">ये फ़ील्ड या तो संपादन योग्य या केवल पढ़ने योग्य हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-163">These fields can be either editable or read-only.</span></span>

### <a name="fieldname-fieldnameshort"></a><span data-ttu-id="785bd-164">fieldName (FieldNameShort)</span><span class="sxs-lookup"><span data-stu-id="785bd-164">fieldName (FieldNameShort)</span></span>

<span data-ttu-id="785bd-165">यह प्रॉपर्टी फील्ड को चिह्नित करता है जब ऐप द्वारा उपलब्ध मूल्य डेटाबेस में वापस सुरक्षित रखा जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-165">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="tablename-tablenameshort"></a><span data-ttu-id="785bd-166">tableName (TableNameShort)</span><span class="sxs-lookup"><span data-stu-id="785bd-166">tableName (TableNameShort)</span></span>

<span data-ttu-id="785bd-167">यह प्रॉपर्टी फील्ड को चिह्नित करता है जब ऐप द्वारा उपलब्ध मूल्य डेटाबेस में वापस सुरक्षित रखा जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-167">This property identifies the field when values that the app provides are saved back to the database.</span></span>

### <a name="iseditable-noyes"></a><span data-ttu-id="785bd-168">isEditable (NoYes)</span><span class="sxs-lookup"><span data-stu-id="785bd-168">isEditable (NoYes)</span></span>

<span data-ttu-id="785bd-169">प्रॉपर्टी को **हां** में सेट करें, यह दिखाने के लिए टाइमशीट प्रविष्टि सेक्शन में फील्ड उपयोकर्ताओं द्वारा संपादित किया जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="785bd-169">Set this property to **Yes** to specify that the field in the timesheet entry section should be editable by users.</span></span> <span data-ttu-id="785bd-170">फील्ड को रीड-ओनली बनाने के लिए प्रॉपर्टी को **ना** में सेट करें.</span><span class="sxs-lookup"><span data-stu-id="785bd-170">Set the property to **No** to make the field read-only.</span></span>

### <a name="ismandatory-noyes"></a><span data-ttu-id="785bd-171">isMandatory (NoYes)</span><span class="sxs-lookup"><span data-stu-id="785bd-171">isMandatory (NoYes)</span></span>

<span data-ttu-id="785bd-172">प्रॉपर्टी को **हां** में सेट करें, यह दिखाने के लिए टाइमशीट प्रविष्टि सेक्शन में फ़ील्ड अनिवार्य होना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="785bd-172">Set this property to **Yes** to specify that the field in the timesheet entry section should be mandatory.</span></span>

### <a name="label-str"></a><span data-ttu-id="785bd-173">लेबल (str)</span><span class="sxs-lookup"><span data-stu-id="785bd-173">label (str)</span></span>

<span data-ttu-id="785bd-174">प्रॉपर्टी उस लेबल का वर्णन करता है, जो कि ऐप में फील्ड के पास दिखाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-174">This property specifies the label that is shown next the field in the app.</span></span>

### <a name="stringoptions-list-of-strings"></a><span data-ttu-id="785bd-175">stringOptions (स्ट्रिंग की सूची)</span><span class="sxs-lookup"><span data-stu-id="785bd-175">stringOptions (List of Strings)</span></span>

<span data-ttu-id="785bd-176">प्रॉपर्टी तब लागू होती है जब **fieldBaseType** को **स्ट्रिंग** में सेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-176">This property is applicable only when **fieldBaseType** is set to **String**.</span></span> <span data-ttu-id="785bd-177">अगर **stringOptions** सेट है, तो स्ट्रिंग का मूल्य जो कि विकल्प बटन के माध्यम से चयन के लिए उपलब्ध है, उसे सूची में स्ट्रिंग द्वारा स्पष्ट रूप से बताया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-177">If **stringOptions** is set, the string values that are available for selection via option buttons (radio buttons) are specified by the strings in the list.</span></span> <span data-ttu-id="785bd-178">अगर कोई स्ट्रिंग उपलब्ध नहीं कराया जाता, स्ट्रिंग फील्ड में रिक्त-टेक्स्ट प्रविष्टि की अनुमति होती है. (उदाहरण के लिये इस विषय पर बाद में देखें "एक टाइमशीट प्रविष्टि को अनुप्रयोग से डेटाबेस में पुन: सेव करने के लिये TSTimesheetEntryService वर्ग पर कमांड की श्रृंखला का प्रयोग" अनुभाग).</span><span class="sxs-lookup"><span data-stu-id="785bd-178">If no strings are provided, free-text entry in the string field is allowed (see the “Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database” section later in this topic for an example).</span></span>

### <a name="stringlength-int"></a><span data-ttu-id="785bd-179">stringLength (int)</span><span class="sxs-lookup"><span data-stu-id="785bd-179">stringLength (int)</span></span>

<span data-ttu-id="785bd-180">प्रॉपर्टी स्ट्रिंग फील्ड की अधिकतम लंबाई का उल्लेख करता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-180">This property specifies the maximum length for a string field.</span></span> <span data-ttu-id="785bd-181">यह तब लागू होता है जब **fieldBaseType** को **स्ट्रिंग** में सेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-181">It's applicable only when **fieldBaseType** is set to **String**.</span></span>

### <a name="numberofdecimals-int"></a><span data-ttu-id="785bd-182">numberOfDecimals (int)</span><span class="sxs-lookup"><span data-stu-id="785bd-182">numberOfDecimals (int)</span></span>

<span data-ttu-id="785bd-183">प्रॉपर्टी दशमलव स्थानों की संख्या का उल्लेख करती है जो कि वास्तविक फील्ड के लिए दिखाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-183">This property specifies the number of decimal places that are shown for a real field.</span></span> <span data-ttu-id="785bd-184">यह तब लागू होता है जब **fieldBaseType** को **वास्तविक** सेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-184">It's applicable only when **fieldBaseType** is set to **Real**.</span></span>

### <a name="ordersequence-int"></a><span data-ttu-id="785bd-185">orderSequence (int)</span><span class="sxs-lookup"><span data-stu-id="785bd-185">orderSequence (int)</span></span>

<span data-ttu-id="785bd-186">यह प्रॉपर्टी क्रम को नियंत्रित करती है, जिसमें कस्टम फील्ड ऐप में नजर आते हैं, जब एक से अधिक कस्टम फील्ड का उल्लेख किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-186">This property controls the order in which the custom fields are shown in the app when more than one custom field is specified.</span></span> <span data-ttu-id="785bd-187">फील्ड जिनमें सबसे कम संख्याएं होती हैं, वे सबसे पहले दिखाए जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-187">Fields that have lower numbers are shown first.</span></span>

### <a name="booleanvalue-boolean"></a><span data-ttu-id="785bd-188">booleanValue (बूलियन)</span><span class="sxs-lookup"><span data-stu-id="785bd-188">booleanValue (boolean)</span></span>

<span data-ttu-id="785bd-189">**बूलियन** प्रकार के फील्ड के लिए, यह प्रॉपर्टी फील्ड के बूलयिन मूल्य को सर्वर और अनुप्रयोग के बीच हस्तांतरित करता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-189">For fields of the **Boolean** type, this property passes the Boolean value of the field between the server and the app.</span></span>

### <a name="guidvalue-guid"></a><span data-ttu-id="785bd-190">guidValue (guid)</span><span class="sxs-lookup"><span data-stu-id="785bd-190">guidValue (guid)</span></span>

<span data-ttu-id="785bd-191">**GUID** प्रकार के फील्ड के लिए, प्रॉपर्टी फील्ड के ग्लोबली युनीक आइडेंटिफ़ायर (GUID) मूल्य को सर्वर और अनुप्रयोग के बीच हस्तांतरित करती है.</span><span class="sxs-lookup"><span data-stu-id="785bd-191">For fields of the **GUID** type, this property passes the globally unique identifier (GUID) value of the field between the server and the app.</span></span>

### <a name="int64value-int64"></a><span data-ttu-id="785bd-192">int64Value (int64)</span><span class="sxs-lookup"><span data-stu-id="785bd-192">int64Value (int64)</span></span>

<span data-ttu-id="785bd-193">**Int64** प्रकार के फील्ड के लिए प्रॉपर्टी फील्ड के Int64 मूल्य को सर्विर और ऐप के बीच हस्तांतरित करती है.</span><span class="sxs-lookup"><span data-stu-id="785bd-193">For fields of the **Int64** type, this property passes the int64 value of the field between the server and the app.</span></span>

### <a name="intvalue-int"></a><span data-ttu-id="785bd-194">intValue (int)</span><span class="sxs-lookup"><span data-stu-id="785bd-194">intValue (int)</span></span>

<span data-ttu-id="785bd-195">के खेतों के लिए **इंट** प्रकार, यह प्रॉपर्टी सर्वर और ऐप के बीच के क्षेत्र का अंतर मानती है.</span><span class="sxs-lookup"><span data-stu-id="785bd-195">For fields of the **Int** type, this property passes the int value of the field between the server and the app.</span></span>

### <a name="realvalue-real"></a><span data-ttu-id="785bd-196">realValue (वास्तविक)</span><span class="sxs-lookup"><span data-stu-id="785bd-196">realValue (real)</span></span>

<span data-ttu-id="785bd-197">**वास्तविक** प्रकार के फील्ड के लिए, प्रॉपर्टी सर्वर और अनुप्रयोग के बीच फील्ड के मूल्य को हस्तांतरित करती है.</span><span class="sxs-lookup"><span data-stu-id="785bd-197">For fields of the **Real** type, this property passes the real value of the field between the server and the app .</span></span>

### <a name="stringvalue-str"></a><span data-ttu-id="785bd-198">stringValue (str)</span><span class="sxs-lookup"><span data-stu-id="785bd-198">stringValue (str)</span></span>

<span data-ttu-id="785bd-199">**स्ट्रिंग** प्रकार के फील्ड के लिए, प्रॉपर्टी फील्ड के स्ट्रिंग मूल्य को सर्विर और ऐप के बीच हस्तांतरित करती है.</span><span class="sxs-lookup"><span data-stu-id="785bd-199">For fields of the **String** type, this property passes the string value of the field between the server and the app.</span></span> <span data-ttu-id="785bd-200">इसका उपयोग **वास्तविक** प्रकार के फील्ड के लिए होता है, जिसे मुद्रा के रूप में फॉर्मैट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-200">It's also used for fields of the **Real** type that are formatted as currency.</span></span> <span data-ttu-id="785bd-201">उन फील्ड के लिए, प्रॉपर्टी का उपयोग मुद्रा कोड को ऐप में हस्तांतरित करने में होता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-201">For those fields, the property is used to pass the currency code to the app.</span></span>

### <a name="datevalue-date"></a><span data-ttu-id="785bd-202">dateValue (date)</span><span class="sxs-lookup"><span data-stu-id="785bd-202">dateValue (date)</span></span>

<span data-ttu-id="785bd-203">**तारीख** प्रकार के फील्ड के लिए, प्रॉपर्टी फील्ड के तारीख मूल्य को सर्विर और ऐप के बीच हस्तांतरित करती है.</span><span class="sxs-lookup"><span data-stu-id="785bd-203">For fields of the **Date** type, this property passes the date value of the field between the server and the app.</span></span>

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a><span data-ttu-id="785bd-204">टाइमशीट प्रविष्टि सेक्शन में कस्टम फील्ड को दिखाना और सुरक्षित करना</span><span class="sxs-lookup"><span data-stu-id="785bd-204">Show and save a custom field in the timesheet entry section</span></span>

<span data-ttu-id="785bd-205">नीचे एक मोबाइल के टाइमशीट प्रविष्टि निर्माण का स्क्रीनशॉट है.</span><span class="sxs-lookup"><span data-stu-id="785bd-205">Below is a screenshot from the mobile app of a timesheet entry creation.</span></span> <span data-ttu-id="785bd-206">यह "समय प्रविष्टि'' सेक्शन जिसे ''टेस्ट स्ट्रिंग'' कहा जाता है, उसमें पहले से तय "दूसरे विकल्प" के असंख्य मूल्य के साथ एकदम अलग तरह के फील्ड और कस्टम फील्ड को दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-206">It shows the out-of-box fields and a custom field in the "Time entry" section called "Test string" with an enum value of "Second option" already set.</span></span>

![अनुप्रयोग में टेस्ट स्ट्रिंग कस्टम फ़ील्ड](media/timesheet-entry.jpg)



<span data-ttu-id="785bd-208">नीचे मोबाइल ऐप का एक स्क्रीन शॉट है जिसमें "टेस्ट स्ट्रिंग" कस्टम फ़ील्ड के लिए उपलब्ध असंख्य विकल्पों में से एक का चुनाव उपयोगकर्ता कर रहा है.</span><span class="sxs-lookup"><span data-stu-id="785bd-208">Below is a screenshot from the mobile app of the user selecting one of the enum options available for the "Test string" custom field.</span></span>  <span data-ttu-id="785bd-209">दो विकल्प "पहला विकल्प" और "दूसरा विकल्प" है जिसे रेडियो बटन के रूप में दिखाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-209">The two options are "First option" and "Second option" shown as radio buttons.</span></span> <span data-ttu-id="785bd-210">वर्तमान में दूसरा विकल्प चुना गया है.</span><span class="sxs-lookup"><span data-stu-id="785bd-210">The second option is currently selected.</span></span>

![विकल्प बटनों (रेडियो बटन) टेस्ट स्ट्रिंग कस्टम फील्ड के लिए होता है](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="785bd-212">TSTimesheetLine तालिका को विस्तार दें ताकि इसके पास कस्टम फील्ड हो</span><span class="sxs-lookup"><span data-stu-id="785bd-212">Extend the TSTimesheetLine table so that it has a custom field</span></span>

<span data-ttu-id="785bd-213">विशिष्ट परिदृश्यों में, यह संभावना है कि टाइमशीट प्रविष्टि सेक्शन में एक कस्टम फ़ील्ड का डेटा TSTimesheetLine तालिका में सहेजा जाएगा.</span><span class="sxs-lookup"><span data-stu-id="785bd-213">In typical scenarios, it's likely that the data for a custom field in the timesheet entry section will be saved to the TSTimesheetLine table.</span></span> <span data-ttu-id="785bd-214">हालांकि, अन्य तालिकाओं का उपयोग किया जा सकता है यदि आंकड़ा एक TSTimesheetTrans रिकॉर्ड के आधार पर प्राप्त किया जा सकता है जो प्रदान किया गया है, या यदि उसमें विशिष्ट रिकॉर्ड संदर्भ नहीं है (उदाहरण के लिए, यदि फ़ील्ड को केवल परियोजना मानक में रीड-ओनली के रूप में सेट किया जाता है).</span><span class="sxs-lookup"><span data-stu-id="785bd-214">However, other tables can be used if the data can be retrieved based on a TSTimesheetTrans record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="785bd-215">ध्यान दें कि कस्टम फील्ड के पास कोई भी प्रतिभूति डेटाबेस रिकॉर्ड नहीं होगा.</span><span class="sxs-lookup"><span data-stu-id="785bd-215">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="785bd-216">वे X ++ तर्क के आधार पर गतिशील रूप से उत्पन्न हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-216">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="785bd-217">यह दृष्टिकोण केवल-पढ़ने के परिदृश्य में उपयोगी हो सकता है ("टाइमशीट विवरण भरने के लिए TSTimesheetDetails वर्ग के buildCustomFieldListForHeader विधि पर कमांड की श्रृंखला का उपयोग करें" डायनामिक रूप से कस्टम फ़ील्ड मानों के उदाहरण के लिए अनुभाग देखें.)</span><span class="sxs-lookup"><span data-stu-id="785bd-217">This approach can be useful in read-only scenarios (see the “Use chain of command on the TSTimesheetDetails class, buildCustomFieldListForHeader method to fill in timesheet details” section for an example of dynamically generated custom field values.)</span></span>

<span data-ttu-id="785bd-218">नीचे अनुप्रयोग ऑब्जेक्ट ट्री के Visual Studio का स्क्रीनशॉट है.</span><span class="sxs-lookup"><span data-stu-id="785bd-218">Below is a screenshot from Visual Studio of the Application Object Tree.</span></span> <span data-ttu-id="785bd-219">यह TSTimesheetLine तालिका का TestLineString के साथ विस्तार दिखाता है, जिसे कस्टम फील्ड में जोड़ा जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-219">It shows an extension of the TSTimesheetLine table with the TestLineString field added as a custom field.</span></span>

![लाइन का तार](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a><span data-ttu-id="785bd-221">TSTimesheetSettings वर्ग की buildCustomFieldList पद्धति के चेन ऑफ कमांड का इस्तेमाल टाइमशीट प्रविष्टि सेक्शन में फील्ड दिखाने के लिए करता है</span><span class="sxs-lookup"><span data-stu-id="785bd-221">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the timesheet entry section</span></span>

<span data-ttu-id="785bd-222">यह कोड ऐप में फील्ड के लिए डिस्प्ले सेटिंग को नियंत्रित करता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-222">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="785bd-223">उदाहरण के लिए, यह फील्ड, लेबल के प्रकार को नियंत्रित करता है, कि फील्ड अनिवार्य है या नहीं, किस सेक्शन में फील्ड नजर आता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-223">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="785bd-224">उदाहरण के लिए समय प्रविष्टि पर स्ट्रिंग फील्ड दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-224">The following example shows a string field on time entries.</span></span> <span data-ttu-id="785bd-225">फील्ड के दो विकल्प होते हैं, **पहला विकल्प** और **दूसरा विकल्प**, ये विकल्प बटन (रेडियो बटन) के माध्यम से उपलब्ध होते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-225">This field has two options, **First option** and **Second option**, that are available via option buttons (radio buttons).</span></span> <span data-ttu-id="785bd-226">अनुप्रयोग में फील्ड **TestLineString** फील्ड से संबंधित होते हैं, जो कि TSTimesheetLine तालिका से जोड़े जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-226">The field in the app is associated with the **TestLineString** field that is added to the TSTimesheetLine table.</span></span>

<span data-ttu-id="785bd-227">कस्टम फ़ील्ड गुणों के प्रारंभ को सरल बनाने के लिए **TSTimesheetCustomField::newFromMetatdata()** विधि के उपयोग पर ध्यान दें: **fieldBaseType**, **tableName**, **fieldname**, **लेबल**, **isEditable**, **isMandatory**, **stringLength**, and **numberOfDecimals**.</span><span class="sxs-lookup"><span data-stu-id="785bd-227">Note the use of the **TSTimesheetCustomField::newFromMetatdata()** method to simplify the initialization of the custom field properties: **fieldBaseType**, **tableName**, **fieldname**, **label**, **isEditable**, **isMandatory**, **stringLength**, and **numberOfDecimals**.</span></span> <span data-ttu-id="785bd-228">आपको जैसा ठीक लगे, उस अनुसार आप इन मानकों को मैनुअली निर्धारित कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-228">You can also set these parameters manually, as you prefer.</span></span>

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('Second option');
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a><span data-ttu-id="785bd-229">TSTimesheetEntry वर्ग की buildCustomFieldListForEntry पद्धति के चेन ऑफ कमांड का इस्तेमाल टाइमशीट प्रविष्टि में मान दर्ज करने के लिए करता है</span><span class="sxs-lookup"><span data-stu-id="785bd-229">Use chain of command on the buildCustomFieldListForEntry method of the TSTimesheetEntry class to enter values in a timesheet entry</span></span>

<span data-ttu-id="785bd-230">**buildCustomFieldListForEntry** पद्धति का उपयोग मोबाइल ऐप में सहेजी गई टाइमशीट पंक्तियों में मूल्य को दर्ज करने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-230">The **buildCustomFieldListForEntry** method is used to enter values on the saved timesheet lines in the mobile app.</span></span> <span data-ttu-id="785bd-231">TSTimesheetTrans रिकॉर्ड को एक मानक के रूप में लेता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-231">It takes a TSTimesheetTrans record as a parameter.</span></span> <span data-ttu-id="785bd-232">उस रिकॉर्ड से फील्ड का उपयोग ऐप में कस्टम फील्ड मूल्य को भरने में किया जा सकता है</span><span class="sxs-lookup"><span data-stu-id="785bd-232">Fields from that record can be used to fill in the custom field value in the app.</span></span>

```xpp
...
[ExtensionOf(classStr(TsTimesheetEntry))]
final class TsTimesheetEntry_Extension
{
    protected List buildCustomFieldListForEntry(TSTimesheetTrans _tsTimesheetTrans)
    {
        List customFieldList = next buildCustomFieldListForEntry(_tsTimesheetTrans);
        TSTimesheetLine tsTimesheetLine = _tsTimesheetTrans.timesheetLine();
        TSTimesheetCustomField tsTimesheetCustomField;
        tsTimesheetCustomField =
        TSTimesheetCustomField::newFromMetadata(tableNum(TsTimesheetLine),
        fieldNum(TSTimesheetLine, TestLineString));
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Line);
        tsTimesheetCustomField.parmOrderSequence(1);
        tsTimesheetCustomField.parmStringValue(tsTimesheetLine.TestLineString);
        List stringOptions = new List(Types::String);
        stringOptions.addEnd('First option');
        stringOptions.addEnd('second option;);
        tsTimesheetCustomField.parmStringOptions(stringOptions);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a><span data-ttu-id="785bd-233">एक टाइमशीट प्रविष्टि को अनुप्रयोग से डेटाबेस में पुन: सेव करने के लिये TSTimesheetEntryService वर्ग पर कमांड की श्रृंखला का प्रयोग</span><span class="sxs-lookup"><span data-stu-id="785bd-233">Use chain of command on the TSTimesheetEntryService class to save a timesheet entry from the app back to the database</span></span>

<span data-ttu-id="785bd-234">विशिष्ट रूप से उपयोग के लिए डेटाबेस में वापस कस्टम फील्ड को सहेजने के लिए, आपको कई पद्धतियों का विस्तार करना होगा.</span><span class="sxs-lookup"><span data-stu-id="785bd-234">To save a custom field back to the database in typical usage, you must extend multiple methods:</span></span>

- <span data-ttu-id="785bd-235">**timesheetLineNeedsUpdating** पद्धति यह निर्धारित करने के लिए किया जाता है कि अनुप्रयोग में उपयोगकर्ता ने पंक्ति रिकॉर्ड में बदलाव किया गया है या नहीं और डेटाबेस में सहेजा जाना चाहिए.</span><span class="sxs-lookup"><span data-stu-id="785bd-235">The **timesheetLineNeedsUpdating** method is used to determine whether the line record has been changed by the user in the app and must be saved to the database.</span></span> <span data-ttu-id="785bd-236">अगर प्रदर्शन चिंता का विषय़ नहीं है, पद्धति को सरल बनाया जा सकता है ताकि यह हमेशा **सही** तरह से लौटे.</span><span class="sxs-lookup"><span data-stu-id="785bd-236">If performance isn't a concern, this method can be simplified so that it always returns **true**.</span></span>
- <span data-ttu-id="785bd-237">**populateTimesheetLineFromEntryDuringCreate** और **populateTimesheetLineFromEntryDuringUpdate** पद्धतियों का विस्तार किया जा सकता है ताकि, वे TSTimesheetEntry आंकड़ा अनुबंध रिकॉर्ड से TSTimesheetLine मूल्य दर्ज कर सकें, जो कि उपलब्ध कराया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-237">The **populateTimesheetLineFromEntryDuringCreate** and **populateTimesheetLineFromEntryDuringUpdate** methods can be extended so that they enter values in the TSTimesheetLine database record from the TSTimesheetEntry data contract record that is provided.</span></span> <span data-ttu-id="785bd-238">निम्न उदाहरण में, ध्यान दें कि डेटाबेस फील्ड और प्रवृष्टि फ़ील्ड के बीच मैपिंग मैन्युअल रूप से X ++ कोड के माध्यम से कैसे की जाती है.</span><span class="sxs-lookup"><span data-stu-id="785bd-238">In the example that follows, notice how the mapping between the database field and the entry field is manually done via X++ code.</span></span>
- <span data-ttu-id="785bd-239">**populateTimesheetWeekFromEntry** पद्धति का विस्तार किया जा सकता है अगर कस्टम फील्ड जिसे **TSTimesheetEntry** विषय में मैप किया जाता है, उसे TSTimesheetLineweek डेटाबेस तालिका में वापस लिखा जाना होगा.</span><span class="sxs-lookup"><span data-stu-id="785bd-239">The **populateTimesheetWeekFromEntry** method can also be extended if the custom field that is mapped to the **TSTimesheetEntry** object must write back to the TSTimesheetLineweek database table.</span></span>

> [!NOTE]
> <span data-ttu-id="785bd-240">निम्न उदाहरण, **firstOption** या **secondOption** मूल्य को सहेजता है जिसे उपयोगकर्ता जो उपयोगकर्ता अधूरे स्ट्रिंग मूल्य के रूप में डेटाबेस के लिए चुनता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-240">The following example saves the **firstOption** or **secondOption** value that the user selects to the database as a raw string value.</span></span> <span data-ttu-id="785bd-241">अगर डेटाबेस फील्ड **Enum** प्रकार का फ़ील्ड है, तो उन मूल्यों को मैन्युअल रूप से एक असंख्य मूल्य पर मैप किया जा सकता है और फिर डेटाबेस टेबल पर किसी असंख्य फ़ील्ड में सहेजा जा सकता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-241">If the database field is a field of the **Enum** type, those values can be manually mapped to an enum value and then saved to an enum field on the database table.</span></span>

```xpp
...
[ExtensionOf(classStr(TSTimesheetEntryService))]
final class TSTimesheetEntryService_Extension
{
    protected boolean timesheetLineNeedsUpdating(TSTimesheetLine _tsTimesheetLine,
    TsTimesheetEntry _tsTimesheetEntry)
    {
        boolean ret = next timesheetLineNeedsUpdating(_tsTimesheetLine,
        _tsTimesheetEntry);
        if (!ret)
        {
            */ Loop through custom fields to see if value needs updating*/
            ListEnumerator enumerator =  _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    */ If Custom field value for TestLineString field has changed, We need to update the timesheet line.*/
                    if (_tsTimesheetLine.TestLineString != customField.parmStringValue())
                    {
                        ret = true;
                    }
                }
            }
        }
        return ret;
    }
    protected void populateTimesheetLineFromEntryDuringCreate(TSTimesheetLine
    _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
    {
        next populateTimesheetLineFromEntryDuringCreate(_tsTimesheetLine,
        _tsTimesheetEntry);
        this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
        _tsTimesheetEntry);
        }
        protected void populateTimesheetLineFromEntryDuringUpdate(TSTimesheetLine
        \_tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            next populateTimesheetLineFromEntryDuringUpdate(_tsTimesheetLine,
            _tsTimesheetEntry);
            this.populateTimesheetLineFromCustomFields(_tsTimesheetLine,
            _tsTimesheetEntry);
        }
        private void populateTimesheetLineFromCustomFields(TSTimesheetLine
        _tsTimesheetLine, TSTimesheetEntry _tsTimesheetEntry)
        {
            ListEnumerator enumerator =
            _tsTimesheetEntry.parmCustomFields().getEnumerator();
            while (enumerator.moveNext())
            {
                TSTimesheetCustomField customField = enumerator.current();
                if (customField.parmFieldName() == fieldId2Name(tableNum(TsTimesheetLine),
                fieldNum(TSTimesheetLine, TestLineString)))
                {
                    _tsTimesheetLine.TestLineString = customField.parmStringValue();
                }
            }
        }
    }
...
```

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a><span data-ttu-id="785bd-242">टाइमशीट हेडर सेक्शन में कस्टम फील्ड दिखाता है</span><span class="sxs-lookup"><span data-stu-id="785bd-242">Show a custom field in the timesheet header section</span></span>

<span data-ttu-id="785bd-243">नीचे एक मोबाइल के उपयोगकर्ता एक टाइमशीट देख रहा है का स्क्रीनशॉट है.</span><span class="sxs-lookup"><span data-stu-id="785bd-243">Below is a screenshot from the mobile app of a user viewing a timesheet.</span></span> <span data-ttu-id="785bd-244">"और सूचना" बटन सबसे ऊपर दाईं ओर चुनें गए हैं ताकि "और अधिक विवरण" को देखा जा सके.</span><span class="sxs-lookup"><span data-stu-id="785bd-244">The "More information" button has been selected in the upper-right corner to show the "View more details" option.</span></span>  

![अधिक विवरण आदेश देखें](media/show-more.png)

<span data-ttu-id="785bd-246">नीचे मोबाइल ऐप से लिए गया स्क्रीनशॉट है जिसमें टाइमशीट के "और" सेक्शन दिख रहे हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-246">Below is a screenshot from the mobile app showing the “More” section of a timesheet.</span></span> <span data-ttu-id="785bd-247">कस्टम फील्ड को "इस टाइमशीट की उपयोगिता दर (गणना किया हुआ कस्टम फील्ड)" कहा जाता है, जिसे टाइमशीट हेडर सेक्शन से जोड़ा गया है.</span><span class="sxs-lookup"><span data-stu-id="785bd-247">A custom field called “Utilization rate of this timesheet (computed custom field)” has been added to the timesheet header section.</span></span> <span data-ttu-id="785bd-248">रीड-ओनली का "0.667" मूल्य कस्टम फील्ड में सेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-248">A read-only value of "0.667" is set on the custom field.</span></span>

![अधिक सेक्शन](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a><span data-ttu-id="785bd-250">TSTimesheetTable तालिका को विस्तार दें ताकि इसके पास कस्टम फील्ड हो</span><span class="sxs-lookup"><span data-stu-id="785bd-250">Extend the TSTimesheetTable table so that it has a custom field</span></span>

<span data-ttu-id="785bd-251">विशिष्ट परिदृश्यों में, यह संभव है कि हेडर सेक्शन में एक कस्टम फील्ड के आंकड़े को TSTimesheetHeader तालिका से खींचा जाएगा.</span><span class="sxs-lookup"><span data-stu-id="785bd-251">In typical scenarios, it's likely that the data for a custom field in the header section will be pulled from the TSTimesheetHeader table.</span></span> <span data-ttu-id="785bd-252">हालांकि, अन्य तालिकाओं का उपयोग किया जा सकता है यदि आंकड़ा एक TSTimesheetTable रिकॉर्ड के आधार पर प्राप्त किया जा सकता है जो प्रदान किया गया है, या यदि उसमें विशिष्ट रिकॉर्ड संदर्भ नहीं है (उदाहरण के लिए, यदि फ़ील्ड को केवल परियोजना मानक में रीड-ओनली के रूप में सेट किया जाता है).</span><span class="sxs-lookup"><span data-stu-id="785bd-252">However, other tables can be used if the data can be retrieved based on a TSTimesheetTable record that is provided, or if it doesn't have specific record context (for example, if the field is set as read-only in the project parameters).</span></span>

<span data-ttu-id="785bd-253">ध्यान दें कि कस्टम फील्ड के पास कोई भी प्रतिभूति डेटाबेस रिकॉर्ड नहीं होगा.</span><span class="sxs-lookup"><span data-stu-id="785bd-253">Note that custom fields don't have to have any backing database records.</span></span> <span data-ttu-id="785bd-254">वे X ++ तर्क के आधार पर गतिशील रूप से उत्पन्न हो सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-254">They can be dynamically generated based on X++ logic.</span></span> <span data-ttu-id="785bd-255">निम्न उदाहरण इस दृष्टिकोण को दर्शाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-255">The example that follows shows this approach.</span></span>

<span data-ttu-id="785bd-256">किसी ऐप में हेडर सेक्शन में फील्ड हमेशा रीड-ओनली रहते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-256">Fields in the header section are always read-only in the app.</span></span>

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a><span data-ttu-id="785bd-257">TSTimesheetSettings वर्ग की buildCustomFieldList पद्धति के चेन ऑफ कमांड का इस्तेमाल हेडर सेक्शन में फील्ड दिखाने के लिए करता है</span><span class="sxs-lookup"><span data-stu-id="785bd-257">Use chain of command on the buildCustomFieldList method of the TSTimesheetSettings class to show a field in the header section</span></span>

<span data-ttu-id="785bd-258">यह कोड ऐप में फील्ड के लिए डिस्प्ले सेटिंग को नियंत्रित करता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-258">This code controls the display settings for the field in the app.</span></span> <span data-ttu-id="785bd-259">उदाहरण के लिए, यह फील्ड, लेबल के प्रकार को नियंत्रित करता है, कि फील्ड अनिवार्य है या नहीं, किस सेक्शन में फील्ड नजर आता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-259">For example, it controls the type of field, the label, whether the field is mandatory, and what section the field appears in.</span></span>

<span data-ttu-id="785bd-260">निम्न उदाहरण ऐप के हेडर सेक्शन में गणना किए गए मूल्य को दिखाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-260">The following example shows a computed value in the header section in the app.</span></span>

```xpp
...
[ExtensionOf(classStr(TsTimesheetSettings))]
final class TSTimesheetSettings_Extension
{
    protected List buildCustomFieldList()
    {
        List customFieldList = next buildCustomFieldList();
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a><span data-ttu-id="785bd-261">TSTimesheetDetails वर्ग की buildCustomFieldListForHeader पद्धति के चेन ऑफ कमांड का इस्तेमाल टाइमशीट विवरण भरने के लिए करता है</span><span class="sxs-lookup"><span data-stu-id="785bd-261">Use chain of command on the buildCustomFieldListForHeader method of the TSTimesheetDetails class to fill in timesheet details</span></span>

<span data-ttu-id="785bd-262">**buildCustomFieldListForHeader** पद्धति का इस्तेमाल किसी मोबाइल में टाइमशीट हेडल विवरण भरने के लिए किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-262">The **buildCustomFieldListForHeader** method is used to fill in the timesheet header details in the mobile app.</span></span> <span data-ttu-id="785bd-263">TSTimesheetTable रिकॉर्ड को एक मानक के रूप में लेता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-263">It takes a TSTimesheetTable record as a parameter.</span></span> <span data-ttu-id="785bd-264">उस रिकॉर्ड से फील्ड का उपयोग ऐप में कस्टम फील्ड मूल्य को भरने में किया जा सकता है</span><span class="sxs-lookup"><span data-stu-id="785bd-264">Fields from that record can be used to fill in the custom field value in the app.</span></span> <span data-ttu-id="785bd-265">दिए गए उदाहरण डेटाबेस से किसी मूल्य को नहीं पढ़ते.</span><span class="sxs-lookup"><span data-stu-id="785bd-265">The following example doesn't read any values from the database.</span></span> <span data-ttu-id="785bd-266">इसके स्थान पर, यह X++ तर्क का इस्तेमाल करते हैं ताकि गणना किए गए मूल्य को पैदा किया जा सके, जिसे बाद में ऐप पर दिखाया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-266">Instead, it uses X++ logic to generate a computed value that is then shown in the app.</span></span>


```xpp
...
[ExtensionOf(classStr(TSTimesheetDetails))]
final class TSTimesheetDetails_Extension
{
    protected List buildCustomFieldListForHeader(TSTimesheetTable
    _tsTimesheetTable)
    {
        List customFieldList = next buildCustomFieldListForHeader(_tsTimesheetTable);
        TSTimesheetCustomField tsTimesheetCustomField;

        */ Computed utilization rate*/
        tsTimesheetCustomField = new TSTimesheetCustomField();
        tsTimesheetCustomField.parmFieldBaseType(Types::Real);
        tsTimesheetCustomField.parmLabel("Utilization rate of this timesheet (computed
        custom field)");
        tsTimesheetCustomField.parmFieldSection(TSCustomFieldSection::Header);
        tsTimesheetCustomField.parmOrderSequence(2);
        tsTimesheetCustomField.parmNumberOfDecimals(3);
        real utilizationRate = 0;
        if (_tsTimesheetTable.totalHours() != 0)
        {
            utilizationRate = _tsTimesheetTable.totalHoursBillable() /
            _tsTimesheetTable.totalHours();
        }
        tsTimesheetCustomField.parmRealValue(utilizationRate);
        customFieldList.addEnd(tsTimesheetCustomField);
        return customFieldList;
    }
}
...
```

## <a name="other-configurabilityextensibility-opportunities"></a><span data-ttu-id="785bd-267">अन्य विन्यास/विस्तीर्ण होने की क्षमता अवसर</span><span class="sxs-lookup"><span data-stu-id="785bd-267">Other configurability/extensibility opportunities</span></span>

### <a name="adding-additional-validation-for-the-app"></a><span data-ttu-id="785bd-268">अनुप्रयोग के लिए अतिरिक्त सत्यापन जोड़ना</span><span class="sxs-lookup"><span data-stu-id="785bd-268">Adding additional validation for the app</span></span>

<span data-ttu-id="785bd-269">डेटाबेस स्तर पर टाइमशीट क्रियात्मकता के लिए मौजूदा तर्क अपेक्षा के अनुरूप काम करेगा.</span><span class="sxs-lookup"><span data-stu-id="785bd-269">Existing logic for timesheet functionality at the database level will still work as expected.</span></span> <span data-ttu-id="785bd-270">सहेजने या संचालन को पूरा करने में बाधा डालने और एक विशिष्ट त्रुटि संदेश दिखाने के लिए, आप **थ्रो एरर("उपयोगकर्ता को संदेश")** को चेन ऑफ कमांड एक्सटेंशन के माध्यम से कोड में जोड़ सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-270">To interrupt the completion of save or submit operations and show a specific error message, you can add **throw error("message to user")** to the code via a chain of command extension.</span></span> <span data-ttu-id="785bd-271">विस्तार होने योग्य पद्धतियों के तीन उदाहरण हैं:</span><span class="sxs-lookup"><span data-stu-id="785bd-271">Here are three examples of useful extensible methods:</span></span>

- <span data-ttu-id="785bd-272">TSTimesheetLine तालिका में **validateWrite** टाइमशीट पंक्ति में संचालन को सहेजने के लिए दौरान **गलत** हो जाता है, मोबाइल ऐप में त्रुटि का संदेश दिखता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-272">If **validateWrite** on the TSTimesheetLine table returns **false** during a save operation for a timesheet line, an error message is shown in the mobile app.</span></span>
- <span data-ttu-id="785bd-273">किसी अनुप्रयोग में टाइमशीट दाखिल करने के दौरान TSTimesheetTable तालिका में **validateSubmit** अगर **गलत** हो जाता है, उपयोगकर्ता को त्रुटि का एक संदेश दिखता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-273">If **validateSubmit** on the TSTimesheetTable table returns **false** during timesheet submission in the app, an error message is shown to the user.</span></span>
- <span data-ttu-id="785bd-274">TSTimesheetLine तालिका में **सम्मिलित** पद्धति के दौरान फील्ड में दर्ज किए गए तर्क (उदाहरण के लिए, **पंक्ति प्रॉपर्टी**), अभी भी चलेगी.</span><span class="sxs-lookup"><span data-stu-id="785bd-274">Logic that fills in fields (for example, **Line Property**) during the **insert** method on the TSTimesheetLine table will still run.</span></span>

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a><span data-ttu-id="785bd-275">आउट-ऑफ-बॉक्स फ़ील्ड को केवल कॉन्फ़िगरेशन के माध्यम से पढ़ने के रूप में छुपाना और चिह्नित करना</span><span class="sxs-lookup"><span data-stu-id="785bd-275">Hiding and marking out-of-box fields as read-only via configuration</span></span>

<span data-ttu-id="785bd-276">परियोजना मानक से, मोबाइल ऐप में एकदम अलग रीड-ओनली या छुपी हुई फील्ड तैयार कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-276">From the project parameters, you can make out-of-box fields read-only or hidden in the mobile app.</span></span> <span data-ttu-id="785bd-277">**परियोजना प्रबंधन और लेखांकन मानक** पृष्ठ के **टाइमशीट** टैब पर **मोबाइल टाइमशीट** सेक्शन में विकल्पों को सेट करें.</span><span class="sxs-lookup"><span data-stu-id="785bd-277">Set the options in the **Mobile timesheets** section on the **Timesheet** tab of the **Project management and accounting parameters** page.</span></span>

![प्रोजेक्ट पैरामीटर](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a><span data-ttu-id="785bd-279">गतिविधियों में बदलाव करना, जो कि प्रसारण के माध्यम से चयन के लिए उपलब्ध हैं</span><span class="sxs-lookup"><span data-stu-id="785bd-279">Changing the activities that are available for selection via extensions</span></span>

<span data-ttu-id="785bd-280">किसी परियोजना के चयन के लिए उपलब्ध गतिविधियां **getActivitiesForProject()** और **getActivityQuery()** विधि से **TsTimesheetProjectService** वर्ग में भरी जाती हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-280">The activities that are available for selection for a project are filled in via the **getActivitiesForProject()** and **getActivityQuery()** methods in the **TsTimesheetProjectService** class.</span></span> <span data-ttu-id="785bd-281">आप किसी विशिष्ट परियोजना के लिए चयन के लिए उपलब्ध गतिविधियों के अपने व्यवसाय परिदृश्य से मेल खाने के लिए इस चलन को बदलने के लिए चेन इन कमांड का उपयोग कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-281">You can use chain of command to change this behavior to match your business scenario for the activities that are available for selection for a specific project.</span></span>

### <a name="entering-a-default-project-category-on-timesheet-entries"></a><span data-ttu-id="785bd-282">टाइमशीट प्रविष्टियों पर डिफॉल्ट परियोजना श्रेणी दर्ज करना</span><span class="sxs-lookup"><span data-stu-id="785bd-282">Entering a default project category on timesheet entries</span></span>

<span data-ttu-id="785bd-283">टाइमशीट प्रविष्टियों पर डिफॉल्ट परियोजना श्रेणी की प्रविष्टि तीन स्तर पर उत्पन्न होती है.</span><span class="sxs-lookup"><span data-stu-id="785bd-283">Entry of a default project category on timesheet entries occurs at three levels.</span></span> <span data-ttu-id="785bd-284">आप वांछित चलन प्राप्त करने के लिए चलन को किसी या इन सभी स्तरों पर विस्तार देने के लिए चेन ऑफ कमांड का इस्तेमाल कर सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="785bd-284">You can use chain of command to extend the behavior at any or all of these levels to achieve the desired behavior.</span></span> <span data-ttu-id="785bd-285">निम्नलिखित पदानुक्रम का उपयोग किया जाता है:</span><span class="sxs-lookup"><span data-stu-id="785bd-285">The following hierarchy is used:</span></span>

1. <span data-ttu-id="785bd-286">ऐप परियोजना संसाधन से डिफॉल्ट श्रेणी को रखने की कोशिश करता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-286">The app tries to put the default category from the project resource.</span></span> <span data-ttu-id="785bd-287">डिफॉल्ट श्रेणी **TSTimesheetSettingsService** वर्ग में **getCurrentUserResource** और **getDelegatedResourcesForCurrentUser** पद्धति में सेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-287">This default category is set in the **getCurrentUserResource** and **getDelegatedResourcesForCurrentUser** methods in the **TSTimesheetSettingsService** class.</span></span>
2. <span data-ttu-id="785bd-288">अगर डिफॉल्ट श्रेणी परियोजना संसाधन के स्तर पर उपलब्ध नहीं कराया जाता, ऐप इसे परियोजना गतिविधि से लेने की कोशिश करता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-288">If the default category isn't provided at the project resource level, the app tries to pull it from the project activity.</span></span> <span data-ttu-id="785bd-289">डिफॉल्ट श्रेणी **TSTimesheetProjectService** वर्ग में **getActivitiesForProject** पद्धति में सेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-289">This default category is set in the **getActivitiesForProject** method in the **TSTimesheetProjectService** class.</span></span>
3. <span data-ttu-id="785bd-290">अगर डिफॉल्ट श्रेणी किसी परियोजना गतिविधि के स्तर पर उपलब्ध नहीं कराई जाती, तो डिफॉल्ट श्रेणी इसे परियोजना मानक से लेती है.</span><span class="sxs-lookup"><span data-stu-id="785bd-290">If the default category isn't provided at the project activity level, the default category it taken from the project parameters.</span></span> <span data-ttu-id="785bd-291">डिफॉल्ट श्रेणी **TSTimesheetProjectService** वर्ग में **getProjectDetailsbyRule** पद्धति में सेट किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="785bd-291">This default category is set in the **getProjectDetailsbyRule** method in the **TSTimesheetProjectService** class.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]