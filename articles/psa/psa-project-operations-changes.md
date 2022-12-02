---
title: Project Service Automation से Project Operations में फ़ीचर बदल जाता है
description: यह आलेख Project Service Automation से Dynamics 365 Project Operations तक के लिए सुविधा परिवर्तनों का अवलोकन प्रदान करता है.
author: ruhercul
ms.custom: dyn365-projectservice
ms.date: 02/03/2022
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
ms.reviewer: johnmichalak
ms.openlocfilehash: a9c69fc4296d30763f3994a4955e64ab258ceb4f
ms.sourcegitcommit: 675e9f3615e701c5f998de3a5ea3e25df11ae107
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 09/09/2022
ms.locfileid: "9459928"
---
# <a name="feature-changes-from-project-service-automation-to-project-operations"></a>Project Service Automation से Project Operations में फ़ीचर बदल जाता है

Dynamics 365 Project Service Automation से Dynamics 365 Project Operations लाइट तक के अपग्रेड की डिलीवरी तीन चरणों में की जाएगी। यह आलेख उन प्रमुख परिवर्तनों के बारे में जानकारी प्रदान करता है जिनकी आप नवीनीकरण पूर्ण होने पर देखने की अपेक्षा कर सकते हैं।

| डिलीवरी अपग्रेड करें | फेज़ 1 <br>(जनवरी 2022) | फेज़ 2 <br>(नवंबर 2022) | फेज़ 3  |
|------------------|------------------------|---------------------------|---------------------------|
| परियोजनाओं के लिए वर्क ब्रेकडाउन स्ट्रक्चर (WBS) पर कोई निर्भरता नहीं। | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| Project Operations की वर्तमान में समर्थित सीमाओं के भीतर एक WBS | &nbsp; | :heavy_check_mark: | :heavy_check_mark: |
| Project Desktop Client के लिए समर्थन सहित, Project Operations की वर्तमान में समर्थित सीमाओं के बाहर एक WBS। | &nbsp; | &nbsp; | :heavy_check_mark: |

## <a name="project-management"></a>परियोजना प्रबंधन

उपयोगकर्ता अनुभव में सबसे महत्वपूर्ण परिवर्तन परियोजना नियोजन के क्षेत्र में होंगे। Project Operations द्वारा प्रदान की गई शेड्यूलिंग क्षमताओं का लाभ उठाकर वर्क ब्रेकडाउन स्ट्रक्चर (WBS) के प्रबंधन के लिए एक नया आधुनिक अनुभव अपनाता है [Project for the Web](https://support.microsoft.com/en-us/office/what-is-project-for-the-web-c19b2421-3c9d-4037-97c6-f66b6e1d2eb5).

## <a name="differences-in-the-scheduling-experience"></a>शेड्यूलिंग अनुभव में फ़र्क

निम्न तालिका Project Service Automation और Project Operations के बीच शेड्यूलिंग अंतरों को सारांशित करती है।

|  शेड्यूल करना     |   Project Operations   |   पीएसए   |
|-----------------|------------------------|---------|
| प्रोजेक्ट टेम्प्लेट - प्रोजेक्ट बनाते समय प्रोजेक्ट टेम्प्लेट को परिभाषित करने और लागू करने की क्षमता  |  &nbsp;    | :heavy_check_mark: |
| डेस्कटॉप क्लाइंट के साथ प्रोजेक्ट वर्क ब्रेकडाउन स्ट्रक्चर (WBS) इंटीग्रेशन   |    &nbsp;  | :heavy_check_mark: |
| बाधाएं - पहले नहीं शुरू करें, बाद में खत्म न करें  | :heavy_check_mark: |   &nbsp;  |
| मील के पत्थर - शून्य अवधि वाले कार्य   | :heavy_check_mark:  |  &nbsp;  |
| संसाधन संचालित कार्य सौंपे गए संसाधनों की उपलब्धता का सम्मान करेंगे   | :heavy_check_mark: |  &nbsp;    |
| समय-चरणीय संपादन - योजनाओं को संपादित करें और दिन-प्रतिदिन के आधार पर कार्य करें   |   &nbsp;  | :heavy_check_mark: |
| स्वचालित/मैन्युअल शेड्यूलिंग - स्वचालित रूप से या मैन्युअल रूप से कार्यों को शेड्यूल करने के लिए प्रोजेक्ट शेड्यूलिंग इंजन का उपयोग करें |  &nbsp; | :heavy_check_mark:  |
| बड़ी परियोजनाओं को सीधे उपयोगकर्ता इंटरफ़ेस में संपादित करें: संपादन योग्य योजनाओं के आकार की कोई सीमा नहीं है  | 500 कार्य सीमा  | :heavy_check_mark:       |
| प्रतिशत पूर्ण - कार्य प्रगति चिह्नित करें   | :heavy_check_mark:  |  &nbsp;  |
| [परियोजना अनुसूची मोड](../project-management/scheduling-modes.md) - परियोजना को निश्चित इकाइयों, निश्चित प्रयास या निश्चित अवधि के रूप में परिभाषित करें | :heavy_check_mark: | &nbsp; |
| समयरेखा - शेड्यूल विवरण की कल्पना करने और हितधारकों के साथ संवाद करने के लिए समयरेखा दृश्य बनाएं और अनुकूलित करें। | :heavy_check_mark:  | &nbsp; |
| प्रयास-संचालित कार्य - किसी कार्य को प्रयास संचालित के रूप में शेड्यूल करने के लिए शेड्यूलिंग इंजन समर्थन  | :heavy_check_mark:  | &nbsp; |
| **कार्य की जानकारी** डायलॉग बॉक्स - डायलॉग बॉक्स का उपयोग करके कार्य विवरण सहेजें | :heavy_check_mark:  |  &nbsp;  |
| खींचें और छोड़ें - बहु-चयन कार्य और WBS पर उनकी स्थिति संशोधित करें | :heavy_check_mark: | &nbsp;  |
| लचीले स्थायी विचार - कार्य विशेषताओं के अधिक विस्तृत विचारों को परिभाषित करें   | :heavy_check_mark:  | &nbsp; |
| WBS को सॉर्ट और फ़िल्टर करें  | :heavy_check_mark:  | &nbsp; |
| नॉन-वाटरफॉल परियोजना वितरण के लिए बोर्ड की राय  | :heavy_check_mark:   | &nbsp; |
| समयरेखा दृश्य - इंटरएक्टिव गैंट चार्ट का उपयोग WBS को देखने और संपादित करने के लिए किया जाता है   | :heavy_check_mark:  | &nbsp; |
| कीबोर्ड शॉर्टकट - सामान्य संचालन के लिए कीबोर्ड शॉर्टकट का उपयोग करें, जैसे इंडेंट या इंसर्ट  | :heavy_check_mark:  |  &nbsp; |
| बहु-स्तरीय पूर्ववत करें - संचालन के पूरे सेट को उलटने और पुन: लागू करके परिवर्तनों के प्रभाव को पूरी तरह से समझने के लिए क्या-अगर विश्लेषण करें | :heavy_check_mark: | &nbsp; |
| कट/कॉपी/पेस्ट - आवेदनों के बीच शेड्यूल विवरण को कॉपी और पेस्ट करके शेड्यूल डेवलपमेंट पर सहयोग करें  | :heavy_check_mark: | &nbsp; |
| कार्य चेकलिस्ट - किसी कार्य में अधिकतम 20 चेकलिस्ट आइटम जोड़ें   | :heavy_check_mark: | &nbsp; |

## <a name="project-planning"></a>परियोजना नियोजन

Project Operations में **परियोजना** पेज में Project Service Automation में **परियोजना** पृष्ठ की तुलना में महत्वपूर्ण अंतर है।

निम्नलिखित कार्रवाइयों को चरण 1 अपग्रेड के भाग के रूप में **परियोजना** पृष्ठ से हटा दिया गया है:

  - **MS Project में खोलें**
  - **टेम्पलेट बनाएँ**
  - **MS Project से अनलिंक करें**

Project Operations में **परियोजना** पेज में निम्नलिखित नए टैब शामिल हैं।

- **सामग्री अनुमान**
- **कार्य बिलिंग सेटअप**

**स्टेटस** टैब हटा दिया गया है और **स्टेटस** फील्ड अब प्रोजेक्ट के शेड्यूलिंग मोड के साथ **सारांश** टैब पर है।

   ![प्रोजेक्ट पेज पर अपडेट।](media/projectform.png)

**अनुसूची** टैब का नाम बदलकर **टास्क** टैब कर दिया गया है और Project for the Web के साथ नए प्रोजेक्ट प्लानिंग अनुभव को पेश करता है।

   ![नए प्रोजेक्ट कार्य टैब.](media/tasktab.png)

## <a name="scheduling-modes"></a>शेड्यूलिंग मोड

Project Operations ने एक नई सुविधा पेश की है, [शेड्यूलिंग मोड ](../project-management/scheduling-modes.md). सभी मौजूदा Project Service Automation प्रोजेक्ट Project Operations में **निश्चित अवधि** में डिफ़ॉल्ट होंगे। हालांकि, नई परियोजनाओं के लिए डिफ़ॉल्ट को **समायोजन** > **मापदंडों** > **पैरामीटर** > **अनुसूची मोड** पर जाकर प्रबंधित किया जा सकता है।

   ![शेड्यूल मोड के लिए प्रोजेक्ट पैरामीटर सेटिंग्स।](media/projectparameter.png)

## <a name="project-planning-limits"></a>परियोजना की योजना बनाने की सीमा

Project Operations सभी प्रोजेक्ट शेड्यूलिंग कार्यों के लिए Project for the Web पर निर्भर करता है। Project for the Web निम्न तालिका में सीमाओं का उपयोग करके कार्य विश्लेषण संरचना का प्रबंधन करता है।

| **क्षेत्र**                                          | **सीमा**             |
|----------------------------------------------------|-----------------------|
| परियोजना के लिए अधिकतम कुल कार्य                  | 500                   |
| परियोजना के लिए अधिकतम कुल अवधि               | 3650 दिन (10 वर्ष)  |
| परियोजना के लिए अधिकतम कुल संसाधन              | 300                   |
| परियोजना के लिए अधिकतम कुल लिंक (केवल आनुक्रमिक) | 600                   |
| किसी परियोजना के लिए अधिकतम कुल कस्टम फ़ील्ड          | 10                    |
| अधिकतम पदानुक्रम स्तर                            | 10 स्तर             |
| अधिकतम लिंक (आनुक्रमिक + पूर्ववर्ती)            | 20                    |
| लीफ कार्य की अधिकतम अवधि                      | 1250 दिन             |
| सारांश कार्य की अधिकतम अवधि                 | 3650 दिन (10 वर्ष)  |
| कार्य को सौंपे गए अधिकतम संसाधन               | 20 संसाधन          |
| कार्य के लिए समर्थित दिनांक की श्रेणी                    | 1/1/2000 - 12/31/2149 |
| चेकलिस्ट आइटम                                    | 20                    |

## <a name="project-planning-extensibility-and-development"></a>परियोजना नियोजन विस्तारशीलता और विकास

Project Operations में अपग्रेड करने के बाद, आपको प्रोजेक्ट शेड्यूलिंग एपीआई का उपयोग निम्न निकायों पर ऑपरेशन बनाने, अपडेट करने और हटाने के लिए करना चाहिए:

|   निकाय का नाम           |   निकाय तार्किक नाम       |
|-------------------------|-----------------------------|
| Project                 | msdyn_project               |
| परियोजना कार्य            | msdyn_projecttask           |
| परियोजना कार्य निर्भरता | msdyn_projecttaskdependency |
| संसाधन असाइनमेंट     | msdyn_resourceassignment    |
| परियोजना बकेट          | msdyn_projectbucket         |
| परियोजना टीम सदस्य     | msdyn_projectteam           |

यदि आपके पास वर्तमान में ऐसे अनुकूलन हैं जिनमें ये निकाय शामिल हैं, तो देखें [शेड्यूलिंग निकायों के साथ संचालन करने के लिए प्रोजेक्ट शेड्यूल API का उपयोग करें](../project-management/schedule-api-preview.md) कार्यान्वयन मार्गदर्शन के लिए।

## <a name="data-model-changes"></a>डेटा मॉडल बदलाव

अपग्रेड चरण 1 के भाग के रूप में, डेटा मॉडल में परिवर्तन किए गए हैं। ये परिवर्तन प्राथमिक रूप से मौजूदा निकायों में क्षेत्र परिवर्तन हैं। चरण 1 में, संस्थाएं, **msydn_project** तथा **msdyn_projectteam** अनुकूलन का एक रिफैक्टरिंग हैं। 

> [!IMPORTANT]
> भविष्य के अपग्रेड चरण पूरे होने पर यह अनुभाग अतिरिक्त निकायों के साथ अपडेट हो जाएगा।

निम्नलिखित क्षेत्रों को नए क्षेत्रों से बदल दिया गया है।

|   इकाई          |   पुराने लॉजिकल नाम   |   नए तार्किक नाम    |
|-------------------|----------------------|-----------------------|
| msdyn_project     | msdyn_actualhours    | msdyn_effortcompleted |
| msdyn_project     | msdyn_plannedhours   | msdyn_effort          |
| msdyn_project     | msdyn_remaininghours | msdyn_effortremaining |
| msdyn_project     | msdyn_scheduledend   | msdyn_finish          |
| msdyn_project     | msdyn_wbsduration    | msdyn_duration        |
| msdyn_projectteam | msdyn_assignedhours  | msdyn_effort          |
| msdyn_projectteam | msdyn_from           | msdyn_start           |
| msdyn_projectteam | msdyn_to             | msdyn_finish          |

निम्नलिखित फील्ड को जोड़ा गया है.

|   इकाई          |   तार्किक नाम                               |   विवरण |
|-------------------|----------------------------------------------|---------------|
| msdyn_project     | msdyn_actualfeesales                         | परियोजना पर वास्तविक शुल्क विक्रय के सकल को दिखाता है। केयवल Project Service Automation के उपयोग के लिए। |
| msdyn_project     | msdyn_actualmaterialcost                     | परियोजना पर वास्तविक सामाग्री के समेकित लागत को दिखाता है. केयवल Project Service Automation के उपयोग के लिए। |
| msdyn_project     | msdyn_actualmaterialsales                    | परियोजना पर वास्तविक सामग्री विक्रय के सकल को दिखाता है। केयवल Project Service Automation के उपयोग के लिए। |
| msdyn_project     | msdyn_businesscase                           |                |
| msdyn_project     | msdyn_contractlineproject                    | इस परियोजना से संबद्ध अनुबंध पंक्ति। |
| msdyn_project     | msdyn_copyprojectcorrelationid               | यह एक आंतरिक सिस्टम फ़ील्ड है, जिसका उपयोग परियोजना **संबंधित सहसंबंध आइडेंटिफ़ायर को कॉपी करने** के लिए किया जाता है. केयवल Project Service Automation के उपयोग के लिए। |
| msdyn_project     | msdyn_copyprojectsessionid                   | यह एक आंतरिक सिस्टम फ़ील्ड है, जिसका उपयोग परियोजना **सत्र सहसंबंध आइडेंटिफ़ायर को कॉपी करने** के लिए किया जाता है. केयवल Project Service Automation के उपयोग के लिए। |
| msdyn_project     | msdyn_globalrevisiontoken                    | प्रोजेक्ट शेड्यूलिंग सेवा से अंतिम सिंक xRM ग्लोबल रिवीजन टोकन। |
| msdyn_project     | msdyn_msprojectdocument                      | वह परियोजना जिससे Microsoft Project दस्तावेज़ संबंधित है। |
| msdyn_project     | msdyn_plannedmaterialcost                    | परियोजना पर प्लांड सामग्री की समेकित लागत. केयवल Project Service Automation के उपयोग के लिए। |
| msdyn_project     | msdyn_plannedmaterialsales                   | परियोजना पर प्लांड सामग्री की समेकित लागत. केयवल Project Service Automation के उपयोग के लिए। |
| msdyn_project     | msdyn_program                                | प्रोग्राम, जिससे यह परियोजना संबंधित है. |
| msdyn_project     | msdyn_quotelineproject                       | इस परियोजना से संबद्ध कोट पंक्ति। |
| msdyn_project     | msdyn_replaylogheader                        | रीप्ले लॉग का शीर्षलेख. |
| msdyn_project     | msdyn_schedulemode                           | परियोजना के सभी कार्यों के लिए डिफ़ॉल्ट शेड्यूलिंग मोड उपयोग किया जाता है।  |
| msdyn_project     | msdyn_taskearlieststart                      | परियोजना में किसी भी कार्य की सबसे पहली आरंभ दिनांक.  |
| msdyn_project     | msdyn_valuestatement                         |                |
| msdyn_projectteam | msdyn_copyedfromprojectteammember            | उस परियोजना समूह सदस्य को दिखाता है, जिससे यह परियोजना समूह सदस्य कॉपी किया गया था. |
| msdyn_projectteam | msdyn_creategenericteammemberwithrequirement | इंगित करता है कि क्या नव-निर्मित जेनेरिक टीम के सदस्य के लिए संसाधन की आवश्यकता है.  |
| msdyn_projectteam | msdyn_deletestatus                           | यदि प्रोजेक्ट शेड्यूलिंग सर्विस का कोई डिलीट अनुरोध भेजा गया है और क्या यह सफलतापूर्वक अपेक्षित समय विंडो के भीतर प्रतिक्रिया वापस भेजता है तो ट्रैक करने के लिए टीम मेम्बर का डिलीट स्टेटस। |
| msdyn_projectteam | msdyn_effortcompleted                        | टीम के सदस्य द्वारा अपने असाइनमेंट पर पूरे किए गए प्रयासों की ट्रैकिंग. |
| msdyn_projectteam | msdyn_effortremaining                        | उनके असाइनमेंट पर टीम के सदस्य द्वारा अभी तक पूरे किए जाने वाले प्रयास को ट्रैक करें. |
| msdyn_projectteam | msdyn_markedfordeletiontimer                 | प्रतीक्षा अवधि जब टीम सदस्य प्रोजेक्ट शेड्यूलिंग सेवा को हटाने का अनुरोध भेजता है जब तक कि टीम के सदस्य को Microsoft Dataverse से वास्तव में हटाया नहीं जाता है।|
| msdyn_projectteam | msdyn_markedfordeletiontimestamp             | टीम के सदस्य को हटाने का अनुरोध प्रोजेक्ट शेड्यूलिंग सर्विस को भेजे जाने पर रिकॉर्ड करने का टाइमस्टैम्प. |
| msdyn_projectteam | msdyn_copiedfromprojectteammember            | उस परियोजना टीम सदस्य को दिखाता है, जिससे यह परियोजना टीम सदस्य कॉपी किया गया था.  |

## <a name="project-templates"></a>प्रोजेक्ट टेम्पलेट

Project Operations प्रोजेक्ट टेम्प्लेट के लिए समर्थन प्रदान नहीं करता है। हालाँकि, आप के [प्रोजेक्ट कॉपी एपीआई।](../project-management/dev-copy-project.md) के उपयोग के साथ बहुत सी मुख्य कार्यक्षमता को दोहरा सकते हैं।

## <a name="desktop-add-in-support"></a>डेस्कटॉप ऐड-इन समर्थन

Microsoft Project डेस्कटॉप ऐड-इन के लिए समर्थन नवीनीकरण के पहले 2 चरणों में उपलब्ध नहीं होगा। चरण 3 में, जिन ग्राहकों के पास Project for the Web की वर्तमान समर्थित सीमाओं से बड़े प्रोजेक्ट हैं, वे डेस्कटॉप ऐड-इन का उपयोग करने में सक्षम होंगे।

## <a name="editing-resource-assignment-contours"></a>संसाधन असाइनमेंट कौन्टो संपादित करना

नवीनीकरण के चरण 2 के उपलब्ध होने पर संसाधन असाइनमेंट रूपरेखाओं को संपादित करने की क्षमता उपलब्ध होगी।

## <a name="billing-and-pricing"></a>बिलिंग और मूल्य निर्धारण

Project Operations में शेड्यूल निम्नलिखित सुविधाओं का समर्थन करता है: ये विशेषताएं योगात्मक प्रकृति की हैं और Project Service Automation डेटा मॉडल को प्रभावित नहीं करती हैं।

- [परियोजनाओं और परियोजना कार्यों पर सामग्री उपयोग को रिकॉर्ड करना](../material/material-usage-log.md)
- [उप-अनुबंध प्रबंधन](../pro/subcontracting/managing-subcontracts-overview.md)
- [एडवांसेस और रिटेनर-आधारित अनुबंध](../pro/sales/set-up-advances-retainer-based-contracts-sales.md)
- [सीमा-में-रखें की स्थिति और मान्यताएँ अनुबंध](../pro/proforma-invoicing/manage-nte-status-validations-sales.md)
- [कार्य आधारित बिलिंग](../pro/sales/mapping-projects-tasks-quote-line-sales.md)

## <a name="deprecated-components"></a>बहिष्कृत घटक

निम्न तालिकाएं सभी पदावनत फ़ील्ड का दस्तावेज़ीकरण करती हैं जिन्हें अपग्रेड किए गए घटक समाधान पोस्ट अपग्रेड में ले जाया जाता है। अधिक जानकारी और समाधान के लिंक के लिए देखें [Dynamics 365 Project Service Automation Project Operations के लिए 3x 4x बहिष्कृत घटक  ](https://github.com/microsoft/Dynamics365-Project-Operations-PowerApps/tree/main/3x-4x-deprecated-solution).

### <a name="invoicedetail"></a>invoicedetail

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
|invoicedetail.msdyn_contractline    |

### <a name="msdyn_actual"></a>msdyn_actual

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_actual.msdyn_salescontractline                                                          |

### <a name="msdyn_characteristicreqforteammember"></a>msdyn_characteristicreqforteammember

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_characteristicreqforteammember.msdyn_characteristic                                     |
| msdyn_characteristicreqforteammember.msdyn_characteristicreqforteammemberid                   |
| msdyn_characteristicreqforteammember.msdyn_characteristictype                                 |
| msdyn_characteristicreqforteammember.msdyn_name                                               |
| msdyn_characteristicreqforteammember.msdyn_ratingvalue                                        |
| msdyn_characteristicreqforteammember.msdyn_resourcerequirementid                              |

### <a name="msdyn_contractlineinvoiceschedule"></a>msdyn_contractlineinvoiceschedule

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_contractlineinvoiceschedule.msdyn_contractline                                          |
| msdyn_contractlinescheduleofvalue.msdyn_contractline                                          |
 
### <a name="msdyn_dataexport"></a>msdyn_dataexport

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_dataexport.msdyn_dataexportid                                                           |
| msdyn_dataexport.msdyn_datatoken                                                              |
| msdyn_dataexport.msdyn_entityname                                                             |
| msdyn_dataexport.msdyn_exportedrecordcount                                                    |
| msdyn_dataexport.msdyn_exportstatus                                                           |
| msdyn_dataexport.msdyn_linkedentitydata                                                       |
| msdyn_dataexport.msdyn_name                                                                   |
| msdyn_dataexport.msdyn_pagingdata                                                             |

### <a name="msdyn_fact"></a>msdyn_fact

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_fact.msdyn_salescontractline                                                            |

### <a name="msdyn_findworkevent"></a>msdyn_findworkevent

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_findworkevent.msdyn_bookableresource                                                    |
| msdyn_findworkevent.msdyn_findworkeventid                                                     |
| msdyn_findworkevent.msdyn_name                                                                |
| msdyn_findworkevent.msdyn_timestamp                                                           |
| msdyn_findworkevent.msdyn_type                                                                |
| msdyn_findworkevent.msdyn_value                                                               |
| msdyn_findworkevent.msdyn_work                                                                |

### <a name="msdyn_invoicelinetransaction"></a>msdyn_invoicelinetransaction

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_invoicelinetransaction.msdyn_invoiceline                                                |
| msdyn_invoicelinetransaction.msdyn_salescontractline                                          |

### <a name="msdyn_journalline"></a>msdyn_journalline

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_journalline.msdyn_salescontractline                                                     |

### <a name="msdyn_opportunitylineresourcecategory"></a>msdyn_opportunitylineresourcecategory

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylineresourcecategory.msdyn_billingtype                                       |
| msdyn_opportunitylineresourcecategory.msdyn_description                                       |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylineresourcecategoryid                 |
| msdyn_opportunitylineresourcecategory.msdyn_opportunitylinetransactionclassification          |
| msdyn_opportunitylineresourcecategory.msdyn_resourcecategory                                  |

### <a name="msdyn_opportunitylinetransaction"></a>msdyn_opportunitylinetransaction

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransaction.msdyn_accountcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_accountingdate                                         |
| msdyn_opportunitylinetransaction.msdyn_accountvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_amount                                                 |
| msdyn_opportunitylinetransaction.msdyn_amount_base                                            |
| msdyn_opportunitylinetransaction.msdyn_amountmethod                                           |
| msdyn_opportunitylinetransaction.msdyn_basisamount                                            |
| msdyn_opportunitylinetransaction.msdyn_basisamount_base                                       |
| msdyn_opportunitylinetransaction.msdyn_basisprice                                             |
| msdyn_opportunitylinetransaction.msdyn_basisprice_base                                        |
| msdyn_opportunitylinetransaction.msdyn_basisquantity                                          |
| msdyn_opportunitylinetransaction.msdyn_billingtype                                            |
| msdyn_opportunitylinetransaction.msdyn_bookableresource                                       |
| msdyn_opportunitylinetransaction.msdyn_contactcustomer                                        |
| msdyn_opportunitylinetransaction.msdyn_contactvendor                                          |
| msdyn_opportunitylinetransaction.msdyn_customertype                                           |
| msdyn_opportunitylinetransaction.msdyn_description                                            |
| msdyn_opportunitylinetransaction.msdyn_documentdate                                           |
| msdyn_opportunitylinetransaction.msdyn_enddatetime                                            |
| msdyn_opportunitylinetransaction.msdyn_exchangeratedate                                       |
| msdyn_opportunitylinetransaction.msdyn_opportunityline                                        |
| msdyn_opportunitylinetransaction.msdyn_opportunitylinetransactionid                           |
| msdyn_opportunitylinetransaction.msdyn_percent                                                |
| msdyn_opportunitylinetransaction.msdyn_price                                                  |
| msdyn_opportunitylinetransaction.msdyn_price_base                                             |
| msdyn_opportunitylinetransaction.msdyn_pricelist                                              |
| msdyn_opportunitylinetransaction.msdyn_product                                                |
| msdyn_opportunitylinetransaction.msdyn_project                                                |
| msdyn_opportunitylinetransaction.msdyn_quantity                                               |
| msdyn_opportunitylinetransaction.msdyn_resourcecategory                                       |
| msdyn_opportunitylinetransaction.msdyn_resourceorganizationalunitid                           |
| msdyn_opportunitylinetransaction.msdyn_startdatetime                                          |
| msdyn_opportunitylinetransaction.msdyn_task                                                   |
| msdyn_opportunitylinetransaction.msdyn_transactioncategory                                    |
| msdyn_opportunitylinetransaction.msdyn_transactionclassification                              |
| msdyn_opportunitylinetransaction.msdyn_transactiontypecode                                    |
| msdyn_opportunitylinetransaction.msdyn_unit                                                   |
| msdyn_opportunitylinetransaction.msdyn_unitschedule                                           |
| msdyn_opportunitylinetransaction.msdyn_vendortype                                             |

### <a name="msdyn_opportunitylinetransactioncategory"></a>msdyn_opportunitylinetransactioncategory

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactioncategory.msdyn_billingtype                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_description                                    |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactioncategoryid           |
| msdyn_opportunitylinetransactioncategory.msdyn_opportunitylinetransactionclassification       |
| msdyn_opportunitylinetransactioncategory.msdyn_transactioncategory                            |

### <a name="msdyn_opportunitylinetransactionclassificatio"></a>msdyn_opportunitylinetransactionclassificatio

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_opportunitylinetransactionclassificatio.msdyn_billingtype                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_description                               |
| msdyn_opportunitylinetransactionclassificatio.msdyn_include                                   |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunityline                           |
| msdyn_opportunitylinetransactionclassificatio.msdyn_opportunitylinetransactionclassificatioid |
| msdyn_opportunitylinetransactionclassificatio.msdyn_transactionclassification                 |

### <a name="msdyn_orderlineresourcecategory"></a>msdyn_orderlineresourcecategory

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlineresourcecategory.msdyn_contractline                                            |

### <a name="msdyn_orderlinetransaction"></a>msdyn_orderlinetransaction

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransaction.msdyn_salescontractline                                            |
| msdyn_orderlinetransactioncategory.msdyn_contractline                                         |

### <a name="msdyn_orderlinetransactionclassification"></a>msdyn_orderlinetransactionclassification

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_orderlinetransactionclassification.msdyn_contractline                                   |

### <a name="msdyn_project"></a>msdyn_project

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_project.msdyn_actualdurationminutes                                                     |
| msdyn_project.msdyn_actualhours                                                               |
| msdyn_project.msdyn_istemplate                                                                |
| msdyn_project.msdyn_plannedhours                                                              |
| msdyn_project.msdyn_projecttemplate                                                           |
| msdyn_project.msdyn_remaininghours                                                            |
| msdyn_project.msdyn_scheduleddurationminutes                                                  |
| msdyn_project.msdyn_scheduledend                                                              |
| msdyn_project.msdyn_stagename                                                                 |
| msdyn_project.msdyn_wbsduration                                                               |


### <a name="msdyn_projecttask"></a>msdyn_projecttask

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttask.msdyn_actualdurationminutes                                                 |
| msdyn_projecttask.msdyn_actualeffort                                                          |
| msdyn_projecttask.msdyn_aggregationdirection                                                  |
| msdyn_projecttask.msdyn_assignedresources                                                     |
| msdyn_projecttask.msdyn_assignedteammembers                                                   |
| msdyn_projecttask.msdyn_autoscheduling                                                        |
| msdyn_projecttask.msdyn_costestimatecontour                                                   |
| msdyn_projecttask.msdyn_effortcontour                                                         |
| msdyn_projecttask.msdyn_islinetask                                                            |
| msdyn_projecttask.msdyn_numberofresources                                                     |
| msdyn_projecttask.msdyn_remaininghours                                                        |
| msdyn_projecttask.msdyn_resourceutilization                                                   |
| msdyn_projecttask.msdyn_salesestimatecontour                                                  |
| msdyn_projecttask.msdyn_scheduledhours                                                        |
| msdyn_projecttask.msdyn_wbsid                                                                 |

### <a name="msdyn_projecttaskstatususer"></a>msdyn_projecttaskstatususer

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttaskstatususer.msdyn_bookableresource                                            |
| msdyn_projecttaskstatususer.msdyn_description                                                 |
| msdyn_projecttaskstatususer.msdyn_expectedcompletiondate                                      |
| msdyn_projecttaskstatususer.msdyn_expectedhourstocomplete                                     |
| msdyn_projecttaskstatususer.msdyn_iscompleted                                                 |
| msdyn_projecttaskstatususer.msdyn_name                                                        |
| msdyn_projecttaskstatususer.msdyn_percentcomplete                                             |
| msdyn_projecttaskstatususer.msdyn_projecttaskid                                               |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatusindicator                                  |
| msdyn_projecttaskstatususer.msdyn_projecttaskstatususerid                                     |

### <a name="msdyn_projectteam"></a>msdyn_projectteam

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteam.msdyn_applicantcount                                                        |
| msdyn_projectteam.msdyn_applicantsavailable                                                   |
| msdyn_projectteam.msdyn_assignedhours                                                         |
| msdyn_projectteam.msdyn_description                                                           |
| msdyn_projectteam.msdyn_from                                                                  |
| msdyn_projectteam.msdyn_hoursrequested                                                        |
| msdyn_projectteam.msdyn_membershipstatus                                                      |
| msdyn_projectteam.msdyn_number                                                                |
| msdyn_projectteam.msdyn_to                                                                    |

### <a name="msdyn_projectteammembersignup"></a>msdyn_projectteammembersignup

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projectteammembersignup.msdyn_bookableresource                                          |
| msdyn_projectteammembersignup.msdyn_membershipstatus                                          |
| msdyn_projectteammembersignup.msdyn_name                                                      |
| msdyn_projectteammembersignup.msdyn_projectteammembersignupid                                 |
| msdyn_projectteammembersignup.msdyn_teammembership                                            |

### <a name="msdyn_projecttransactioncategory"></a>msdyn_projecttransactioncategory

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_projecttransactioncategory.msdyn_billingtype                                            |
| msdyn_projecttransactioncategory.msdyn_name                                                   |
| msdyn_projecttransactioncategory.msdyn_project                                                |
| msdyn_projecttransactioncategory.msdyn_projecttransactioncategoryid                           |
| msdyn_projecttransactioncategory.msdyn_transactioncategory                                    |

### <a name="msdyn_quotelineinvoiceschedule"></a>msdyn_quotelineinvoiceschedule

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_quotelineinvoiceschedule.msdyn_quoteline                                                |
| msdyn_quotelineresourcecategory.msdyn_quoteline                                               |
| msdyn_quotelinescheduleofvalue.msdyn_quoteline                                                |
| msdyn_quotelinetransaction.msdyn_quoteline                                                    |
| msdyn_quotelinetransaction.msdyn_quoteline                                            |
| msdyn_quotelinetransactionclassification.msdyn_quoteline                                      |

### <a name="msdyn_resourceassignment"></a>msdyn_resourceassignment

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| msdyn_resourceassignment.msdyn_hours                                                          |
| msdyn_resourceassignment.msdyn_fromdate                                                       |
| msdyn_resourceassignment.msdyn_msprojectclientid                                              |
| msdyn_resourceassignment.msdyn_todate                                                         |
| msdyn_resourceassignmentdetail.msdyn_duration                                                 |
| msdyn_resourceassignmentdetail.msdyn_from                                                     |
| msdyn_resourceassignmentdetail.msdyn_name                                                     |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentdetailid                               |
| msdyn_resourceassignmentdetail.msdyn_resourceassignmentid                                     |

### <a name="salesorderdetail"></a>salesorderdetail

| फील्ड                                                    |
|-----------------------------------------------------------------------------------------------|
| salesorderdetail.msdyn_quoteline                                                              |

