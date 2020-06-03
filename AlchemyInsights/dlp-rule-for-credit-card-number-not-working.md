---
title: 信用卡號碼的 DLP 規則無法運作
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507397"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="36882-102">使用信用卡問題的 DLP 問題</span><span class="sxs-lookup"><span data-stu-id="36882-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="36882-103">**重要**：在這些前所未有的情況下，我們會採取下列步驟以確保 SharePoint Online 和 OneDrive 服務保持高度可用 – 請造訪 [SharePoint Online 暫時功能調整](https://aka.ms/ODSPAdjustments)以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="36882-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="36882-104">**使用信用卡問題的 DLP 問題**</span><span class="sxs-lookup"><span data-stu-id="36882-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="36882-105">當您在 O365 使用 DLP 敏感資訊類型時，**資料遺失防護（DLP）** 未針對包含**信用卡號碼**的內容運作時，是否發生問題？</span><span class="sxs-lookup"><span data-stu-id="36882-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="36882-106">如果是的話，請確定您的內容包含必要資訊，以便在評估時觸發 DLP 原則。</span><span class="sxs-lookup"><span data-stu-id="36882-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="36882-107">例如，對於設定為信賴等級85% 的**信用卡原則**，會評估下列專案，而且必須偵測到要觸發的規則：</span><span class="sxs-lookup"><span data-stu-id="36882-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="36882-108">**[格式：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 位數可格式化或未格式化（dddddddddddddddd），且必須通過 Luhn 測試。</span><span class="sxs-lookup"><span data-stu-id="36882-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="36882-109">**[模式：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** 非常複雜且健全的模式，可偵測全球所有主要品牌的卡，包括簽證、MasterCard、探索卡、JCB、美洲 Express、禮品卡和 diner 卡。</span><span class="sxs-lookup"><span data-stu-id="36882-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="36882-110">**[Checksum：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** 是，Luhn 檢查碼</span><span class="sxs-lookup"><span data-stu-id="36882-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="36882-111">**[定義：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** 如果接近300個字元以內，則 DLP 原則偵測到此敏感資訊類型的置信量是85%：</span><span class="sxs-lookup"><span data-stu-id="36882-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="36882-112">函數 Func_credit_card 找到符合模式的內容。</span><span class="sxs-lookup"><span data-stu-id="36882-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="36882-113">下列其中一項為真：</span><span class="sxs-lookup"><span data-stu-id="36882-113">One of the following is true:</span></span>

  - <span data-ttu-id="36882-114">會找到來自 Keyword_cc_verification 的關鍵字。</span><span class="sxs-lookup"><span data-stu-id="36882-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="36882-115">找到來自 Keyword_cc_name 的關鍵字</span><span class="sxs-lookup"><span data-stu-id="36882-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="36882-116">函數 Func_expiration_date 會找到正確日期格式的日期。</span><span class="sxs-lookup"><span data-stu-id="36882-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="36882-117">Checksum 會通過</span><span class="sxs-lookup"><span data-stu-id="36882-117">The checksum passes</span></span>

    <span data-ttu-id="36882-118">例如，下列範例會觸發 DLP 信用卡號碼原則：</span><span class="sxs-lookup"><span data-stu-id="36882-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="36882-119">簽證： 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="36882-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="36882-120">到期：2/2009</span><span class="sxs-lookup"><span data-stu-id="36882-120">Expires: 2/2009</span></span>

<span data-ttu-id="36882-121">如需針對您的內容偵測**信用卡號碼**所需的詳細資訊，請參閱本文中的下一節：[機密資訊類型針對信用卡號碼的外觀](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="36882-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="36882-122">使用不同的內建機密資訊類型，請參閱下列文章，以瞭解其他類型所需的資訊：[機密資訊類型的外觀](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="36882-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  