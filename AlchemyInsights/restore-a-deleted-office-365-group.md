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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597434"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>還原已刪除的 Microsoft 365 群組

您可以從刪除的30天內，還原已刪除的 Microsoft 365 群組或 Microsoft 團隊。

1. 移至 [Microsoft 365 系統管理中心](https://aka.ms/RestoreDeletedGroup) ，登入並列出已刪除的群組和團隊。

    **附注：** 使用指派給承租人管理員或群組管理員角色的帳戶登入。

1. 選取要還原的 [已刪除的 Microsoft 365 群組/小組]，然後按一下 [ **還原群組**]。

    若由於 SMTP 位址衝突而無法還原群組，請使用下列命令來找出導致衝突的物件，並移除 SMTP 位址：

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **附注：** 在某些情況下，您可能需要24小時的時間才能還原群組及其所有資料。

    如需詳細資訊，或若要瞭解如何使用 PowerShell 還原群組，請參閱 [還原已刪除的 Microsoft 365 群組](https://go.microsoft.com/fwlink/?linkid=867802)。