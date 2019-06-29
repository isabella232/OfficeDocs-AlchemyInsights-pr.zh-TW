---
title: 針對在 Microsoft Intune 中註冊 Android 裝置的問題進行疑難排解
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 9cdfda0d7dd45af260f46738cbc85aac46f53960
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367280"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>針對在 Microsoft Intune 中註冊 Android 裝置的問題進行疑難排解

請查看下面所列的資源, 立即解決您的問題。
  
一些常見的問題和解決步驟:
  
 **公司入口網站中的裝置未加密錯誤:** 較新版本的 Android (特別是從 v 7.0 開始) 需要啟動密碼, 以確保您的裝置已完全加密。 常見的解決方案是啟用啟動 pin 或對裝置進行完全加密。 如需詳細資訊, 請參閱[本檔](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)。
  
 **在 intune 管理主控台中, 裝置無法以 intune 服務存回, 或顯示為「狀況不良」:** 某些 Samsung 4.4 和5.5 裝置可能無法存回服務。 此問題有三種可行的解決方案:
  
1. 手動開啟 [Intune 公司入口網站應用程式], 它會自動啟動裝置同步處理。

2. 將裝置更新為 Android 6.0 或更高版本。

3. 停用 Samsung Smart Manager 管理 Intune 公司入口網站。 如需這些問題和解決方法的詳細資訊, 請參閱[本檔](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)。

 **使用者授權類型無效**或**無法辨識使用者名稱錯誤:** 使用者必須被指派 Intune 或 EMS 授權。 檢查這些檔, 以指派授權至: Office 系統管理中心或 Azure 入口網站。
  
可協助您解決問題的其他資源:
  
1. 使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷和解決常見的註冊失敗。 如需詳細資訊, 請參閱[本檔](https://docs.microsoft.com/intune/help-desk-operators)。

2. 請參閱[本檔](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune), 以取得防止每個專案的註冊和解析度的常見錯誤清單。

3. [瞭解如何在 Microsoft Intune 中註冊 Android 裝置](https://docs.microsoft.com/intune/android-enroll)。
