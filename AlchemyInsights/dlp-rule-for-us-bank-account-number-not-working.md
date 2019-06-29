---
title: 適用于 US 銀行帳戶號碼的 DLP 規則無法運作
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 83050b05cffacd3e81d34f05383c213eb0042fae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389460"
---
<span data-ttu-id="3cbf1-102">當您在 O365 中使用 DLP 敏感資訊類型時, 遇到**資料遺失防護 (DLP)** 無法使用包含**US 銀行帳戶號碼**的內容時, 是否發生問題？</span><span class="sxs-lookup"><span data-stu-id="3cbf1-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="3cbf1-103">若是如此, 請確定您的內容包含在評估時, DLP 原則所尋找的必要資訊。</span><span class="sxs-lookup"><span data-stu-id="3cbf1-103">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="3cbf1-104">例如, 對於以信賴等級 85% 設定的**US 銀行帳戶號碼**原則, 會評估下列專案, 並且必須偵測到要觸發的規則:</span><span class="sxs-lookup"><span data-stu-id="3cbf1-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="3cbf1-105">**[格式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 位數</span><span class="sxs-lookup"><span data-stu-id="3cbf1-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="3cbf1-106">**[模式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 連續數位。</span><span class="sxs-lookup"><span data-stu-id="3cbf1-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="3cbf1-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否, 沒有任何 Checksum</span><span class="sxs-lookup"><span data-stu-id="3cbf1-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="3cbf1-108">**[定義:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** 如果接近300個字元以內, 則 DLP 原則偵測到此敏感資訊類型的置信度 75%:</span><span class="sxs-lookup"><span data-stu-id="3cbf1-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="3cbf1-109">正則運算式 Regex_usa_bank_account_number 找到符合模式的內容</span><span class="sxs-lookup"><span data-stu-id="3cbf1-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="3cbf1-110">找到 Keyword_usa_Bank_Account 中的關鍵字。</span><span class="sxs-lookup"><span data-stu-id="3cbf1-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="3cbf1-111">例如, 下列範例會觸發**美國銀行帳戶號碼**原則: 檢查帳戶78344011</span><span class="sxs-lookup"><span data-stu-id="3cbf1-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="3cbf1-112">如需針對您的內容偵測到**美國銀行帳戶**所需的詳細資訊, 請參閱本文中的下列章節:[敏感資訊類型對美國銀行帳戶號碼的檢查](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="3cbf1-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="3cbf1-113">使用不同的內建機密資訊類型, 請參閱下列文章, 以瞭解其他類型所需的資訊:[敏感資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="3cbf1-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  