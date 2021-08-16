---
title: 針對具有 CompletedWithErrors 狀態的公用資料夾遷移批次
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
- "3500007"
- "3532"
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068155"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>針對具有 CompletedWithErrors 狀態的公用資料夾遷移批次

使用下列步驟完成批次，並略過大型/壞專案： 
1. 核准遷移批次中略過的專案：

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. 使用下列命令來核准已「同步處理」但未完成之遷移要求上略過的專案：

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. 在幾分鐘內，遷移批次和要求應該會繼續並完成。

