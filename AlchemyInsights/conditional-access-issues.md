---
title: 條件式存取問題
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013928"
---
# <a name="conditional-access-issues"></a>條件式存取問題

**解決登入診斷的問題**

您可以使用登 [入診斷](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)，快速找出或診斷使用者登入相關問題：

1. 啟動 登入診斷。
1. 輸入您所擁有的使用者、應用程式、登入時間、要求識別碼或相互關聯識別碼的詳細資料，以尋找要分析的事件。
1. 查看診斷結果，顯示發生什麼情況的詳細資料，以及您可以採取哪些動作進行變更 (若) 需要任何變更。

**疑難排解 Sign-In 的步驟** 

1. 流覽至 Azure AD 登入頁面。
1. 篩選登入的使用者、時間範圍、應用程式、狀態、用戶端應用程式等等。
1. 選取登入事件，然後查看 [條件存取] 索引標籤，以查看已評估的原則。
1. 按一下原則的列，以查看原則詳細資料並瞭解其應用原因。

**設定條件式存取原則疑難排解的工具**

- 僅限報告模式可讓您評估原則，而不會影響使用者。
- 假設工具可讓您模擬登入事件，並查看適用的原則。
- Insights 與報告活頁簿會顯示每個原則的即時影響。

**基準保護原則**

已棄用基準保護原則。 它們不再執行，很快就會從 Azure 入口網站移除。 建議啟用 [安全性預設值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)。

如需條件式存取的詳細資訊，請參閱：

[在 Azure Active Directory 中進行條件式存取的最佳作法](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
[條件式存取](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 中的條件[條件式存取](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 中的控制項[條件式存取中的位置](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
