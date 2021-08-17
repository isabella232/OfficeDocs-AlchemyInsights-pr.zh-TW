---
title: 網域服務的密碼雜湊同步處理
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 3c00105a67f70ae9ce11cd8bb922c4d84a320010d021414b9159948f7dc87dbc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040857"
---
# <a name="password-hash-synchronization-for-domain-service"></a>網域服務的密碼雜湊同步處理

**如果您的 Azure AD DS 執行個體提示您啟用密碼雜湊同步處理**

在內部部署 Azure Active Directory Domain Services (AD DS) 環境同步處理使用者的情況下，您遇到執行混合式環境的情形。 如果將來自內部部署 AD DS 的密碼雜湊同步處理到 Azure AD 租用戶，就會發生此情況。

**原因**

發生這種情況的原因是，Azure AD Connect 預設不會同步處理 Azure AD DS 所需的舊版 New Technology LAN Manager (NTLM) 和 Kerberos 密碼雜湊。

**因應措施** 

您需要設定 Azure AD Connect，以同步處理 NTLM 和 Kerberos 驗證所需的密碼雜湊。

設定 Azure AD Connect 之後，內部部署帳戶建立或密碼變更事件也會同步處理到 Azure AD。 如需有關此功能的詳細資訊，以及如何在 Azure AD DS 混合式環境中啟用密碼同步處理的指導方針，請參閱[這裡](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync)。