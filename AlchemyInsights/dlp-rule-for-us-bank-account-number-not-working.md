---
title: 美國銀行帳戶號碼無法運作的 DLP 規則
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
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932506"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="1f96b-102">美國銀行帳戶號碼的 DLP 問題</span><span class="sxs-lookup"><span data-stu-id="1f96b-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="1f96b-103">**重要**：許多 SharePoint 線上及 OneDrive 客戶對在後臺執行的服務執行業務關鍵型應用程式。</span><span class="sxs-lookup"><span data-stu-id="1f96b-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="1f96b-104">包括內容遷移、資料遺失防護（DLP）及備份解決方案。</span><span class="sxs-lookup"><span data-stu-id="1f96b-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="1f96b-105">在這些空前的時間內，我們採取的步驟，確定在遠端工作案例中，線上和 OneDrive 服務的 SharePoint，都為您的使用者提供高可用性和更可靠的服務。</span><span class="sxs-lookup"><span data-stu-id="1f96b-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="1f96b-106">為了支援這專案標，我們已在星期幾的白天時段內，對背景應用程式（遷移、DLP 和備份解決方案）進行更為緊密的節流限制。</span><span class="sxs-lookup"><span data-stu-id="1f96b-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="1f96b-107">您應該會認為，這些應用程式在這段時間內可達到非常有限的輸送量。</span><span class="sxs-lookup"><span data-stu-id="1f96b-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="1f96b-108">不過，當地區的晚上和週末時，服務會準備好處理來自背景應用程式的大量要求。</span><span class="sxs-lookup"><span data-stu-id="1f96b-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="1f96b-109">**美國銀行帳戶號碼的 DLP 問題**</span><span class="sxs-lookup"><span data-stu-id="1f96b-109">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="1f96b-110">當您在 O365 中使用 DLP 敏感資訊類型時，**資料遺失防護（DLP）** 的內容無法使用包含**US 銀行帳號**的內容時，是否發生問題？</span><span class="sxs-lookup"><span data-stu-id="1f96b-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="1f96b-111">如果是的話，請確定您的內容中包含 DLP 原則在評估時所需的資訊。</span><span class="sxs-lookup"><span data-stu-id="1f96b-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="1f96b-112">例如，對於以信賴等級85% 設定的**US 銀行帳戶號碼**原則，會評估下列專案，而且必須偵測到要觸發的規則：</span><span class="sxs-lookup"><span data-stu-id="1f96b-112">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="1f96b-113">**[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 位數</span><span class="sxs-lookup"><span data-stu-id="1f96b-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="1f96b-114">**[Pattern：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 連續數位。</span><span class="sxs-lookup"><span data-stu-id="1f96b-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="1f96b-115">**[Checksum：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，沒有檢查</span><span class="sxs-lookup"><span data-stu-id="1f96b-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="1f96b-116">**[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** 如果接近300個字元以內，則 DLP 原則偵測到此敏感資訊類型的置信量是75%：</span><span class="sxs-lookup"><span data-stu-id="1f96b-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="1f96b-117">正則運算式 Regex_usa_bank_account_number 找到符合模式的內容。</span><span class="sxs-lookup"><span data-stu-id="1f96b-117">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="1f96b-118">會找到來自 Keyword_usa_Bank_Account 的關鍵字。</span><span class="sxs-lookup"><span data-stu-id="1f96b-118">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="1f96b-119">例如，下列範例會觸發**US 銀行帳戶號碼**原則：檢查帳戶78344011</span><span class="sxs-lookup"><span data-stu-id="1f96b-119">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="1f96b-120">如需針對您的內容偵測到**US 銀行帳戶**所需的資訊，請參閱本文中的下列章節：[機密資訊類型針對 US 銀行帳戶所尋找的功能](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)。</span><span class="sxs-lookup"><span data-stu-id="1f96b-120">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="1f96b-121">使用不同的內建機密資訊類型，請參閱下列文章，以瞭解其他類型所需的資訊：[機密資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="1f96b-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  