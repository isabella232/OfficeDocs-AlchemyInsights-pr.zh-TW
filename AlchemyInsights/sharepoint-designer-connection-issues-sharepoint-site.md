---
title: SharePoint 設計工具連接問題
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
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511535"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint 設計工具連接問題 

如果 SharePoint 設計工具遇到 SharePoint 網站的連線問題，請嘗試下列一般解決方案。

步驟1：確認 SharePoint 設計工具2013已使用[SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)和[8 月2日的2016更新（SharePoint Designer 2013）](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)進行更新。



步驟2：清除本機快取檔：

1. 關閉 SharePoint 設計工具2013。

2. 在本機電腦上，移除每個下列資料夾中找到的所有檔案。

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. 開啟 SharePoint 設計工具2013，然後再次輸入帳戶，查看是否運作正常。

步驟3：[在 Windows 裝置上啟用 Office 2013 的新式驗證](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)。

步驟4：系統管理員必須允許 SharePoint 系統管理中心設定中的**自訂腳本**，才能允許 SharePoint Designer 連線。 如需詳細資訊，請參閱[Allow 或預防自訂腳本](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)。


