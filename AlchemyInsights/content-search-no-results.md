---
title: 沒有結果的內容搜尋
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680638"
---
# <a name="no-results-from-content-searchexports"></a>內容搜尋/匯出沒有任何結果

內容搜尋/匯出的問題未傳回任何資料可能是由於特定系統管理員所設定的某些規範安全性篩選，但未與所有系統管理員通訊。

若要解決此問題，請查看是否有任何可能導致問題的相容性安全性篩選：
1. 連接到安全性與合規性中心 Powershell
2. 執行下列 commandlets：
<br>$org = "yourdomain.com"
<br>Remove-compliancesecurityfilter-組織 $org