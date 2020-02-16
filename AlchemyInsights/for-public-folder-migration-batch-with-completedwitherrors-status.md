---
title: CompletedWithErrors 狀態的公用資料夾移轉批次
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043571"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>CompletedWithErrors 狀態的公用資料夾移轉批次

使用下列步驟來完成的批次，略過的大型/錯誤項目： 
1. 核准遷移批次已略過的項目：

    Set-migrationbatch \<batchname>-ApproveSkippedItems 
2. 使用下列命令來核准略過的項目，在 「 同步處理 」 的移轉要求，但未完成：

    $pf = Get-publicfoldermailboxmigrationrequest |Get-publicfoldermailboxmigrationrequeststatistics IncludeReport;ForEach ($i 中 $pf) {如果 ($i.LargeItemsEncountered-gt 0-或 $i.BadItemsEncountered-gt 0) {組 PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid-SkippedItemApprovalTime $([日期時間]:: UtcNow)}}
3. 遷移批次要求應繼續並在幾分鐘內完成。

