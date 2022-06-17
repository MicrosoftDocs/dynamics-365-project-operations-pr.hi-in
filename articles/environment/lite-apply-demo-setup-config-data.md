---
title: डेमो सेटअप और कॉन्फ़िगरेशन डेटा लागू करें - लाइट
description: यह आलेख प्रोजेक्ट संचालन के लिए डेमो सेटअप और कॉन्फ़िगरेशन डेटा को लागू करने के तरीके के बारे में जानकारी प्रदान करता है।
author: sigitac
ms.date: 01/27/2021
ms.topic: article
ms.reviewer: johnmichalak
ms.author: sigitac
ms.openlocfilehash: 68e504dd031596b295b1383a8e81621744cae8d2
ms.sourcegitcommit: 6cfc50d89528df977a8f6a55c1ad39d99800d9b4
ms.translationtype: MT
ms.contentlocale: hi-IN
ms.lasthandoff: 06/03/2022
ms.locfileid: "8922316"
---
# <a name="apply-demo-setup-and-configuration-data-for-project-operations---lite"></a>Project Operations के लिए डेमो सेटअप और कॉन्फ़िगरेशन डेटा लागू करें - लाइट 

_**लाइट परिनियोजन - प्रोफ़ॉर्मा इनवॉइस करने के लिए डील_



## <a name="prerequisites"></a>पूर्वावश्यकताएँ

कॉन्फ़िगरेशन शुरू करने से पहले, आपके पास Dynamics 365 Project Operations के लिए एक Common Data Service (CDS) परिवेश प्रोविज़न किया गया होना चाहिए.


## <a name="instructions"></a>निर्देश

1. [मास्टर डेटा पैकेज](https://download.microsoft.com/download/3/4/1/341bf279-a64f-4baa-af31-ce624859b518/ProjOpsSampleSetupData-%20CE%20only.zip) डाउनलोड करें. 
2. *ProjOpsSampleSetupData - CE केवल CMT* फ़ोल्डर में नेविगेट करें और निष्पादन योग्य फ़ाइल, *DataMigrationUtility* चलाएं.
3. Common Data Service कॉन्फ़िगरेशन माइग्रेशन (CMT) विज़ार्ड के पेज 1 पर, **डेटा आयात करें** चुनें और फिर **जारी रखें** चुनें.

    ![कॉन्फ़िगरेशन माइग्रेशन.](./media/1ConfigurationMigration.png)

4. CMT विज़ार्ड के पृष्ठ 2 पर **Microsoft 365** के रूप में **परिनियोजन प्रकार**।
5. **उपलब्ध संगठनों की सूची प्रदर्शित करें** और **उन्नत दिखाएं** चेक बॉक्स चुनें।
6. अपने किरायेदार के क्षेत्र का चयन करें, अपनी साख दर्ज करें, और फिर **लॉग-इन** का चयन करें.

   ![साइन इन का कॉन्फ़िगरेशन करें.](./media/2ConfigurationSignin.png)

7. पृष्ठ 3 पर, किरायेदार पर संगठनों की सूची से, चुनें कि आप किस संगठन में डेमो डेटा आयात करना चाहते/चाहती हैं और फिर **लॉग-इन** का चयन करें.
8. पृष्ठ 4 पर, ज़िप फ़ाइल, *SampleSetupAndConfigData* को अनपैक किए गए फ़ोल्डर, *ProjOpsSampleSetupData - CE केवल CMT* से चुनें.

   ![ज़िप फ़ाइल.](./media/3ZipFile.png)

   ![एक फ़ाइल चुनें.](./media/4SelectAFile.png)

9. ज़िप फ़ाइल चुनने के बाद **डेटा आयात करें** चुनें।

   ![डेटा आयात करें.](./media/5ImportData.png)

10. आपके नेटवर्क की स्पीड के आधार पर आयात लगभग दो-दस मिनट तक चलेगा। इसके पूरा होने के बाद, CMT विजार्ड से बाहर निकलें. 
11. डेटा के लिए अपने संगठन की निम्नलिखित 18 निकायों में जांच करें:

    -   मुद्रा
    -   खाता
    -   संगठनात्मक इकाई
    -   संपर्क
    -   इकाई
    -   इकाई समूह
    -   मूल्य सूची
    -   परियोजना पैरामीटर मूल्य सूची 
    -   इनवॉइस आवृत्ति
    -   बुक करने योग्य संसाधन श्रेणी
    -   लेनदेन श्रेणी
    -   व्यय श्रेणी
    -   भूमिका मू्ल्य
    -   लेनदेन श्रेणी मूल्य
    -   विशेषता
    -   बुक करने योग्य संसाधन
    -   बुक करने योग्य संसाधन श्रेणी Assn
    -   बुक करने योग्य संसाधन विशेषता

    ![पूरा आयात.](./media/6CompleteImport.png)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
