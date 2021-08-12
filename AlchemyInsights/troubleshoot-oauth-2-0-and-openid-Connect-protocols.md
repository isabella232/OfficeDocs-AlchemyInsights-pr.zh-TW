---
title: 疑難排解 OAuth 2.0 和 OpenID Connect 通訊協定
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: 7584d8f6f2e24812c1fdded76332edc6dd671034011e262c15756567cb467c26
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921034"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>疑難排解 OAuth 2.0 和 OpenID Connect 通訊協定

若要解決 OAuth 2.0 和 OpenID Connect 問題，請執行下列建議步驟：

請參閱下列與 OAuth 2.0 和 OpenID Connect 通訊協定之組態和疑難排解的相關文章：

- [Microsoft 身分識別平台和 OAuth 2.0 授權碼流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) (部分機器翻譯) - 本文說明如何使用任何語言直接對應用程式中的 **程式碼授權 (PKCE) 流程** 進行程式設計。
- [Microsoft 身分識別平台和 OAuth 2.0 用戶端認證流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) (部分機器翻譯) - 本文說明如何直接對應用程式中的 **用戶端認證流程** 進行程式設計。
- [Microsoft 身分識別平台和 OAuth 2.0 資源擁有者密碼認證](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) (部分機器翻譯) - 本文說明如何直接對應用程式中的 **ROPC 流程** 進行程式設計。
    - Microsoft 身分識別平台僅支援適用於 Azure AD 租用戶 (而非個人帳戶) 的 ROPC。 這表示您必須使用租用戶特定的端點 **(https://login.microsoftonline.com/{TenantId_or_Name})** 或 **組織** 端點。
    - 受邀加入 Azure AD 租用戶的個人帳戶無法使用 ROPC。
    - 沒有密碼的帳戶無法透過 ROPC 進行登入。 針對此案例，建議您改為針對應用程式使用不同的流程。
    - 如果使用者需要[多重要素驗證 (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) (部分機器翻譯) 登入應用程式，他們將被封鎖。
    - 在[混合式識別身分同盟](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (部分機器翻譯) 案例 (例如，用來驗證內部部署帳戶的 Azure AD 和 ADFS) 中不支援 ROPC。 如果使用者全頁重新導向至內部部署身分識別提供者，Azure AD 無法針對該身分識別提供者測試使用者名稱和密碼。 不過，[傳遞驗證](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) (部分機器翻譯) 支援 ROPC。
    - 混合式識別身分同盟案例的例外如下：將 **AllowCloudPasswordValidation** 的主領域探索原則設定為 **TRUE**，當內部部署密碼同步處理至雲端時，讓 ROPC 流程對同盟使用者有效。 如需詳細資訊，請參閱[針對舊版應用程式啟用同盟使用者的直接 ROPC 驗證](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) (部分機器翻譯) 
- [Microsoft 身分識別平台和 OAuth 2.0 代理者流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) (部分機器翻譯) - 本文說明如何直接對應用程式中的 **代理者 (OBO) 流程** 進行程式設計。
- [Microsoft 身分識別平台和 OpenID Connect 通訊協定](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) (部分機器翻譯) - 本文說明如何獨立於語言來實作 OpenID Connect 通訊協定，並說明如何在不使用任何 Microsoft 開放原始碼程式庫的情況下傳送和接收 HTTP 訊息。

**存取權杖**

[Microsoft 身分識別平台存取權杖](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) (部分機器翻譯) - 了解 API 如何驗證和使用存取權杖內的宣告。 本文中的所有文件 (除非有說明)，僅適用於針對您註冊的 API 所發行的權杖。 它不適用於針對 Microsoft 擁有的 API 所發行的權杖，也無法使用這些權杖來驗證 Microsoft 身分識別平台如何針對您建立的 API 發行權杖。

**應用程式設定**

[重新導向 URI (回覆 URL) 限制](https://docs.microsoft.com/azure/active-directory/develop/reply-url) (部分機器翻譯) - 了解如何設定重新導向 URI (回覆 URL)。 重新導向 URI 或回覆 URL 是授權伺服器成功授權應用程式並授與授權碼或存取權杖後，傳送使用者的位置。 授權伺服器會將代碼或權杖傳送至重新導向 URI；因此，您必須在應用程式註冊過程中註冊正確的位置。

**應用程式佈建**

[教學課程：針對 SCIM 端點進行開發和規劃佈建](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) (部分機器翻譯) - 本文說明如何建立 SCIM 端點，並與 AAD 佈建服務整合。


