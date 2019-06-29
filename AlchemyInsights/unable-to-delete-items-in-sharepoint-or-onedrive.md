---
title: 無法刪除 SharePoint 或 OneDrive 中的專案
ms.author: kirks
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
ms.openlocfilehash: d25214f26a3168e3e350b5cc31ca870e65d48ad9
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35366524"
---
# <a name="unable-to-delete-items"></a>無法刪除專案

在刪除專案時有問題嗎？

- 請務必確定您有[適當的許可權](https://docs.microsoft.com/sharepoint/default-sharepoint-groups)可刪除專案, 或讓[網站集合管理員](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator)嘗試移除專案。

- 確定專案上沒有[保留原則](https://docs.microsoft.com/office365/securitycompliance/retention-policies)設定。

- 確定專案未[取出](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)給另一位使用者。

- 最後, 系統管理員可以使用[SharePoint 模式和作法](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation)(PnP), 其中包含 PowerShell 命令庫, 可讓您執行複雜的管理動作, 例如強制刪除 stubborn 的專案。
- [移除 PNP 檔案](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [移除 PNP 資料夾](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [移除 PNP 清單專案](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [移除 PNP 清單](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [移除 PNP 欄位 (資料行)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)