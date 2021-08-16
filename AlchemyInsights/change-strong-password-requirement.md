---
title: 變更強式密碼需求
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070675"
---
# <a name="change-strong-password-requirement"></a>變更強式密碼需求

Microsoft 預設會需要強密碼。

使用 PowerShell，您可以使用下列命令，針對特定使用者停用強式密碼：

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

若要對所有使用者停用強式密碼，請使用：

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [密碼原則的詳細資訊](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [如何使用 PowerShell 連接至 Microsoft 365](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [PowerShell Get-msoluser 命令的詳細資訊](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
