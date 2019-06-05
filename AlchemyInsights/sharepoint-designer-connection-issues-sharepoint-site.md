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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716883"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer 連線問題 

<p>如果 SharePoint Designer 遇到至 SharePoint 網站的連線問題，請嘗試下列常見的解決方案。</p> <p><strong>步驟 1:</strong><strong>更新確認 SharePoint Designer&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">SharePoint Designer 2013 (KB3114721) 更新</a></li> </ul> <p><strong>步驟 2:</strong><strong>清除本機快取檔案</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">關閉 SharePoint Designer 2013。&nbsp;</li> <li style="font-weight: 400;">本機電腦上，瀏覽至下列資料夾移除快取的檔案。&nbsp;</li> <li style="font-weight: 400;">按一下 [<strong>開始-&gt;執行</strong>及刪除下每個找到的所有檔案位置下方。&nbsp;<br /><br />%APPDATA%\Microsoft\Web 伺服器 Extensions\Cache<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">開啟 SharePoint Designer 2013，並輸入一次若要查看是否它的運作方式的帳戶。</li> </ol> <p><strong>步驟 3:</strong><a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"><strong>的 Windows 裝置上的 Office 2013 啟用新式驗證</strong></a>&nbsp;</p> <p><strong>步驟 4:</strong><strong>系統管理員就必須允許自訂指令碼，以允許 SharePoint Designer 連接</strong>。</p> <p>如需詳細的步驟、 範例及考量請參閱<a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">允許或防止自訂指令碼</a>。&nbsp;</p>


