---
title: 新式網站作為根網站
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057679"
---
# <a name="modern-site-as-root-site"></a>新式網站作為根網站

[目標版本](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide)客戶現在可以啟用新式通訊的網站經驗，其 SharePoint 租用戶的傳統的根網站。

藉由執行簡單的 PowerShell cmdlet，就可以啟動這項功能。 在 PowerShell 命令執行成功，根網站會有新的通訊網站首頁。 關於 PowerShell 指令程式和功能需求的詳細資料可[啟用 SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps)」 文件中。 

我們將會逐漸循環時，關閉依預設，在早期 2019 年，已設定目標發行客戶，首度發行將提供使用全球年 6 月 2019年結束。 若要參照在[訊息中心](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)的其他新功能與現代化繼續執行。 

**重要**： 請不要刪除傳統的根網站以建立新式通訊網站。 Microsoft 不支援此。 刪除根網站會使所有的 SharePoint 網站組織中所有使用者，無法存取直到您還原的網站，或在相同的 URL 建立新的網站。 
 
 