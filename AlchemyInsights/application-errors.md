---
title: 應用程式錯誤
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976893"
---
# <a name="application-errors"></a>應用程式錯誤

要尋找從 Azure Active Directory (Azure AD) Security Token Service (STS) 傳回的 **AADSTS 錯誤碼** 資訊嗎？ 請閱讀 [AZURE AD 驗證和授權錯誤碼](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) ，以找出 AADSTS 的錯誤描述、修正，以及一些建議的解決方法。

授權錯誤可能是幾個不同問題的結果，大部分會產生401或403錯誤。 例如，下列各項會導致授權錯誤：

- [存取權杖採集流程](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)不正確 
- 設定不良的 [許可權範圍](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- 缺乏 [同意](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

若要解決常見的授權錯誤，請嘗試下列與您接收的錯誤最接近的步驟。 可以套用超過一個以上的應用。

**401未授權的錯誤：您的權杖是否有效？**

確定您的應用程式在要求中呈現有效的存取權杖至 Microsoft Graph。 此錯誤通常表示 HTTP 驗證要求標頭中的存取權杖可能遺失，或是權杖無效或已過期。 強烈建議您使用 [Microsoft 驗證程式庫 (MSAL) ](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) ，以進行 access token 採集。 此外，如果您嘗試使用授與個人 Microsoft 帳戶的委派存取權杖來存取只支援工作或學校帳戶 (組織帳戶) 的 API，也可能會發生這個錯誤。

**403禁止訪問錯誤：是否已選擇正確的許可權集？**

請檢查您是否已根據您的應用程式所呼叫的 Microsoft Graph APIs 所要求的適當許可權集。 所有 Microsoft Graph API 參考方法主題都提供建議的最小特權許可權。 此外，使用者或系統管理員必須將這些許可權授與應用程式。 一般會透過同意頁面或使用 Azure 入口網站應用程式註冊 blade 授與許可權來授與許可權。 從應用程式的 [ **設定** ] 邊欄中，按一下 [ **必要許可權**]，然後按一下 **[授與許可權**]。

- [Microsoft Graph 許可權](https://docs.microsoft.com/graph/permissions-reference) 
- [瞭解 Azure AD 許可權和同意](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403禁止訪問錯誤：您的應用程式是否取得權杖，以符合所選的許可權？**

請確定要求或授與的許可權類型符合您的應用程式取得的訪問權杖類型。 您可能要求並授與應用程式的許可權，但使用委派的互動式程式碼流程權杖，而非用戶端認證程式的憑證權杖，或是要求和授與委派的許可權，但使用用戶端認證流程權杖，而不是委派的程式碼

- [代表使用者或委派的許可權取得存取權](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD hyper-v 2.0-OAuth 2.0 授權碼流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [在沒有使用者 (多工緩衝處理程式服務) 與應用程式許可權的情況下取得存取權](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD hyper-v 2.0-OAuth 2.0 用戶端認證流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403禁止訪問錯誤：重設密碼**

目前沒有任何應用程式許可權後臺服務可讓使用者密碼重設為服務的許可權。 只有使用互動式委派的程式碼流程與登入的系統管理員，才支援這些 APIs。

- [Microsoft Graph 許可權](https://docs.microsoft.com/graph/permissions-reference)

**403禁止訪問：使用者是否可以存取和授權？**

在委派的程式碼流程中，Microsoft Graph 會評估是否允許根據授與登入使用者所擁有之許可權的要求。 一般來說，此錯誤指出使用者沒有足夠的許可權可執行要求，或使用者未獲授權存取資料。 只有具備必要許可權或授權的使用者才可成功進行要求。

**403禁止訪問：您是否選取正確的資源 API？**

類似 Microsoft Graph 的 API 服務會檢查接收到的存取權杖中) 的 aud 宣告 (物件是否符合其自身所要求的值，如果不是，則會導致403禁止的錯誤。 導致此錯誤的常見錯誤是，嘗試使用 Azure AD Graph （已取得的 token） APIs、Outlook APIs 或 SharePoint/OneDrive APIs 來呼叫 Microsoft Graph (（或相反) ）。 確定您的應用程式) 資源 (或範圍已取得權杖，使其符合應用程式呼叫的 API。

**400錯誤要求或403禁止：使用者是否符合組織的條件式存取 (CA) 原則？**

根據組織的 CA 原則，透過您的應用程式存取 Microsoft Graph 資源的使用者，可能面臨的其他資訊不存在於最初取得應用程式的 access token 中。 在此情況下，您的應用程式會在呼叫 Microsoft Graph 時，在取得存取權杖或403時，收到具有 *insufficient_claims* 錯誤的 400 *interaction_required* 錯誤。 在這兩種情況下，錯誤回應都會包含其他可呈現給授權端點的資訊，以挑戰使用者 (如多重要素驗證或裝置註冊) 的其他資訊。

- [使用 MSAL 處理條件式存取挑戰 ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Azure Active Directory 條件式存取的開發人員指南](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
