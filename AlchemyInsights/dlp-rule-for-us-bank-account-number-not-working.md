---
title: 美國銀行帳戶號碼無法運作的 DLP 規則
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 45aa50f6c3505468e902e58faf698205f93f9264
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704030"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="52dc8-102">美國銀行帳戶號碼的 DLP 問題</span><span class="sxs-lookup"><span data-stu-id="52dc8-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="52dc8-103">**重要**：在這些前所未有的情況下，我們會採取下列步驟以確保 SharePoint Online 和 OneDrive 服務保持高度可用 – 請造訪 [SharePoint Online 暫時功能調整](https://aka.ms/ODSPAdjustments)以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="52dc8-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="52dc8-104">**美國銀行帳戶號碼的 DLP 問題**</span><span class="sxs-lookup"><span data-stu-id="52dc8-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="52dc8-105">當您在 O365 中使用 DLP 敏感資訊類型時，**資料遺失防護（DLP）** 的內容無法使用包含**US 銀行帳號**的內容時，是否發生問題？</span><span class="sxs-lookup"><span data-stu-id="52dc8-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="52dc8-106">如果是的話，請確定您的內容中包含 DLP 原則在評估時所需的資訊。</span><span class="sxs-lookup"><span data-stu-id="52dc8-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="52dc8-107">例如，對於以信賴等級85% 設定的**US 銀行帳戶號碼**原則，會評估下列專案，而且必須偵測到要觸發的規則：</span><span class="sxs-lookup"><span data-stu-id="52dc8-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="52dc8-108">**[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 位數</span><span class="sxs-lookup"><span data-stu-id="52dc8-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="52dc8-109">**[Pattern：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 連續數位。</span><span class="sxs-lookup"><span data-stu-id="52dc8-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="52dc8-110">**[Checksum：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，沒有檢查</span><span class="sxs-lookup"><span data-stu-id="52dc8-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="52dc8-111">**[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** 如果接近300個字元以內，則 DLP 原則偵測到此敏感資訊類型的置信量是75%：</span><span class="sxs-lookup"><span data-stu-id="52dc8-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="52dc8-112">正則運算式 Regex_usa_bank_account_number 找到符合模式的內容。</span><span class="sxs-lookup"><span data-stu-id="52dc8-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="52dc8-113">會找到來自 Keyword_usa_Bank_Account 的關鍵字。</span><span class="sxs-lookup"><span data-stu-id="52dc8-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="52dc8-114">例如，下列範例會觸發**US 銀行帳戶號碼**原則：檢查帳戶78344011</span><span class="sxs-lookup"><span data-stu-id="52dc8-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="52dc8-115">如需針對您的內容偵測到**US 銀行帳戶**所需的資訊，請參閱本文中的下列章節：[機密資訊類型針對 US 銀行帳戶所尋找的功能](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)。</span><span class="sxs-lookup"><span data-stu-id="52dc8-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="52dc8-116">使用不同的內建機密資訊類型，請參閱下列文章，以瞭解其他類型所需的資訊：[機密資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="52dc8-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  