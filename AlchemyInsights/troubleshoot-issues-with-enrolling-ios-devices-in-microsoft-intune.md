---
title: 疑難排解問題註冊 Microsoft Intune 中的 iOS 裝置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29460959"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>疑難排解問題註冊 Microsoft Intune 中的 iOS 裝置

請檢閱下面列出現在解決問題的資源。 
  
一些常見的錯誤訊息和解決步驟：
  
- **連線至裝置限制**使用者有多個裝置註冊於裝置限制。檢閱這些文件[中移除裝置](https://docs.microsoft.com/en-us/intune/devices-wipe)或[變更裝置限制](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions)。
    
- 不支援**此新服務。註冊無原則：** Apple 推入通知服務 (APNS) 需要設定或更新。請檢閱[本文件](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get)如需如何執行作業的指示。 
    
- **使用者授權類型不正確或無法辨識的使用者名稱：** 使用者必須被指派 Intune 或 EMS 授權。檢閱這些文件以透過將授權指派： [Office 系統管理中心](https://docs.microsoft.com/en-us/intune/licenses-assign)或[Azure 入口網站](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups)。
    
若要協助解決問題的其他資源：
  
1. 使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷及解決常見的註冊失敗。請檢閱[本文件](https://docs.microsoft.com/en-us/intune/help-desk-operators)如需詳細資訊。 
    
2. 檢閱這些文件的每個防止註冊和解決方法的常見錯誤的清單：[疑難排解指南](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune)及[疑難排解 doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。
    
3. [解如何註冊 Microsoft Intune 中的 iOS 裝置](https://docs.microsoft.com/en-us/intune/ios-enroll)。
    

