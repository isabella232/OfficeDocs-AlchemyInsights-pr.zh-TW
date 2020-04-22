---
title: 存取服務退休
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687249"
---
# <a name="access-services-retirement"></a>存取服務退休

如我們最初于 MC97576 宣佈，在3月2017，繼續透過過去一年的通訊存取服務即將停用。 此程式的下一個階段是移除使用 SharePoint 清單作為其基礎資料儲存區的 Access Web 資料庫。

**這對我有何影響？**

從2019年6月開始，我們將停止在 SharePoint Online 中建立新的 Access 資料庫，並在4月2020後關閉服務和任何剩餘的應用程式。

**若要準備這項變更，需要執行什麼動作？**

我們鼓勵您為組織的 Access web 資料庫建立過渡計畫。 系統管理員可以使用[SharePoint Access 應用程式掃描器](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner)，以取得網站所使用的 Access 應用程式清單。

有幾種方式可以遷移 Access web 資料庫資料：

- 匯入至本機 Access 資料庫（。.ACCDB）或 Excel 檔案。
- 我們也建議您探索 Microsoft PowerApps 做為替代平臺，以建立 web 和行動裝置的無程式碼商務解決方案。