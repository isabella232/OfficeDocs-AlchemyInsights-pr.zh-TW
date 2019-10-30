---
title: MFA 的問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768828"
---
# <a name="issues-with-azure-mfa"></a>Azure MFA 的問題
有幾個事項檢查是否使用者無法登入使用多重要素驗證 (MFA)

1. 受影響的使用者可能被封鎖在 Azure Active Directory 入口網站。 如果是這種情況，驗證嘗試的特定使用者會自動拒絕。 [請遵循本篇文章以解除封鎖這些檔案中的步驟。](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. 如果解除封鎖使用者沒有幫助或使用者不會遭到封鎖您可以嘗試使用重設使用者的 MFA，他們會再次經過註冊程序。 [請遵循本文中的步驟。](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

如果這是您已啟用的 MFA 和您的使用者都無法登入非瀏覽器用戶端，例如 Outlook、 Skype 等至第一次，或許 ADAL (Active Directory Authentication Library) 上未啟用您的 O365 訂閱。 在此情況下必須連線至 Exchange Online Powershell 並執行此 cmdlet:  *Set-organizationconfig-OAuth2ClientProfileEnabled: $true*