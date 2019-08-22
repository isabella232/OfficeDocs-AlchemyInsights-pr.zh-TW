---
title: 變更強式密碼需求
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: f8790a26ec7c5de57f5dbfc9e1c162767c599f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36518750"
---
# <a name="change-strong-password-requirement"></a>變更強式密碼需求

根據預設，Microsoft 會要求強式密碼。 

使用 PowerShell，您可以停用特定使用者使用此命令的強式的密碼：<br>
*Set-msoluser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [在 [密碼原則的詳細資訊](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [如何連線到 Office 365 powershell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [在 PowerShell MsolUser 命令的詳細資訊](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)