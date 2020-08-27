---
title: 公用資料夾在進度 95% 時移轉失敗
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: fc8da45d91d5c32be52e48770e469cf25eb068f5
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903536"
---
# <a name="public-folder-migration-fails-at-95"></a>公用資料夾在進度 95% 時移轉失敗

公用資料夾在進度 95% 時移轉失敗，且錯誤為 FailedToMailEnablePublicFoldersException：

1. 在 Exchange 內部部署伺服器上下載並執行 [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) 指令碼。

2. 執行指令碼所建議的修正動作。

3. 執行 Sync-MailPublicFolders (若為 Exchange 2010) 或 Sync-ModernMailPublicFolders (若為 Exchange 2013 及更新版本)。

4. 繼續公用資料夾移轉。
