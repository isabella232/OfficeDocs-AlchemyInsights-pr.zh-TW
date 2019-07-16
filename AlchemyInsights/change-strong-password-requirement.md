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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="4dcd7-102">變更強式密碼需求</span><span class="sxs-lookup"><span data-stu-id="4dcd7-102">Change strong password requirement</span></span>

<span data-ttu-id="4dcd7-103">強式密碼所需的預設值。</span><span class="sxs-lookup"><span data-stu-id="4dcd7-103">Strong passwords are required by default.</span></span> 

<span data-ttu-id="4dcd7-104">使用 PowerShell 您可以停用特定使用者使用此命令的強式的密碼：</span><span class="sxs-lookup"><span data-stu-id="4dcd7-104">Using PowerShell you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="4dcd7-105">*Set-msoluser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="4dcd7-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- <span data-ttu-id="4dcd7-106">[在 [密碼原則的詳細資訊](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="4dcd7-106">[More information on password policy](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- [<span data-ttu-id="4dcd7-107">如何連接至 O365 使用 PowerShell</span><span class="sxs-lookup"><span data-stu-id="4dcd7-107">How to connect to O365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="4dcd7-108">在 PowerShell MsolUser 命令的詳細資訊</span><span class="sxs-lookup"><span data-stu-id="4dcd7-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)