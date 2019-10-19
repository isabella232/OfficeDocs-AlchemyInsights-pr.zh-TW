---
title: 疑難排解問題註冊 Microsoft Intune 中的 iOS 裝置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/18/2019
ms.locfileid: "36506910"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>疑難排解問題註冊 Microsoft Intune 中的 iOS 裝置

請先檢閱下列資源以立即解決您的問題。 
  
一些常見的錯誤訊息及解決步驟：
  
- **達到裝置限制**使用者有多個裝置註冊比裝置的限制。 檢閱這些文件以[移除裝置](https://docs.microsoft.com/intune/devices-wipe)，或[變更裝置的限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。
    
- 不支援**此服務。沒有註冊的原則：** Apple 推播通知服務 (APNS) 需要設定或更新。 檢閱[本文件](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)如需如何執行這項作業的指示。 
    
- **使用者授權類型不正確或無法辨識的使用者名稱：** 使用者需要已獲得 Intune 或 EMS 授權。 檢閱這些文件以透過將授權指派： [Office 系統管理中心](https://docs.microsoft.com/intune/licenses-assign)或[Azure 入口網站](https://docs.microsoft.com/azure/active-directory/license-users-groups)。
    
其他資源，可以協助解決您的問題：
  
1. 使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷和解決常見註冊失敗。 檢閱[本文件](https://docs.microsoft.com/intune/help-desk-operators)如需詳細資訊。 
    
2. 檢閱這些文件的每個防止註冊和解決方法的常見錯誤清單：[疑難排解指南](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)和[疑難排解 doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。
    
3. [了解如何註冊 Microsoft Intune 中的 iOS 裝置](https://docs.microsoft.com/intune/ios-enroll)。
    

