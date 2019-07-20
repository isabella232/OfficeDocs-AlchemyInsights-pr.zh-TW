---
title: 內容搜尋任何結果
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800218"
---
# <a name="no-results-from-content-searchexports"></a>從內容搜尋/匯出任何結果

問題使用內容搜尋/匯出不傳回任何資料可能會因為某些法規安全性篩選器所安裝的特定的系統管理員並沒有通訊用於所有的系統管理員。

若要解決此問題，請檢查是否有可能原因包括下列任何法規安全性篩選器：
1. 連接到安全性與合規性中心 Powershell
2. 執行下列 commandlets:
<br>$org ="yourdomain.com 」
<br>取得 ComplianceSecurityFilter-組織 $org