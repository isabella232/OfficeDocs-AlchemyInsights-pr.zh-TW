---
title: 'SAML 斷言 (權杖) '
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109231"
---
# <a name="saml-assertions-tokens"></a>SAML 斷言 (權杖) 

1. 安全性聲明標記語言 (SAML) token 是宣告的 XML 標記法。 根據預設，同盟安全性案例中的 SAML 權杖 Windows Communication Foundation (WCF) 會發佈權杖。 如需詳細資訊，請參閱 [SAML 權杖和宣告](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)。
2. Microsoft 身分識別平臺會在處理每個驗證流程時發出多種類型的安全性權杖。 [Saml 權杖宣告參考](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) 說明 saml 2.0 token 的格式、安全性特性和內容。
3. 遵循[Microsoft 身分識別平臺中可設定權杖生命週期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)的指導方針，瞭解如何設定權杖存留期。
4. 請依照 [本文](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) 所述的步驟，瞭解如何設定 AZURE AD SAML 權杖加密。
5. 在 Azure AD 中，您可以設定憑證簽署選項和憑證簽署演算法。 如需詳細資訊，請參閱[Azure Active Directory 中畫廊應用程式的 SAML 權杖中的高級憑證簽署選項](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)。
