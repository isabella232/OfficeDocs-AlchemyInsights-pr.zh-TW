---
title: 變更 EWS 節流設定
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075888"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="e4e02-102">變更 EWS 節流設定</span><span class="sxs-lookup"><span data-stu-id="e4e02-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="e4e02-103">請執行我們的自動測試，讓您在移轉期間修改 EWS 節流原則。</span><span class="sxs-lookup"><span data-stu-id="e4e02-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="e4e02-104">請注意，即使在執行這項作業之後，EWS 匯入仍會限制為每個信箱 150MB，每 5 分鐘一次；若要達到更高的移轉輸送速度，請同時移轉更多使用者。</span><span class="sxs-lookup"><span data-stu-id="e4e02-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="e4e02-105">請注意，EWS 節流原則變更對下列移轉類型 (使用 Microsoft 工具) 沒有任何影響：混合式、完全移轉/分段 (RPC/HTTP)、IMAP、G Suite、公用資料夾或 PST 匯入服務。</span><span class="sxs-lookup"><span data-stu-id="e4e02-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>