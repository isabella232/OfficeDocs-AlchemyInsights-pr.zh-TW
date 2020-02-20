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
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158589"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="a5054-102">CompletedWithErrors 狀態的公用資料夾移轉批次</span><span class="sxs-lookup"><span data-stu-id="a5054-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="a5054-103">使用下列步驟來完成的批次，略過的大型/錯誤項目：</span><span class="sxs-lookup"><span data-stu-id="a5054-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="a5054-104">核准遷移批次已略過的項目：</span><span class="sxs-lookup"><span data-stu-id="a5054-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="a5054-105">使用下列命令來核准略過的項目，在 「 同步處理 」 的移轉要求，但未完成：</span><span class="sxs-lookup"><span data-stu-id="a5054-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="a5054-106">遷移批次要求應繼續並在幾分鐘內完成。</span><span class="sxs-lookup"><span data-stu-id="a5054-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

