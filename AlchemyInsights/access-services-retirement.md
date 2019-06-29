---
title: Access services 退休
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 5f171050479f34077f3dc155bec40437f86b84c0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35359330"
---
# <a name="access-services-retirement"></a>Access services 退休

如我們最初于 MC97576 所宣告, 于2006年3月 2017, 且持續與過去一年的通訊, Access Services 會從 Office 365 中撤銷。 此程式的下一個階段就是移除使用 SharePoint 清單作為基礎資料儲存區的 Access Web 資料庫。

**這會對我有何影響？**

從2019年6月開始, 我們將停止在 SharePoint Online 中建立新的 Access 資料庫, 並在4月2020關閉服務及任何剩餘的應用程式。

**我需要做什麼才能準備此變更？**

我們建議您為組織的 Access web 資料庫建立轉換計畫。 系統管理員可以使用[SharePoint access 應用程式掃描器](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner)來取得網站所使用之 Access 應用程式的清單。

有幾種方式可以遷移 Access web 資料庫資料:

- 匯入至本機 Access 資料庫 (。.ACCDB) 或 Excel 檔案。
- 我們也建議您探索 Microsoft PowerApps 做為替代平臺, 以建立 web 和行動裝置的無程式碼商務解決方案。