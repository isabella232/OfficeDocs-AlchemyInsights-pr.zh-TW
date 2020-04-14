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
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286240"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="a26a7-102">變更強式密碼需求</span><span class="sxs-lookup"><span data-stu-id="a26a7-102">Change strong password requirement</span></span>

<span data-ttu-id="a26a7-103">Microsoft 預設會需要強密碼。</span><span class="sxs-lookup"><span data-stu-id="a26a7-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="a26a7-104">使用 PowerShell，您可以使用此命令，針對特定使用者停用強式密碼：</span><span class="sxs-lookup"><span data-stu-id="a26a7-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="a26a7-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="a26a7-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="a26a7-106">密碼原則的詳細資訊</span><span class="sxs-lookup"><span data-stu-id="a26a7-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="a26a7-107">如何使用 PowerShell 連接至 Office 365</span><span class="sxs-lookup"><span data-stu-id="a26a7-107">How to connect to Office 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="a26a7-108">PowerShell Get-msoluser 命令的詳細資訊</span><span class="sxs-lookup"><span data-stu-id="a26a7-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [<span data-ttu-id="a26a7-109">設定個別使用者的密碼永不過期</span><span class="sxs-lookup"><span data-stu-id="a26a7-109">Set an individual user's password to never expire</span></span>](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
