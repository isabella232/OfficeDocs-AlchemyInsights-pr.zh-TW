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
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="24ad1-102">無法啟用整合審計</span><span class="sxs-lookup"><span data-stu-id="24ad1-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="24ad1-103">當您嘗試為您的 Office 365 組織啟用整合的審計時, 可能會收到類似下列的錯誤:</span><span class="sxs-lookup"><span data-stu-id="24ad1-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="24ad1-104">若要解決此問題, 請遵循下列步驟:</span><span class="sxs-lookup"><span data-stu-id="24ad1-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="24ad1-105">[連線至 Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)。</span><span class="sxs-lookup"><span data-stu-id="24ad1-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="24ad1-106">執行下列 Cmdlet：</span><span class="sxs-lookup"><span data-stu-id="24ad1-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="24ad1-107">請等候60分鐘, 讓先前的設定生效。</span><span class="sxs-lookup"><span data-stu-id="24ad1-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="24ad1-108">在 Exchange Online PowerShell 中執行下列命令:</span><span class="sxs-lookup"><span data-stu-id="24ad1-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="24ad1-109">如需其他資訊, 請參閱下列文章:</span><span class="sxs-lookup"><span data-stu-id="24ad1-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="24ad1-110">使用多重要素驗證連線至 Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="24ad1-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="24ad1-111">開啟或關閉 Office 365 稽核記錄搜尋</span><span class="sxs-lookup"><span data-stu-id="24ad1-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
