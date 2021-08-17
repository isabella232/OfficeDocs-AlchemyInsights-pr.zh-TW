---
title: 沒有結果的內容搜尋
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057993"
---
# <a name="no-results-from-content-searchexports"></a>內容搜尋/匯出沒有任何結果

內容搜尋/匯出的問題未傳回任何資料可能是由於特定系統管理員所設定的某些規範安全性篩選，但未與所有系統管理員通訊。

若要解決此問題，請查看是否有任何可能導致問題的相容性安全性篩選：
1. 連線至安全性與合規性中心 Powershell
2. 執行下列 commandlets：
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-組織 $org