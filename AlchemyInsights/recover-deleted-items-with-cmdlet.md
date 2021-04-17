---
title: 使用 Cmdlet 復原刪除的郵件
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835802"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="6de23-102">使用 Cmdlet 復原刪除的郵件</span><span class="sxs-lookup"><span data-stu-id="6de23-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="6de23-103">使用 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) Cmdlet 來檢視信箱中已刪除的郵件。</span><span class="sxs-lookup"><span data-stu-id="6de23-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="6de23-104">找到已刪除的郵件之後，您可以使用 [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) Cmdlet 來還原它們。</span><span class="sxs-lookup"><span data-stu-id="6de23-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="6de23-105">請參閱 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) 中的完整詳細資料。</span><span class="sxs-lookup"><span data-stu-id="6de23-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="6de23-106">您必須先獲指派「信箱匯入匯出」角色，才能執行此 Cmdlet。</span><span class="sxs-lookup"><span data-stu-id="6de23-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="6de23-107">如需詳細資訊，請參閱 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="6de23-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
