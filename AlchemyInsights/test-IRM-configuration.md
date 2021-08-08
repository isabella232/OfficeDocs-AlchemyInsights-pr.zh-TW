---
title: 測試新 OME 功能的 IRM 組配置
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53908969"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>測試新 OME 功能的 IRM 組配置

若要驗證您的 Microsoft 365 租用戶已設為使用新 OME 功能，在連線至 [Exchange Online PowerShell](/powershell/exchange/exchange-online-powershell) 時執行下列 cmdlets：


1. 執行 `Get-IRMConfiguration` 以檢查租用戶的 IRM 設定。 請確定已將這些值設定為 **True**：
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. 使用網域、寄件者電子郵件地址和收件者，執行 `Test-IRMConfiguration`。 如果未通過此測試，請調查您的 IRM 設定。

如需有關如何驗證 IRM 設定的詳細資訊，請參閱 [在 Exchange Online PowerShell 中驗證新的 OME 設定](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)。