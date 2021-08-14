---
title: SSO 設定問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7760"
- "9004346"
ms.openlocfilehash: c843e9315776f3dbab2f25c864ebe8b0c41000b8ce70046fe4eb386fce143635
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54009563"
---
# <a name="sso-configuration-issues"></a>SSO 設定問題

1. 遵循[快速入門：針對應用程式設定屬性](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure)指南中的屬性來設定您的應用程式。
2. 視您選擇的應用程式和[單一登入選項](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options)而定，請遵循以下的適當指導方針：a. 若要設定 **內部部署應用程式** 使用 **SAML 型單一登入 (SSO)**，請參閱 [對使用應用程式 Proxy 的內部部署應用程式進行 SAML 單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)。
    b. 若要為 **密碼型 SSO** 設定 **雲端應用程式**，請參閱 [設定密碼單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)。
    c. 若要設定 **內部部署應用程式** 使用 **透過應用程式 Proxy 的 SSO**，請參閱 [用於使用應用程式 Proxy 單一登入的密碼保存庫](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)。
3. **疑難排解應用程式 Proxy 問題**：建議您從檢查疑難排解流程 [偵錯應用程式 Proxy 連接器問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)開始，以判斷是否正確已設定應用程式 Proxy 連接器。 如果您仍然無法連線到應用程式，請遵循[偵錯應用程式 Proxy 應用程式問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)中的疑難排解步驟進行。 您可以執行下列瀏覽器偵錯步驟來[識別 CORS 問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues)：a. 啟動瀏覽器並瀏覽至 Web 應用程式。
    b. 按 **F12** 以顯示偵錯主控台。
    c. 嘗試重現該交易，並檢閱主控台訊息。 CORS 違規產生關於來源的主控台錯誤。
    d. 某些 CORS 問題無法解決，例如，當您的應用程式重新導向到 login.microsoftonline.com 以進行驗證時，存取權杖到期。 由於存取權杖過期，CORS 呼叫會失敗。 此案例的因應措施是延長存取權杖的存留期，以避免它在使用者工作階段期間過期。 如需如何執行此作業的詳細資訊，請參閱 [Microsoft 身分識別平台中可設定的權杖生命週期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。
4. **疑難排解 SAML 型 SSO**：建議您查看 [登入設定 SAML 型單一登入的應用程式時發生問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)，以尋找您最可能遇到的問題的解決方案。
5. **疑難排解密碼型 SSO**：建議您查看 [疑難排解 Azure AD 中的密碼型單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)，以尋找您最可能遇到的問題的解決方案。
6. **我遇到設定錯誤**：若要疑難排解設定錯誤，建議您查看下列文章：a. [登入設定 SAML 型單一登入的應用程式時發生問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) b. [已填寫認證，但擴充功能未提交認證](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso#credentials-are-filled-in-but-the-extension-does-not-submit-them) c. [已填寫並提交認證，但是頁面指出認證不正確](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) d. [使用者登入後，應用程式頁面顯示錯誤訊息](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
7. **將無縫 SSO 與我的內部部署應用程式整合發生問題**：若要針對有關無縫 SSO 與內部部署應用程式整合的問題進行疑難排解，建議您查看下列文章：a. [如何設定單一登入到應用程式 Proxy 應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to) b. [對使用應用程式 Proxy 的內部部署應用程式進行 SAML 單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps) c. [了解並解決 Azure Active Directory 應用程式 Proxy CORS 問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues) d. [疑難排解應用程式 Proxy 的 Kerberos 限制委派設定](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)
8. **我需要修正宣告或延長權杖的存留期。我需要變更工作階段的長度**：若要這麼做，建議您查看下列文章：a. [自訂傳送到應用程式的 SAML 宣告](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) b. [使用宣告感知應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) c. [Microsoft 身分識別平台中可設定的權杖生命週期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) d. [使用條件式存取設定驗證工作階段管理](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) e. [用於存取內部部署應用程式的 Cookie 設定](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings)
9. **我需要協助管理使用者和來賓使用者的 (B2B) 存取**：如需有關管理使用者和來賓使用者的存取的詳細資訊，建議您查看下列文章：a. [管理應用程式的存取](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-access-management) b. [管理 Azure Active Directory 中應用程式的使用者指派](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) c. [設定適用於 B2B 共同作業的 SaaS 應用程式](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) d. [為 Azure AD 中的 B2B 使用者授與您的內部部署應用程式的存取](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) e. [使用 Azure AD B2B 共同作業為本機管理的合作夥伴帳戶授與的雲端資源的存取](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)
10. **我想要自訂我的應用程式**：如需有關自訂應用程式的詳細資訊，建議您查看下列文章：a. [設定使用 Azure AD 應用程式 Proxy 的自訂網域](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain) b. [為已發佈的應用程式設定自訂首頁](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-home-page) c. [萬用字元應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-wildcard)
11. **我在將應用程式從 AD FS 移轉至 Azure 時遇到問題**：若要針對將應用程式從 AD FS 移轉至 Azure 時遇到的問題進行疑難排解，建議您查看下列文章：a. [將應用程式驗證從 Active Directory 同盟服務移至 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/migrate-adfs-apps-to-azure) b. [用於將應用程式移轉至 Azure Active Directory 的資源](https://docs.microsoft.com/azure/active-directory/manage-apps/migration-resources)

