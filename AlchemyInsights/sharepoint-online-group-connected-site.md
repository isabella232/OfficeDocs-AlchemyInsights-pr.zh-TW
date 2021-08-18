---
title: 將群組新增至 SharePoint 網站
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318115"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>在 SharePoint 中建立群組連線的網站時的常見問題

1. 如果您已刪除群組及其連線的網站，且想要使用相同的 URL 建立另一個網站，則必須永久移除之前的網站。

   - 下載[SPO 管理命令](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)介面
   - 如需有關如何開始使用 Powershell 的詳細資訊，請參閱[SharePoint Online 管理命令介面快速](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)入門。
   - 使用 [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell Cmdlet，從刪除的網站中移除網站。 需要有 Powershell 才能永久刪除群組網站。

1. 如果您正在建立群組連線的網站，並收到警告：**另一個具有相同別名的群組已存在**，請從 [Microsoft 365 系統管理中心](https://admin.microsoft.com/AdminPortal/Home#/groups)檢查現有的群組。 若要解決此問題，請刪除現有的群組（如果不再需要的話），或建立網站並指派不同的別名。

1. 有不同的方式可用來建立及使用 SharePoint 的現代群組。

   - 您可以將現有的網站連接至 Microsoft 365 群組。 如需詳細資訊，請參閱[使用 SharePoint 使用者介面連線 Microsoft 365 群組](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)。
   - 若要建立 Microsoft 365 群組連線的網站，您必須建立[小組網站](https://admin.microsoft.com/sharepoint)。
