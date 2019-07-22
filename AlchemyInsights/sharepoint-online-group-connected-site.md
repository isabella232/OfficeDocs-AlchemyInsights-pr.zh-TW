---
title: 新增群組至 SharePoint 網站
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758722"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>在 Sharepoint Online 中建立群組連線網站

有幾個建立或重新建立連線網站時常見的問題。

 如果您已刪除群組及其連線網站，且想要使用的相同 URL 建立另一個網站，您必須永久移除舊版的網站。

下載 [SPO 管理命令介面](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 如需開始使用 PowerShell 的詳細資訊，請參閱[開始使用 SharePoint Online 管理命令介面](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) (英文)

使用 [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell Cmdlet 將網站從已刪除的網站移除。

如果您正在建立群組連線網站，卻收到具有相同別名的群組已存在的警告，請從 [Office 365 的系統管理中心](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)查看現有的群組。 請刪除不再需要的現有群組或建立不同別名的網站來解決此問題。

建立及使用 SharePoint 的新式群組的方式有很多種。

您可以連線現有的網站至 Office 365 群組。 如需詳細資訊，請參閱[使用 SharePoint 使用者介面連線 Office 365 群組](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface) (英文)。

若要建立 Office 365 群組連線網站，您必須建立小組網站。 如需詳細資訊，請參閱[在 SharePoint 中建立小組網站](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)。

