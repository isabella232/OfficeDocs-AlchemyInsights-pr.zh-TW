---
title: 驗證應用程式
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082933"
---
# <a name="authentication-app"></a>驗證應用程式

如果您是全域系統管理員，您可以使用登 [入診斷](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)，快速找出與使用者登入相關的問題。

1. 按一下 [[啟動診斷](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)] 按鈕，啟動診斷程式。 
1. 輸入您所擁有的使用者、應用程式、登入時間、要求識別碼或相互關聯識別碼的詳細資料，以尋找要分析的事件。
1. 檢閱診斷結果 - 顯示有關所發生的事件以及可採取哪些動作以進行變更的詳細資料 (如果需要變更的話)。

**檢查適用的案例：**

1. 如果使用者未在 Microsoft Authenticator 應用程式中取得推播通知，請在 [MFA][或 [解除封鎖使用者](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)] 中所述的 [MFA 封鎖的使用者] 下，確認未出現推播通知。
1. 如果使用者未被封鎖進行 MFA，但沒有收到推播通知，則他們可以開啟 Microsoft Authenticator 應用程式，該應用程式會拉入待處理的核准要求。
1. 另一種登入方法，使用者也可以按一下登入另一種方式，然後選擇 [使用我的行動應用程式的驗證碼。
1. Microsoft Authenticator 應用程式是許多使用者唯一可用的方法。 [深入瞭解安全性預設值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)，請參閱常見問題及其解決方法的[Authenticator 應用程式常見問題](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq)。
 
**建議影片**

[如何在新電話上設定 Authenticator App (2min) ](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)。
