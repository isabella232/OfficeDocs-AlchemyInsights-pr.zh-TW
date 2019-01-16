---
title: 美國銀行帳戶號碼無法正常運作的 DLP 規則
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 6eae9146d33f5fc307085dbf931d57bdbb28b82e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28279469"
---
<span data-ttu-id="3334a-p101">您已有**資料遺失防護 (DLP)** 無法正常運作的內容時使用 DLP 敏感資訊類型 O365 中包含**美國銀行帳戶號碼**的問題嗎？若是如此，請確定您的內容包含的 DLP 原則會尋找的項目時會評估當中所需的資訊。</span><span class="sxs-lookup"><span data-stu-id="3334a-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="3334a-104">例如 85%的信賴等級以設定為**US 銀行帳戶號碼**原則，下列會評估和必須偵測到的工作流程觸發此規則：</span><span class="sxs-lookup"><span data-stu-id="3334a-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="3334a-105">**[格式：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8 17 位數</span><span class="sxs-lookup"><span data-stu-id="3334a-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="3334a-106">**[模式：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8 17 連續的數字。</span><span class="sxs-lookup"><span data-stu-id="3334a-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="3334a-107">**[總和檢查碼：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，沒有任何總和檢查碼</span><span class="sxs-lookup"><span data-stu-id="3334a-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="3334a-108">**[定義：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP 原則就是有信心它已偵測到這種敏感資訊類型的 75 %if，300 個字元的距離：</span><span class="sxs-lookup"><span data-stu-id="3334a-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="3334a-109">規則運算式 Regex_usa_bank_account_number 會找出符合模式的內容</span><span class="sxs-lookup"><span data-stu-id="3334a-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="3334a-110">找到來自於 Keyword_usa_Bank_Account 的關鍵字。</span><span class="sxs-lookup"><span data-stu-id="3334a-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="3334a-111">例如，下列範例會觸發**美國銀行帳戶號碼**原則： 檢查帳戶 78344011</span><span class="sxs-lookup"><span data-stu-id="3334a-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="3334a-112">什麼是**美國銀行帳戶號碼**來偵測的內容所需的詳細資訊，請參閱本文的下列章節：[什麼敏感資訊類型尋找美國銀行帳戶號碼](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="3334a-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="3334a-113">使用不同的內建敏感資訊類型，請參閱上功能所需的其他類型的資訊的下列文章：[尋找什麼敏感資訊類型](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="3334a-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

