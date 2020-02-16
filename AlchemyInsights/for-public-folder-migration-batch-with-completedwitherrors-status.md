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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="adf62-102">CompletedWithErrors 狀態的公用資料夾移轉批次</span><span class="sxs-lookup"><span data-stu-id="adf62-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="adf62-103">使用下列步驟來完成的批次，略過的大型/錯誤項目：</span><span class="sxs-lookup"><span data-stu-id="adf62-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="adf62-104">核准遷移批次已略過的項目：</span><span class="sxs-lookup"><span data-stu-id="adf62-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="adf62-105">Set-migrationbatch \<batchname>-ApproveSkippedItems</span><span class="sxs-lookup"><span data-stu-id="adf62-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="adf62-106">使用下列命令來核准略過的項目，在 「 同步處理 」 的移轉要求，但未完成：</span><span class="sxs-lookup"><span data-stu-id="adf62-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="adf62-107">$pf = Get-publicfoldermailboxmigrationrequest |Get-publicfoldermailboxmigrationrequeststatistics IncludeReport;ForEach ($i 中 $pf) {如果 ($i.LargeItemsEncountered-gt 0-或 $i.BadItemsEncountered-gt 0) {組 PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid-SkippedItemApprovalTime $([日期時間]:: UtcNow)}}</span><span class="sxs-lookup"><span data-stu-id="adf62-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="adf62-108">遷移批次要求應繼續並在幾分鐘內完成。</span><span class="sxs-lookup"><span data-stu-id="adf62-108">The migration batch and requests should resume and complete in a few minutes.</span></span>

