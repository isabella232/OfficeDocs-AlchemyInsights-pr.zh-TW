---
title: 無法變更使用者名稱
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431508"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="e51b1-102">無法變更使用者名稱</span><span class="sxs-lookup"><span data-stu-id="e51b1-102">Unable to change UserName</span></span>

<span data-ttu-id="e51b1-103">在某些情況下，UPN (UserPrincipalName) 變更不會傳播至雲端。</span><span class="sxs-lookup"><span data-stu-id="e51b1-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="e51b1-104">您可能會在 Office 365 入口網站收到驗證錯誤，或無法變更使用者名稱或電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="e51b1-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="e51b1-105">若要解決此問題，請使用此 PowerShell 命令手動設定 UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="e51b1-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="e51b1-106">**範例：重新命名使用者**</span><span class="sxs-lookup"><span data-stu-id="e51b1-106">**Example: Rename a user**</span></span>

<span data-ttu-id="e51b1-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="e51b1-107">PowerShellCopy</span></span>

<span data-ttu-id="e51b1-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="e51b1-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="e51b1-109">此命令會將 davidc@contoso.com 重新命名為 davidchew@contoso.com。</span><span class="sxs-lookup"><span data-stu-id="e51b1-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="e51b1-110">如需詳細資訊，請參閱 [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0) (英文)。</span><span class="sxs-lookup"><span data-stu-id="e51b1-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>