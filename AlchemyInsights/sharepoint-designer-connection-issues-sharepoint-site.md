---
title: SharePoint Designer 連線問題
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051704"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer 連線問題 

如果 SharePoint Designer 遇到至 SharePoint 網站的連線問題，請嘗試下列常見的解決方案。

步驟 1： 確認 SharePoint Designer 2013 會更新為[SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)和[2016 年 8 月 2 日更新的 SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)。



步驟 2： 清除本機快取檔案：

1. 關閉 SharePoint Designer 2013。

2. 本機電腦上，移除在每個下列資料夾中找到的所有檔案。

    - %APPDATA%\Microsoft\Web 伺服器 Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. 開啟 SharePoint Designer 2013，並輸入一次若要查看是否它的運作方式的帳戶。

步驟 3：[的 Windows 裝置上的 Office 2013 啟用新式驗證](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)。

步驟 4： 系統管理員必須**允許自訂指令碼**中的 SharePoint 系統管理中心設定以允許 SharePoint Designer 連線。 請參閱[允許或防止自訂指令碼](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)如需詳細資訊。


