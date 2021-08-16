---
title: 將無縫 SSO 與我的內部部署應用程式整合的問題
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028283"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>將無縫 SSO 與我的內部部署應用程式整合的問題

若要疑難排解與內部部署應用程式整合無縫 SSO 的問題，請執行下列操作：

**建議的步驟**

1. 若要將 **內部部署應用程式** 設定為 **透過應用程式 proxy 進行單一登入**，請參閱 [密碼保險存儲搭配應用程式 proxy 的單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)。
1. **疑難排解應用程式 Proxy 問題**：建議您先開始檢查疑難排解流程（ [調試應用程式 proxy 連接器問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)），以判斷是否正確設定應用程式 proxy 連接器。 如果您仍然無法連線到應用程式，請遵循[偵錯應用程式 Proxy 應用程式問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)中的疑難排解步驟進行。 您可以使用下列瀏覽器調試工具來 [識別 CORS 問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ：
    1. 啟動瀏覽器並瀏覽至 Web 應用程式。
    1. 按 **F12** 以顯示偵錯主控台。
    1. 請嘗試再現交易，並複查主控台訊息。 CORS 違規產生關於來源的主控台錯誤。
    1. 無法解析某些 CORS 問題，例如當您的應用程式重新導向至 login.microsoftonline.com 以進行驗證，以及存取權杖到期時。 否則，CORS 呼叫會失敗。 此案例的因應措施是延長存取權杖的存留期，以避免它在使用者工作階段期間過期。 如需如何執行此作業的詳細資訊，請參閱 [Microsoft 身分識別平台中可設定的權杖生命週期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。

**建議的文件**

- [如何設定單一登入至應用程式 Proxy 應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [具有應用程式 Proxy 之內部部署應用程式的 SAML 單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [瞭解並解決 Azure Active Directory 應用程式 Proxy CORS 問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [疑難排解應用程式 Proxy 的 Kerberos 限制委派設定](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)