---
title: 在 SharePoint 或 OneDrive 中限制存取
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223703"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>在 SharePoint 或 OneDrive 中限制存取

有許多方法可以限制對 SharePoint Online/OneDrive 服務的存取。 下列各種訪問限制方法如下所示。 

**許可權限制**

在 SharePoint Online 和商務用 OneDrive 中, 我們只會授與應該具有存取權的群組/個人存取權, 以限制網站、檔案和資料夾等專案的存取權。

- [自訂 SharePoint 清單或文件庫的許可權](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [自訂 SharePoint 網站的權限](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions) (機器翻譯)

- [變更子資料夾的權限](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [從未受控裝置中控制存取權](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

在 Office 365 中為 SharePoint 或全域系統管理員, 您可以封鎖或限制存取未受管理裝置 (不是在 Intune 中加入或相容的使用者) 的 SharePoint 和 OneDrive 內容。

**網路位置限制**

作為 IT 系統管理員, 您可以根據您信任的定義網路位置, 來控制 SharePoint 和 OneDrive 資源的存取權。 這也稱為位置型原則。 如需詳細資訊, 請參閱[根據網路位置控制對 SharePoint Online 和 OneDrive 資料的存取](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**網站鎖定限制** 

在 SharePoint Online 中, 您可以鎖定網站集合, 讓任何人都無法存取。 這是透過 PowerShell 和使用[get-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState 屬性的[SharePoint Online 管理命令](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)介面進行設定。

**限制使用者建立網站或子網站**

作為 SharePoint 系統管理員或 Office 365 全域管理員, 您可以讓您的使用者建立及管理自己的 SharePoint 網站、決定他們可以建立的網站類型, 以及指定網站的位置。 如需詳細資訊, 請參閱[在 SharePoint Online 中管理網站建立](https://docs.microsoft.com/sharepoint/manage-site-creation)

