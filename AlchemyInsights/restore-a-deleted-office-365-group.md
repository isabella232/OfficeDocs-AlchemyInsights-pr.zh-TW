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
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959017"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>還原已刪除的 Microsoft 365 群組

您可以從刪除的30天內，還原已刪除的 Microsoft 365 群組或 Microsoft Teams。

1. 移至 [ [Microsoft 365 系統管理中心](https://aka.ms/RestoreDeletedGroup)]，登入您已刪除之群組和小組的清單。

    **附注：** 使用指派給承租人管理員或群組管理員角色的帳戶登入。

1. 選取要還原的已刪除 Microsoft 365 group/Teams，然後按一下 [**還原群組**]。

    若由於 SMTP 位址衝突而無法還原群組，請使用下列命令來找出導致衝突的物件，並移除 SMTP 位址：

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **附注：** 在某些情況下，您可能需要24小時的時間才能還原群組及其所有資料。

    如需詳細資訊，或若要瞭解如何使用 PowerShell 還原群組，請參閱[還原已刪除的 Microsoft 365 群組](https://go.microsoft.com/fwlink/?linkid=867802)。