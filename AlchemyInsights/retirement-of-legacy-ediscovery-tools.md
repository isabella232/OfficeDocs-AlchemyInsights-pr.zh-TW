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
# <a name="retirement-of-legacy-ediscovery-tools"></a>舊的 eDiscovery 工具退休

由於 Microsoft 365 規範中心的新的和改良的 eDiscovery 功能的結果，下列舊的 eDiscovery 工具和 commandlets 將在未來的幾個月內淘汰：

- 在 Exchange 系統管理中心中[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)和[In-Place 存放](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)。

- 支援 In-Place eDiscovery 和 In-Place 保留的 Exchange Online PowerShell Cmdlet。  (這些 Cmdlet 會共同識別成 *-MailboxSearch Cmdlet。 ) 這包括下列 Cmdlet：

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Exchange Online PowerShell 中的 [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) Cmdlet。
- Exchange Web 服務 API 中的下列作業：
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v 1。0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**退休的時程表**：
- **2020 年7月1日** 您無法再建立新的搜尋和保留，但是您可以自行承擔執行、編輯和刪除現有的搜尋。 Microsoft 支援不再支援 EAC 中 In-Place eDiscovery & 保留。
    
- **2020 年10月1日** In-Place EDiscovery & 保留 EAC 中的功能將處於唯讀模式，因此您只能移除現有的搜尋和保留。

**如需詳細資訊，請參閱**：

 - [將舊版 eDiscovery 搜尋和保留遷移至 Microsoft 365 規範中心](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [舊版電子文件探索工具淘汰](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [有關 In-Place eDiscovery 和 In-Place 保留的 FAQs](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



