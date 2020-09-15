---
title: 公用資料夾在進度 95% 時移轉失敗
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662420"
---
# <a name="public-folder-migration-fails-at-95"></a>公用資料夾在進度 95% 時移轉失敗

您可能已開始完成遷移批次，而且遷移批次的狀態會持續顯示**已同步**一段時間。 這是預期的行為。

通常轉移批次的狀態會保持**已同步**幾小時，再切換至**正在完成**。 如果涉及大量目標信箱的遷移作業，只要沒有基本的公用資料夾遷移要求失敗或遭到隔離，通常情況下狀態會保持已同步超過 24 小時。 請為遷移批次作業提供 24 至 48 小時來完成工作。

公用資料夾在進度 95% 時移轉失敗，且錯誤為 FailedToMailEnablePublicFoldersException：

1. 在 Exchange 內部部署伺服器上下載並執行 [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) 指令碼。

2. 執行指令碼所建議的修正動作。

3. 執行 Sync-MailPublicFolders (若為 Exchange 2010) 或 Sync-ModernMailPublicFolders (若為 Exchange 2013 及更新版本)。

4. 繼續公用資料夾移轉。
