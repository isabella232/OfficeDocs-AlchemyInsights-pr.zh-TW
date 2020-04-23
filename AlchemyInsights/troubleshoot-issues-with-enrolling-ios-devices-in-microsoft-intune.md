---
title: 在 Microsoft Intune 中登記 iOS 裝置的問題疑難排解
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736149"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>在 Microsoft Intune 中登記 iOS 裝置的問題疑難排解

立即查看下列資源，以解決您的問題。 
  
一些常見的錯誤訊息和解決步驟：
  
- 已**達到裝置 Cap**使用者已註冊的裝置數目超過裝置限制。 請檢查這些檔，以[移除裝置](https://docs.microsoft.com/intune/devices-wipe)或[變更裝置限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。
    
- **不支援此服務。無註冊原則：** 必須設定或更新 Apple Push Notification 服務（apn）。 如需如何執行此作業的指示，請參閱[本檔](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)。 
    
- **使用者授權類型無效或無法識別使用者名稱：** 使用者必須被指派 Intune 或 EMS 授權。 檢查這些檔，以指派授權至： [Office 系統管理中心](https://docs.microsoft.com/intune/licenses-assign)或[Azure 入口網站](https://docs.microsoft.com/azure/active-directory/license-users-groups)。
    
其他可協助您解決問題的資源：
  
1. 使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷及解決一般註冊失敗。 如需詳細資訊，請參閱[本檔](https://docs.microsoft.com/intune/help-desk-operators)。 
    
2. 請查看這些檔，以取得阻止每個專案之註冊和解析度的常見錯誤清單：[疑難排解指南](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)和[疑難排解 doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。
    
3. [瞭解如何在 Microsoft Intune 中註冊 iOS 裝置](https://docs.microsoft.com/intune/ios-enroll)。
    

