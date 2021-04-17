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
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

在 Sharepoint Online 中使用 PowerShell 或腳本？ 如需詳細資訊，請流覽下列連結。
- [開始使用 SharePoint Online 管理命令介面](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [使用多重要素驗證 (MFA) 連接至 SPO PowerShell ](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint 模式和慣例 (PnP) ](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) 包含 PowerShell 命令的文件庫，可讓您對 SPO 執行複雜的管理動作。

> [!NOTE]
> - 如果您使用 SPO 管理命令介面來連線，請確定您已更新至最新版本，然後嘗試使用 *"Import-Module SharePoint PowerShell"* [重新匯入模組](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1)。
> - 如果您嘗試執行用戶端物件模型腳本，您必須將 [Sharepoint Online 用戶端元件 SDK](https://www.microsoft.com/download/details.aspx?id=42038) 安裝在您的本機電腦上。
> - 如果您從 PowerShell 執行腳本時發生問題，您可以考慮以系統管理員身分執行 PowerShell，並變更 [執行原則](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)。