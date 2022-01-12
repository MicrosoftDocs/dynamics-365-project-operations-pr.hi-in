---
title: Project Service Automation से Project Operations में अपग्रेड करें
description: यह विषय . से अपग्रेड करने की प्रक्रिया का अवलोकन प्रदान करता है Microsoft Dynamics 365 Project Service Automation प्रति ।Dynamics 365 Project Operations
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 01/05/2022
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
ms.openlocfilehash: 9363fd5a06b6b1ba023961b03228e13a53a82002
ms.sourcegitcommit: 5789766efae1e0cb513ea533e4f9ac1e553158a5
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 01/10/2022
ms.locfileid: "7954292"
---
# <a name="upgrade-from-project-service-automation-to-project-operations"></a>Project Service Automation से Project Operations में अपग्रेड करें

हम अपग्रेड के लिए तीन चरणों में से पहले की घोषणा करते हुए उत्साहित हैं Microsoft Dynamics 365 Project Service Automation प्रति ।Dynamics 365 Project Operations यह विषय उन ग्राहकों के लिए एक सिंहावलोकन प्रदान करता है जो इस रोमांचक यात्रा की शुरुआत कर रहे हैं। भविष्य के विषयों में डेवलपर के विचार और फीचर एन्हांसमेंट के बारे में विवरण शामिल होंगे। वे न केवल आपको प्रोजेक्ट ऑपरेशंस में अपग्रेड के लिए तैयार करने में मदद करने के लिए मार्गदर्शन प्रदान करेंगे बल्कि यह भी बताएंगे कि अपग्रेड करने के बाद आप क्या उम्मीद कर सकते हैं।

उन्नयन वितरण कार्यक्रम को तीन चरणों में विभाजित किया जाएगा।

| डिलीवरी अपग्रेड करें | चरण 1 (जनवरी 2022) | चरण 2 (अप्रैल वेव 2022) | चरण 3 (अप्रैल वेव 2022) |
|------------------|------------------------|---------------------------|---------------------------|
| परियोजनाओं के लिए वर्क ब्रेकडाउन स्ट्रक्चर (डब्ल्यूबीएस) पर कोई निर्भरता नहीं | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| परियोजना संचालन की वर्तमान में समर्थित सीमाओं के भीतर WBS | | :heavy_check_mark: | :heavy_check_mark: |
| प्रोजेक्ट ऑपरेशंस की वर्तमान में समर्थित सीमाओं के बाहर WBS, प्रोजेक्ट डेस्कटॉप क्लाइंट के लिए समर्थन सहित | | | :heavy_check_mark: |

## <a name="upgrade-process-features"></a>प्रक्रिया सुविधाओं को अपग्रेड करें 

अपग्रेड प्रक्रिया के हिस्से के रूप में, हमने साइट मैप में अपग्रेड लॉग जोड़े हैं, ताकि व्यवस्थापक विफलताओं का अधिक आसानी से निदान कर सकें। नए इंटरफ़ेस के अलावा, अपग्रेड के बाद डेटा अखंडता सुनिश्चित करने के लिए नए सत्यापन नियम जोड़े जाएंगे। निम्नलिखित सत्यापन अपग्रेड प्रक्रिया में जोड़े जाएंगे।

| सत्यापन | चरण 1 (जनवरी 2022) | चरण 2 (अप्रैल वेव 2022) | चरण 3 (अप्रैल वेव 2022) |
|-------------|------------------------|---------------------------|---------------------------|
| WBS को सामान्य डेटा अखंडता उल्लंघनों के खिलाफ मान्य किया जाएगा (उदाहरण के लिए, संसाधन असाइनमेंट जो एक ही मूल कार्य से जुड़े हैं लेकिन अलग-अलग पैरेंट प्रोजेक्ट हैं)। | | :heavy_check_mark: | :heavy_check_mark: |
| WBS के विरुद्ध मान्य किया जाएगा[वेब के लिए परियोजना की ज्ञात सीमाएँ।](/project-for-the-web/project-for-the-web-limits-and-boundaries) | | :heavy_check_mark: | :heavy_check_mark: |
| WBS को प्रोजेक्ट डेस्कटॉप क्लाइंट की ज्ञात सीमाओं के विरुद्ध मान्य किया जाएगा। | | :heavy_check_mark: | :heavy_check_mark: |
| सामान्य असंगत कैलेंडर नियम अपवादों के विरुद्ध बुक करने योग्य संसाधनों और प्रोजेक्ट कैलेंडर का मूल्यांकन किया जाएगा। | | :heavy_check_mark: | :heavy_check_mark: |

चरण 2 में, जो ग्राहक प्रोजेक्ट संचालन में अपग्रेड करते हैं, उनकी मौजूदा परियोजनाओं को प्रोजेक्ट प्लानिंग के लिए केवल-पढ़ने के अनुभव में अपग्रेड किया जाएगा। इस केवल-पढ़ने के अनुभव में, संपूर्ण WBS ट्रैकिंग ग्रिड में दिखाई देगा। WBS को संपादित करने के लिए, परियोजना प्रबंधक चुन सकते हैं **धर्मांतरित** मुख्य पर **परियोजनाओं** पृष्ठ। एक पृष्ठभूमि प्रक्रिया तब प्रोजेक्ट को अपडेट करेगी ताकि वह वेब के लिए प्रोजेक्ट से नए प्रोजेक्ट शेड्यूलिंग अनुभव का समर्थन कर सके। यह चरण उन ग्राहकों के लिए उपयुक्त है जिनके पास ऐसी परियोजनाएं हैं जो के भीतर फिट होती हैं [वेब के लिए परियोजना की ज्ञात सीमाएँ](/project-for-the-web/project-for-the-web-limits-and-boundaries).

चरण 3 में, प्रोजेक्ट डेस्कटॉप क्लाइंट के लिए समर्थन जोड़ा जाएगा, उन ग्राहकों के लाभ के लिए जो उस एप्लिकेशन से अपनी परियोजनाओं को संपादित करना जारी रखना चाहते हैं। हालांकि, यदि मौजूदा प्रोजेक्ट वेब अनुभव के लिए नए प्रोजेक्ट में कनवर्ट किए जाते हैं, तो प्रत्येक रूपांतरित प्रोजेक्ट के लिए ऐड-इन तक पहुंच अक्षम कर दी जाएगी।

## <a name="prerequisites"></a>पूर्वावश्यकताएँ

चरण 1 अपग्रेड के लिए पात्र होने के लिए, ग्राहक को निम्नलिखित मानदंडों को पूरा करना होगा:

- लक्ष्य परिवेश में कोई रिकॉर्ड नहीं होना चाहिए **msdyn_projecttask** कंपनी।
- वैध परियोजना संचालन लाइसेंस ग्राहक के सभी सक्रिय उपयोगकर्ताओं को सौंपे जाने चाहिए। 
- ग्राहक को अपग्रेड प्रक्रिया को कम से कम एक गैर-उत्पादन परिवेश में मान्य करना चाहिए जिसमें एक प्रतिनिधि डेटासेट हो जो उत्पादन डेटा के साथ संरेखित हो।
- लक्ष्य परिवेश को Project Service Automation Update रिलीज़ 38 या बाद के संस्करण में अद्यतन किया जाना चाहिए।

चरण 2 और चरण 3 के लिए पूर्वापेक्षाएँ सामान्य उपलब्धता तिथियों के दृष्टिकोण के रूप में अद्यतन की जाएंगी।

## <a name="licensing"></a>लाइसेंसिंग

यदि आपके पास Project Service Automation के लिए सक्रिय लाइसेंस हैं, तो आप Project Operations को स्थापित और उपयोग कर सकते हैं, जिसमें Project Service Automation की सभी क्षमताएँ और बहुत कुछ शामिल हैं। इस तरह, जब आप उत्पादन में Project Service Automation का उपयोग करना जारी रखते हैं, तब आप Project संचालन की क्षमताओं का परीक्षण कर सकते हैं। आपके Project Service Automation लाइसेंस की समय सीमा समाप्त होने के बाद, आपको Project Operations में संक्रमण करना होगा। जब आप इस संक्रमण की योजना बनाते हैं, तो आपको इस तथ्य पर ध्यान देना चाहिए कि Project Operations लाइसेंस में Project Service Automation लाइसेंस शामिल नहीं है।

## <a name="testing-and-refactoring-customizations"></a>अनुकूलन का परीक्षण और रीफैक्टरिंग

एक प्रारंभिक बिंदु के रूप में, सभी अनुकूलन को एक स्वच्छ परियोजना संचालन (लाइट) वातावरण में आयात करें ताकि यह पुष्टि हो सके कि आयात सफल है, और यह कि व्यवसाय संचालन अपेक्षा के अनुरूप व्यवहार करता है।

देखने के लिए यहां कुछ चीजें दी गई हैं:

- अनुपलब्ध निर्भरता के कारण आयात विफल हो सकता है। दूसरे शब्दों में, अनुकूलन संदर्भ फ़ील्ड या अन्य घटक जिन्हें प्रोजेक्ट संचालन में हटा दिया गया है। इस स्थिति में, इन निर्भरताओं को विकास परिवेश से हटा दें।
- यदि आपके अप्रबंधित और प्रबंधित समाधानों में ऐसे घटक शामिल हैं जो अनुकूलित नहीं हैं, तो उन घटकों को समाधान से निकाल दें। उदाहरण के लिए, जब आप इसे अनुकूलित करते हैं **परियोजना** निकाय, अपने समाधान में केवल निकाय शीर्षलेख जोड़ें. सभी फ़ील्ड न जोड़ें। यदि आपने पहले सभी उप-घटक जोड़े हैं, तो आपको मैन्युअल रूप से एक नया समाधान बनाना होगा और उसमें प्रासंगिक घटक जोड़ना होगा।
- प्रपत्र और दृश्य अप्रत्याशित रूप से प्रकट नहीं हो सकते हैं। कुछ परिस्थितियों में, यदि आपने किसी भी आउट-ऑफ़-बॉक्स प्रपत्र या दृश्य को अनुकूलित किया है, तो अनुकूलन प्रोजेक्ट संचालन में नए अपडेट को प्रभावी होने से रोक सकता है। इन मुद्दों की पहचान करने के लिए, हम अनुशंसा करते हैं कि आप प्रोजेक्ट ऑपरेशन की क्लीन इंस्टॉलेशन और प्रोजेक्ट ऑपरेशंस की स्थापना की साथ-साथ समीक्षा करें जिसमें आपके अनुकूलन शामिल हैं। यह पुष्टि करने के लिए अपने व्यवसाय में सबसे अधिक उपयोग किए जाने वाले फ़ॉर्म की तुलना करें कि फ़ॉर्म का आपका संस्करण अभी भी समझ में आता है और फ़ॉर्म के स्वच्छ संस्करण से कुछ छूट नहीं रहा है। आपके द्वारा अनुकूलित किए गए किसी भी दृश्य के लिए उसी प्रकार की साथ-साथ समीक्षा करें।
- व्यावसायिक तर्क रनटाइम पर विफल हो सकता है। चूंकि आयात के समय आपके प्लग-इन में फ़ील्ड के संदर्भ मान्य नहीं हैं, इसलिए उन फ़ील्ड के संदर्भों के कारण व्यावसायिक तर्क विफल हो सकता है जो अब मौजूद नहीं हैं, और आपको निम्न उदाहरण के जैसा एक त्रुटि संदेश प्राप्त हो सकता है: "'प्रोजेक्ट' इकाई में नाम = 'msdyn_plannedhours' और नाममैपिंग = 'लॉजिकल' के साथ विशेषता नहीं है।" इस मामले में, अपने अनुकूलन संशोधित करें ताकि वे नए क्षेत्रों का उपयोग करें। यदि आप अपने प्लग-इन लॉजिक में स्वचालित रूप से जेनरेट की गई प्रॉक्सी कक्षाओं और मजबूत प्रकार के संदर्भों का उपयोग करते हैं, तो उन प्रॉक्सी को क्लीन इंस्टॉलेशन से पुन: उत्पन्न करने पर विचार करें। इस तरह, आप आसानी से उन सभी स्थानों की पहचान कर सकते हैं जहां आपके प्लग-इन बहिष्कृत फ़ील्ड पर निर्भर करते हैं।

प्रोजेक्ट ऑपरेशन को साफ़-साफ़ आयात करने के लिए अपने कस्टमाइज़ेशन को अपडेट करने के बाद, अगले चरणों पर जाएँ।

## <a name="end-to-end-testing-in-lower-environments"></a>निचले वातावरण में एंड-टू-एंड परीक्षण

### <a name="run-the-upgrade-in-production"></a>उत्पादन में उन्नयन चलाएँ

1. में Power Platform व्यवस्थापन केंद्र, अपना परिवेश ढूंढें और चुनें. फिर, अनुप्रयोगों में, ढूंढें और चुनें **Dynamics 365 Project Operations**.
2. चुनते हैं **इंस्टॉल** उन्नयन शुरू करने के लिए। Power Platform व्यवस्थापक केंद्र इस स्थापना को एक नई स्थापना के रूप में प्रस्तुत करेगा। हालांकि, Project Service Automation के पुराने संस्करण की उपस्थिति का पता लगाया जाएगा, और मौजूदा स्थापना को अपग्रेड किया जाएगा।

    नवीनीकरण पूर्ण होने के बाद, परिवेश को यह दिखाना चाहिए कि Project Operations स्थापित है, और Project Service Automation स्थापित नहीं है।

    > [!NOTE]
    > परिवेश में डेटा की मात्रा के आधार पर, नवीनीकरण में कई घंटे लग सकते हैं। अपग्रेड का प्रबंधन करने वाली कोर टीम को तदनुसार योजना बनानी चाहिए और गैर-व्यावसायिक घंटों के दौरान अपग्रेड चलाना चाहिए। कुछ मामलों में, यदि डेटा वॉल्यूम बड़ा है, तो नवीनीकरण सप्ताहांत के दौरान चलाया जाना चाहिए। शेड्यूलिंग के बारे में निर्णय निचले वातावरण में परीक्षण के परिणामों पर आधारित होना चाहिए।

3. उपयुक्त के रूप में कस्टम समाधान अपग्रेड करें। इस बिंदु पर, आपके द्वारा अपने अनुकूलन में किए गए किसी भी परिवर्तन को लागू करें [अनुकूलन का परीक्षण और रीफैक्टरिंग](#testing-and-refactoring-customizations) इस विषय का खंड।
4. के लिए जाओ **समायोजन** \> **समाधान**, और अनइंस्टॉल करने के लिए चुनें **परियोजना संचालन बहिष्कृत घटक** उपाय।

    यह समाधान एक अस्थायी समाधान है जो मौजूदा डेटा मॉडल और अपग्रेड के दौरान मौजूद घटकों को रखता है। इस समाधान को हटाकर, आप उन सभी फ़ील्ड और घटकों को हटा देते हैं जिनका अब उपयोग नहीं किया जाता है। इस तरह, आप इंटरफ़ेस को सरल बनाने और एकीकरण और विस्तार को आसान बनाने में मदद करते हैं।

## <a name="major-changes-between-project-service-automation-and-project-operations"></a>प्रोजेक्ट सर्विस ऑटोमेशन और प्रोजेक्ट ऑपरेशंस के बीच बड़े बदलाव

यह खंड उन प्रमुख परिवर्तनों का सारांश प्रदान करता है जिनकी आप Project Service Automation और Project Operations के बीच अपेक्षा कर सकते हैं।

### <a name="project-planning"></a>परियोजना नियोजन

प्रोजेक्ट ऑपरेशंस में प्रोजेक्ट प्लानिंग क्षमताएं अब क्लाइंट-साइड लॉजिक और सर्वर-साइड लॉजिक के संयोजन पर निर्भर नहीं हैं। इसके बजाय, प्रोजेक्ट ऑपरेशंस वेब के लिए प्रोजेक्ट को शेड्यूलिंग इंजन के रूप में उपयोग करता है। शेड्यूलिंग क्षमताओं में यह परिवर्तन कई नई सुविधाओं को सक्षम बनाता है, जैसे बोर्ड और गैंट विचार, संसाधन-संचालित योजना,[कार्य चेकलिस्ट आइटम](https://support.microsoft.com/office/use-task-checklists-in-microsoft-project-for-the-web-c69bcf73-5c75-4ad3-9893-6d6f92360e9c), और प्रोजेक्ट शेड्यूलिंग मोड। नई शेड्यूलिंग क्षमताएं भी नए . के समृद्ध सेट द्वारा समर्थित हैं [एप्लिकेशन प्रोग्रामिंग इंटरफेस (एपीआई)](../project-management/schedule-api-preview.md). इन एपीआई का उद्देश्य यह सुनिश्चित करने में मदद करना है कि डब्ल्यूबीएस में किसी इकाई को बनाने, अपडेट करने या हटाने के लिए कोई प्रोग्रामेटिक ऑपरेशन शेड्यूल में परिकलित फ़ील्ड को दूषित नहीं करता है।

## <a name="billing-and-pricing"></a>बिलिंग और मूल्य निर्धारण

परियोजना संचालन में निरंतर निवेश के हिस्से के रूप में, बिलिंग और मूल्य निर्धारण में कई नई क्षमताएं उपलब्ध हैं। यहाँ कुछ उदाहरण दिए गए हैं:

- [परियोजनाओं और परियोजना कार्यों पर सामग्री के उपयोग की रिकॉर्डिंग](../material/material-usage-log.md)
- [उपसंविदा प्रबंधन](../pro/subcontracting/managing-subcontracts-overview.md)
- [एडवांसेस और रिटेनर-आधारित अनुबंध](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [अनुबंध से अधिक नहीं स्थिति और मान्यताएं](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- कार्य-आधारित बिलिंग

## <a name="frequently-asked-questions"></a>सामान्य प्रश्‍न

### <a name="which-deployment-types-are-currently-supported-for-upgrade"></a>वर्तमान में अपग्रेड के लिए कौन से परिनियोजन प्रकार समर्थित हैं?

| स्रोत                                                 | लक्ष्य                                                    | स्थिति                  |
|--------------------------------------------------------|-----------------------------------------------------------|-------------------------|
| परियोजना सेवा स्वचालन                             | परियोजना संचालन लाइट परिनियोजन                        | समर्थित               |
| Dynamics 365 Finance परियोजना प्रबंधन और लेखा | परियोजना संचालन लाइट परिनियोजन                        | वर्तमान में समर्थित नहीं है |
| वित्त परियोजना प्रबंधन और लेखा              | संसाधन/गैर-स्टॉक परिदृश्यों के लिए Project Operations     | वर्तमान में समर्थित नहीं है |
| वित्त परियोजना प्रबंधन और लेखा              | स्टॉक/उत्पादन ऑर्डर परिदृश्यों के लिए Project Operations | वर्तमान में समर्थित नहीं है |
| परियोजना सेवा स्वचालन 3.x                         | संसाधन/गैर-स्टॉक परिदृश्यों के लिए Project Operations     | वर्तमान में समर्थित नहीं है |
| वेब के लिए परियोजना (समर्पित वातावरण)            | परियोजना संचालन लाइट परिनियोजन                        | वर्तमान में समर्थित नहीं है |

### <a name="how-can-i-install-project-operations-before-the-upgrade-tooling-is-available"></a>अपग्रेड टूलिंग उपलब्ध होने से पहले मैं प्रोजेक्ट ऑपरेशंस को कैसे स्थापित कर सकता हूं?

अपग्रेड टूलिंग उपलब्ध होने से पहले प्रोजेक्ट ऑपरेशंस को स्थापित करने के लिए दो विकल्प हैं:

- एक नया वातावरण प्रदान करें।
- किसी भी बिक्री संगठन पर प्रोजेक्ट संचालन को अलग से परिनियोजित करें जहां Project Service Automation मौजूद नहीं है।

> [!NOTE]
> यदि किसी संगठन पर Project Service Automation स्थापित है, लेकिन उसका उपयोग नहीं किया गया था, तो उसे अनइंस्टॉल किया जा सकता है। आपके द्वारा Project Service Automation को पूरी तरह से हटाने के बाद, Project Operations को उसी संगठन पर स्थापित किया जा सकता है।