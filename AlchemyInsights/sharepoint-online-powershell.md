---
title: Sharepoint Online PowerShell
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
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830573"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="ca3fa-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="ca3fa-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="ca3fa-103">在 Sharepoint Online 中使用 PowerShell 或腳本？</span><span class="sxs-lookup"><span data-stu-id="ca3fa-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="ca3fa-104">如需詳細資訊，請流覽下列連結。</span><span class="sxs-lookup"><span data-stu-id="ca3fa-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="ca3fa-105">開始使用 SharePoint Online 管理命令介面</span><span class="sxs-lookup"><span data-stu-id="ca3fa-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="ca3fa-106">使用多重要素驗證 (MFA) 連接至 SPO PowerShell </span><span class="sxs-lookup"><span data-stu-id="ca3fa-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="ca3fa-107">[SharePoint 模式和慣例 (PnP) ](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) 包含 PowerShell 命令的文件庫，可讓您對 SPO 執行複雜的管理動作。</span><span class="sxs-lookup"><span data-stu-id="ca3fa-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="ca3fa-108">如果您使用 SPO 管理命令介面來連線，請確定您已更新至最新版本，然後嘗試使用 *"Import-Module SharePoint PowerShell"* [重新匯入模組](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1)。</span><span class="sxs-lookup"><span data-stu-id="ca3fa-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="ca3fa-109">如果您嘗試執行用戶端物件模型腳本，您必須將 [Sharepoint Online 用戶端元件 SDK](https://www.microsoft.com/download/details.aspx?id=42038) 安裝在您的本機電腦上。</span><span class="sxs-lookup"><span data-stu-id="ca3fa-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="ca3fa-110">如果您從 PowerShell 執行腳本時發生問題，您可以考慮以系統管理員身分執行 PowerShell，並變更 [執行原則](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)。</span><span class="sxs-lookup"><span data-stu-id="ca3fa-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>