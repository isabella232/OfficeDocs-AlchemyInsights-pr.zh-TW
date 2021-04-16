---
title: 舊的 eDiscovery 工具退休
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798540"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="5d657-102">舊的 eDiscovery 工具退休</span><span class="sxs-lookup"><span data-stu-id="5d657-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="5d657-103">由於 Microsoft 365 規範中心的新的和改良的 eDiscovery 功能的結果，下列舊的 eDiscovery 工具和 commandlets 將在未來的幾個月內淘汰：</span><span class="sxs-lookup"><span data-stu-id="5d657-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="5d657-104">在 Exchange 系統管理中心中[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)和[In-Place 存放](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)。</span><span class="sxs-lookup"><span data-stu-id="5d657-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="5d657-105">支援 In-Place eDiscovery 和 In-Place 保留的 Exchange Online PowerShell Cmdlet。</span><span class="sxs-lookup"><span data-stu-id="5d657-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="5d657-106"> (這些 Cmdlet 會共同識別成\ *-MailboxSearch Cmdlet。 ) 這包括下列 Cmdlet：</span><span class="sxs-lookup"><span data-stu-id="5d657-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="5d657-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="5d657-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="5d657-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="5d657-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="5d657-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="5d657-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="5d657-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="5d657-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="5d657-111">Exchange Online PowerShell 中的 [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) Cmdlet。</span><span class="sxs-lookup"><span data-stu-id="5d657-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="5d657-112">Exchange Web 服務 API 中的下列作業：</span><span class="sxs-lookup"><span data-stu-id="5d657-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="5d657-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="5d657-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="5d657-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="5d657-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="5d657-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="5d657-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="5d657-116">Advanced eDiscovery v 1。0</span><span class="sxs-lookup"><span data-stu-id="5d657-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="5d657-117">**退休的時程表**：</span><span class="sxs-lookup"><span data-stu-id="5d657-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="5d657-118">**2020 年7月1日** 您無法再建立新的搜尋和保留，但是您可以自行承擔執行、編輯和刪除現有的搜尋。</span><span class="sxs-lookup"><span data-stu-id="5d657-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="5d657-119">Microsoft 支援不再支援 EAC 中 In-Place eDiscovery & 保留。</span><span class="sxs-lookup"><span data-stu-id="5d657-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="5d657-120">**2020 年10月1日** In-Place EDiscovery & 保留 EAC 中的功能將處於唯讀模式，因此您只能移除現有的搜尋和保留。</span><span class="sxs-lookup"><span data-stu-id="5d657-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="5d657-121">**如需詳細資訊，請參閱**：</span><span class="sxs-lookup"><span data-stu-id="5d657-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="5d657-122">將舊版 eDiscovery 搜尋和保留遷移至 Microsoft 365 規範中心</span><span class="sxs-lookup"><span data-stu-id="5d657-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="5d657-123">舊版電子文件探索工具淘汰</span><span class="sxs-lookup"><span data-stu-id="5d657-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="5d657-124">有關 In-Place eDiscovery 和 In-Place 保留的 FAQs</span><span class="sxs-lookup"><span data-stu-id="5d657-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



