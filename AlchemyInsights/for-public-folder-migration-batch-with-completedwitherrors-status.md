---
title: 針對具有 CompletedWithErrors 狀態的公用資料夾遷移批次
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744104"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="043d0-102">針對具有 CompletedWithErrors 狀態的公用資料夾遷移批次</span><span class="sxs-lookup"><span data-stu-id="043d0-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="043d0-103">使用下列步驟完成批次，並略過大型/壞專案：</span><span class="sxs-lookup"><span data-stu-id="043d0-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="043d0-104">核准遷移批次中略過的專案：</span><span class="sxs-lookup"><span data-stu-id="043d0-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="043d0-105">使用下列命令來核准已「同步處理」但未完成之遷移要求上略過的專案：</span><span class="sxs-lookup"><span data-stu-id="043d0-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="043d0-106">在幾分鐘內，遷移批次和要求應該會繼續並完成。</span><span class="sxs-lookup"><span data-stu-id="043d0-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

