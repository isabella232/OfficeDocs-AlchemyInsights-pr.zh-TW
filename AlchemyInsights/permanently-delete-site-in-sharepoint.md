---
title: 在 SharePoint 中永久刪除網站
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: f461963c4a5719957258349d667731231023721ab3ee4641538c94371bf3f56d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944302"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>在 SharePoint 中永久刪除網站

若要重複使用已刪除網站中的 URL (以重建網站)，或因為網站已不再使用而永久刪除網站，您可從新版 SharePoint 系統管理中心使用 [永久刪除]。 

1. 移至[新版 SharePoint 系統管理中心的 [已刪除網站]](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) 頁面，並使用具有組織系統管理員權限的帳戶登入。 

2. 在左側資料行中，選取網站。 

3. 按一下 [永久刪除]。 

**附註**：無法從新版 SharePoint 系統管理中心永久刪除群組連線的網站。 必須改用 [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite)。  

如需詳細資訊，請參閱[永久刪除網站](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site)。 
