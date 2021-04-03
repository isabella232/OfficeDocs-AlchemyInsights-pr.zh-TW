---
title: 還原已刪除的 Microsoft 365 群組
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505673"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>還原已刪除的 Microsoft 365 群組

您可以從刪除的30天內，還原已刪除的 Microsoft 365 群組或 Microsoft 團隊。

1. 若要登入 Microsoft 365 系統管理中心，並列出已刪除的群組和小組，請移至 [Microsoft 365 系統管理中心](https://aka.ms/RestoreDeletedGroup)。

    **附注：** 使用指派給承租人管理員或群組管理員角色的帳戶登入。

1. 選取要還原的 [已刪除的 Microsoft 365 群組/小組]，然後按一下 [ **還原群組**]。

    若由於 SMTP 位址衝突而無法還原群組，請使用下列命令來找出導致衝突的物件，並移除 SMTP 位址：

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **附注：** 在某些情況下，您可能需要24小時的時間才能還原群組及其所有資料。

    如需詳細資訊，或若要瞭解如何使用 PowerShell 還原群組，請參閱 [還原已刪除的 Microsoft 365 群組](https://go.microsoft.com/fwlink/?linkid=867802)。