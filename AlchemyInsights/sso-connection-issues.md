---
title: SSO 連接問題
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
- "9004357"
- "7810"
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084337"
---
# <a name="sso-connection-issues"></a>SSO 連接問題

1. 遵循[快速入門：針對應用程式設定屬性](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure)指南中的屬性來設定您的應用程式。
2. 根據您所選擇的 [應用程式] 和 [ [單一登入] 選項](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) ，遵循下列適當的指導：
    - 若要設定 **內部部署應用程式** **SAML-based 單一登入**，請參閱內部 [部署應用程式的 SAML 單一登入與應用程式 Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)。
    - 若要設定 **cloud 應用程式** 的 **密碼型單一登入**，請參閱  [設定密碼單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)。
    - 若要將 **內部部署應用程式** 設定為 **透過應用程式 proxy 進行單一登入**，請參閱 [密碼保險存儲搭配應用程式 proxy 的單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)。
3. **疑難排解應用程式 Proxy 問題**：我們建議您先查看疑難排解流程（ [調試應用程式 proxy 連接器問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)），以判斷應用程式 proxy 連接器是否設定正確。 如果您在連線至應用程式時仍然有問題，請遵循 [調試應用程式 Proxy 應用程式的問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)中的疑難排解流程。 您可以使用瀏覽器調試工具來 [識別 CORS 問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ：
    - 啟動瀏覽器並瀏覽至 Web 應用程式。
    - 按 **F12** 以顯示偵錯主控台。
    - 請嘗試再現交易，並複查主控台訊息。 CORS 違規產生關於來源的主控台錯誤。
    - 無法解析某些 CORS 問題，例如當您的應用程式重新導向至 login.microsoft.com 以進行驗證，以及存取權杖到期時。 否則，CORS 呼叫會失敗。 此案例的因應措施是延長存取權杖的存留期，以避免它在使用者工作階段期間過期。 如需如何執行此作業的詳細資訊，請參閱 [Microsoft 身分識別平台中可設定的權杖生命週期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。
4. **疑難排解 SAML-based 單一登入**：我們建議您檢查登 [入 SAML-based 單一登入已設定的應用程式的問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)，以找出您最可能遇到之問題的解決方案。
5. **疑難排解密碼型單一登入**：建議您 [在 Azure AD 中檢查密碼型單一登入的疑難排解](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)，以找出您最可能遇到之問題的解決方案。
6. 如需使用 VPN 的連線問題，請參閱 how [to use single 登 (SSO) OVER VPN 和 Wi-Fi](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)連線。
