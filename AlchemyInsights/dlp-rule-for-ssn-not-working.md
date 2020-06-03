---
title: SSN 無法運作的 DLP 規則
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507361"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="8732a-102">使用社交安全性號碼的 DLP 問題</span><span class="sxs-lookup"><span data-stu-id="8732a-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="8732a-103">**重要**：在這些前所未有的情況下，我們會採取下列步驟以確保 SharePoint Online 和 OneDrive 服務保持高度可用 – 請造訪 [SharePoint Online 暫時功能調整](https://aka.ms/ODSPAdjustments)以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="8732a-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="8732a-104">**主旨 ssn 的 DLP 問題**</span><span class="sxs-lookup"><span data-stu-id="8732a-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="8732a-105">當您在 Microsoft 365 中使用敏感資訊類型時，**資料遺失防護（DLP）** 未使用包含**社交安全性號碼（SSN）** 的內容時，是否發生問題？</span><span class="sxs-lookup"><span data-stu-id="8732a-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="8732a-106">如果是的話，請確定您的內容包含 DLP 原則所要的內容所需的資訊。</span><span class="sxs-lookup"><span data-stu-id="8732a-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="8732a-107">例如，對於設定置信級為85% 的 SSN 原則，會評估下列專案，而且必須偵測到要觸發的規則：</span><span class="sxs-lookup"><span data-stu-id="8732a-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="8732a-108">**[格式：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 位數（可能是格式化或未格式化的模式）</span><span class="sxs-lookup"><span data-stu-id="8732a-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="8732a-109">**[模式：](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 四種功能會在四種不同的模式中尋找主旨 ssn：</span><span class="sxs-lookup"><span data-stu-id="8732a-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="8732a-110">Func_ssn 會2011以主旨 ssn 的強格式格式化，並以短劃線或空格格式化（ddd-dd-dddd 或 ddd dd dddd）來尋找</span><span class="sxs-lookup"><span data-stu-id="8732a-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="8732a-111">Func_unformatted_ssn 會以預先2011的強格式格式化，以格式化為九個連續數位（ddddddddd）的主旨 ssn，來尋找</span><span class="sxs-lookup"><span data-stu-id="8732a-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="8732a-112">Func_randomized_formatted_ssn 會找到以短劃線或空格格式化的2011後主旨 ssn （ddd-dd-dddd 或 ddd dd dddd）</span><span class="sxs-lookup"><span data-stu-id="8732a-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="8732a-113">Func_randomized_unformatted_ssn 尋找未格式化為九個連續數位的2011後主旨 ssn （ddddddddd）</span><span class="sxs-lookup"><span data-stu-id="8732a-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="8732a-114">**[Checksum：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** 否，沒有檢查</span><span class="sxs-lookup"><span data-stu-id="8732a-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="8732a-115">**[定義：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** 如果接近300個字元以內，則 DLP 原則偵測到此敏感資訊類型的置信量是85%：</span><span class="sxs-lookup"><span data-stu-id="8732a-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="8732a-116">[函數 Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80)找到符合模式的內容。</span><span class="sxs-lookup"><span data-stu-id="8732a-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="8732a-117">會找到來自[Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn)的關鍵字。</span><span class="sxs-lookup"><span data-stu-id="8732a-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="8732a-118">關鍵字的範例包括：「*社會保險」、「社交安全性 #，Soc Sec，SSN* 。</span><span class="sxs-lookup"><span data-stu-id="8732a-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="8732a-119">例如，下列範例會觸發 DLP SSN 原則： **SSN： 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="8732a-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="8732a-120">如需針對您的內容偵測主旨 ssn 時所需的詳細資訊，請參閱本文的下列章節：[機密資訊類型針對主旨 ssn 的外觀](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)。</span><span class="sxs-lookup"><span data-stu-id="8732a-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="8732a-121">使用不同的內建機密資訊類型，請參閱下列文章，以瞭解其他類型所需的資訊：[機密資訊類型的外觀](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="8732a-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  