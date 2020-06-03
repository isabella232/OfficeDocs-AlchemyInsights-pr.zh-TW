---
title: 2419-無法啟用-審計
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510419"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="0f0f5-102">無法啟用整合的審計</span><span class="sxs-lookup"><span data-stu-id="0f0f5-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="0f0f5-103">當您嘗試為組織啟用整合的審計時，可能會收到類似下列的錯誤：</span><span class="sxs-lookup"><span data-stu-id="0f0f5-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="0f0f5-104">若要解決此問題，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="0f0f5-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="0f0f5-105">[連接至 Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)。</span><span class="sxs-lookup"><span data-stu-id="0f0f5-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="0f0f5-106">執行下列 Cmdlet：</span><span class="sxs-lookup"><span data-stu-id="0f0f5-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="0f0f5-107">請等候60分鐘，上一個設定才會生效。</span><span class="sxs-lookup"><span data-stu-id="0f0f5-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="0f0f5-108">在 Exchange Online 中執行下列命令 PowerShell:</span><span class="sxs-lookup"><span data-stu-id="0f0f5-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="0f0f5-109">如需詳細資訊，請參閱下列文章：</span><span class="sxs-lookup"><span data-stu-id="0f0f5-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="0f0f5-110">使用多重要素驗證連線至 Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="0f0f5-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="0f0f5-111">開啟或關閉稽核記錄搜尋</span><span class="sxs-lookup"><span data-stu-id="0f0f5-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
