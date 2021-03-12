---
title: 在 Microsoft Intune 中註冊 Android 裝置的問題疑難排解
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708989"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>在 Microsoft Intune 中註冊 Android 裝置的問題疑難排解

立即查看下列資源，以解決您的問題。
  
一些常見的問題和解決步驟：
  
 **公司入口網站中的裝置未加密錯誤：** 較新版本的 Android （特別是從 v 7.0 開始）需要啟動密碼，以確保您的裝置已完全加密。 常見的解決方案是啟用啟動 pin 碼或完全加密裝置。 如需詳細資訊，請參閱 [本檔](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) 。
  
 在 **intune 管理主控台中，裝置無法存回 intune 服務或顯示為「不良」：** 有些 Samsung 4.4 和5.5 裝置可能無法存回服務。 此問題有三種可能的解決方案：
  
1. 手動開啟 Intune 公司入口網站應用程式，此應用程式會自動啟動裝置同步處理。

2. 將裝置更新為 Android 6.0 或更高版本。

3. 停用 Samsung Smart Manager 管理 Intune 公司入口網站。 如需這些問題和解決方法的詳細資訊，請參閱 [本檔](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) 。

 **使用者授權類型無效** 或 **使用者名稱無法辨識錯誤：** 使用者必須被指派一個 Intune 或 EMS 授權。 檢查這些檔，以指派授權至： Office 系統管理中心或 Azure 入口網站。
  
其他可協助您解決問題的資源：
  
1. 使用 [Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 來診斷及解決一般註冊失敗。 如需詳細資訊，請參閱 [本檔](https://docs.microsoft.com/intune/help-desk-operators) 。

2. 請參閱 [本檔](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) ，以取得避免每個專案的註冊和解析度的常見錯誤清單。

3. [瞭解如何在 Microsoft Intune 中註冊 Android 裝置](https://docs.microsoft.com/intune/android-enroll)。
