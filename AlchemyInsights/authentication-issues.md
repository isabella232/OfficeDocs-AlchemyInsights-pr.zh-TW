---
title: 驗證問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976840"
---
# <a name="authentication-issues"></a>驗證問題

**正在尋找有關從 Azure Active Directory (Azure AD) Security Token Service (STS) 傳回的 AADSTS 錯誤碼資訊嗎？** 如需 AADSTS 錯誤描述、修正程式和建議的因應措施，請參閱 [Azure AD 驗證及授權錯誤碼](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) (部分機器翻譯)。

授權錯誤可能是由多個不同的問題所導致，其中大部分都會產生 401 或 403 錯誤。 例如，下列問題可能會導致授權錯誤：

- 不正確的[存取權杖取得流程](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) (部分機器翻譯) 
- 設定錯誤的 [權限範圍](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) (部分機器翻譯) 
- 缺少[同意](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent) (部分機器翻譯)

若要解決常見的授權錯誤，請嘗試以下所提供的與您收到錯誤最接近之步驟。 一個以上的步驟可能適用於您收到的錯誤。

**401 未經授權的錯誤：您的權杖是否有效？**

請確認您的應用程式向 Microsoft Graph 提供有效的存取權杖，做為要求的一部分。 此錯誤通常表示 HTTP 驗證要求標頭中的存取權杖可能遺失，或者權杖無效或已過期。 強烈建議您使用 Microsoft 驗證程式庫 (MSAL) 來取得存取權杖。 此外，如果您嘗試使用授權給個人 Microsoft 帳戶的委派存取權杖來存取只支援公司或學校帳戶 (組織帳戶) 的 API，可能會發生此錯誤。

**403 禁止錯誤：您是否已選擇正確的權限集？**

根據您應用程式呼叫的 Microsoft Graph API，確認您已要求正確的權限集。 所有 Microsoft Graph API 參考方法主題中提供建議的最低權限。 此外，必須由使用者或系統管理員授與這些權限給應用程式。 通常是透過同意頁面或 Azure 入口網站應用程式註冊刀鋒視窗的使用來授與權限。 從應用程式的 [設定] 刀鋒視窗中，按一下 [必要權限]，然後按一下 [授與權限]。 如需詳細資訊，請參閱：

- [Microsoft Graph 權限](https://docs.microsoft.com/graph/permissions-reference) (英文) 
- [了解 Azure AD 權限與同意](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) (部分機器翻譯)

**403 禁止錯誤：您的應用程式是否取得權杖以符合所選的權限？**

確保要求或授與的權限類型符合應用程式取得的存取權杖類型。 您可能會要求並授與應用程式權限，但使用委派的互動式程式碼流程權杖，而不是用戶端認證流程權杖，或要求並授與委派權限，但使用用戶端認證流程權杖，而不是委派的程式碼流程權杖。

如需取得權杖的詳細資訊，請參閱：

- [代表使用者和委派權限取得存取權](https://docs.microsoft.com/graph/auth-v2-user) (英文) 
- [Azure AD v2.0 - OAuth 2.0 授權碼流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) (部分機器翻譯) 
- [不需使用者 (精靈服務) 和應用程式權限就能存取](https://docs.microsoft.com/graph/auth-v2-service) (英文) 
- [Azure AD v2.0 - OAuth 2.0 用戶端認證流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) (部分機器翻譯)

**403 禁止錯誤：重設密碼**

目前沒有應用程式權限精靈服務到服務權限，以重設使用者密碼。 只有在使用互動式委派程式碼和登入系統管理員的流程中，才支援這些 API。 如需詳細資訊，請參閱 [Microsoft Graph 權限](https://docs.microsoft.com/graph/permissions-reference) (部分機器翻譯)。

**403 禁止：使用者是否擁有存取權且是否獲得授權？**

對於委派的程式碼流程，Microsoft Graph 會根據授與給該應用程式的權限和登入使用者所擁有的權限，評估是否允許該要求。 通常，此錯誤表示使用者的權限不足，無法執行要求 **或** 使用者未取得要存取之資料的授權。 只有具備所需權限或授權的使用者才能成功提出要求。

**403 禁止：您是否選取正確的資源 API？**

API 服務，例如 Microsoft Graph，檢查收到的存取權杖中的 *aud* 宣告 (對象) 是否符合其自身預期的值，如果沒有，則會發生 403 禁止錯誤。 導致此錯誤的常見錯誤是，嘗試使用 Azure AD Graph API、Outlook API 或 SharePoint/OneDrive API 所取得的權杖來呼叫 Microsoft Graph (反之亦然)。 請確認您的應用程式正在取得權杖的資源 (或範圍)，以符合應用程式正在呼叫的 API。

**400 錯誤要求或 403 禁止：使用者是否符合其組織的條件式存取 (CA) 原則？**

根據組織的條件式存取 (CA) 原則，透過應用程式存取 Microsoft Graph 資源的使用者，可能會面臨應用程式最初取得的存取權杖中沒有額外資訊。 在此情況下，您的應用程式會在存取權杖取得過程中收到 ***interaction_required* 400** 錯誤，或在呼叫 Microsoft Graph 時發生 ***insufficient_claims* 403** 錯誤。 在這兩種情況下，錯誤回應都包含可以提供給授權端點的額外信息，以詢問使用者是否需要其他資訊 (例如多重要素驗證或裝置註冊)。

如需關於條件式存取的詳細資訊，請參閱：

- [使用 MSAL 處理條件式存取挑戰](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Azure Active Directory 條件式存取的開發人員指引](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide) (英文)

**_Azure Active Directory 驗證程式庫 (ADAL)和 Azure AD Graph API (AAD Graph) 的終止支援_* _

- 從 2020 年 6 月 30 日起，我們不再將任何新功能新增至 Azure Active Directory 驗證程式庫 (ADAL) 和 Azure AD Graph API (AAD Graph)。 我們會繼續提供技術支援和安全性更新，但將不再提供功能更新。
- 從 2022 年 6 月 30 日起，我們將結束支援 ADAL 和 AAD Graph，並不再提供技術支援或安全性更新。
    - 在目前的 OS 版本上使用 ADAL 的應用程式將在此時間後繼續運作，但不會取得任何技術支援或安全性更新。
    - 在此時間之後使用 AAD Graph 的應用程式可能無法再收到 AAD Graph 端點的回應。

_ *ADAL 移轉**

我們建議您更新至 [Microsoft 驗證程式庫 (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) (部分機器翻譯)，其中包含最新的功能和安全性更新。 本建議是 Microsoft 在終止支援期限之前，將其應用程式遷移到 MSAL。 Microsoft 應用程式的目標是移轉到 MSAL，以確保應用程式從 MSAL 持續的安全性與功能增強中受益。

- [閱讀 ADAL 常見問題集](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) (部分機器翻譯) 
- [了解如何在每個平台上移轉應用程式](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) (部分機器翻譯) 
- 如果您需要協助了解您的哪些應用程式使用 ADAL，我們建議您檢閱所有應用程式的原始程式碼，如果適用的話，請向任何獨立軟體廠商 (ISV) 或應用程式提供者諮詢。 Microsoft 支援服務也可提供您租用戶的所有非 Microsoft ADAL 應用程式清單。

**AAD Graph 移轉**

如果應用程式使用 AAD Graph，請依照我們的指引，[將 Azure AD Graph 應用程式移轉至 Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true) (英文)。

- [我們的移轉檢查清單提供開始使用點](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) (英文)。 
- 您的 Azure 應用程式註冊入口網站顯示哪些應用程式正在使用 AAD Graph。 我們建議您檢閱所有應用程式的原始程式碼，如果適用的話，請向任何 ISV 或應用程式提供者諮詢。 Microsoft 支援服務也可為您提供租使用者中所有 AAD Graph 使用狀況的資訊。

 










