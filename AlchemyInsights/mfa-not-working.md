---
title: MFA 的問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098593"
---
# <a name="issues-with-azure-mfa"></a>Azure MFA 的問題
有幾個事項可檢查使用者是否無法使用多重要素驗證 (MFA) 進行登入

1. 受影響的使用者可能會在 Azure Active Directory 入口網站中封鎖。 如果是這種情況，該特定使用者的驗證嘗試將會自動遭到拒絕。 [請依照本文中的步驟加以取消封鎖。](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. 如果解除封鎖使用者沒有説明，或使用者未封鎖，您可以嘗試為使用者重設 MFA，然後再次進行註冊程式。 [請依照本文中的步驟進行。](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

如果這是您第一次啟用 MFA，而且使用者無法登入非瀏覽器用戶端，例如，Outlook、Skype 等等，您的 O365 訂閱上可能並未啟用 ADAL (Active Directory 驗證程式庫) 。 在此情況下，您將需要連線到 Exchange Online Powershell，並執行此 Cmdlet： *Set-OrganizationConfig-OAuth2ClientProfileEnabled： $true*