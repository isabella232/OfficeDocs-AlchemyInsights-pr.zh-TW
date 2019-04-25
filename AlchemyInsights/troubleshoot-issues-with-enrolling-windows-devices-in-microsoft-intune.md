---
title: 疑難排解問題註冊 Microsoft Intune 中的 Windows 裝置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390634"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>疑難排解問題註冊 Microsoft Intune 中的 Windows 裝置

請先檢閱下列資源以立即解決您的問題。 
  
一些常見的錯誤訊息及解決步驟：
  
 **無法安裝軟體，0x80cf4017:** 您的帳戶憑證已過期。 重新下載 Intune 管理主控台的電腦用戶端軟體封裝。 檢閱此文件的詳細資訊。 
  
 **錯誤碼 0x801c0003:** 在下列案例中，會發生錯誤： 
  
1. 使用者有多個裝置註冊比裝置的限制。 檢閱這些文件以[移除裝置](https://docs.microsoft.com/intune/devices-wipe)，或[變更裝置的限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。
    
2. 「 使用者可能會加入裝置到 Azure AD 」 設為"none"。 將它設為所有或選取使用者。 檢閱[此文件](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)的詳細資訊。 
    
3. 由其他使用者已經註冊裝置。 如果是這種情況，若要從 Azure Intune 主控台移除裝置，或手動重新嘗試之前取消裝置。
    
4. 裝置是 Windows 10 家用版。 僅限 Windows 10 專業版、 教育版和企業 Sku 可加入 Azure Active Directory。
    
其他資源，可以協助解決您的問題：
  
1. 使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷和解決常見註冊失敗。 檢閱[本文件](https://docs.microsoft.com/intune/help-desk-operators)如需詳細資訊。 
    
2. 檢閱這些文件的每個防止註冊和解決方法的常見錯誤清單：[疑難排解指南](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)和[疑難排解 doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。
    
[了解如何註冊 Microsoft Intune 中的 Windows 裝置](https://docs.microsoft.com/intune/windows-enroll)。
  

