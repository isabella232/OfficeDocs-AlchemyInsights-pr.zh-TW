---
title: 適用于美國/英國護照號碼的 DLP 規則未運作
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
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977097"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="dab7b-102">DLP-US/英國護照號碼的問題</span><span class="sxs-lookup"><span data-stu-id="dab7b-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="dab7b-103">**重要**事項：在這些空前的時間內，我們採取步驟來確保 SharePoint 線上和 OneDrive 服務保持高可用性–請流覽[SharePoint 線上暫存功能](https://aka.ms/ODSPAdjustments)，以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="dab7b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="dab7b-104">**美國/英國護照號碼的 DLP 問題**</span><span class="sxs-lookup"><span data-stu-id="dab7b-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="dab7b-105">當您在 O365 使用 DLP 敏感資訊類型時，**資料遺失防護（DLP）** 未使用包含**美國/英國護照號碼**的內容時，是否發生問題？</span><span class="sxs-lookup"><span data-stu-id="dab7b-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="dab7b-106">如果是的話，請確定您的內容中包含 DLP 原則在評估時所需的資訊。</span><span class="sxs-lookup"><span data-stu-id="dab7b-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="dab7b-107">例如，對於設定為信賴等級為75% 的**美國/英國護照號碼**原則，會評估下列各項，而且必須偵測到規則才能觸發</span><span class="sxs-lookup"><span data-stu-id="dab7b-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="dab7b-108">**[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 九位數</span><span class="sxs-lookup"><span data-stu-id="dab7b-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="dab7b-109">**[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 九個連續數位</span><span class="sxs-lookup"><span data-stu-id="dab7b-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="dab7b-110">**[Checksum：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，沒有檢查</span><span class="sxs-lookup"><span data-stu-id="dab7b-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="dab7b-111">**[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** 如果接近300個字元以內，則 DLP 原則偵測到此敏感資訊類型的置信量是75%：</span><span class="sxs-lookup"><span data-stu-id="dab7b-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="dab7b-112">函數 Func_usa_uk_passport 找到符合模式的內容。</span><span class="sxs-lookup"><span data-stu-id="dab7b-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="dab7b-113">會找到來自 Keyword_passport 的關鍵字。</span><span class="sxs-lookup"><span data-stu-id="dab7b-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="dab7b-114">例如，下列範例會觸發**美國/英國護照號碼**原則：美國護照號碼123456789</span><span class="sxs-lookup"><span data-stu-id="dab7b-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="dab7b-115">如需針對您的內容偵測 US/英國護照號碼時所需的詳細資訊，請參閱本文的下列章節：[機密資訊類型針對美國/英國護照號碼所尋找的功能](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)。</span><span class="sxs-lookup"><span data-stu-id="dab7b-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="dab7b-116">使用不同的內建機密資訊類型，請參閱下列文章，以瞭解其他類型所需的資訊：[機密資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="dab7b-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  