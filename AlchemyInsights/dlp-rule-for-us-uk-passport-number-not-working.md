---
title: 美國的 DLP 規則 / 無法正常運作的英國護照號碼
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29460676"
---
<span data-ttu-id="fcc04-p101">您有問題與無法正常運作的內容包含**資料遺失防護 (DLP)** **美國 / 英國護照號碼**時 O365 中使用 DLP 敏感資訊類型？若是如此，請確定您的內容包含的 DLP 原則會尋找的項目時會評估當中所需的資訊。</span><span class="sxs-lookup"><span data-stu-id="fcc04-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="fcc04-104">例如，用於**美國 / 英國護照號碼**原則的 75%的信賴等級以設定下列會評估和必須以觸發規則偵測到</span><span class="sxs-lookup"><span data-stu-id="fcc04-104">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="fcc04-105">**[格式：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 9 的數字</span><span class="sxs-lookup"><span data-stu-id="fcc04-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="fcc04-106">**[模式：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 九個連續的數字</span><span class="sxs-lookup"><span data-stu-id="fcc04-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="fcc04-107">**[總和檢查碼：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，沒有任何總和檢查碼</span><span class="sxs-lookup"><span data-stu-id="fcc04-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="fcc04-108">**[定義：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP 原則就是有信心它已偵測到這種敏感資訊類型的 75 %if，300 個字元的距離：</span><span class="sxs-lookup"><span data-stu-id="fcc04-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="fcc04-109">函數 Func_usa_uk_passport 找到符合模式的內容。</span><span class="sxs-lookup"><span data-stu-id="fcc04-109">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="fcc04-110">找到來自於 Keyword_passport 的關鍵字。</span><span class="sxs-lookup"><span data-stu-id="fcc04-110">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="fcc04-111">例如，下列範例會觸發的**美國 / 英國護照號碼**原則： US 護照號碼 123456789</span><span class="sxs-lookup"><span data-stu-id="fcc04-111">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="fcc04-112">如需有關功能需要美國 / 英國護照號碼來偵測的內容，請參閱本文的下列章節：[什麼敏感資訊類型外觀如美國 / 英國護照號碼](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="fcc04-112">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="fcc04-113">使用不同的內建敏感資訊類型，請參閱上功能所需的其他類型的資訊的下列文章：[尋找什麼敏感資訊類型](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="fcc04-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

