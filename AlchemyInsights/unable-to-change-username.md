---
title: 無法變更使用者名稱
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 76891b3abe156b736c3bb6da0f6cd1135346dbe2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798655"
---
# <a name="unable-to-change-username"></a>無法變更使用者名稱

在某些情況下，UPN (UserPrincipalName) 變更不會傳播至雲端。 您可能會在 Office 365 入口網站收到驗證錯誤，或無法變更使用者名稱或電子郵件地址。 若要解決此問題，請使用此 PowerShell 命令手動設定 UserPrincipalName。

**範例：重新命名使用者**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

此命令會將 davidc@contoso.com 重新命名為 davidchew@contoso.com。

如需詳細資訊，請參閱 [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0) (英文)。