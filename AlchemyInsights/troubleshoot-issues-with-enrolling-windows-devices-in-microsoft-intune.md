---
title: 在 Microsoft Intune 中對 Windows 裝置的註冊問題進行疑難排解
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: fa48b76fb49cdeef0734e77520c9bf95c150f317
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353528"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>在 Microsoft Intune 中對 Windows 裝置的註冊問題進行疑難排解

請查看下面所列的資源, 立即解決您的問題。
  
一些常見的錯誤訊息和解決步驟:
  
 **無法安裝軟體, 0x80cf4017:** 您的帳戶憑證已過期。 在 Intune 管理主控台中重新下載電腦用戶端軟體套件。 如需詳細資訊, 請參閱本檔。
  
 **錯誤碼 0x801c0003:** 在下列案例中, 可能會發生此錯誤:
  
1. 使用者所註冊的裝置數目超過裝置限制。 請查看這些檔, 以[移除裝置](https://docs.microsoft.com/intune/devices-wipe)或[變更裝置限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。

2. [使用者可以將裝置加入 Azure AD] 設定為 "none"。 將它設為 [所有] 或 [選取使用者]。 如需詳細資訊, 請參閱[本檔](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)。

3. 裝置已由另一位使用者註冊。 如果是這種情況, 請從 Azure Intune 主控台移除裝置, 或先手動取消註冊裝置, 再重試。

4. 裝置是 Windows 10 家用版。 只有 Windows 10 專業版、教育版和企業版 Sku 可以加入 Azure Active Directory。

可協助您解決問題的其他資源:
  
1. 使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷和解決常見的註冊失敗。 如需詳細資訊, 請參閱[本檔](https://docs.microsoft.com/intune/help-desk-operators)。

2. 請查看這些檔, 以取得防止每個專案的註冊和解析度的常見錯誤清單:[疑難排解指南](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)和[疑難排解 doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。

[瞭解如何在 Microsoft Intune 中註冊 Windows 裝置](https://docs.microsoft.com/intune/windows-enroll)。
