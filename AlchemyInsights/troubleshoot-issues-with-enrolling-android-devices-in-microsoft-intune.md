---
title: 疑難排解問題註冊 Microsoft Intune 中的 Android 裝置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420583"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>疑難排解問題註冊 Microsoft Intune 中的 Android 裝置

請先檢閱下列資源以立即解決您的問題。
  
部分一般問題及解決步驟：
  
 **裝置未加密的公司入口網站中的錯誤：** 較新版本的 Android，尤其開頭 v7.0，需要啟動密碼以確保您的裝置已完全加密。 若要啟用啟動 pin 碼，或完全加密裝置是常見的解決方案。 檢閱[本文件](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)如需詳細資訊。 
  
 **裝置無法簽入 Intune 服務或 Intune 管理主控台中顯示為 「 Unhealthy 」:** 某些 Samsung 4.4 和 5.5 裝置可能會檢查恢復服務。 有 3 可能的解決方案，此問題： 
  
1. 以手動方式開啟 Intune 公司入口網站應用程式，將會自動啟動裝置同步處理。
    
2. 更新裝置 Android 6.0 或更高版本。
    
3. 停用 Samsung 智慧管理員從管理 Intune 公司入口網站。 檢閱[本文件](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)如需這些問題與解決方法的詳細資訊。 
    
 **使用者授權類型不正確**或**使用者名稱無法辨識的錯誤：** 使用者需要已獲得 Intune 或 EMS 授權。 檢閱這些文件以透過將授權指派： Office 系統管理中心或 Azure 入口網站。 
  
其他資源，可以協助解決您的問題：
  
1. 使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷和解決常見註冊失敗。 檢閱[本文件](https://docs.microsoft.com/intune/help-desk-operators)如需詳細資訊。 
    
2. 檢閱[本文件](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)的清單中的每個防止註冊和解決方法的常見錯誤。 
    
3. [了解如何註冊 Microsoft Intune 中的 Android 裝置](https://docs.microsoft.com/intune/android-enroll)。
    

