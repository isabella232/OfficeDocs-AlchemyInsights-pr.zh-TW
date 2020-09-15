---
title: 在 Microsoft Intune 中註冊 Windows 裝置的問題疑難排解
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658869"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>在 Microsoft Intune 中註冊 Windows 裝置的問題疑難排解

立即查看下列資源，以解決您的問題。
  
一些常見的錯誤訊息和解決步驟：
  
 **無法安裝軟體，0x80cf4017：** 您的帳戶憑證已過期。 在 Intune 管理主控台中重新下載 PC 用戶端軟體套件。 如需詳細資訊，請參閱本檔。
  
 **錯誤碼0x801c0003：** 在下列情況中，可能會發生此錯誤：
  
-  使用者已註冊的裝置數目超過裝置限制。 請檢查這些檔，以 [移除裝置](https://docs.microsoft.com/intune/devices-wipe) 或 [變更裝置限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。

-  「使用者可以加入至 Azure AD 的裝置」設定為 "none"。 將它設定為 [全部] 或 [選取使用者]。 如需詳細資訊，請參閱 [本檔](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) 。

-  其他使用者已註冊此裝置。 如果是這種情況，請從 Azure Intune 主控台移除裝置，或手動取消註冊裝置，再重試。

-  裝置為 Windows 10 家用版。 只有 Windows 10 專業版、教育版和 Enterprise SKUs 可以加入 Azure Active Directory。

其他可協助您解決問題的資源：
  
-  使用 [Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 來診斷及解決一般註冊失敗。 如需詳細資訊，請參閱 [本檔](https://docs.microsoft.com/intune/help-desk-operators) 。

-  檢閱這些文件，以取得會防止註冊的常見錯誤清單與各項的解決方式：[疑難排解指南](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)和[疑難排解文件](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。

[瞭解如何在 Microsoft Intune 中註冊 Windows 裝置](https://docs.microsoft.com/intune/windows-enroll)。
