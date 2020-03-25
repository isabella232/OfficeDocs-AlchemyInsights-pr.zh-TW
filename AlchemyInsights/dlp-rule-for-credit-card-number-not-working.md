---
title: 信用卡號碼的 DLP 規則無法運作
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932434"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="67202-102">使用信用卡問題的 DLP 問題</span><span class="sxs-lookup"><span data-stu-id="67202-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="67202-103">**重要**：許多 SharePoint 線上及 OneDrive 客戶對在後臺執行的服務執行業務關鍵型應用程式。</span><span class="sxs-lookup"><span data-stu-id="67202-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="67202-104">包括內容遷移、資料遺失防護（DLP）及備份解決方案。</span><span class="sxs-lookup"><span data-stu-id="67202-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="67202-105">在這些空前的時間內，我們採取的步驟，確定在遠端工作案例中，線上和 OneDrive 服務的 SharePoint，都為您的使用者提供高可用性和更可靠的服務。</span><span class="sxs-lookup"><span data-stu-id="67202-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="67202-106">為了支援這專案標，我們已在星期幾的白天時段內，對背景應用程式（遷移、DLP 和備份解決方案）進行更為緊密的節流限制。</span><span class="sxs-lookup"><span data-stu-id="67202-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="67202-107">您應該會認為，這些應用程式在這段時間內可達到非常有限的輸送量。</span><span class="sxs-lookup"><span data-stu-id="67202-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="67202-108">不過，當地區的晚上和週末時，服務會準備好處理來自背景應用程式的大量要求。</span><span class="sxs-lookup"><span data-stu-id="67202-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="67202-109">**使用信用卡問題的 DLP 問題**</span><span class="sxs-lookup"><span data-stu-id="67202-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="67202-110">當您在 O365 使用 DLP 敏感資訊類型時，**資料遺失防護（DLP）** 未針對包含**信用卡號碼**的內容運作時，是否發生問題？</span><span class="sxs-lookup"><span data-stu-id="67202-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="67202-111">如果是的話，請確定您的內容包含必要資訊，以便在評估時觸發 DLP 原則。</span><span class="sxs-lookup"><span data-stu-id="67202-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="67202-112">例如，對於設定為信賴等級85% 的**信用卡原則**，會評估下列專案，而且必須偵測到要觸發的規則：</span><span class="sxs-lookup"><span data-stu-id="67202-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="67202-113">**[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 位數可格式化或未格式化（dddddddddddddddd），且必須通過 Luhn 測試。</span><span class="sxs-lookup"><span data-stu-id="67202-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="67202-114">**[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** 非常複雜且健全的模式，可偵測全球所有主要品牌的卡，包括簽證、MasterCard、探索卡、JCB、美洲 Express、禮品卡和 diner 卡。</span><span class="sxs-lookup"><span data-stu-id="67202-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="67202-115">**[Checksum：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** 是，Luhn 檢查碼</span><span class="sxs-lookup"><span data-stu-id="67202-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="67202-116">**[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** 如果接近300個字元以內，則 DLP 原則偵測到此敏感資訊類型的置信量是85%：</span><span class="sxs-lookup"><span data-stu-id="67202-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="67202-117">函數 Func_credit_card 找到符合模式的內容。</span><span class="sxs-lookup"><span data-stu-id="67202-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="67202-118">下列其中一項為真：</span><span class="sxs-lookup"><span data-stu-id="67202-118">One of the following is true:</span></span>

  - <span data-ttu-id="67202-119">會找到來自 Keyword_cc_verification 的關鍵字。</span><span class="sxs-lookup"><span data-stu-id="67202-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="67202-120">找到來自 Keyword_cc_name 的關鍵字</span><span class="sxs-lookup"><span data-stu-id="67202-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="67202-121">函數 Func_expiration_date 會找到正確日期格式的日期。</span><span class="sxs-lookup"><span data-stu-id="67202-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="67202-122">Checksum 會通過</span><span class="sxs-lookup"><span data-stu-id="67202-122">The checksum passes</span></span>

    <span data-ttu-id="67202-123">例如，下列範例會觸發 DLP 信用卡號碼原則：</span><span class="sxs-lookup"><span data-stu-id="67202-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="67202-124">簽證： 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="67202-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="67202-125">到期：2/2009</span><span class="sxs-lookup"><span data-stu-id="67202-125">Expires: 2/2009</span></span>

<span data-ttu-id="67202-126">如需針對您的內容偵測**信用卡號碼**所需的詳細資訊，請參閱本文中的下一節：[機密資訊類型針對信用卡號碼的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="67202-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="67202-127">使用不同的內建機密資訊類型，請參閱下列文章，以瞭解其他類型所需的資訊：[機密資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="67202-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  