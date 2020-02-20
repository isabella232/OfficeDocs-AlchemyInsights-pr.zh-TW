---
title: 淘汰網站的舊版電子文件探索工具
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157524"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="e7165-102">淘汰網站的舊版電子文件探索工具</span><span class="sxs-lookup"><span data-stu-id="e7165-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="e7165-103">在 Microsoft 365 合規性中心的新增和改善 eDiscovery 功能，因為下列舊版電子文件探索工具和 commandlets 即將停用在接下來的月份中：</span><span class="sxs-lookup"><span data-stu-id="e7165-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="e7165-104">[就地 eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)和[就地保留](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)在 Exchange 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="e7165-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="e7165-105">支援就地 eDiscovery 和就地保留 Exchange Online PowerShell cmdlet。</span><span class="sxs-lookup"><span data-stu-id="e7165-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="e7165-106">(這些 cmdlet 統稱會被識別為 \*-MailboxSearch cmdlet。)這包括下列 cmdlet:</span><span class="sxs-lookup"><span data-stu-id="e7165-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="e7165-107">新 MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="e7165-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="e7165-108">Start-mailboxsearch</span><span class="sxs-lookup"><span data-stu-id="e7165-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="e7165-109">Stop-mailboxsearch</span><span class="sxs-lookup"><span data-stu-id="e7165-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="e7165-110">Set-mailboxsearch</span><span class="sxs-lookup"><span data-stu-id="e7165-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="e7165-111">在 Exchange Online PowerShell [Search-mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps)指令程式。</span><span class="sxs-lookup"><span data-stu-id="e7165-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="e7165-112">Exchange Web Services API 中的下列作業：</span><span class="sxs-lookup"><span data-stu-id="e7165-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="e7165-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="e7165-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="e7165-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="e7165-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="e7165-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="e7165-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="e7165-116">Office 365 進階電子文件 v1.0</span><span class="sxs-lookup"><span data-stu-id="e7165-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="e7165-117">**退休時間表**：</span><span class="sxs-lookup"><span data-stu-id="e7165-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="e7165-118">2020 年 4 月 1： 您無法建立新的搜尋及保留，但您可以仍執行、 編輯和刪除現有的搜尋自行承擔風險。</span><span class="sxs-lookup"><span data-stu-id="e7165-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="e7165-119">Microsoft 支援服務將沒有較長的支援就地 eDiscovery & 保留在 EAC 中。</span><span class="sxs-lookup"><span data-stu-id="e7165-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="e7165-120">2020 年 7 月 1： 在 EAC 中的就地 eDiscovery & 保留功能將會處於唯讀模式。</span><span class="sxs-lookup"><span data-stu-id="e7165-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="e7165-121">這表示您只可以移除現有的搜尋並保留。</span><span class="sxs-lookup"><span data-stu-id="e7165-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="e7165-122">**如需詳細資訊，請參閱**：</span><span class="sxs-lookup"><span data-stu-id="e7165-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="e7165-123">移轉舊版的 eDiscovery 搜尋，並保留至 Microsoft 365 合規性中心</span><span class="sxs-lookup"><span data-stu-id="e7165-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="e7165-124">淘汰網站的舊版電子文件探索工具</span><span class="sxs-lookup"><span data-stu-id="e7165-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="e7165-125">就地 eDiscovery 和就地保留相關的常見問題集</span><span class="sxs-lookup"><span data-stu-id="e7165-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



