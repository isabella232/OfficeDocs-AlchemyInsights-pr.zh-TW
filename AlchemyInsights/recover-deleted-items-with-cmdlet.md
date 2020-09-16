---
title: 使用 Cmdlet 復原刪除的郵件
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
- "1800008"
- "5718"
ms.openlocfilehash: 91a9bcf75b13881b903a1d3b6f2da53f65811c9c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741294"
---
# <a name="recover-deleted-items-with-cmdlet"></a>使用 Cmdlet 復原刪除的郵件

- 使用 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) Cmdlet 來檢視信箱中已刪除的郵件。 找到已刪除的郵件之後，您可以使用 [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) Cmdlet 來還原它們。

- 請參閱 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) 中的完整詳細資料。

- 您必須先獲指派「信箱匯入匯出」角色，才能執行此 Cmdlet。 如需詳細資訊，請參閱 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)。
