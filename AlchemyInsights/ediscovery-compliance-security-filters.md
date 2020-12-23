---
title: 內容搜尋/匯出期間未傳回任何結果
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727214"
---
# <a name="no-results-returned-during-content-searchexport"></a>內容搜尋/匯出期間未傳回任何結果

如果您在下列 eDiscovery 案例中遇到問題：

- 內容搜尋/匯出會傳回沒有資料或非預期的資料
- eDiscovery 搜尋或匯出失敗

這可能是因為特定系統管理員所設定的某些規範安全性篩選器，但未傳遞給所有系統管理員。

若要解決此問題，請檢查是否有任何可能導致這些問題的相容性安全性篩選：

1. 連接到安全性與合規性中心 Powershell
2. 執行下列 commandlets：

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

如需有關相容性安全性篩選的詳細資訊，請參閱 [內容搜尋的許可權篩選](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
