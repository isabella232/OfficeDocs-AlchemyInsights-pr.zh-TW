---
title: 無法刪除 SharePoint 或 OneDrive 中的專案
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806102"
---
# <a name="unable-to-delete-items"></a>無法刪除專案

保留原則可能會造成這種情況，您必須停用或排除導致此問題的個別保留。 在刪除保留原則或保留後，最多可能需要24小時的時間，變更才會生效。 確定沒有專案的 [保留原則](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) 設定。

網站可能已超過儲存量限制、增加 [網站配額](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ，以及刪除專案。

確定專案尚未 [取出](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) 給另一位使用者。

最後，系統管理員可以使用 [SharePoint 模式和慣例](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) ，其中包含 PowerShell 命令的文件庫，可讓您執行複雜的管理動作，例如強制刪除 stubborn 專案。
- [移除 PNP 檔](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [移除 PNP 資料夾](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [移除 PNP 清單專案](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [移除 PNP 清單](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [移除 PNP 欄位 (欄) ](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)