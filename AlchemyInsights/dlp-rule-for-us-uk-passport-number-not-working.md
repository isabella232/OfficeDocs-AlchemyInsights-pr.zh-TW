---
title: 美國/UK Passport 號碼無法運作的 DLP 規則
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 0567e9521507bcc192b187d0e5a8a0658332ff99
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389532"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="5b18e-102">DLP-美國/英國護照號碼的問題</span><span class="sxs-lookup"><span data-stu-id="5b18e-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="5b18e-103">當您在 O365 中使用 DLP 敏感資訊類型時, 遇到**資料遺失防護 (DLP)** 無法使用包含**美國/英國護照號碼**的內容時, 是否發生問題？</span><span class="sxs-lookup"><span data-stu-id="5b18e-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="5b18e-104">若是如此, 請確定您的內容包含在評估時, DLP 原則所尋找的必要資訊。</span><span class="sxs-lookup"><span data-stu-id="5b18e-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="5b18e-105">例如, 對於設定為信賴等級 75% 的**美國/英國護照號碼**原則, 會評估並偵測規則, 以觸發</span><span class="sxs-lookup"><span data-stu-id="5b18e-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="5b18e-106">**[格式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 九位數</span><span class="sxs-lookup"><span data-stu-id="5b18e-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="5b18e-107">**[模式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 九個連續數位</span><span class="sxs-lookup"><span data-stu-id="5b18e-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="5b18e-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否, 沒有任何 Checksum</span><span class="sxs-lookup"><span data-stu-id="5b18e-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="5b18e-109">**[定義:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** 如果接近300個字元以內, 則 DLP 原則偵測到此敏感資訊類型的置信度 75%:</span><span class="sxs-lookup"><span data-stu-id="5b18e-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="5b18e-110">函數 Func_usa_uk_passport 找到符合模式的內容。</span><span class="sxs-lookup"><span data-stu-id="5b18e-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="5b18e-111">找到 Keyword_passport 中的關鍵字。</span><span class="sxs-lookup"><span data-stu-id="5b18e-111">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="5b18e-112">例如, 下列範例會觸發**美國/英國護照號碼**原則: 美國護照號碼123456789</span><span class="sxs-lookup"><span data-stu-id="5b18e-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="5b18e-113">如需針對您的內容偵測美國/英國護照號碼所需的詳細資訊, 請參閱本文的下列章節:[敏感資訊類型對美國/英國護照號碼的瞭解](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="5b18e-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="5b18e-114">使用不同的內建機密資訊類型, 請參閱下列文章, 以瞭解其他類型所需的資訊:[敏感資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="5b18e-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  