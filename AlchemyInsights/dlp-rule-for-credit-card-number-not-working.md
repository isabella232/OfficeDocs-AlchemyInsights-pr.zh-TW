---
title: 信用卡號無法正常運作的 DLP 規則
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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919071"
---
<span data-ttu-id="ab4c3-p101">您已有**資料遺失防護 (DLP)** 無法正常運作的內容時使用 DLP 敏感資訊類型 O365 中包含**信用卡號**的問題嗎？若是如此，請確定您的內容包含所需的資訊來觸發時會評估當中的 DLP 原則。例如**信用卡原則**設定的 85%的信賴等級，下列會評估和必須偵測到的工作流程觸發此規則：</span><span class="sxs-lookup"><span data-stu-id="ab4c3-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="ab4c3-105">**[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 位數可格式化 (dddddddddddddddd) 和必須通過 Luhn 測試。</span><span class="sxs-lookup"><span data-stu-id="ab4c3-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="ab4c3-106">**[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** 偵測從所有主要品牌全世界，包括因為撰寫、 Mastercard、 探索卡片、 JCB、 American Express、 gift 卡及大來卡卡很複雜且完善圖樣。</span><span class="sxs-lookup"><span data-stu-id="ab4c3-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="ab4c3-107">**[總和檢查碼：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** 是、 Luhn 總和檢查碼</span><span class="sxs-lookup"><span data-stu-id="ab4c3-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="ab4c3-108">**[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP 原則是 85%有信心它已偵測到這種類型的機密資訊時，300 個字元的距離：</span><span class="sxs-lookup"><span data-stu-id="ab4c3-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="ab4c3-109">函數 Func_credit_card 找到符合模式的內容。</span><span class="sxs-lookup"><span data-stu-id="ab4c3-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="ab4c3-110">下列其中一項為真：</span><span class="sxs-lookup"><span data-stu-id="ab4c3-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="ab4c3-111">找到來自於 Keyword_cc_verification 的關鍵字。</span><span class="sxs-lookup"><span data-stu-id="ab4c3-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="ab4c3-112">找到從 Keyword_cc_name 關鍵字</span><span class="sxs-lookup"><span data-stu-id="ab4c3-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="ab4c3-113">函數 Func_expiration_date 找到正確日期格式的日期。</span><span class="sxs-lookup"><span data-stu-id="ab4c3-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="ab4c3-114">總和檢查碼會傳遞</span><span class="sxs-lookup"><span data-stu-id="ab4c3-114">The checksum passes</span></span>
    
    <span data-ttu-id="ab4c3-115">例如，在下列範例會觸發 DLP 信用卡號碼原則：</span><span class="sxs-lookup"><span data-stu-id="ab4c3-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="ab4c3-116">因為撰寫： 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="ab4c3-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="ab4c3-117">到期： 2/2009</span><span class="sxs-lookup"><span data-stu-id="ab4c3-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="ab4c3-118">什麼是**信用卡號**來偵測的內容所需的詳細資訊，請參閱本文的下列章節：[什麼敏感資訊類型尋找信用卡 #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="ab4c3-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="ab4c3-119">使用不同的內建敏感資訊類型，請參閱上功能所需的其他類型的資訊的下列文章：[尋找什麼敏感資訊類型](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="ab4c3-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

