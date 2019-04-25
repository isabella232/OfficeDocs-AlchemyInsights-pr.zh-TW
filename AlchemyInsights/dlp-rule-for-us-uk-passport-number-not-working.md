---
title: DLP 規則如美國 / 不使用 UK 護照號碼
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404372"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="17db5-102">問題 DLP-美國 / 英國護照號碼</span><span class="sxs-lookup"><span data-stu-id="17db5-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="17db5-103">您有問題**的資料外洩防護 (DLP)** 無法使用的內容包含**美國 / 英國護照號碼**時使用 O365 中的 DLP 敏感資訊類型？</span><span class="sxs-lookup"><span data-stu-id="17db5-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="17db5-104">如果是的話，請確定您的內容包含的 DLP 原則會尋找的項目在評估時所需的資訊。</span><span class="sxs-lookup"><span data-stu-id="17db5-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="17db5-105">例如，針對**美國 / 英國護照號碼**75%的信賴等級所設定的原則，下列會評估和必須偵測到要觸發的規則</span><span class="sxs-lookup"><span data-stu-id="17db5-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="17db5-106">**[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 九位數</span><span class="sxs-lookup"><span data-stu-id="17db5-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="17db5-107">**[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 九個連續數字</span><span class="sxs-lookup"><span data-stu-id="17db5-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="17db5-108">**[總和檢查碼：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，沒有任何總和檢查碼</span><span class="sxs-lookup"><span data-stu-id="17db5-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="17db5-109">**[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP 原則是 75%以內，已偵測到此敏感資訊類型的如果鄰近性是 300 個字元：</span><span class="sxs-lookup"><span data-stu-id="17db5-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="17db5-110">函數 Func_usa_uk_passport 找到符合模式的內容。</span><span class="sxs-lookup"><span data-stu-id="17db5-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="17db5-111">找不到來自 Keyword_passport 的關鍵字。</span><span class="sxs-lookup"><span data-stu-id="17db5-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="17db5-112">例如，下列範例會觸發的**美國 / 英國護照號碼**原則： 美國護照號碼 123456789</span><span class="sxs-lookup"><span data-stu-id="17db5-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="17db5-113">如需有關為何需要美國 / 英國護照號碼，才能偵測到您的內容，請參閱本文中的下列區段：[美國的項目敏感資訊類型尋找 / 英國護照號碼](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="17db5-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="17db5-114">使用不同的內建敏感資訊類型，請參閱 < 上為何需要其他類型的資訊的下列文章：<b0>項目敏感資訊類型在找</b0></span><span class="sxs-lookup"><span data-stu-id="17db5-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

