---
title: 啟用 SMTP 驗證和疑難排解
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077642"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>啟用 SMTP 驗證和疑難排解

如果您想要為信箱啟用 SMTP 驗證，或您在嘗試向 Microsoft 365 驗證裝置或應用程式來轉送電子郵件時，遇到代碼為 5.7.57 或 5.7.3 或 5.7.139 的「用戶端未驗證」、「驗證失敗」或 "SmtpClientAuthentication" 錯誤，請執行這三個動作以解決問題：

1. 將 [啟用安全性預設值] 切換為 [否] 以停用 [Azure 安全性預設值](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) (部分機器翻譯)。

    a. 以安全性系統管理員、條件式存取系統管理員或全域系統管理員的身分登入 Azure 入口網站。<BR/>
    b. 瀏覽至 [Azure Active Directory] > [屬性] ****。<BR/>
    c. 選取 [管理安全性預設]。<BR/>
    d. 將 [啟用安全性預設值] 設定為 [否]。<BR/>
    e. 選取 [儲存]。

2. 在授權信箱上[啟用用戶端 SMTP 提交](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes)。

    a. 從 Microsoft 365 系統管理中心，移至 [作用中使用者]，然後選取使用者。<BR/>
    b. 前往 [郵件] 索引標籤，然後在 [電子郵件 App] 下選取 [管理電子郵件 App]。<BR/>
    d. 確定已勾選 (已啟用) [已驗證的 SMTP **]**。<BR/>
    e. 選取 [儲存變更]。<BR/>

3. 在授權信箱上[停用多重要素驗證 (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa)。

    a. 前往 Microsoft 365 系統管理中心，然後在左側瀏覽功能表中選取 [使用者] > [作用中使用者]。<BR/>
    b. 選取 [多重要素驗證]。<BR/>
    c. 選取使用者並停用 [多重要素驗證]。<BR/>
