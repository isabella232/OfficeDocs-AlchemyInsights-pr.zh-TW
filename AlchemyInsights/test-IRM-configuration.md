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
ms.openlocfilehash: 22430e2b8a00023f9922fd59d6fcabd308d08453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317223"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>測試新 OME 功能的 IRM 組配置

若要驗證您的 Microsoft 365 租用戶已設為使用新 OME 功能，在連線至 [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online-powershell) 時執行下列 cmdlets：


1. 執行 `Get-IRMConfiguration` 以檢查租用戶的 IRM 設定。 請確定已將這些值設定為 **True**：
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. 使用網域、寄件者電子郵件地址和收件者，執行 `Test-IRMConfiguration`。 如果未通過此測試，請調查您的 IRM 設定。

如需有關如何驗證 IRM 設定的詳細資訊，請參閱 [在 Exchange Online PowerShell 中驗證新的 OME 設定](https://docs.microsoft.com/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)。