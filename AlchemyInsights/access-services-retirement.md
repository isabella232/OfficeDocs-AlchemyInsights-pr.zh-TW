---
title: 存取服務退休
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938686"
---
# <a name="access-services-retirement"></a>存取服務退休

如我們最初于 MC97576 宣佈，在2017年3月，繼續與過去一年通訊 Access Services 即將報廢。 此程式的下一個階段是移除使用 SharePoint 清單作為其基礎資料儲存區的 Access Web 資料庫。

**這對我有何影響？**

從2019年6月開始，我們將停止在 SharePoint Online 中建立新的 Access 資料庫，並在4月2020後關閉服務和任何剩餘的應用程式。

**若要準備這項變更，需要執行什麼動作？**

我們鼓勵您為組織的 Access web 資料庫建立過渡計畫。 系統管理員可以使用[SharePoint Access 應用程式掃描器](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner)，以取得網站所使用的 Access 應用程式清單。

有幾種方式可以遷移 Access web 資料庫資料：

- 匯入至本機 Access 資料庫 (。.accdb) 或 Excel 檔案。
- 我們也建議您探索 Microsoft PowerApps 做為替代平臺，以為 web 和行動裝置建立無程式碼商務解決方案。