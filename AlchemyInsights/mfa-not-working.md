---
title: MFA 的問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755122"
---
# <a name="issues-with-azure-mfa"></a>Azure MFA 的問題
有幾個事項可檢查使用者是否無法使用多重要素驗證 (MFA) 進行登入

1. 受影響的使用者可能會在 Azure Active Directory 入口網站中封鎖。 如果是這種情況，該特定使用者的驗證嘗試將會自動遭到拒絕。 [請依照本文中的步驟加以取消封鎖。](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. 如果解除封鎖使用者沒有説明，或使用者未封鎖，您可以嘗試為使用者重設 MFA，然後再次進行註冊程式。 [請依照本文中的步驟進行。](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

如果這是您第一次啟用 MFA，而且使用者無法登入非瀏覽器用戶端（例如 Outlook、Skype 等等），則您的 O365 訂閱上沒有啟用該 (Active Directory 驗證程式庫) 。 在此情況下，您將需要連線到 Exchange Online Powershell，並執行此 Cmdlet：  *Set-OrganizationConfig-OAuth2ClientProfileEnabled： $true*