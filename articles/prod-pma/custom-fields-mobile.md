---
title: iOS और Android पर Microsoft Dynamics 365 Project Timesheet मोबाइल अनुप्रयोग के लिए कस्टम फ़ील्ड लागू करें
description: यह विषय कस्टम फील्ड के क्रियान्वयन के लिए विस्तार के इस्तेमाल का आम पैटर्न उपलब्ध कराता है.
author: Yowelle
manager: AnnBe
ms.date: 05/29/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
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
ms.openlocfilehash: 1ea1ca002a8f68f86808831b398e452244471322
ms.sourcegitcommit: 5c4c9bf3ba018562d6cb3443c01d550489c415fa
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/16/2020
ms.locfileid: "4077754"
---
# <a name="implement-custom-fields-for-the-microsoft-dynamics-365-project-timesheet-mobile-app-on-ios-and-android"></a>iOS और Android पर Microsoft Dynamics 365 Project Timesheet मोबाइल अनुप्रयोग के लिए कस्टम फ़ील्ड लागू करें

[!include [banner](../includes/banner.md)]

यह विषय कस्टम फील्ड के क्रियान्वयन के लिए विस्तार के इस्तेमाल का आम पैटर्न उपलब्ध कराता है. निम्नलिखित विषय शामिल हैं:

- डेटा के विभिन्न प्रकार, जिसका कस्टम फील्ड फ्रेमवर्क समर्थन करता है
- टाइमशीट एंट्री में रीड-ऑनली या संपादित होने लायक फील्ड को कैसे दिखाएं, और उपयोगकर्ता द्वारा उपलब्ध मूल्य को डेटाबेस में कैसे सुरक्षित रखें
- टाइमशीट हेडर में रीड-ओनली फील्ड को कैसे दिखाएं
- फील्ड में डिफॉल्ट मूल्य दर्ज करने के लिए अन्य कस्टम बिजनस लॉजिक को कैसे एकीकृत करें और अतिरिक्त सत्यापन करें

## <a name="audience"></a>श्रोता

यह विषय उन डेवलपर के लिए है जो Microsoft Dynamics 365 Project Timesheet मोबाइल एप्लिकेशन में अपने कस्टम फील्ड को एकीकृत कर रहे हैं, जो कि Apple iOS और Google Android के लिए उपलब्ध है. ऐसा माना जाता है कि पाठक X++ डेवलपमेंट से प्रॉजेक्ट टाइमशीट की कार्यप्रणाली से परिचित हैं.

## <a name="data-contract--tstimesheetcustomfield-x-class"></a>डेटा अनुबंध- TSTimesheetCustomField X++ क्लास

**TSTimesheetCustomField** क्लास X++ डेटा अनुबंध क्लास है जो कि टाइमशीट कार्यप्रणाली के लिए कस्टम फील्ड की सूचना का प्रतिनिधित्व करता है. कस्टम फील्ड वस्तुओं की सूची TSTimesheetDetails आंकड़ा अनुबंध और TSTimesheetEntry आंकड़ा अनुबंध दोनों में डाला जाता है, ताकि कस्टम फील्ड मोबाइल ऐप में दिख सकें.

- **TSTimesheetDetails** - टाइमशीट हैडर अनुबंध.
- **TSTimesheetEntry** - टाइमशीट लेनदेन अनुबंध. इन वस्तुओं के समूह के पास समान परियोजना सूचना होती है और **timesheetLineRecId** मूल्य में एक पंक्ति बनाती है.

### <a name="fieldbasetype-types"></a>fieldBaseType (प्रकार)

**TsTimesheetCustom** वस्तु में **FieldBaseType** प्रॉपर्टी वस्तु फील्ड को निर्धारित करती जो कि अनुप्रयोग में नजर आती है. दिए गए **प्रकार** मूल्य, जिसका समर्थन किया जाता है.

| प्रकार मान | प्रकार              | नोट्स |
|-------------|-------------------|-------|
| 12           | स्ट्रिंग (और Enum) | फ़ील्ड टेक्स्ट फ़ील्ड के रूप में प्रकट होती है. |
| 1           | Integer           | मूल्य को बिना दशमलव स्थान के एक संख्या के रूप में दिखाया गया है. |
| 2           | वास्तविक              | मान को संख्या के रूप में दिखाया जाता है जिसमें दशमलव स्थान होता है.<p>अनुप्रयोग में वास्तविक मूल्य को एक मुद्रा के रूप में दिखाने के लिए **fieldExtenededType** प्रॉपर्टी का इस्तेमाल किया जाता है. आप **दशमलों की संख्या** प्रॉपर्टी का इस्तेमाल कर दिखाए जाने वाले दशमलव स्थान की संख्या तय कर सकते हैं.</p> |
| 3           | दिनांक              | तारीख का फ़ॉर्मेट उपयोगकर्ता के **तारीख, समय और संख्या फ़ॉर्मेट** सेटिंग द्वारा निर्धारित किया जाता है, जिसका वर्णन **उपयोगकर्ता विकल्पों** में **भाषा व देश/क्षेत्र वरीयता** के अंदर किया जाता है. |
| 4           | Boolean           | |
| 15          | GUID              | |
| 16          | Int64             | |

- अगर **stringOptions** प्रॉपर्टी **TSTimesheetCustomField** विषय में उपलब्ध नहीं कराया जाता, तो उपयोगकर्ता को एक रिक्त-टेक्स्ट फील्ड उपलब्ध कराया जाता है.

    **stringLength** गुण का इस्तेमाल अधिक से अधिक स्ट्रिंग की लंबाई निर्धारित करने के लिए किया जा सकता है जो कि उपयोगकर्ता दर्ज कर सकते हैं.

- अगर **stringOptions** प्रॉपर्टी **TSTimesheetCustomField** विषय में उपलब्ध कराया जाता है, तो सूचीबद्ध किए गए अवयव एकमात्र मूल्य होते हैं, जो कि उपयोगकर्ता विकल्प बटन (रेडियो बटन) का उपयोग कर चुन सकते हैं.

    इस मामले में, स्ट्रिंग फील्ड यूजर एंट्री के उद्देश्य से असंख्य मूल्य के रूप में काम कर सकती है. डेटाबेस के मान को इनम के रूप में सेव करने के लिए, कमांड की श्रृंखला का उपयोग करके डेटाबेस में सेव करने से पहले मैन्युअल रूप से स्ट्रिंग मान को एनम मान पर मैप करें (उदाहरण के लिये इस विषय पर बाद में देखें "एक टाइमशीट प्रविष्टि को अनुप्रयोग से डेटाबेस में पुन: सेव करने के लिये TSTimesheetEntryService वर्ग पर कमांड की श्रृंखला का प्रयोग" अनुभाग).

### <a name="fieldextendedtype-tscustomfieldextendedtype"></a>fieldExtendedType (TSCustomFieldExtendedType)

आप वास्तविक मूल्य को मुद्रा के रूप में फॉर्मैट करने के लिए इस प्रॉपर्टी का उपयोग कर सकते हैं. यह दृष्टिकोण तब लागू होता है जब **fieldBaseType** मूल्य **वास्तविक** हो.

- **TSCustomFieldExtendedType:कोई नहीं** – में कोई फॉर्मैटिंग लागू नहीं होता.
- **TSCustomFieldExtendedType::मुद्रा** – मूल्य को मुद्रा के रूप में फॉर्मैट करता है.

    जब मुद्रा फॉर्मैटिंग सक्रिय है, तब **stringValue** फील्ड का इस्तमाल मुद्रा कोड डालने में किया जा सकता है, जो कि ऐप में दिखना चाहिए. मान केवल पढ़ने के लिए मान है.

    **वास्तविक मूल्य** फ़ील्ड में धन राशि है जिसे डेटाबेस में सहेजा जाना चाहिए.

### <a name="fieldsection-tscustomfieldsection"></a>fieldSection (TSCustomFieldSection)

आप इस निर्दिष्ट प्रॉपर्टी का इस्तेमाल कर सकते हैं जहां कस्टम फील्ड गुण में नजर आने चाहिए.

- **TSCustomFieldSection::हेडर** – फील्ड अनुप्रयोग में **और ब्यौरा देखें** सेक्शन में नजर आएगा. ये फील्ड हमेशा रीड-ओनली रहते हैं.
- **TSCustomFieldSection::पंक्ति** – फील्ड टाइमशीट प्रविष्टियों में सबसे अलग सभी पंक्ति फील्ड के बाद नजर आएगा. ये फ़ील्ड या तो संपादन योग्य या केवल पढ़ने योग्य हो सकते हैं.

### <a name="fieldname-fieldnameshort"></a>fieldName (FieldNameShort)

यह प्रॉपर्टी फील्ड को चिह्नित करता है जब ऐप द्वारा उपलब्ध मूल्य डेटाबेस में वापस सुरक्षित रखा जाता है.

### <a name="tablename-tablenameshort"></a>tableName (TableNameShort)

यह प्रॉपर्टी फील्ड को चिह्नित करता है जब ऐप द्वारा उपलब्ध मूल्य डेटाबेस में वापस सुरक्षित रखा जाता है.

### <a name="iseditable-noyes"></a>isEditable (NoYes)

प्रॉपर्टी को **हां** में सेट करें, यह दिखाने के लिए टाइमशीट प्रविष्टि सेक्शन में फील्ड उपयोकर्ताओं द्वारा संपादित किया जाना चाहिए. फील्ड को रीड-ओनली बनाने के लिए प्रॉपर्टी को **ना** में सेट करें.

### <a name="ismandatory-noyes"></a>isMandatory (NoYes)

प्रॉपर्टी को **हां** में सेट करें, यह दिखाने के लिए टाइमशीट प्रविष्टि सेक्शन में फ़ील्ड अनिवार्य होना चाहिए.

### <a name="label-str"></a>लेबल (str)

प्रॉपर्टी उस लेबल का वर्णन करता है, जो कि ऐप में फील्ड के पास दिखाया जाता है.

### <a name="stringoptions-list-of-strings"></a>stringOptions (स्ट्रिंग की सूची)

प्रॉपर्टी तब लागू होती है जब **fieldBaseType** को **स्ट्रिंग** में सेट किया जाता है. अगर **stringOptions** सेट है, तो स्ट्रिंग का मूल्य जो कि विकल्प बटन के माध्यम से चयन के लिए उपलब्ध है, उसे सूची में स्ट्रिंग द्वारा स्पष्ट रूप से बताया जाता है. अगर कोई स्ट्रिंग उपलब्ध नहीं कराया जाता, स्ट्रिंग फील्ड में रिक्त-टेक्स्ट प्रविष्टि की अनुमति होती है. (उदाहरण के लिये इस विषय पर बाद में देखें "एक टाइमशीट प्रविष्टि को अनुप्रयोग से डेटाबेस में पुन: सेव करने के लिये TSTimesheetEntryService वर्ग पर कमांड की श्रृंखला का प्रयोग" अनुभाग).

### <a name="stringlength-int"></a>stringLength (int)

प्रॉपर्टी स्ट्रिंग फील्ड की अधिकतम लंबाई का उल्लेख करता है. यह तब लागू होता है जब **fieldBaseType** को **स्ट्रिंग** में सेट किया जाता है.

### <a name="numberofdecimals-int"></a>numberOfDecimals (int)

प्रॉपर्टी दशमलव स्थानों की संख्या का उल्लेख करती है जो कि वास्तविक फील्ड के लिए दिखाया जाता है. यह तब लागू होता है जब **fieldBaseType** को **वास्तविक** सेट किया जाता है.

### <a name="ordersequence-int"></a>orderSequence (int)

यह प्रॉपर्टी क्रम को नियंत्रित करती है, जिसमें कस्टम फील्ड ऐप में नजर आते हैं, जब एक से अधिक कस्टम फील्ड का उल्लेख किया जाता है. फील्ड जिनमें सबसे कम संख्याएं होती हैं, वे सबसे पहले दिखाए जाते हैं.

### <a name="booleanvalue-boolean"></a>booleanValue (बूलियन)

**बूलियन** प्रकार के फील्ड के लिए, यह प्रॉपर्टी फील्ड के बूलयिन मूल्य को सर्वर और अनुप्रयोग के बीच हस्तांतरित करता है.

### <a name="guidvalue-guid"></a>guidValue (guid)

**GUID** प्रकार के फील्ड के लिए, प्रॉपर्टी फील्ड के ग्लोबली युनीक आइडेंटिफ़ायर (GUID) मूल्य को सर्वर और अनुप्रयोग के बीच हस्तांतरित करती है.

### <a name="int64value-int64"></a>int64Value (int64)

**Int64** प्रकार के फील्ड के लिए प्रॉपर्टी फील्ड के Int64 मूल्य को सर्विर और ऐप के बीच हस्तांतरित करती है.

### <a name="intvalue-int"></a>intValue (int)

के खेतों के लिए **इंट** प्रकार, यह प्रॉपर्टी सर्वर और ऐप के बीच के क्षेत्र का अंतर मानती है.

### <a name="realvalue-real"></a>realValue (वास्तविक)

**वास्तविक** प्रकार के फील्ड के लिए, प्रॉपर्टी सर्वर और अनुप्रयोग के बीच फील्ड के मूल्य को हस्तांतरित करती है.

### <a name="stringvalue-str"></a>stringValue (str)

**स्ट्रिंग** प्रकार के फील्ड के लिए, प्रॉपर्टी फील्ड के स्ट्रिंग मूल्य को सर्विर और ऐप के बीच हस्तांतरित करती है. इसका उपयोग **वास्तविक** प्रकार के फील्ड के लिए होता है, जिसे मुद्रा के रूप में फॉर्मैट किया जाता है. उन फील्ड के लिए, प्रॉपर्टी का उपयोग मुद्रा कोड को ऐप में हस्तांतरित करने में होता है.

### <a name="datevalue-date"></a>dateValue (date)

**तारीख** प्रकार के फील्ड के लिए, प्रॉपर्टी फील्ड के तारीख मूल्य को सर्विर और ऐप के बीच हस्तांतरित करती है.

## <a name="show-and-save-a-custom-field-in-the-timesheet-entry-section"></a>टाइमशीट प्रविष्टि सेक्शन में कस्टम फील्ड को दिखाना और सुरक्षित करना

नीचे एक मोबाइल के टाइमशीट प्रविष्टि निर्माण का स्क्रीनशॉट है. यह "समय प्रविष्टि'' सेक्शन जिसे ''टेस्ट स्ट्रिंग'' कहा जाता है, उसमें पहले से तय "दूसरे विकल्प" के असंख्य मूल्य के साथ एकदम अलग तरह के फील्ड और कस्टम फील्ड को दिखाता है.

![अनुप्रयोग में टेस्ट स्ट्रिंग कस्टम फ़ील्ड](media/timesheet-entry.jpg)



नीचे मोबाइल ऐप का एक स्क्रीन शॉट है जिसमें "टेस्ट स्ट्रिंग" कस्टम फ़ील्ड के लिए उपलब्ध असंख्य विकल्पों में से एक का चुनाव उपयोगकर्ता कर रहा है.  दो विकल्प "पहला विकल्प" और "दूसरा विकल्प" है जिसे रेडियो बटन के रूप में दिखाया जाता है. वर्तमान में दूसरा विकल्प चुना गया है.

![विकल्प बटनों (रेडियो बटन) टेस्ट स्ट्रिंग कस्टम फील्ड के लिए होता है](media/enum-option.jpg)



### <a name="extend-the-tstimesheetline-table-so-that-it-has-a-custom-field"></a>TSTimesheetLine तालिका को विस्तार दें ताकि इसके पास कस्टम फील्ड हो

विशिष्ट परिदृश्यों में, यह संभावना है कि टाइमशीट प्रविष्टि सेक्शन में एक कस्टम फ़ील्ड का डेटा TSTimesheetLine तालिका में सहेजा जाएगा. हालांकि, अन्य तालिकाओं का उपयोग किया जा सकता है यदि आंकड़ा एक TSTimesheetTrans रिकॉर्ड के आधार पर प्राप्त किया जा सकता है जो प्रदान किया गया है, या यदि उसमें विशिष्ट रिकॉर्ड संदर्भ नहीं है (उदाहरण के लिए, यदि फ़ील्ड को केवल परियोजना मानक में रीड-ओनली के रूप में सेट किया जाता है).

ध्यान दें कि कस्टम फील्ड के पास कोई भी प्रतिभूति डेटाबेस रिकॉर्ड नहीं होगा. वे X ++ तर्क के आधार पर गतिशील रूप से उत्पन्न हो सकते हैं. यह दृष्टिकोण केवल-पढ़ने के परिदृश्य में उपयोगी हो सकता है ("टाइमशीट विवरण भरने के लिए TSTimesheetDetails वर्ग के buildCustomFieldListForHeader विधि पर कमांड की श्रृंखला का उपयोग करें" डायनामिक रूप से कस्टम फ़ील्ड मानों के उदाहरण के लिए अनुभाग देखें.)

नीचे अनुप्रयोग ऑब्जेक्ट ट्री के Visual Studio का स्क्रीनशॉट है. यह TSTimesheetLine तालिका का TestLineString के साथ विस्तार दिखाता है, जिसे कस्टम फील्ड में जोड़ा जाता है.

![लाइन का तार](media/b6756b4a3fc5298093327a088a7710fd.png)

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-timesheet-entry-section"></a>TSTimesheetSettings वर्ग की buildCustomFieldList पद्धति के चेन ऑफ कमांड का इस्तेमाल टाइमशीट प्रविष्टि सेक्शन में फील्ड दिखाने के लिए करता है

यह कोड ऐप में फील्ड के लिए डिस्प्ले सेटिंग को नियंत्रित करता है. उदाहरण के लिए, यह फील्ड, लेबल के प्रकार को नियंत्रित करता है, कि फील्ड अनिवार्य है या नहीं, किस सेक्शन में फील्ड नजर आता है.

उदाहरण के लिए समय प्रविष्टि पर स्ट्रिंग फील्ड दिखाता है. फील्ड के दो विकल्प होते हैं, **पहला विकल्प** और **दूसरा विकल्प** , ये विकल्प बटन (रेडियो बटन) के माध्यम से उपलब्ध होते हैं. अनुप्रयोग में फील्ड **TestLineString** फील्ड से संबंधित होते हैं, जो कि TSTimesheetLine तालिका से जोड़े जाते हैं.

कस्टम फ़ील्ड गुणों के प्रारंभ को सरल बनाने के लिए **TSTimesheetCustomField::newFromMetatdata()** विधि के उपयोग पर ध्यान दें: **fieldBaseType** , **tableName** , **fieldname** , **लेबल** , **isEditable** , **isMandatory** , **stringLength** , and **numberOfDecimals**. आपको जैसा ठीक लगे, उस अनुसार आप इन मानकों को मैनुअली निर्धारित कर सकते हैं.

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforentry-method-of-the-tstimesheetentry-class-to-enter-values-in-a-timesheet-entry"></a>TSTimesheetEntry वर्ग की buildCustomFieldListForEntry पद्धति के चेन ऑफ कमांड का इस्तेमाल टाइमशीट प्रविष्टि में मान दर्ज करने के लिए करता है

**buildCustomFieldListForEntry** पद्धति का उपयोग मोबाइल ऐप में सहेजी गई टाइमशीट पंक्तियों में मूल्य को दर्ज करने के लिए किया जाता है. TSTimesheetTrans रिकॉर्ड को एक मानक के रूप में लेता है. उस रिकॉर्ड से फील्ड का उपयोग ऐप में कस्टम फील्ड मूल्य को भरने में किया जा सकता है

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

### <a name="use-chain-of-command-on-the-tstimesheetentryservice-class-to-save-a-timesheet-entry-from-the-app-back-to-the-database"></a>एक टाइमशीट प्रविष्टि को अनुप्रयोग से डेटाबेस में पुन: सेव करने के लिये TSTimesheetEntryService वर्ग पर कमांड की श्रृंखला का प्रयोग

विशिष्ट रूप से उपयोग के लिए डेटाबेस में वापस कस्टम फील्ड को सहेजने के लिए, आपको कई पद्धतियों का विस्तार करना होगा.

- **timesheetLineNeedsUpdating** पद्धति यह निर्धारित करने के लिए किया जाता है कि अनुप्रयोग में उपयोगकर्ता ने पंक्ति रिकॉर्ड में बदलाव किया गया है या नहीं और डेटाबेस में सहेजा जाना चाहिए. अगर प्रदर्शन चिंता का विषय़ नहीं है, पद्धति को सरल बनाया जा सकता है ताकि यह हमेशा **सही** तरह से लौटे.
- **populateTimesheetLineFromEntryDuringCreate** और **populateTimesheetLineFromEntryDuringUpdate** पद्धतियों का विस्तार किया जा सकता है ताकि, वे TSTimesheetEntry आंकड़ा अनुबंध रिकॉर्ड से TSTimesheetLine मूल्य दर्ज कर सकें, जो कि उपलब्ध कराया जाता है. निम्न उदाहरण में, ध्यान दें कि डेटाबेस फील्ड और प्रवृष्टि फ़ील्ड के बीच मैपिंग मैन्युअल रूप से X ++ कोड के माध्यम से कैसे की जाती है.
- **populateTimesheetWeekFromEntry** पद्धति का विस्तार किया जा सकता है अगर कस्टम फील्ड जिसे **TSTimesheetEntry** विषय में मैप किया जाता है, उसे TSTimesheetLineweek डेटाबेस तालिका में वापस लिखा जाना होगा.

> [!NOTE]
> निम्न उदाहरण, **firstOption** या **secondOption** मूल्य को सहेजता है जिसे उपयोगकर्ता जो उपयोगकर्ता अधूरे स्ट्रिंग मूल्य के रूप में डेटाबेस के लिए चुनता है. अगर डेटाबेस फील्ड **Enum** प्रकार का फ़ील्ड है, तो उन मूल्यों को मैन्युअल रूप से एक असंख्य मूल्य पर मैप किया जा सकता है और फिर डेटाबेस टेबल पर किसी असंख्य फ़ील्ड में सहेजा जा सकता है.

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

## <a name="show-a-custom-field-in-the-timesheet-header-section"></a>टाइमशीट हेडर सेक्शन में कस्टम फील्ड दिखाता है

नीचे एक मोबाइल के उपयोगकर्ता एक टाइमशीट देख रहा है का स्क्रीनशॉट है. "और सूचना" बटन सबसे ऊपर दाईं ओर चुनें गए हैं ताकि "और अधिक विवरण" को देखा जा सके.  

![अधिक विवरण आदेश देखें](media/show-more.png)

नीचे मोबाइल ऐप से लिए गया स्क्रीनशॉट है जिसमें टाइमशीट के "और" सेक्शन दिख रहे हैं. कस्टम फील्ड को "इस टाइमशीट की उपयोगिता दर (गणना किया हुआ कस्टम फील्ड)" कहा जाता है, जिसे टाइमशीट हेडर सेक्शन से जोड़ा गया है. रीड-ओनली का "0.667" मूल्य कस्टम फील्ड में सेट किया जाता है.

![अधिक सेक्शन](media/more-section.jpg)

### <a name="extend-the-tstimesheettable-table-so-that-it-has-a-custom-field"></a>TSTimesheetTable तालिका को विस्तार दें ताकि इसके पास कस्टम फील्ड हो

विशिष्ट परिदृश्यों में, यह संभव है कि हेडर सेक्शन में एक कस्टम फील्ड के आंकड़े को TSTimesheetHeader तालिका से खींचा जाएगा. हालांकि, अन्य तालिकाओं का उपयोग किया जा सकता है यदि आंकड़ा एक TSTimesheetTable रिकॉर्ड के आधार पर प्राप्त किया जा सकता है जो प्रदान किया गया है, या यदि उसमें विशिष्ट रिकॉर्ड संदर्भ नहीं है (उदाहरण के लिए, यदि फ़ील्ड को केवल परियोजना मानक में रीड-ओनली के रूप में सेट किया जाता है).

ध्यान दें कि कस्टम फील्ड के पास कोई भी प्रतिभूति डेटाबेस रिकॉर्ड नहीं होगा. वे X ++ तर्क के आधार पर गतिशील रूप से उत्पन्न हो सकते हैं. निम्न उदाहरण इस दृष्टिकोण को दर्शाता है.

किसी ऐप में हेडर सेक्शन में फील्ड हमेशा रीड-ओनली रहते हैं.

### <a name="use-chain-of-command-on-the-buildcustomfieldlist-method-of-the-tstimesheetsettings-class-to-show-a-field-in-the-header-section"></a>TSTimesheetSettings वर्ग की buildCustomFieldList पद्धति के चेन ऑफ कमांड का इस्तेमाल हेडर सेक्शन में फील्ड दिखाने के लिए करता है

यह कोड ऐप में फील्ड के लिए डिस्प्ले सेटिंग को नियंत्रित करता है. उदाहरण के लिए, यह फील्ड, लेबल के प्रकार को नियंत्रित करता है, कि फील्ड अनिवार्य है या नहीं, किस सेक्शन में फील्ड नजर आता है.

निम्न उदाहरण ऐप के हेडर सेक्शन में गणना किए गए मूल्य को दिखाता है.

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

### <a name="use-chain-of-command-on-the-buildcustomfieldlistforheader-method-of-the-tstimesheetdetails-class-to-fill-in-timesheet-details"></a>TSTimesheetDetails वर्ग की buildCustomFieldListForHeader पद्धति के चेन ऑफ कमांड का इस्तेमाल टाइमशीट विवरण भरने के लिए करता है

**buildCustomFieldListForHeader** पद्धति का इस्तेमाल किसी मोबाइल में टाइमशीट हेडल विवरण भरने के लिए किया जाता है. TSTimesheetTable रिकॉर्ड को एक मानक के रूप में लेता है. उस रिकॉर्ड से फील्ड का उपयोग ऐप में कस्टम फील्ड मूल्य को भरने में किया जा सकता है दिए गए उदाहरण डेटाबेस से किसी मूल्य को नहीं पढ़ते. इसके स्थान पर, यह X++ तर्क का इस्तेमाल करते हैं ताकि गणना किए गए मूल्य को पैदा किया जा सके, जिसे बाद में ऐप पर दिखाया जाता है.


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

## <a name="other-configurabilityextensibility-opportunities"></a>अन्य विन्यास/विस्तीर्ण होने की क्षमता अवसर

### <a name="adding-additional-validation-for-the-app"></a>अनुप्रयोग के लिए अतिरिक्त सत्यापन जोड़ना

डेटाबेस स्तर पर टाइमशीट क्रियात्मकता के लिए मौजूदा तर्क अपेक्षा के अनुरूप काम करेगा. सहेजने या संचालन को पूरा करने में बाधा डालने और एक विशिष्ट त्रुटि संदेश दिखाने के लिए, आप **थ्रो एरर("उपयोगकर्ता को संदेश")** को चेन ऑफ कमांड एक्सटेंशन के माध्यम से कोड में जोड़ सकते हैं. विस्तार होने योग्य पद्धतियों के तीन उदाहरण हैं:

- TSTimesheetLine तालिका में **validateWrite** टाइमशीट पंक्ति में संचालन को सहेजने के लिए दौरान **गलत** हो जाता है, मोबाइल ऐप में त्रुटि का संदेश दिखता है.
- किसी अनुप्रयोग में टाइमशीट दाखिल करने के दौरान TSTimesheetTable तालिका में **validateSubmit** अगर **गलत** हो जाता है, उपयोगकर्ता को त्रुटि का एक संदेश दिखता है.
- TSTimesheetLine तालिका में **सम्मिलित** पद्धति के दौरान फील्ड में दर्ज किए गए तर्क (उदाहरण के लिए, **पंक्ति प्रॉपर्टी** ), अभी भी चलेगी.

### <a name="hiding-and-marking-out-of-box-fields-as-read-only-via-configuration"></a>आउट-ऑफ-बॉक्स फ़ील्ड को केवल कॉन्फ़िगरेशन के माध्यम से पढ़ने के रूप में छुपाना और चिह्नित करना

परियोजना मानक से, मोबाइल ऐप में एकदम अलग रीड-ओनली या छुपी हुई फील्ड तैयार कर सकते हैं. **परियोजना प्रबंधन और लेखांकन मानक** पृष्ठ के **टाइमशीट** टैब पर **मोबाइल टाइमशीट** सेक्शन में विकल्पों को सेट करें.

![प्रोजेक्ट पैरामीटर](media/5753b8ecccd1d8bb2b002dd538b3f762.png)

### <a name="changing-the-activities-that-are-available-for-selection-via-extensions"></a>गतिविधियों में बदलाव करना, जो कि प्रसारण के माध्यम से चयन के लिए उपलब्ध हैं

किसी परियोजना के चयन के लिए उपलब्ध गतिविधियां **getActivitiesForProject()** और **getActivityQuery()** विधि से **TsTimesheetProjectService** वर्ग में भरी जाती हैं. आप किसी विशिष्ट परियोजना के लिए चयन के लिए उपलब्ध गतिविधियों के अपने व्यवसाय परिदृश्य से मेल खाने के लिए इस चलन को बदलने के लिए चेन इन कमांड का उपयोग कर सकते हैं.

### <a name="entering-a-default-project-category-on-timesheet-entries"></a>टाइमशीट प्रविष्टियों पर डिफॉल्ट परियोजना श्रेणी दर्ज करना

टाइमशीट प्रविष्टियों पर डिफॉल्ट परियोजना श्रेणी की प्रविष्टि तीन स्तर पर उत्पन्न होती है. आप वांछित चलन प्राप्त करने के लिए चलन को किसी या इन सभी स्तरों पर विस्तार देने के लिए चेन ऑफ कमांड का इस्तेमाल कर सकते हैं. निम्नलिखित पदानुक्रम का उपयोग किया जाता है:

1. ऐप परियोजना संसाधन से डिफॉल्ट श्रेणी को रखने की कोशिश करता है. डिफॉल्ट श्रेणी **TSTimesheetSettingsService** वर्ग में **getCurrentUserResource** और **getDelegatedResourcesForCurrentUser** पद्धति में सेट किया जाता है.
2. अगर डिफॉल्ट श्रेणी परियोजना संसाधन के स्तर पर उपलब्ध नहीं कराया जाता, ऐप इसे परियोजना गतिविधि से लेने की कोशिश करता है. डिफॉल्ट श्रेणी **TSTimesheetProjectService** वर्ग में **getActivitiesForProject** पद्धति में सेट किया जाता है.
3. अगर डिफॉल्ट श्रेणी किसी परियोजना गतिविधि के स्तर पर उपलब्ध नहीं कराई जाती, तो डिफॉल्ट श्रेणी इसे परियोजना मानक से लेती है. डिफॉल्ट श्रेणी **TSTimesheetProjectService** वर्ग में **getProjectDetailsbyRule** पद्धति में सेट किया जाता है.
