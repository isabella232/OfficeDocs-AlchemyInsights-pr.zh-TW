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
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931440"
---
# <a name="application-errors"></a>應用程式錯誤

要尋找從 Azure Active Directory (Azure AD) Security Token Service (STS) 傳回之 **AADSTS 錯誤碼** 的資訊嗎？ 閱讀[Azure AD 驗證和授權錯誤碼](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)，以找出 AADSTS 的錯誤描述、修正，以及一些建議的解決方法。

授權錯誤可能是由多個不同的問題所導致，其中大部分都會產生 401 或 403 錯誤。 例如，下列各項會導致授權錯誤：

- 不正確的[存取權杖取得流程](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) (部分機器翻譯) 
- 設定錯誤的 [權限範圍](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) (部分機器翻譯) 
- 缺少[同意](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) (部分機器翻譯)

若要解決常見的授權錯誤，請嘗試下列與您接收的錯誤最接近的步驟。 可以套用超過一個以上的應用。

**401 未經授權的錯誤：您的權杖是否有效？**

確定您的應用程式在要求中提供有效的存取權杖給 Microsoft Graph。 此錯誤通常表示 HTTP 驗證要求標頭中的存取權杖可能遺失，或者權杖無效或已過期。 強烈建議您使用 [Microsoft 驗證程式庫 (MSAL) ](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) ，以進行 access token 採集。 此外，如果您嘗試使用授與個人 Microsoft 帳戶的委派存取權杖來存取只支援工作或學校帳戶 (組織帳戶) 的 API，也可能會發生這個錯誤。

**403 禁止錯誤：您是否已選擇正確的權限集？**

請檢查您是否已根據 Microsoft Graph APIs 應用程式呼叫要求正確的許可權集。 所有 Microsoft Graph API 參考方法主題中都提供建議的最小特權許可權。 此外，必須由使用者或系統管理員授與這些權限給應用程式。 一般會透過同意頁面或使用 Azure 入口網站應用程式註冊 blade 授與許可權來授與許可權。 從應用程式的 [設定] 刀鋒視窗中，按一下 [必要權限]，然後按一下 [授與權限]。

- [Microsoft Graph 權限](https://docs.microsoft.com/graph/permissions-reference) (英文) 
- [了解 Azure AD 權限與同意](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) (部分機器翻譯) 

**403 禁止錯誤：您的應用程式是否取得權杖以符合所選的權限？**

請確定要求或授與的許可權類型符合您的應用程式取得的訪問權杖類型。 您可能要求並授與應用程式的許可權，但使用委派的互動式程式碼流程權杖，而非用戶端認證程式的憑證權杖，或是要求和授與委派的許可權，但使用用戶端認證流程權杖，而不是委派的程式碼

- [代表使用者和委派權限取得存取權](https://docs.microsoft.com/graph/auth_v2_user) (英文) 
- [Azure AD v2.0 - OAuth 2.0 授權碼流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) (部分機器翻譯) 
- [不需使用者 (精靈服務) 和應用程式權限就能存取](https://docs.microsoft.com/graph/auth_v2_service) (英文) 
- [Azure AD v2.0 - OAuth 2.0 用戶端認證流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) (部分機器翻譯) 

**403 禁止錯誤：重設密碼**

目前沒有應用程式權限精靈服務到服務權限，以重設使用者密碼。 只有在使用互動式委派程式碼和登入系統管理員的流程中，才支援這些 API。

- [Microsoft Graph 權限](https://docs.microsoft.com/graph/permissions-reference) (英文)

**403 禁止：使用者是否擁有存取權且是否獲得授權？**

在委派的程式碼流程中，Microsoft Graph 會根據授與使用者所擁有的許可權以及已登入使用者的許可權，評估是否允許要求。 通常，此錯誤表示使用者的權限不足，無法執行要求或使用者未取得要存取之資料的授權。 只有具備所需權限或授權的使用者才能成功提出要求。

**403 禁止：您是否選取正確的資源 API？**

API 服務，如 Microsoft Graph 檢查接收到之存取權杖中的 aud 宣告 (物件) 是否與其所要求的值相符，如果不是，則會產生403禁止的錯誤。 導致此錯誤的常見錯誤是，嘗試使用 Azure AD Graph API、Outlook API 或 SharePoint/OneDrive API 所取得的權杖來呼叫 Microsoft Graph (反之亦然)。 請確認您的應用程式正在取得權杖的資源 (或範圍)，以符合應用程式正在呼叫的 API。

**400 錯誤要求或 403 禁止：使用者是否符合其組織的條件式存取 (CA) 原則？**

根據組織的 CA 原則，透過您的應用程式存取 Microsoft Graph 資源的使用者，可能面臨的其他資訊不會出現在先前取得的應用程式存取權杖中。 在此情況下，您的應用程式會在存取權杖取得過程中收到 *interaction_required* 400 錯誤，或在呼叫 Microsoft Graph 時發生 *insufficient_claims 403* 錯誤。 在這兩種情況下，錯誤回應都會包含其他可呈現給授權端點的資訊，以挑戰使用者 (如多重要素驗證或裝置註冊) 的其他資訊。

- [使用 MSAL 處理條件式存取挑戰 ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Azure Active Directory 條件式存取的開發人員指引](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide) (英文)
