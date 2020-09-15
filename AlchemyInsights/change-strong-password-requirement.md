---
title: 變更強式密碼需求
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: d888f4a208ccbc6f54469f5e1eb88f9f4197e5c9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47681863"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="e2144-102">變更強式密碼需求</span><span class="sxs-lookup"><span data-stu-id="e2144-102">Change strong password requirement</span></span>

<span data-ttu-id="e2144-103">Microsoft 預設會需要強密碼。</span><span class="sxs-lookup"><span data-stu-id="e2144-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="e2144-104">使用 PowerShell，您可以使用此命令，針對特定使用者停用強式密碼：</span><span class="sxs-lookup"><span data-stu-id="e2144-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="e2144-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="e2144-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="e2144-106">密碼原則的詳細資訊</span><span class="sxs-lookup"><span data-stu-id="e2144-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="e2144-107">如何使用 PowerShell 連接至 Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e2144-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="e2144-108">PowerShell Get-msoluser 命令的詳細資訊</span><span class="sxs-lookup"><span data-stu-id="e2144-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
