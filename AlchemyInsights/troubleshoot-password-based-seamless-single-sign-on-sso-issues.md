---
title: 疑難排解以密碼為基礎的無縫單一登入 (SSO) 問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709492"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>疑難排解以密碼為基礎的無縫單一登入 (SSO) 問題

若要瞭解密碼型 SSO 的基礎知識，請參閱以密碼為基礎的 [Azure Active Directory 驗證](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)。

**設定密碼型 SSO**

1. [設定密碼型單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) -本文將詳細說明密碼型 SSO 選項。 如果您要新增的應用程式需要自訂設定，而您需要使用以密碼為基礎的 SSO，則本文適用于您。
2. [針對部署的應用程式設定密碼型單一登入，](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) 應用程式 Proxy 支援數種單一登入模式。 密碼型登入適用于使用使用者名稱/密碼組合進行驗證的應用程式。 當您為應用程式設定密碼型簽入時，您的使用者必須登入內部部署應用程式一次。 之後，Azure Active Directory 會儲存登入資訊，並在使用者遠端存取它時，自動將其提供給應用程式。
    - 您應該已經發佈並測試您的應用程式與應用程式 Proxy。 如果不是，請依照 [使用 AZURE AD 應用程式 Proxy 發行應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) 中的步驟，繼續設定部署應用程式的密碼型 SSO。

若要疑難排解以密碼為基礎的 SSO，請參閱 [在 AZURE AD 中疑難排解以密碼為基礎的單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
