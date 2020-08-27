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
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="08524-102">公用資料夾在進度 95% 時移轉失敗</span><span class="sxs-lookup"><span data-stu-id="08524-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="08524-103">公用資料夾在進度 95% 時移轉失敗，且錯誤為 FailedToMailEnablePublicFoldersException：</span><span class="sxs-lookup"><span data-stu-id="08524-103">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="08524-104">在 Exchange 內部部署伺服器上下載並執行 [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) 指令碼。</span><span class="sxs-lookup"><span data-stu-id="08524-104">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="08524-105">執行指令碼所建議的修正動作。</span><span class="sxs-lookup"><span data-stu-id="08524-105">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="08524-106">執行 Sync-MailPublicFolders (若為 Exchange 2010) 或 Sync-ModernMailPublicFolders (若為 Exchange 2013 及更新版本)。</span><span class="sxs-lookup"><span data-stu-id="08524-106">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="08524-107">繼續公用資料夾移轉。</span><span class="sxs-lookup"><span data-stu-id="08524-107">Resume public folder migration.</span></span>
