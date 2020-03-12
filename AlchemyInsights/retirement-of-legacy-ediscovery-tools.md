---
title: 舊的 eDiscovery 工具退休
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
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600351"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>舊的 eDiscovery 工具退休

由於 Microsoft 365 規範中心的新的和改良的 eDiscovery 功能的結果，下列舊的 eDiscovery 工具和 commandlets 將在未來的幾個月內淘汰：

- 在 Exchange 系統管理中心中[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)和[In-Place 存放](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)。

- 支援 In-Place eDiscovery 和 In-Place 保留的 Exchange Online PowerShell Cmdlet。 （這些 Cmdlet 共同識別為 *-MailboxSearch Cmdlet。）這包括下列 Cmdlet：

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Exchange Online PowerShell 中的[Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) Cmdlet。
- Exchange Web 服務 API 中的下列作業：
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 Advanced eDiscovery 1.0 版](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**退休的時程表**：
- 2020年4月1日：您將無法建立新的搜尋和保留，但是您仍然可以自行承擔執行、編輯和刪除現有的搜尋。 Microsoft 支援將不再支援 EAC 中 In-Place eDiscovery & 保留。

- 2020年7月1日： In-Place eDiscovery & 保留 EAC 中的功能將會置於唯讀模式。 這表示您只可以移除現有的搜尋和保留。

**如需詳細資訊，請參閱**：

 - [將舊版 eDiscovery 搜尋和保留遷移至 Microsoft 365 規範中心](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [舊的 eDiscovery 工具退休](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [有關 In-Place eDiscovery 和 In-Place 保留的 FAQs](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



