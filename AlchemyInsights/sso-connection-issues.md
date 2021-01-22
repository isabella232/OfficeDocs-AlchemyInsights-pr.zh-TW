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
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/21/2021
ms.locfileid: "49918136"
---
# <a name="sso-connection-issues"></a>SSO 連接問題

1. 遵循[快速入門：針對應用程式設定屬性](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure)指南中的屬性來設定您的應用程式。
2. 根據您選擇的應用程式和 [單一登入選項](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) ，請遵循下列適當的指引：
    - 若要為以 **SAML** 為基礎的單一登入設定內部部署應用程式，請參閱使用應用程式 Proxy 之內部部署應用程式的 [SAML 單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)。
    - 若要為以 **密碼****為基礎的單一** 登錄設定雲端應用程式，請參閱設定 [密碼單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)。
    - 若要 **透過應用程式** Proxy 設定單一登錄之內部部署應用程式，請參閱使用應用程式 Proxy 單一登入的密碼 [保存庫](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)。
3. **應用程式 Proxy** 問題疑難排解：建議您先檢查疑難排解流程、為 [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)應用程式 Proxy 連接器問題進行疑難排解，判斷應用程式 Proxy 連接器是否正確配置。 如果仍然無法連接到應用程式，請遵循針對應用程式 Proxy 應用程式問題進行疑難排解 [流程](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)。 您可以使用瀏覽器的錯錯工具來識別 [CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) 問題：
    - 啟動瀏覽器並瀏覽至 Web 應用程式。
    - 按 **F12** 以顯示偵錯主控台。
    - 嘗試重現交易，並查看主機訊息。 CORS 違規產生關於來源的主控台錯誤。
    - 某些 CORS 問題無法解決，例如當您的應用程式重新導向至 login.microsoft.com進行驗證時，存取權杖會過期。 然後 CORS 通話會失敗。 此案例的因應措施是延長存取權杖的存留期，以避免它在使用者工作階段期間過期。 如需如何執行此作業的詳細資訊，請參閱 [Microsoft 身分識別平台中可設定的權杖生命週期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。
4. **疑難排解以 SAML** 為基礎的單一登入：建議您檢查在以 [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)為基礎的單一登入已進行 App 的登錄問題，以找出最可能遇到的問題的解決方案。
5. **針對以密碼為基礎的單** 一登錄進行疑難排解：建議您檢查 [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)中以密碼為基礎的單一登入疑難排解，以找出最可能遇到的問題的解決方案。
6. 有關使用 VPN 時的連接問題，請參閱如何在 VPN 和 Wi-Fi SSO ([SSO](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)) 單一登入。
