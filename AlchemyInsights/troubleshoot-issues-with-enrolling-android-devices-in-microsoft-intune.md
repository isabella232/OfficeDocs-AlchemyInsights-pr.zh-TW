---
title: 疑難排解問題註冊 Microsoft Intune 在 Android 裝置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28279475"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>疑難排解問題註冊 Microsoft Intune 在 Android 裝置

請檢閱下面列出現在解決問題的資源。
  
部分一般問題與解決步驟：
  
 **裝置未加密的公司入口網站中的錯誤：** Android，特別開頭 v7.0、 較新版本需要啟動密碼以確定您的裝置已完全加密。若要啟用啟動 pin 或完全加密裝置是常見的方案。請檢閱[本文件](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)的詳細資訊。 
  
 **裝置無法檢查使用 Intune 服務或 Intune 系統管理主控台中顯示為"Unhealthy":** 某些 Samsung 4.4 和 5.5 裝置可能會檢查服務。有這個問題 3 可能的解決方案： 
  
1. 以手動方式開啟 Intune 的公司入口網站應用程式，將會自動啟動裝置同步處理。
    
2. 更新裝置 Android 6.0 或更高。
    
3. 停用 Samsung 智慧管理員從管理 Intune 的公司入口網站。請檢閱[本文件](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)如需這些問題及解決方法的詳細資訊。 
    
 **使用者授權類型不正確**或**使用者名稱不會辨識錯誤：** 使用者必須被指派 Intune 或 EMS 授權。檢閱這些文件以透過將授權指派： Office 系統管理中心或 Azure 入口網站。 
  
若要協助解決問題的其他資源：
  
1. 使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷及解決常見的註冊失敗。請檢閱[本文件](https://docs.microsoft.com/en-us/intune/help-desk-operators)如需詳細資訊。 
    
2. 請檢閱[本文件](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)的每個防止註冊和解決方法的常見錯誤的清單。 
    
3. [解如何註冊 Microsoft Intune 在 Android 裝置](https://docs.microsoft.com/en-us/intune/android-enroll)。
    

