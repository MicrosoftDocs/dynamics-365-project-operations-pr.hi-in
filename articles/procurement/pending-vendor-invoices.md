---
title: लंबित विक्रेता चालान का उपयोग करके स्टॉक-नहीं की गयी सामग्री खरीदें
description: यह विषय बताता है कि लंबित विक्रेता चालान को कैसे रिकॉर्ड किया जाए.
author: sigitac
ms.date: 04/12/2021
ms.topic: article
ms.prod: ''
ms.reviewer: kfend
ms.author: sigitac
ms.openlocfilehash: b5e6632d73c8a211b1f0d568be8e10ef47be77e2
ms.sourcegitcommit: 40f68387f594180af64a5e5c748b6efa188bd300
ms.translationtype: HT
ms.contentlocale: hi-IN
ms.lasthandoff: 05/10/2021
ms.locfileid: "5993797"
---
# <a name="purchase-non-stocked-materials-using-a-pending-vendor-invoice"></a><span data-ttu-id="4cc05-103">लंबित विक्रेता चालान का उपयोग करके स्टॉक-नहीं की गयी सामग्री खरीदें</span><span class="sxs-lookup"><span data-stu-id="4cc05-103">Purchase non-stocked materials using a pending vendor invoice</span></span>

<span data-ttu-id="4cc05-104">_**इस पर लागू होता है:** संसाधन/गैर-स्टॉक आधारित परिदृश्यों के लिए Project Operations_</span><span class="sxs-lookup"><span data-stu-id="4cc05-104">_**Applies To:** Project Operations for resource/non-stocked based scenarios_</span></span>

<span data-ttu-id="4cc05-105">जैसा कि एक कंपनी एक परियोजना के लिए स्टॉक-नहीं की गयी सामग्री खरीदती है, परियोजना के समक्ष तुरंत लागत रिकॉर्ड की जा सकती है.</span><span class="sxs-lookup"><span data-stu-id="4cc05-105">As a company procures non-stocked materials for a project, the costs can be immediately recorded against the project.</span></span> 

<span data-ttu-id="4cc05-106">उदाहरण के लिए, Contoso रोबोटिक्स US एक उपकरण नवीनीकरण परियोजना का प्रदर्शन कर रहा है और उसे सॉफ्टवेयर लाइसेंस की आवश्यकता है.</span><span class="sxs-lookup"><span data-stu-id="4cc05-106">For example, Contoso Robotics US is performing an equipment renewal project and needs software licenses.</span></span> <span data-ttu-id="4cc05-107">ये लाइसेंस किसी तीसरे पक्ष के विक्रेता से खरीदे जाते हैं.</span><span class="sxs-lookup"><span data-stu-id="4cc05-107">These licenses are procured from a third-party vendor.</span></span>  <span data-ttu-id="4cc05-108">Dynamics 365 Finance का उपयोग करते हुए, लेखा देय क्लर्क एक लंबित वेंडर इनवॉइस दस्तावेज़ को रिकॉर्ड करता है और उपकरण नवीनीकरण परियोजना के समक्ष लाइसेंस की लागत को सीधे संबन्धित करता है.</span><span class="sxs-lookup"><span data-stu-id="4cc05-108">Using Dynamics 365 Finance, the Accounts payable clerk records a pending vendor invoice document and attributes the license costs directly against the equipment renewal project.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="4cc05-109">इससे पहले कि आप इस विषय में वर्णित कार्यक्षमता का उपयोग करें, आवश्यक कॉन्फ़िगरेशन की समीक्षा करें और उसे लागू करें.</span><span class="sxs-lookup"><span data-stu-id="4cc05-109">Before you use the functionality described in this topic, review and apply the required configurations.</span></span> <span data-ttu-id="4cc05-110">अधिक जानकारी के लिए, [स्टॉक-नहीं की गई सामग्री और लंबित वेंडर इनवॉइस को सक्षम करें](configure-materials-nonstocked.md) देखें.</span><span class="sxs-lookup"><span data-stu-id="4cc05-110">For more information, see [Enable non-stocked materials and pending vendor invoices](configure-materials-nonstocked.md).</span></span> 

## <a name="post-a-project-related-pending-vendor-invoice"></a><span data-ttu-id="4cc05-111">परियोजना से संबंधित लंबित वेंडर इनवॉइस पोस्ट करें</span><span class="sxs-lookup"><span data-stu-id="4cc05-111">Post a project-related pending vendor invoice</span></span> 

<span data-ttu-id="4cc05-112">लंबित विक्रेता चालानों को **लंबित विक्रेता चालान** पृष्ठ (**देय खातों** > **चालान** > **लंबित विक्रेता चालान**) पर रिकॉर्ड किये जा सकते हैं.</span><span class="sxs-lookup"><span data-stu-id="4cc05-112">Pending vendor invoices can be recorded on the **Pending vendor invoices** page (**Accounts payable** > **Invoices** > **Pending vendor invoices**).</span></span> <span data-ttu-id="4cc05-113">परियोजना से संबंधित लंबित वेंडर चालान को पोस्ट करने के लिए निम्नलिखित चरणों को पूरा करें:</span><span class="sxs-lookup"><span data-stu-id="4cc05-113">Complete the following steps to post a project-related pending vendor invoice:</span></span>

1. <span data-ttu-id="4cc05-114">**देय खातों** > **चालान** पर जाएं और **नया** चुनें.</span><span class="sxs-lookup"><span data-stu-id="4cc05-114">Go to **Accounts payable** > **Invoices** and select **New**.</span></span> 
2. <span data-ttu-id="4cc05-115">**चालान खाता** फ़ील्ड में, एक विक्रेता को चुनें और **नंबर** फ़ील्ड में, विक्रेता चालान पहचान दर्ज करें.</span><span class="sxs-lookup"><span data-stu-id="4cc05-115">In the **Invoice account** field, select a vendor and in the **Number** field, enter the vendor invoice identification.</span></span>
3. <span data-ttu-id="4cc05-116">विक्रेता चालान और **आइटम नंबर** फ़ील्ड में एक लाइन जोड़ें, विक्रेता से खरीदे गए स्टॉक-नहीं किए गए आइटम का चयन करें.</span><span class="sxs-lookup"><span data-stu-id="4cc05-116">Add a line to the vendor invoice and in the **Item number** field, select the non-stocked item purchased from the vendor.</span></span> 

    > [!NOTE]
    > <span data-ttu-id="4cc05-117">एक खरीद श्रेणी पर आधारित विक्रेता चालान लाइन्स परियोजना के समक्ष रिकॉर्ड नहीं की जा सकती हैं.</span><span class="sxs-lookup"><span data-stu-id="4cc05-117">Vendor invoice lines that are based on a procurement category can't be recorded against the project.</span></span> 
    
5. <span data-ttu-id="4cc05-118">खरीदी गई मात्रा जोड़ें.</span><span class="sxs-lookup"><span data-stu-id="4cc05-118">Add the quantity purchased.</span></span> <span data-ttu-id="4cc05-119">सिस्टम स्टॉक-नहीं किए गए आइटम मूल्य कॉन्फ़िगरेशन के आधार पर यूनिट मूल्य को पॉप्युलेट करेगा.</span><span class="sxs-lookup"><span data-stu-id="4cc05-119">The system will populate the unit price based on the non-stocked item price configuration.</span></span> 
6. <span data-ttu-id="4cc05-120">लाइन पर कुल राशि और अन्य आवश्यक विवरण सत्यापित करें.</span><span class="sxs-lookup"><span data-stu-id="4cc05-120">Verify the total amount and other required details on the line.</span></span>
7. <span data-ttu-id="4cc05-121">लाइन विवरण पर, **परियोजना** टैब पर, उस परियोजना की आईडी चुनें, जिसमें इस आइटम को रिकॉर्ड किया जाएगा.</span><span class="sxs-lookup"><span data-stu-id="4cc05-121">On the line details, on the **Project** tab, select the ID of the project that this item will be recorded to.</span></span>
8. <span data-ttu-id="4cc05-122">वैकल्पिक रूप से, गतिविधि नंबर चुनें, और परियोजना श्रेणी और लाइन संपत्ति को अपडेट करें.</span><span class="sxs-lookup"><span data-stu-id="4cc05-122">Optionally, select the activity number, and update the project category and line property.</span></span>
9. <span data-ttu-id="4cc05-123">लंबित विक्रेता चालान पोस्ट करें.</span><span class="sxs-lookup"><span data-stu-id="4cc05-123">Post pending vendor invoice.</span></span> <span data-ttu-id="4cc05-124">जब चालान पोस्ट किया जाता है, तब प्रणाली रिकॉर्ड करता है:</span><span class="sxs-lookup"><span data-stu-id="4cc05-124">When the invoice is posted, the system records:</span></span>
    
    - <span data-ttu-id="4cc05-125">विक्रेता की बैलेंस राशि.</span><span class="sxs-lookup"><span data-stu-id="4cc05-125">The vendor balance amount.</span></span>
    - <span data-ttu-id="4cc05-126">बिक्री कर राशि.</span><span class="sxs-lookup"><span data-stu-id="4cc05-126">The sales tax amount.</span></span>
    - <span data-ttu-id="4cc05-127">परियोजना की लागत खरीद एकीकरण खाते में दर्ज की जाती है.</span><span class="sxs-lookup"><span data-stu-id="4cc05-127">The cost against the project is recorded to the procurement integration account.</span></span>
    - <span data-ttu-id="4cc05-128">Dataverse में परियोजना वास्तविक लेनदेन.</span><span class="sxs-lookup"><span data-stu-id="4cc05-128">The project actual transaction in Dataverse.</span></span> <span data-ttu-id="4cc05-129">इस लेन-देन को आगे चलकर [Project Operations एकीकरण पत्रिका](../project-accounting/project-operations-integration-journal.md) का उपयोग करके संसाधित किया जाता है.</span><span class="sxs-lookup"><span data-stu-id="4cc05-129">This transaction is further processed using the [Project Operations Integration journal](../project-accounting/project-operations-integration-journal.md).</span></span> <span data-ttu-id="4cc05-130">इस पत्रिका को पोस्ट करने से राशि खरीद एकीकरण खाते से परियोजना लागत खाते में चली जाती है.</span><span class="sxs-lookup"><span data-stu-id="4cc05-130">Posting this journal moves the amount from the procurement integration account to the project cost account.</span></span>
