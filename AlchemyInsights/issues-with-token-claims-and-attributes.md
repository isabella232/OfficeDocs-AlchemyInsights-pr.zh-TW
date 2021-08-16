---
title: 權杖宣告和屬性的問題
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012875"
---
# <a name="issues-with-token-claims-and-attributes"></a>權杖宣告和屬性的問題

**Update、configure 或 remove token 宣告**

1. 透過使用 Azure Active Directory (Azure AD) ，您可以在授權的應用程式之後收到的回應權杖中，[為角色宣告自訂宣告類型](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)。
2. 應用程式開發人員可以在其 Azure AD 應用程式中使用選用的宣告，在傳送至其應用程式的標記中指定要使用的宣告。 如需詳細資訊，請參閱為 [您的應用程式提供選用的宣告](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)。
3. [使用 Azure Active Directory 設定應用程式的群組宣告](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)。
4. 若在您的應用程式中使用無縫單一登入，請參閱 [自訂宣告中在企業應用程式的 SAML 權杖中發出的宣告](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)。

**宣告屬性對應**

1. 若要使用 PowerShell 來設定宣告對應原則，請參閱 [自訂承租人中的特定應用程式在標記中發出的宣告 (Preview) ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)。
2. 目錄架構擴充屬性提供一種方式，可將其他資料儲存在使用者物件及其他目錄物件（例如群組、租使用者詳細資料、服務主體）上的 Azure Active Directory。 只有使用者物件上的分機屬性可用於發出宣告給應用程式。 [使用宣告中的目錄架構擴充屬性](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) 說明如何使用目錄架構擴充屬性，將使用者資料傳送至權杖宣告中的應用程式。

如需權杖宣告的詳細資訊，請參閱：

- [存取權杖中的宣告](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Id_token 中的宣告](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- 您可以期望的識別碼權杖和 Azure AD B2C 所發出之存取權杖的[宣告](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims)
- [SAML 權杖宣告參考](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
