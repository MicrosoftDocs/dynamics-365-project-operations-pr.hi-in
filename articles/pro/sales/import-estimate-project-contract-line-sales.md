---
title: किसी अनुमान को एक परियोजना-आधारित अनुबंध पंक्ति में आयात करें - लाइट
description: यह विषय किसी परियोजना से अनुबंध लाइन तक वित्तीय अनुमान आयात करने के बारे में जानकारी प्रदान करता है.
author: rumant
manager: Annbe
ms.date: 10/19/2020
ms.topic: article
ms.service: project-operations
ms.reviewer: kfend
ms.author: rumant
ms.openlocfilehash: b462af163fef1bfcbbc4f945df722d4e8a71fb1a
ms.sourcegitcommit: 625878bf48ea530f3381843be0e778cebbbf1922
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 10/30/2020
ms.locfileid: "4177468"
---
# <a name="import-an-estimate-to-a-project-based-contract-line---lite"></a>किसी अनुमान को एक परियोजना-आधारित अनुबंध पंक्ति में आयात करें - लाइट

_**लागू होता है:** लाइट नियोजन-प्रोफार्मा इनवॉयसिंग करने के लिए समझौता_

Dynamics 365 Project Operations में, आप किसी परियोजना से परियोजना-आधारित अनुबंध लाइन में अनुमान आयात कर सकते हैं.

1. सत्यापित करें कि परियोजना-आधारित अनुबंध लाइन पर **परियोजना** फ़ील्ड भरा गया है.
2. **अनुबंध लाइन विवरण** टैब पर, सबग्रिड पर, **परियोजना अनुमान से आयात** का चयन करें. संक्षेपण विकल्पों वाला एक संवाद पृष्ठ खुलता है. उपलब्ध संक्षेपण विकल्प **लेनदेन वर्ग**, **श्रेणी**, **भूमिका**, और **परियोजना टास्क** हैं.
3. संक्षेप के चयन के आधार पर, इस अनुबंध लाइन पर शामिल सभी लेनदेन वर्गों और टास्कों के लिए परियोजना से अनुमान की कॉपी की जाती है. यह जांचने के लिए कि परियोजना-आधारित अनुबंध लाइन पर **सामान्य** टैब पर कौन सी लेनदेन वर्गें शामिल हैं, **समय शामिल करें**, **ख़र्च शामिल करें**, और **शुल्क शामिल करें** फ़ील्डों में मानों की जाँच करें. 
4. यह देखने के लिए कि कौन से टास्क शामिल हैं, अनुबंध लाइन पर **शुल्क योग्य टास्क** टैब का चयन करें. संबंधित टास्कों के आधार पर जिनके पास **शामिल लेनदेन वर्ग** फ़ील्ड **हाँ** के लिए सेट है, उन टास्कों और लेनदेन वर्ग के मेल के लिए सभी अनुमान अनुबंध लाइन पर आयात किए जाते हैं.

जब आप अनुमान आयात करते हैं, तो सिस्टम अनुबंध से जुड़ी परियोजना मूल्य सूचियों और अनुबंध लाइन पर सेट बिलिंग के प्रकार के आधार पर डिफ़ॉल्ट मूल्य निर्धारण करता है. यदि कोई टास्क, भूमिका या श्रेणी अनुबंध लाइन पर बिना-शुल्क योग्य के रूप में सेट की जाती है, तो आयातित अनुमान लाइन बिना-शुल्क योग्य होगी और अनुबंध लाइन के अनुबंधित मान में नहीं जुड़ेगी.

जब एक अनुबंध लाइन में लाइन विवरण होता है, तो अनुबंध लाइन पर **अनुबंध मान** और **अनुमानित कर** फ़ील्डों को संक्षेपित किया जाता है और उन्हें संपादित नहीं किया जा सकता है.

जब कई संक्षेपण विकल्पों का चयन किया जाता है, तो सिस्टम सभी चयनित विकल्पों द्वारा संक्षेपित करने का प्रयास करता है. यदि आप केवल एक संक्षेपण विकल्प चुनते हैं, तो संक्षेपण आउटपुट के परिणामस्वरूप अधिक आयातित अनुबंध लाइनें होती हैं.

उदाहरण के लिए, यदि परियोजना में ख़र्चों के लिए निम्नलिखित अनुमान लाइन हैं.

| कार्य | वर्ग | तिथि | मात्रा | इकाई मूल्य | राशि |
| --- | --- | --- | --- | --- | --- |
| कार्य A | विमान किराया | 10/1/2020 | 4 | 400 | 1600 |
| कार्य बी | होटल | 10/1/2020 | 4 | 200 | 800 |
| टास्क सी | होटल | 11/1/2020 | 2 | 200 | 400 |

जब उपयोगकर्ता **लेन-देन वर्ग** द्वारा संक्षेप में प्रस्तुत करने का चयन करता है, तो निम्नलिखित जानकारी आयात की जाएगी.

| कार्य | वर्ग | तिथि | मात्रा | इकाई मूल्य | राशि |
| --- | --- | --- | --- | --- | --- |
| &nbsp; | &nbsp; | 10/1/2020 | 3.34 | 840 | 2800 |

जब उपयोगकर्ता **लेन-देन वर्ग** और **श्रेणी** द्वारा संक्षेप में प्रस्तुत करने का चयन करता है, तो निम्नलिखित जानकारी आयात की जाएगी.

| कार्य | वर्ग | तिथि | मात्रा | इकाई मूल्य | राशि |
| --- | --- | --- | --- | --- | --- |
| कार्य A | विमान किराया | 10/1/2020 | 4 | 400 | 1600 |
| &nbsp;| होटल | 10/1/2020 | 6 | 200 | 1200 |

जब उपयोगकर्ता **लेनदेन वर्ग**, **श्रेणी** और **लीफ नोड टास्क** द्वारा संक्षेपित करने का चयन करता हैं, तो निम्नलिखित आयात की जाएगी. ध्यान दें कि यह परिणाम वही है जो परियोजना पर हैं:

| कार्य | वर्ग | तिथि | मात्रा | इकाई मूल्य | राशि |
| --- | --- | --- | --- | --- | --- |
| कार्य A | विमान किराया | 10/1/2020 | 4 | 400 | 1600 |
| कार्य बी | होटल | 10/1/2020 | 4 | 200 | 800 |
| टास्क सी | होटल | 11/1/2020 | 2 | 200 | 400 |