---
title: 無法刪除 SharePoint 或 OneDrive 中的項目
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571229"
---
# <a name="unable-to-delete-items"></a>無法刪除項目

保留原則可能會導致此，您必須停用或排除此問題所造成的個別保留。 會移除保留原則或保留之後，可能需要 24 小時的時間，變更才會生效。 請確定沒有在[保留原則](https://docs.microsoft.com/office365/securitycompliance/retention-policies)設定的項目。

網站可能已超過儲存限制、 增加的[網站配額](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)和刪除的項目。

確保項目不是另一個使用者[取出](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)。

最後，系統管理員可以使用[SharePoint 典範與實例](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation)(PnP) 其中包含文件庫的 PowerShell 命令，可讓您在執行複雜的管理動作，例如強制刪除頑固項目。
- [移除 PNP 檔案](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [移除 PNP 資料夾](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [移除 PNP 清單項目](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [移除 PNP 清單](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [移除 PNP 欄位 （欄）](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)