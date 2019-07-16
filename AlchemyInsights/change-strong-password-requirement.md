---
title: 變更強式密碼需求
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 53affd2a347c004e7b21b353c2b3df98bc30a585
ms.sourcegitcommit: a7e5ca472000dfec471950bafd12eee8d7144f74
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/16/2019
ms.locfileid: "35701575"
---
# <a name="change-strong-password-requirement"></a>變更強式密碼需求

強式密碼所需的預設值。 

使用 PowerShell 您可以停用特定使用者使用此命令的強式的密碼：<br>
*Set-msoluser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [在 [密碼原則的詳細資訊](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [如何連接至 O365 使用 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [在 PowerShell MsolUser 命令的詳細資訊](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)