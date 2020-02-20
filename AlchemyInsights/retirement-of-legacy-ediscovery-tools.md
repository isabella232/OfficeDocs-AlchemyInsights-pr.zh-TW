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
# <a name="retirement-of-legacy-ediscovery-tools"></a>淘汰網站的舊版電子文件探索工具

在 Microsoft 365 合規性中心的新增和改善 eDiscovery 功能，因為下列舊版電子文件探索工具和 commandlets 即將停用在接下來的月份中：

- [就地 eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)和[就地保留](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)在 Exchange 系統管理中心。

- 支援就地 eDiscovery 和就地保留 Exchange Online PowerShell cmdlet。 (這些 cmdlet 統稱會被識別為 *-MailboxSearch cmdlet。)這包括下列 cmdlet:

    - [新 MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-mailboxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- 在 Exchange Online PowerShell [Search-mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps)指令程式。
- Exchange Web Services API 中的下列作業：
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Office 365 進階電子文件 v1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**退休時間表**：
- 2020 年 4 月 1： 您無法建立新的搜尋及保留，但您可以仍執行、 編輯和刪除現有的搜尋自行承擔風險。 Microsoft 支援服務將沒有較長的支援就地 eDiscovery & 保留在 EAC 中。

- 2020 年 7 月 1： 在 EAC 中的就地 eDiscovery & 保留功能將會處於唯讀模式。 這表示您只可以移除現有的搜尋並保留。

**如需詳細資訊，請參閱**：

 - [移轉舊版的 eDiscovery 搜尋，並保留至 Microsoft 365 合規性中心](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [淘汰網站的舊版電子文件探索工具](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [就地 eDiscovery 和就地保留相關的常見問題集](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



