---
title: 在 SharePoint 或 OneDrive 中限制存取權
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700446"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>在 SharePoint 或 OneDrive 中限制存取權

有許多方式可以限制存取 SharePoint 線上/OneDrive 服務。 下列列出各種訪問限制方法。 

**許可權限制**

在 SharePoint Online 和商務 OneDrive 中，我們只會將存取權授與網站、檔案和資料夾等專案的存取權授與應該具有存取權的那些群組/個人。

- [自訂 SharePoint 清單或文件庫的許可權](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [自訂 SharePoint 網站權限](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [變更子資料夾的權限](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [從未受控裝置中控制存取權](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

做為 SharePoint 或全域系統管理員，您可以封鎖或限制存取不受管理的裝置的 SharePoint 和 OneDrive 內容 (Intune) 中未結合的混合式廣告或相容性。

**網路位置限制**

做為 IT 管理員，您可以根據您信任的定義網路位置，控制對 SharePoint 和 OneDrive 資源的存取。 這也稱為位置型原則。 如需詳細資訊，請參閱 [以網路位置為基礎的 SharePoint 線上及 OneDrive 資料的控制存取權](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**網站鎖定限制** 

在 SharePoint Online 中，您可以鎖定網站集合，因此沒有人能夠存取。 這是透過 PowerShell 和使用[Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) LockState 屬性[SharePoint Online 管理命令](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)介面來設定。

**限制使用者建立網站或子網站**

做為 SharePoint 系統管理員或全域管理員，您可以讓您的使用者建立及管理自己的 SharePoint 網站、決定可以建立的網站類型，並指定網站的位置。 如需詳細資訊，請參閱 [在 SharePoint Online 中管理網站建立](https://docs.microsoft.com/sharepoint/manage-site-creation)

