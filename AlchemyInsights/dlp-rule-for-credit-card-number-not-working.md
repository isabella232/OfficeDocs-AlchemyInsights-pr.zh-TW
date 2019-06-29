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
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389568"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="3e3cf-102">信用卡號碼的 DLP 問題</span><span class="sxs-lookup"><span data-stu-id="3e3cf-102">DLP issues with Credit Card Numbers</span></span>

<span data-ttu-id="3e3cf-103">您在 O365 中使用 DLP 敏感資訊類型時, 遇到**資料遺失防護 (DLP)** 無法使用包含**信用卡號碼**的內容時, 是否發生問題？</span><span class="sxs-lookup"><span data-stu-id="3e3cf-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="3e3cf-104">如果是的話, 請確定您的內容包含在評估時觸發 DLP 原則所需的資訊。</span><span class="sxs-lookup"><span data-stu-id="3e3cf-104">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="3e3cf-105">例如, 對於設定為信賴等級 85% 的**信用卡原則**, 會評估下列專案, 並且必須偵測到要觸發的規則:</span><span class="sxs-lookup"><span data-stu-id="3e3cf-105">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="3e3cf-106">**[格式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 位數可以格式化或未格式化 (dddddddddddddddd), 且必須通過 Luhn 測試。</span><span class="sxs-lookup"><span data-stu-id="3e3cf-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="3e3cf-107">**[模式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** 一種非常複雜且健全的模式, 可偵測全球所有主要品牌的卡, 包括簽證、MasterCard、探索卡、JCB、北美版、禮品卡及 diner 卡。</span><span class="sxs-lookup"><span data-stu-id="3e3cf-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="3e3cf-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** 是, Luhn 校驗和</span><span class="sxs-lookup"><span data-stu-id="3e3cf-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="3e3cf-109">**[定義:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** 如果接近300個字元以內, 則 DLP 原則偵測到此敏感資訊類型的置信度 85%:</span><span class="sxs-lookup"><span data-stu-id="3e3cf-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="3e3cf-110">函數 Func_credit_card 找到符合模式的內容。</span><span class="sxs-lookup"><span data-stu-id="3e3cf-110">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="3e3cf-111">下列其中一項為真:</span><span class="sxs-lookup"><span data-stu-id="3e3cf-111">One of the following is true:</span></span>

  - <span data-ttu-id="3e3cf-112">找到 Keyword_cc_verification 中的關鍵字。</span><span class="sxs-lookup"><span data-stu-id="3e3cf-112">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="3e3cf-113">找到 Keyword_cc_name 中的關鍵字</span><span class="sxs-lookup"><span data-stu-id="3e3cf-113">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="3e3cf-114">函數 Func_expiration_date 會找到正確日期格式的日期。</span><span class="sxs-lookup"><span data-stu-id="3e3cf-114">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="3e3cf-115">Checksum 會通過</span><span class="sxs-lookup"><span data-stu-id="3e3cf-115">The checksum passes</span></span>

    <span data-ttu-id="3e3cf-116">例如, 下列範例會觸發 DLP 信用卡號碼原則:</span><span class="sxs-lookup"><span data-stu-id="3e3cf-116">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="3e3cf-117">簽證: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="3e3cf-117">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="3e3cf-118">過期: 2/2009</span><span class="sxs-lookup"><span data-stu-id="3e3cf-118">Expires: 2/2009</span></span>

<span data-ttu-id="3e3cf-119">如需針對您的內容偵測**信用卡號碼**所需的詳細資訊, 請參閱本文的下列章節:[有關信用卡號碼的敏感資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="3e3cf-119">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="3e3cf-120">使用不同的內建機密資訊類型, 請參閱下列文章, 以瞭解其他類型所需的資訊:[敏感資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="3e3cf-120">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  