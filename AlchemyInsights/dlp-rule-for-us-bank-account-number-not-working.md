---
title: 美國銀行帳戶號碼不使用 DLP 規則
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404260"
---
<span data-ttu-id="9aa3f-102">您遇到問題的**資料外洩防護 (DLP)** 無法運作時使用 O365 中的 DLP 敏感資訊類型，其中包含**美國銀行帳戶號碼**的內容？</span><span class="sxs-lookup"><span data-stu-id="9aa3f-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="9aa3f-103">如果是的話，請確定您的內容包含的 DLP 原則會尋找的項目在評估時所需的資訊。</span><span class="sxs-lookup"><span data-stu-id="9aa3f-103">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="9aa3f-104">例如，對於**美國銀行帳戶號碼**原則設定信賴等級的 85%，下列進行評估，並必須要觸發的規則偵測到：</span><span class="sxs-lookup"><span data-stu-id="9aa3f-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="9aa3f-105">**[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 位數</span><span class="sxs-lookup"><span data-stu-id="9aa3f-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span> 
    
- <span data-ttu-id="9aa3f-106">**[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 個連續數字。</span><span class="sxs-lookup"><span data-stu-id="9aa3f-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span> 
    
- <span data-ttu-id="9aa3f-107">**[總和檢查碼：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，沒有任何總和檢查碼</span><span class="sxs-lookup"><span data-stu-id="9aa3f-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="9aa3f-108">**[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP 原則是 75%以內，已偵測到此敏感資訊類型的如果鄰近性是 300 個字元：</span><span class="sxs-lookup"><span data-stu-id="9aa3f-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="9aa3f-109">規則運算式 Regex_usa_bank_account_number 找到符合模式的內容</span><span class="sxs-lookup"><span data-stu-id="9aa3f-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>
    
  - <span data-ttu-id="9aa3f-110">找不到來自 Keyword_usa_Bank_Account 的關鍵字。</span><span class="sxs-lookup"><span data-stu-id="9aa3f-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>
    
    <span data-ttu-id="9aa3f-111">例如，下列範例會觸發**美國銀行帳戶號碼**原則： 檢查帳戶 78344011</span><span class="sxs-lookup"><span data-stu-id="9aa3f-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span> 
    
<span data-ttu-id="9aa3f-112">如需有關什麼是**美國銀行帳戶號碼**，才能偵測到您的內容所需的詳細資訊，請參閱這篇文章中的下列章節：[項目敏感資訊類型尋找美國銀行帳戶號碼](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="9aa3f-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="9aa3f-113">使用不同的內建敏感資訊類型，請參閱 < 上為何需要其他類型的資訊的下列文章：<b0>項目敏感資訊類型在找</b0></span><span class="sxs-lookup"><span data-stu-id="9aa3f-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

