---
title: 451 4.7.0 暫時性伺服器錯誤。 請稍後再試。 PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: 16e16f087c2b13a9ad5fec7223b4f3395e42646e
ms.sourcegitcommit: 380ee556007d2be389b1a99795bca04bc1f9f60f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/27/2021
ms.locfileid: "53604916"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 暫時性伺服器錯誤。 請稍後再試。 PRX4

當您使用 SMTP 用戶端提交方法，透過智慧主機 "smtp.office365.com" 傳送電子郵件時，可能會面臨問題，並收到錯誤： "451 4.7.0 暫時性伺服器錯誤。 請稍後再試。 PRX4 大多是暫時的。 

請確認您未使用共用信箱進行 SMTP 用戶端提交，因為 SMTP 用戶端提交方法需要已授權的信箱才能傳送郵件。 不過，如果您不是使用共用信箱，但問題仍然存在，請檢查下列各項：

1. 執行此 PowerShell 命令，以在使用的授權信箱上啟用用戶端 SMTP 提交：

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    或

    1. 移至 Microsoft 365 系統管理中心 > 作用中 **使用者**]，然後選取使用者。
    1. 前往 [郵件] 索引標籤 > **電子郵件應用程式** > 選取 [ **管理電子郵件應用程式**] 
    1. 請確定已 (啟用) 檢查已 **驗證的 SMTP** 設定。
    1. 選取 **[儲存變更]**。
    
    若要對整個組織啟用 SMTP 驗證，請執行下列命令：

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **附注**：基於安全性考慮，建議您只對所使用的信箱啟用 SMTP 驗證。 [使用者層級] 設定會覆寫 [組織層級] 設定。

2. 透過切換停用 Azure 安全性預設值 **啟用安全性預設值** **：**

    1. 以安全性管理員、條件式存取管理員或全域管理員的身分登入 Azure 入口網站。
    1. 流覽至 Azure Active Directory >**  屬性**]，然後選取 [**管理安全性預設值**]。
    1. 設定 [ **啟用安全性預設值** ] 切換為 [ **否**]。
    1. 選取 **[儲存]**。

3. 在使用的授權信箱上，停用多重因素驗證 (MFA) 。

    1. 移至 [Microsoft 365 系統管理中心]，然後在左導覽功能表中，選擇 [**使用者** 作用  >  中 **使用者**]。
    1. 在 **[使用中的使用者]** 頁面中，選擇 **[多重要素驗證]**。
    1. 選取使用者，並停用 **多重要素驗證**。

