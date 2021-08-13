---
title: '設定無縫單一登入 (SSO) '
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966028"
---
# <a name="configure-seamless-single-sign-on-sso"></a>設定無縫單一登入 (SSO) 

**設定應用程式**

1. 您應該取得應用程式廠商的價值。 您可以手動輸入值或上傳元資料檔案，以提取欄位的值。
2. 許多應用程式已預先設定為搭配 Azure AD 使用。 在您將應用程式新增至 Azure AD 租使用者時，您可以流覽的應用程式庫中會列出這些應用程式。 [快速入門數列](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure)可引導您完成此程式。
3. 若要建立非圖庫應用程式，您可以按一下 [ **建立您自己的應用程式** ] 按鈕，並提供應用程式的名稱。
    - 根據預設，它會選取 **[整合沒有在圖庫中找到的任何其他應用程式** （非圖庫應用程式的正確選項）。
    - 當您在放置應用程式的名稱之後進行 [**建立**] 之後，它會建立新的非圖庫 Enterprise 應用程式。
    - 然後，您可以在該應用程式的 [**管理**] 下流覽 **單一登入**，這樣您就能看到在環境中執行它時所用的不同技術。

**為特定的應用程式設定無縫 SSO**

在圖庫中的應用程式中，您會找到詳細的逐步指示。 若要存取步驟，您可以在 [SaaS 應用程式設定教程](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)上流覽所有 app configuration 教學課程的清單。

**設定 SAML-based SSO**

1. [快速入門：針對 Azure Active Directory 中的應用程式，設定 SAML-based 單一登入 (SSO)  (Azure AD) 租使用者](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)。
2. 若要深入瞭解單一登入的 SAML-based 選項，請參閱 [瞭解 SAML-based 單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)。
3. 若要深入瞭解 Azure Active Directory (Azure AD) 支援單一 Sign-On (SSO) 的 saml 2.0 驗證要求和回應，請參閱[Single Sign-On SAML protocol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)。
4. 若要瞭解如何在 Azure Active Directory (Azure AD) 使用 microsoft Graph api 中的應用程式中建立及設定 SAML-based 單一登入 (SSO) ，請參閱[configure the SAML-based single sign for a 應用程式使用 microsoft Graph api](https://docs.microsoft.com/graph/application-saml-sso-configure-api)。
5. 若要瞭解 Azure AD 如何使用 saml 通訊協定，請參閱[Microsoft 身分識別平臺如何使用 saml 通訊協定](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)。

**設定權杖和宣告**

1. [操作方法：自訂在適用于企業應用程式的 SAML 權杖中發出的宣告](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)。
2. 若要瞭解如何使用 PowerShell 設定宣告，請參閱 how [to：自訂租使用者的宣告中的特定應用程式 (Preview) 中發出的宣告 ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)。
3. 若要瞭解如何設定選用宣告，請參閱 how [to：為您的應用程式提供選用的宣告](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)。
4. 若要瞭解如何使用目錄架構擴充屬性將使用者資料傳送至權杖宣告中的應用程式，請參閱 [在宣告中使用目錄架構擴充屬性](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)。
5. 若要瞭解如何設定權杖存留期，請參閱[Microsoft 身分識別平臺 (preview) 中的「可設定權杖生命週期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)」。
6. [設定權杖存留期原則 (預覽) ](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) -在本文中，我們將逐步說明可協助您將新規則強加于權杖生命週期的常見原則案例。 在此範例中，您將瞭解如何建立原則，以要求使用者在您的 web 應用程式中更頻繁地進行驗證。

**對 SSO 設定進行疑難排解**

- 如需 Azure Active Directory 無縫單一 Sign-On (無縫 SSO) 的常見問題，請參閱[Azure Active Directory 無縫單一 Sign-On：常見問題](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)。
- 如需 Azure Active Directory (Azure AD) 無縫單一 Sign-On (無縫 SSO) 的常見問題疑難排解資訊，請參閱[疑難排解 Azure Active Directory 無縫單一 Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)。
