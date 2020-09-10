---
title: 公用資料夾移轉批次未完成，顯示已同步
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
ms.openlocfilehash: 7a87d8dafae2b0f3ff3f4e1ecdb6e02d73e9caf2
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406550"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="17b71-102">公用資料夾移轉批次未完成，顯示已同步</span><span class="sxs-lookup"><span data-stu-id="17b71-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="17b71-103">您可能已開始完成移轉批次，而且移轉批次的狀態會持續顯示為 [已同步] 一段時間。</span><span class="sxs-lookup"><span data-stu-id="17b71-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="17b71-104">這是預期的行為。</span><span class="sxs-lookup"><span data-stu-id="17b71-104">This is expected behavior.</span></span>

<span data-ttu-id="17b71-105">通常移轉批次的狀態會保持 [已同步] 幾小時，才切換為 [正在完成]。</span><span class="sxs-lookup"><span data-stu-id="17b71-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="17b71-106">如果涉及大量目標信箱的移轉作業，只要沒有基本的公用資料夾移轉要求失敗或遭到隔離，通常情況下狀態會保持 [已同步] 24 小時以上。</span><span class="sxs-lookup"><span data-stu-id="17b71-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="17b71-107">請為移轉批次作業提供 24 至 48 小時來完成工作。</span><span class="sxs-lookup"><span data-stu-id="17b71-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>
