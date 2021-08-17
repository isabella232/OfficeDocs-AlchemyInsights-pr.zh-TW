---
title: 疑難排解以 OIDC 為基礎的無縫單一登入 (SSO) 問題
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
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105756"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>疑難排解以 OIDC 為基礎的無縫單一登入 (SSO) 問題

- 若要瞭解如何將以 OIDC 為基礎的應用程式新增至您的 Azure 租使用者，請參閱[快速入門：針對 Azure Active Directory (Azure AD) 承租人中的應用程式，設定 OIDC 型單一登入 (SSO) ](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)。
- 如需使用 OpenID 連線 standard 以執行單一登入的應用程式的詳細資訊，請參閱[瞭解以 OIDC 為基礎的單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)。
- 如需以直接傳送和處理 HTTP 要求或使用協力廠商開放來源程式庫的方式撰寫程式碼的資訊，請參閱[OAuth 2.0 和 OpenID 連線的通訊協定 Microsoft 身分識別平臺](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)。

**通訊協定**

1. [Microsoft 身分識別平臺和隱含授與流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)-隱含授與的定義特性是指直接從/authorize 端點（而非/token 端點）傳回識別碼 (ID 權杖或存取) 權杖。 這通常是用來做為「混合式流程」的授權程式碼流程的一部分，也就是在 **/authorize 要求上檢索識別碼權杖的方式，以及授權碼**。 本文說明如何直接針對應用程式中的通訊協定，向 Azure AD 要求權杖。
2. [Microsoft 身分識別平臺和 OAuth 2.0 授權程式碼流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow)-OAuth 2.0 授權碼授與可用於裝置上安裝的應用程式，以存取受保護的資源，例如 web APIs。 使用 OAuth 2.0 的 Microsoft 身分識別平臺實現，您可以在行動裝置 **和桌面應用程式中新增登入和 API 存取**。 本文說明如何在應用程式中使用任何語言的通訊協定直接程式設計。
3. [Microsoft 身分識別平臺和 OpenID 連線通訊協定](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc)-當您使用 Microsoft 身分識別平臺 OpenID 連線的實施時，您可以新增應用程式的登入和 API 存取。 本文說明如何獨立于語言執行這項作業，並說明如何在 **不使用任何 Microsoft 開放來源庫的情況下傳送和接收 HTTP 郵件**。
4. [Microsoft 身分識別平臺和 OAuth 2.0 用戶端認證流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)-您可以使用 RFC 6749 中指定的 OAuth 2.0 用戶端認證授與（有時稱為 **legged OAuth**），以使用應用程式的身分識別來存取網路主控的資源。 這種類型的授與必須在後臺執行的伺服器對伺服器互動（無需立即與使用者互動）使用。 這些類型的應用程式通常稱為 **守護** 程式或 **服務帳戶**。 本文說明如何直接針對應用程式中的通訊協定進行程式設計。
