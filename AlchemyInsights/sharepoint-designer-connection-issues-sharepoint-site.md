---
title: SharePoint Online 的權限等級
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760684"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer 連線問題 

如果 SharePoint Designer 遇到至 SharePoint 網站的連線問題，請嘗試下列常見的解決方案。

步驟 1： 驗證已更新 SharePoint Designer。

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [SharePoint Designer 2013 (KB3114721) 更新](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

步驟 2： 清除本機快取檔案

- 關閉 SharePoint Designer 2013。

- 本機電腦上，瀏覽至下列資料夾移除快取的檔案。

- 按一下 [開始]、 [執行] 和 [刪除所有檔案都位於 [每個位置下方。

%APPDATA%\Microsoft\Web 伺服器 Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

開啟 SharePoint Designer 2013，並輸入一次若要查看是否它的運作方式的帳戶。

步驟 3：[的 Windows 裝置上的 Office 2013 啟用新式驗證](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

步驟 4： 系統管理員必須允許自訂指令碼以允許 SharePoint Designer 連線。

如需詳細的步驟、 範例及考量請參閱[允許或防止自訂指令碼](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)。


