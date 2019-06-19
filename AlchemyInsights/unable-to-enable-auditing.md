---
title: 2419-無法啟用-審計
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065609"
---
# <a name="unable-to-enable-unified-auditing"></a>無法啟用整合審計

當您嘗試為您的 Office 365 組織啟用整合的審計時, 可能會收到類似下列的錯誤:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

若要解決此問題, 請遵循下列步驟:

1. [連線至 Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)。

2. 執行下列 Cmdlet：

   ```
   Enable-OrganizationCustomization
   ```

3. 請等候60分鐘, 讓先前的設定生效。

4. 在 Exchange Online PowerShell 中執行下列命令:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

如需其他資訊, 請參閱下列文章:

- [使用多重要素驗證連線至 Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [開啟或關閉 Office 365 稽核記錄搜尋](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
