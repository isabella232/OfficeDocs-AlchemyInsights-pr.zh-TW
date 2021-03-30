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
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403801"
---
# <a name="authentication-app"></a>驗證應用程式

如果您是全域系統管理員，您可以使用登 [入診斷](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)，快速找出與使用者登入相關的問題。

1. 按一下 [[啟動診斷](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)] 按鈕，啟動診斷程式。 
1. 輸入您所擁有的使用者、應用程式、登入時間、要求識別碼或相互關聯識別碼的詳細資料，以尋找要分析的事件。
1. 檢閱診斷結果 - 顯示有關所發生的事件以及可採取哪些動作以進行變更的詳細資料 (如果需要變更的話)。

**檢查適用的案例：**

1. 如果使用者未在 Microsoft 驗證器應用程式中取得推播通知，請確認在 [MFA 封鎖] 使用者未如 [封鎖和解除封鎖使用者](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)中所述的那樣顯示這些使用者。
1. 如果使用者未被封鎖進行 MFA，但沒有收到推播通知，則可以開啟 Microsoft 驗證者應用程式，它會拉出擱置的核准要求。
1. 另一種登入方法，使用者也可以按一下登入另一種方式，然後選擇 [使用我的行動應用程式的驗證碼。
1. Microsoft 驗證應用程式是許多使用者唯一可用的方法。 [深入瞭解安全性預設值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)，請參閱 [驗證器 App 應用程式](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) 常見問題，以取得常見問題及其解決方法。
 
**建議影片**

[如何在新電話上設定驗證器應用程式 (2min) ](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)。
