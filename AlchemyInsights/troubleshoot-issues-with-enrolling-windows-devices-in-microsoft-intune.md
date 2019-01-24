---
title: 疑難排解問題註冊 Microsoft Intune 中的 Windows 裝置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29460671"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>疑難排解問題註冊 Microsoft Intune 中的 Windows 裝置

請檢閱下面列出現在解決問題的資源。 
  
一些常見的錯誤訊息和解決步驟：
  
 **無法安裝軟體、 0x80cf4017:** 帳戶憑證已過期。重新下載 Intune 系統管理主控台的電腦用戶端軟體封裝。請檢閱此文件的詳細資訊。 
  
 **錯誤碼 0x801c0003:** 在下列情況會發生錯誤： 
  
1. 使用者有多個裝置註冊於裝置限制。檢閱這些文件[中移除裝置](https://docs.microsoft.com/en-us/intune/devices-wipe)或[變更裝置限制](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions)。
    
2. 「 使用者可能會加入裝置 Azure AD"設為"none"。將它設為所有或選取使用者。請檢閱[此文件](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings)的詳細資訊。 
    
3. 裝置已經由另一個使用者註冊。如果這是大小寫、 Azure Intune 主控台中移除裝置或手動重新嘗試之前 unenroll 裝置。
    
4. 裝置首頁 Windows 10。僅限 Windows 10 專業人員、 教育版與企業 Sku 可加入 Azure Active Directory。
    
若要協助解決問題的其他資源：
  
1. 使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷及解決常見的註冊失敗。請檢閱[本文件](https://docs.microsoft.com/en-us/intune/help-desk-operators)如需詳細資訊。 
    
2. 檢閱這些文件的每個防止註冊和解決方法的常見錯誤的清單：[疑難排解指南](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)及[疑難排解 doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。
    
[解如何註冊 Microsoft Intune 中的 Windows 裝置](https://docs.microsoft.com/en-us/intune/windows-enroll)。
  

