---
title: 識別 Windows 虛擬桌面問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590275"
---
# <a name="identify-windows-virtual-desktop-issues"></a>識別 Windows 虛擬桌面問題

Windows 虛擬桌面診斷僅使用 PowerShell Cmdlet，但包含許多選用參數以協助縮小和隔離問題。 若要開始使用： 

1. 下載並匯入 Windows 虛擬桌面 PowerShell 模組。 如需詳細資訊，請參閱[適用於 Windows PowerShell 的 Windows 虛擬桌面 Cmdlet](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)。

1. 執行下列 Cmdlet 登入您的帳戶：
    
    範例：`Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**注意：** 所有使用 PowerShell 的査詢都必須包含 -UserName 或 -ActivityID 參數。 如需有關監視功能的資訊，請參閱使用[診斷功能的記錄分析](https://go.microsoft.com/fwlink/?linkid=2126847)。

若要依使用者篩選診斷活動，請執行以下 Cmdlet：

範例：`Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

您可以執行一個篩選器清單來診斷問題。 若要深入了解診斷問題，請參閱[識別和診斷 Windows 虛擬桌面問題](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)。

若要深入瞭解常見錯誤，請參閲[常見錯誤案例](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)。
