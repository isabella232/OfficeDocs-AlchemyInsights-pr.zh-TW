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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/13/2021
ms.locfileid: "49848769"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>將無縫 SSO 與我的內部部署應用程式整合的問題

若要疑難排解與內部部署應用程式整合無縫 SSO 的問題，請執行下列操作：

**建議的步驟**

1. 若要將 **內部部署應用程式** 設定為 **透過應用程式 proxy 進行單一登入**，請參閱 [密碼保險存儲搭配應用程式 proxy 的單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)。
1. **疑難排解應用程式 Proxy 問題**：建議您先開始檢查疑難排解流程（ [調試應用程式 proxy 連接器問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)），以判斷是否正確設定應用程式 proxy 連接器。 如果您在連線至應用程式時仍然有問題，請遵循 [調試應用程式 Proxy 應用程式問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)中的疑難排解步驟。 您可以使用下列瀏覽器調試工具來 [識別 CORS 問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ：
    1. 啟動瀏覽器，並流覽至 web 應用程式。
    1. 按 **F12** 以顯示調試主控台。
    1. 請嘗試再現交易，並複查主控台訊息。 CORS 違規產生有關原創的主控台錯誤。
    1. 無法解析某些 CORS 問題，例如當您的應用程式重新導向至 login.microsoftonline.com 以進行驗證，以及存取權杖到期時。 否則，CORS 呼叫會失敗。 此案例的解決方法是擴充存取權杖的存留期，以防止在使用者會話期間到期。 如需如何執行此動作的詳細資訊，請參閱 [Microsoft identity platform 中的可設定權杖生命週期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。

**建議的檔**

- [如何設定單一登入至應用程式 Proxy 應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [具有應用程式 Proxy 之內部部署應用程式的 SAML 單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [瞭解並解決 Azure Active Directory 應用程式 Proxy CORS 問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [針對應用程式 Proxy 的 Kerberos 限制委派設定疑難排解](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)