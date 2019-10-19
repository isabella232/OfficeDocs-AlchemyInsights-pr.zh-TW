---
title: 無法刪除 SharePoint 或 OneDrive 中的項目
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3cc168846999c6880b95edfaedb2df8cf6e843a6
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/18/2019
ms.locfileid: "36748527"
---
# <a name="unable-to-delete-items"></a>無法刪除項目

有問題刪除 SharePoint 項目嗎？

- 永遠確定您已刪除的項目或已移除之項目的[網站集合管理員](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator)嘗試[適當的權限](https://docs.microsoft.com/sharepoint/default-sharepoint-groups)。

- 請確定沒有在[保留原則](https://docs.microsoft.com/office365/securitycompliance/retention-policies)設定的項目。

- 確保項目不是另一個使用者[取出](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)。

- 最後，系統管理員可以使用[SharePoint 典範與實例](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation)(PnP) 其中包含文件庫的 PowerShell 命令，可讓您在執行複雜的管理動作，例如強制刪除頑固項目。
- [移除 PNP 檔案](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [移除 PNP 資料夾](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [移除 PNP 清單項目](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [移除 PNP 清單](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [移除 PNP 欄位 （欄）](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)