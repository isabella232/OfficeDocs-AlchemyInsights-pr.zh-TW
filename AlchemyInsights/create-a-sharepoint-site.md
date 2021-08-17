---
title: 建立 SharePoint 網站
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: bf9380727fff415357884a5122e633f2254337d3db50e2b8656d94938f76d394
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080881"
---
# <a name="create-a-sharepoint-site"></a>建立 SharePoint 網站

從 SharePoint 系統管理中心的使用中[網站](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true)建立或管理網站。 如需詳細資訊，請參閱[Manage sites in new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation)。 

## <a name="tips"></a>提示：

- 您 **無法** 使用現有網站的相同 URL 來建立網站。 如果您已刪除網站，且想要重新使用 URL，則已刪除的網站可能仍然存在於 [ [已刪除的網站](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)] 底下。 網站必須永久刪除，才能重複使用 URL。 若要使用 Powershell 完全移除網站，請參閱 [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) Cmdlet 範例。
- 有些使用者可能無法建立網站。 [請參閱管理 SharePoint Online 中的網站建立](https://docs.microsoft.com/sharepoint/manage-site-creation)。
- 網站可能會在 **建立** 比預期更長的時間停滯。 如果從您第一次看到此問題起已經過去超過24小時，請記錄支援票證。 多數情況下，我們已經著手研究解決方案。 請至少為我們提供24小時的時間來完成解決方案。
