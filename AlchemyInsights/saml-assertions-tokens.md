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
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884566"
---
# <a name="saml-assertions-tokens"></a>SAML 斷言 (權杖) 

1. 安全性聲明標記語言 (SAML) token 是宣告的 XML 標記法。 依預設，同盟安全性案例中 (WCF) 使用的 SAML 權杖 Windows Communication Foundation 是由發行的權杖使用。 如需詳細資訊，請參閱 [SAML 權杖和宣告](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)。
2. Microsoft identity 平臺會在處理每個驗證流程時發出多種類型的安全性權杖。 [Saml 權杖宣告參考](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) 說明 saml 2.0 token 的格式、安全性特性和內容。
3. 遵循 [Microsoft identity 平臺的可設定權杖生命週期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) 中的指導方針，以瞭解如何設定權杖存留期。
4. 請依照 [本文](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) 所述的步驟，瞭解如何設定 AZURE AD SAML 權杖加密。
5. 在 Azure AD 中，您可以設定憑證簽署選項和憑證簽署演算法。 如需詳細資訊，請參閱在 [Azure Active Directory 中的畫廊應用程式的 SAML 權杖中的「高級憑證簽署選項](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)」。
