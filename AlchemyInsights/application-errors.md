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
# <a name="application-errors"></a><span data-ttu-id="b7b8b-102">應用程式錯誤</span><span class="sxs-lookup"><span data-stu-id="b7b8b-102">Application errors</span></span>

<span data-ttu-id="b7b8b-103">要尋找從 Azure Active Directory (Azure AD) Security Token Service (STS) 傳回的 **AADSTS 錯誤碼** 資訊嗎？</span><span class="sxs-lookup"><span data-stu-id="b7b8b-103">Looking for info about the **AADSTS error codes** that are returned from the Azure Active Directory (Azure AD) security token service (STS)?</span></span> <span data-ttu-id="b7b8b-104">請閱讀 [AZURE AD 驗證和授權錯誤碼](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) ，以找出 AADSTS 的錯誤描述、修正，以及一些建議的解決方法。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-104">Read [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>

<span data-ttu-id="b7b8b-105">授權錯誤可能是幾個不同問題的結果，大部分會產生401或403錯誤。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-105">Authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="b7b8b-106">例如，下列各項會導致授權錯誤：</span><span class="sxs-lookup"><span data-stu-id="b7b8b-106">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="b7b8b-107">[存取權杖採集流程](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)不正確</span><span class="sxs-lookup"><span data-stu-id="b7b8b-107">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)</span></span> 
- <span data-ttu-id="b7b8b-108">設定不良的 [許可權範圍](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="b7b8b-108">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span> 
- <span data-ttu-id="b7b8b-109">缺乏 [同意](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="b7b8b-109">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="b7b8b-110">若要解決常見的授權錯誤，請嘗試下列與您接收的錯誤最接近的步驟。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-110">To resolve common authorization errors, try the steps provided below that most closely matches the error you are receiving.</span></span> <span data-ttu-id="b7b8b-111">可以套用超過一個以上的應用。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-111">More than one may apply.</span></span>

<span data-ttu-id="b7b8b-112">**401未授權的錯誤：您的權杖是否有效？**</span><span class="sxs-lookup"><span data-stu-id="b7b8b-112">**401 Unauthorized error: Is your token valid?**</span></span>

<span data-ttu-id="b7b8b-113">確定您的應用程式在要求中呈現有效的存取權杖至 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-113">Ensure that your application is presenting a valid access token to Microsoft Graph as part of the request.</span></span> <span data-ttu-id="b7b8b-114">此錯誤通常表示 HTTP 驗證要求標頭中的存取權杖可能遺失，或是權杖無效或已過期。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-114">This error often means that the access token may be missing in the HTTP authenticate request header or that the token is invalid or has expired.</span></span> <span data-ttu-id="b7b8b-115">強烈建議您使用 [Microsoft 驗證程式庫 (MSAL) ](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) ，以進行 access token 採集。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-115">We strongly recommend that you use the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) for access token acquisition.</span></span> <span data-ttu-id="b7b8b-116">此外，如果您嘗試使用授與個人 Microsoft 帳戶的委派存取權杖來存取只支援工作或學校帳戶 (組織帳戶) 的 API，也可能會發生這個錯誤。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-116">Additionally this error may occur if you try to use a delegated access token granted to a personal Microsoft account to access an API that only supports work or school accounts (organizational accounts).</span></span>

<span data-ttu-id="b7b8b-117">**403禁止訪問錯誤：是否已選擇正確的許可權集？**</span><span class="sxs-lookup"><span data-stu-id="b7b8b-117">**403 Forbidden error: Have you chosen the right set of permissions?**</span></span>

<span data-ttu-id="b7b8b-118">請檢查您是否已根據您的應用程式所呼叫的 Microsoft Graph APIs 所要求的適當許可權集。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-118">Check that you have requested the correct set of permissions based on the Microsoft Graph APIs your app calls.</span></span> <span data-ttu-id="b7b8b-119">所有 Microsoft Graph API 參考方法主題都提供建議的最小特權許可權。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-119">Recommended least privileged permissions are provided in all the Microsoft Graph API reference method topics.</span></span> <span data-ttu-id="b7b8b-120">此外，使用者或系統管理員必須將這些許可權授與應用程式。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-120">Additionally, those permissions must be granted to the application by a user or an administrator.</span></span> <span data-ttu-id="b7b8b-121">一般會透過同意頁面或使用 Azure 入口網站應用程式註冊 blade 授與許可權來授與許可權。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-121">Granting permissions normally happens through a consent page or by granting permissions using the Azure Portal application registration blade.</span></span> <span data-ttu-id="b7b8b-122">從應用程式的 [ **設定** ] 邊欄中，按一下 [ **必要許可權**]，然後按一下 **[授與許可權**]。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-122">From the **Settings** blade for the application, click **Required Permissions**, and then click **Grant Permissions**.</span></span>

- [<span data-ttu-id="b7b8b-123">Microsoft Graph 許可權</span><span class="sxs-lookup"><span data-stu-id="b7b8b-123">Microsoft Graph permissions</span></span>](https://docs.microsoft.com/graph/permissions-reference) 
- [<span data-ttu-id="b7b8b-124">瞭解 Azure AD 許可權和同意</span><span class="sxs-lookup"><span data-stu-id="b7b8b-124">Understanding Azure AD permissions and consent</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

<span data-ttu-id="b7b8b-125">**403禁止訪問錯誤：您的應用程式是否取得權杖，以符合所選的許可權？**</span><span class="sxs-lookup"><span data-stu-id="b7b8b-125">**403 Forbidden error: Did your app acquire a token to match chosen permissions?**</span></span>

<span data-ttu-id="b7b8b-126">請確定要求或授與的許可權類型符合您的應用程式取得的訪問權杖類型。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-126">Make sure that the type of permissions requested or granted matches the type of access token that your app acquires.</span></span> <span data-ttu-id="b7b8b-127">您可能要求並授與應用程式的許可權，但使用委派的互動式程式碼流程權杖，而非用戶端認證程式的憑證權杖，或是要求和授與委派的許可權，但使用用戶端認證流程權杖，而不是委派的程式碼</span><span class="sxs-lookup"><span data-stu-id="b7b8b-127">You might be requesting and granting application permissions but using delegated interactive code flow tokens instead of client credential flow tokens, or requesting and granting delegated permissions but using client credential flow tokens instead of delegated code flow tokens.</span></span>

- [<span data-ttu-id="b7b8b-128">代表使用者或委派的許可權取得存取權</span><span class="sxs-lookup"><span data-stu-id="b7b8b-128">Get access on behalf of users and delegated permissions</span></span>](https://docs.microsoft.com/graph/auth_v2_user) 
- [<span data-ttu-id="b7b8b-129">Azure AD hyper-v 2.0-OAuth 2.0 授權碼流程</span><span class="sxs-lookup"><span data-stu-id="b7b8b-129">Azure AD v2.0 - OAuth 2.0 authorization code flow</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [<span data-ttu-id="b7b8b-130">在沒有使用者 (多工緩衝處理程式服務) 與應用程式許可權的情況下取得存取權</span><span class="sxs-lookup"><span data-stu-id="b7b8b-130">Get access without a user (daemon service) and application permissions</span></span>](https://docs.microsoft.com/graph/auth_v2_service) 
- [<span data-ttu-id="b7b8b-131">Azure AD hyper-v 2.0-OAuth 2.0 用戶端認證流程</span><span class="sxs-lookup"><span data-stu-id="b7b8b-131">Azure AD v2.0 - OAuth 2.0 client credentials flow</span></span>](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

<span data-ttu-id="b7b8b-132">**403禁止訪問錯誤：重設密碼**</span><span class="sxs-lookup"><span data-stu-id="b7b8b-132">**403 Forbidden error: Resetting password**</span></span>

<span data-ttu-id="b7b8b-133">目前沒有任何應用程式許可權後臺服務可讓使用者密碼重設為服務的許可權。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-133">Currently, there are no application permission daemon service-to-service permissions that allow resetting user passwords.</span></span> <span data-ttu-id="b7b8b-134">只有使用互動式委派的程式碼流程與登入的系統管理員，才支援這些 APIs。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-134">These APIs are only supported using the interactive delegated code flows with a signed-in administrator.</span></span>

- [<span data-ttu-id="b7b8b-135">Microsoft Graph 許可權</span><span class="sxs-lookup"><span data-stu-id="b7b8b-135">Microsoft Graph permissions</span></span>](https://docs.microsoft.com/graph/permissions-reference)

<span data-ttu-id="b7b8b-136">**403禁止訪問：使用者是否可以存取和授權？**</span><span class="sxs-lookup"><span data-stu-id="b7b8b-136">**403 Forbidden: Does the user have access and are they licensed?**</span></span>

<span data-ttu-id="b7b8b-137">在委派的程式碼流程中，Microsoft Graph 會評估是否允許根據授與登入使用者所擁有之許可權的要求。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-137">For delegated code flows, Microsoft Graph evaluates if the request is allowed based on the permissions granted to the app and the permissions that the signed-in user has.</span></span> <span data-ttu-id="b7b8b-138">一般來說，此錯誤指出使用者沒有足夠的許可權可執行要求，或使用者未獲授權存取資料。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-138">Generally, this error indicates that the user is not privileged enough to perform the request or the user is not licensed for the data being accessed.</span></span> <span data-ttu-id="b7b8b-139">只有具備必要許可權或授權的使用者才可成功進行要求。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-139">Only users with the required permissions or licenses can make the request successfully.</span></span>

<span data-ttu-id="b7b8b-140">**403禁止訪問：您是否選取正確的資源 API？**</span><span class="sxs-lookup"><span data-stu-id="b7b8b-140">**403 Forbidden: Did you select the correct resource API?**</span></span>

<span data-ttu-id="b7b8b-141">類似 Microsoft Graph 的 API 服務會檢查接收到的存取權杖中) 的 aud 宣告 (物件是否符合其自身所要求的值，如果不是，則會導致403禁止的錯誤。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-141">API services like Microsoft Graph check that the aud claim (audience) in the received access token matches the value it expects for itself, and if not, it results in a 403 Forbidden error.</span></span> <span data-ttu-id="b7b8b-142">導致此錯誤的常見錯誤是，嘗試使用 Azure AD Graph （已取得的 token） APIs、Outlook APIs 或 SharePoint/OneDrive APIs 來呼叫 Microsoft Graph (（或相反) ）。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-142">A common mistake resulting in this error is trying to use a token acquired for Azure AD Graph APIs, Outlook APIs, or SharePoint/OneDrive APIs to call Microsoft Graph (or vice versa).</span></span> <span data-ttu-id="b7b8b-143">確定您的應用程式) 資源 (或範圍已取得權杖，使其符合應用程式呼叫的 API。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-143">Ensure that the resource (or scope) your app is acquiring a token for matches the API that the app is calling.</span></span>

<span data-ttu-id="b7b8b-144">**400錯誤要求或403禁止：使用者是否符合組織的條件式存取 (CA) 原則？**</span><span class="sxs-lookup"><span data-stu-id="b7b8b-144">**400 Bad Request or 403 Forbidden: Does the user comply with their organization's conditional access (CA) policies?**</span></span>

<span data-ttu-id="b7b8b-145">根據組織的 CA 原則，透過您的應用程式存取 Microsoft Graph 資源的使用者，可能面臨的其他資訊不存在於最初取得應用程式的 access token 中。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-145">Based on an organization's CA policies, a user accessing Microsoft Graph resources via your app may be challenged for additional information that is not present in the access token your app originally acquired.</span></span> <span data-ttu-id="b7b8b-146">在此情況下，您的應用程式會在呼叫 Microsoft Graph 時，在取得存取權杖或403時，收到具有 *insufficient_claims* 錯誤的 400 *interaction_required* 錯誤。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-146">In this case, your app receives a 400 with an *interaction_required* error during access token acquisition or a 403 with *insufficient_claims* error when calling Microsoft Graph.</span></span> <span data-ttu-id="b7b8b-147">在這兩種情況下，錯誤回應都會包含其他可呈現給授權端點的資訊，以挑戰使用者 (如多重要素驗證或裝置註冊) 的其他資訊。</span><span class="sxs-lookup"><span data-stu-id="b7b8b-147">In both cases, the error response contains additional information that can be presented to the authorize endpoint to challenge the user for additional information (like multi-factor authentication or device enrollment).</span></span>

- [<span data-ttu-id="b7b8b-148">使用 MSAL 處理條件式存取挑戰 </span><span class="sxs-lookup"><span data-stu-id="b7b8b-148">Handling conditional access challenges using MSAL </span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [<span data-ttu-id="b7b8b-149">Azure Active Directory 條件式存取的開發人員指南</span><span class="sxs-lookup"><span data-stu-id="b7b8b-149">Developer guidance for Azure Active Directory conditional access</span></span>](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
