---
title: 圖表顯示格線中不同數量的記錄
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 68ba6caf602a5cf60e2c96c80703f19dd07c3b6430c2a66f40fea4a2f3d06e75
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950071"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>圖表顯示格線中不同數量的記錄

**徵狀**

在儀表板頁面上，當您按一下 [圖表] “…” 並按一下 [查看記錄] 時，將瀏覽至格線頁查看所有記錄。有時候，記錄數會發變更。

**原因**

這是因為原始儀表板頁面上的圖表與格線首頁上的圖表有所不同。  

**解決方案**

1. 檢查原始頁面和格線中的視圖，查看它們是否不同。
2. 變更格線中的視圖，使之與原始頁面中的視圖相符。
3. 如果找不到正確的視圖，通常表示應用程式設計工具中沒有啟用該視圖。
4. 移至特定應用程式的的 [應用程式設計工具]，選擇實體及其視圖，檢查您要啟用、儲存、發佈和關閉的視圖。
5. 重新整理頁面。