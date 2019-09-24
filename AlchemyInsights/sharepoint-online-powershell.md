---
title: Sharepoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/23/2019
ms.locfileid: "37122990"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="85995-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="85995-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="85995-103">使用 PowerShell 或指令碼在 Sharepoint Online 嗎？</span><span class="sxs-lookup"><span data-stu-id="85995-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="85995-104">瀏覽下列連結，如需詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="85995-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="85995-105">開始使用 SharePoint Online 管理命令介面</span><span class="sxs-lookup"><span data-stu-id="85995-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="85995-106">以多重要素驗證 (MFA) 連線至 SPO PowerShell</span><span class="sxs-lookup"><span data-stu-id="85995-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="85995-107">[SharePoint 典範與實例 (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)會包含文件庫的 PowerShell 命令，可讓您在執行複雜的管理動作向 SPO。</span><span class="sxs-lookup"><span data-stu-id="85995-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="85995-108">如果您有使用 SPO 管理命令介面連接的問題，請確定您已更新至最新版本，然後試著[重新匯入模組](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module)使用 *」 匯入模組 Microsoft.Online.SharePoint.PowerShell 」。*</span><span class="sxs-lookup"><span data-stu-id="85995-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="85995-109">如果您試圖執行用戶端物件模型指令碼，您將需要有本機電腦上安裝[Sharepoint Online 用戶端元件 SDK](https://www.microsoft.com/download/details.aspx?id=42038) 。</span><span class="sxs-lookup"><span data-stu-id="85995-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="85995-110">如果您有從 PowerShell 執行指令碼的問題，您可能要考慮以系統管理員身分執行 PowerShell 及變更[執行原則](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)。</span><span class="sxs-lookup"><span data-stu-id="85995-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>