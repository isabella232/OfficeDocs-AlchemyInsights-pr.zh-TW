---
title: 無法使用的信用卡號碼的 DLP 規則
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404470"
---
<span data-ttu-id="37cfa-102">您遇到問題的**資料外洩防護 (DLP)** 無法運作時使用 O365 中的 DLP 敏感資訊類型，其中包含**信用卡號碼**的內容？</span><span class="sxs-lookup"><span data-stu-id="37cfa-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="37cfa-103">如果是的話，請確定您的內容包含要觸發的所需的資訊的 DLP 原則評估時。</span><span class="sxs-lookup"><span data-stu-id="37cfa-103">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="37cfa-104">例如，對於**信用卡原則**設定信賴等級的 85%，下列會評估，並必須要觸發的規則偵測到：</span><span class="sxs-lookup"><span data-stu-id="37cfa-104">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="37cfa-105">**[格式為：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 位數，可格式化或未格式化 (dddddddddddddddd)，且必須通過 Luhn 測試。</span><span class="sxs-lookup"><span data-stu-id="37cfa-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="37cfa-106">**[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** 偵測全球，包括 Visa、 Mastercard、 Discover Card、 JCB、 American Express、 禮品卡和大來卡所有主要品牌的非常複雜且健全的模式。</span><span class="sxs-lookup"><span data-stu-id="37cfa-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="37cfa-107">**[總和檢查碼：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** 是，Luhn 總和檢查碼</span><span class="sxs-lookup"><span data-stu-id="37cfa-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="37cfa-108">**[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP 原則是 85%以內，已偵測到此敏感資訊類型的如果鄰近性是 300 個字元：</span><span class="sxs-lookup"><span data-stu-id="37cfa-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="37cfa-109">函數 Func_credit_card 找到符合模式的內容。</span><span class="sxs-lookup"><span data-stu-id="37cfa-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="37cfa-110">下列其中一項為真：</span><span class="sxs-lookup"><span data-stu-id="37cfa-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="37cfa-111">找不到來自 Keyword_cc_verification 的關鍵字。</span><span class="sxs-lookup"><span data-stu-id="37cfa-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="37cfa-112">找到來自 Keyword_cc_name 的關鍵字</span><span class="sxs-lookup"><span data-stu-id="37cfa-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="37cfa-113">函數 Func_expiration_date 找到正確日期格式的日期。</span><span class="sxs-lookup"><span data-stu-id="37cfa-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="37cfa-114">總和檢查碼通過</span><span class="sxs-lookup"><span data-stu-id="37cfa-114">The checksum passes</span></span>
    
    <span data-ttu-id="37cfa-115">例如，下列範例會觸發 DLP 信用卡號碼原則：</span><span class="sxs-lookup"><span data-stu-id="37cfa-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="37cfa-116">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="37cfa-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="37cfa-117">到期： 2/2009</span><span class="sxs-lookup"><span data-stu-id="37cfa-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="37cfa-118">如需有關為何需要**Credit Card Number** ，偵測到您的內容的詳細資訊，請參閱這篇文章中的下列章節：[項目敏感資訊類型尋找信用卡 #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="37cfa-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="37cfa-119">使用不同的內建敏感資訊類型，請參閱 < 上為何需要其他類型的資訊的下列文章：<b0>項目敏感資訊類型在找</b0></span><span class="sxs-lookup"><span data-stu-id="37cfa-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

