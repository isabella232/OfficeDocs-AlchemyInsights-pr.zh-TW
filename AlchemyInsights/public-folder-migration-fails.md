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
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="5442f-102">公用資料夾在進度 95% 時移轉失敗</span><span class="sxs-lookup"><span data-stu-id="5442f-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="5442f-103">您可能已開始完成遷移批次，而且遷移批次的狀態會持續顯示**已同步**一段時間。</span><span class="sxs-lookup"><span data-stu-id="5442f-103">You might have initiated completion of a migration batch, and the status of the migration batch continues showing **Synced** for a very long time.</span></span> <span data-ttu-id="5442f-104">這是預期的行為。</span><span class="sxs-lookup"><span data-stu-id="5442f-104">This is expected behavior.</span></span>

<span data-ttu-id="5442f-105">通常轉移批次的狀態會保持**已同步**幾小時，再切換至**正在完成**。</span><span class="sxs-lookup"><span data-stu-id="5442f-105">It's common for the status of a migration batch to remain on **Synced** for a few hours before it switches to **Completing**.</span></span> <span data-ttu-id="5442f-106">如果涉及大量目標信箱的遷移作業，只要沒有基本的公用資料夾遷移要求失敗或遭到隔離，通常情況下狀態會保持已同步超過 24 小時。</span><span class="sxs-lookup"><span data-stu-id="5442f-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="5442f-107">請為遷移批次作業提供 24 至 48 小時來完成工作。</span><span class="sxs-lookup"><span data-stu-id="5442f-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

<span data-ttu-id="5442f-108">公用資料夾在進度 95% 時移轉失敗，且錯誤為 FailedToMailEnablePublicFoldersException：</span><span class="sxs-lookup"><span data-stu-id="5442f-108">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="5442f-109">在 Exchange 內部部署伺服器上下載並執行 [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) 指令碼。</span><span class="sxs-lookup"><span data-stu-id="5442f-109">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="5442f-110">執行指令碼所建議的修正動作。</span><span class="sxs-lookup"><span data-stu-id="5442f-110">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="5442f-111">執行 Sync-MailPublicFolders (若為 Exchange 2010) 或 Sync-ModernMailPublicFolders (若為 Exchange 2013 及更新版本)。</span><span class="sxs-lookup"><span data-stu-id="5442f-111">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="5442f-112">繼續公用資料夾移轉。</span><span class="sxs-lookup"><span data-stu-id="5442f-112">Resume public folder migration.</span></span>
