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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="421e0-102">變更強式密碼需求</span><span class="sxs-lookup"><span data-stu-id="421e0-102">Change strong password requirement</span></span>

<span data-ttu-id="421e0-103">根據預設，Microsoft 會要求強式密碼。</span><span class="sxs-lookup"><span data-stu-id="421e0-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="421e0-104">使用 PowerShell，您可以停用特定使用者使用此命令的強式的密碼：</span><span class="sxs-lookup"><span data-stu-id="421e0-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="421e0-105">*Set-msoluser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="421e0-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- <span data-ttu-id="421e0-106">[在 [密碼原則的詳細資訊](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="421e0-106">[More information on password policy](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- [<span data-ttu-id="421e0-107">如何連線到 Office 365 powershell</span><span class="sxs-lookup"><span data-stu-id="421e0-107">How to connect to Office 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="421e0-108">在 PowerShell MsolUser 命令的詳細資訊</span><span class="sxs-lookup"><span data-stu-id="421e0-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)