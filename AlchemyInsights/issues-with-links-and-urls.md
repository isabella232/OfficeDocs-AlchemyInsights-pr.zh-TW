---
title: 連結和 URL 的問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707873"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="33851-102">連結和 URL 的問題</span><span class="sxs-lookup"><span data-stu-id="33851-102">Issues with links and URLs</span></span>

<span data-ttu-id="33851-103">重新導向 URI/回覆 URL (這兩個表示可互換) 是 Microsoft 身分識別平台用來傳回應用程式要求權杖的 URL。</span><span class="sxs-lookup"><span data-stu-id="33851-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="33851-104">如需這些 URL 的相關資訊，請參閱下列文章：</span><span class="sxs-lookup"><span data-stu-id="33851-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="33851-105">[驗證流程和應用程式案例](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - 每個案例的 [應用程式註冊 **]** 頁面中重新導向 URI 的相關資訊。</span><span class="sxs-lookup"><span data-stu-id="33851-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="33851-106">重新導向 URI/回覆 URL 限制和限制</span><span class="sxs-lookup"><span data-stu-id="33851-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="33851-107">**我不知道如何為我的應用程式註冊正確的重新導向 URI/回覆 URL**</span><span class="sxs-lookup"><span data-stu-id="33851-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="33851-108">使用您正在開發的應用程式登入時，如果登入對話方塊顯示 **AADSTS50011：要求中指定的回覆 URL 與為應用程式 <your app ID> 設定的回覆 URL 不符**，您需要將您的程式碼在對 Microsoft 身分識別平台的權杖要求中使用的重新導向 URI 新增至您的應用程式註冊。</span><span class="sxs-lookup"><span data-stu-id="33851-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="33851-109">若要新增回覆 URL，請移至 Azure 入口網站中 [應用程式註冊 **]** 頁面中的 [驗證 **]** 索引標籤，然後在 [重新導向 URI **]** 區段中新增項目。</span><span class="sxs-lookup"><span data-stu-id="33851-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="33851-110">您需要輸入的值取決於您正在建立的應用程式類型，如下所述：</span><span class="sxs-lookup"><span data-stu-id="33851-110">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="33851-111">針對單一頁面應用程式和 Web應用程式，則回覆 URL 是您應用程式中的 URL。</span><span class="sxs-lookup"><span data-stu-id="33851-111">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="33851-112">請參閱[單一頁面應用程式註冊](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri)或[使用 Azure 入口網站註冊 Web 應用程式](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="33851-112">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="33851-113">針對傳統型應用程式，您需要選擇的值取決於：</span><span class="sxs-lookup"><span data-stu-id="33851-113">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="33851-114">平台 (MacOS 與 Windows 或 Linux 不同)</span><span class="sxs-lookup"><span data-stu-id="33851-114">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="33851-115">取得權杖的方式 (互動式、使用裝置代碼流程、使用整合式 Windows 驗證 [IWA] 或使用使用者名稱/密碼)。</span><span class="sxs-lookup"><span data-stu-id="33851-115">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="33851-116">如需詳細資訊，請參閱[傳統型應用程式 - 應用程式註冊 - 重新導向 URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="33851-116">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="33851-117">針對行動裝置應用程式，重新導向 URI 取決於：</span><span class="sxs-lookup"><span data-stu-id="33851-117">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="33851-118">平台 (iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="33851-118">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="33851-119">用來建立您的應用程式的資訊，例如 iOS 中的組建識別碼，以及 Android 上的套件名稱和簽名雜湊。Azure 入口網站應用程式註冊將協助您。</span><span class="sxs-lookup"><span data-stu-id="33851-119">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="33851-120">如需詳細資訊，請參閱[平台設定和重新導向 URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)。</span><span class="sxs-lookup"><span data-stu-id="33851-120">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="33851-121">Web API 和某些取得權杖的無訊息方式 (IWA 和使用者名稱/密碼) 不需要重新導向 URI。</span><span class="sxs-lookup"><span data-stu-id="33851-121">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="33851-122">**我已部署我的 Web 應用程式，當我測試部署的應用程式時，收到回覆 URL 不相符的訊息**</span><span class="sxs-lookup"><span data-stu-id="33851-122">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="33851-123">為您要部署 Web 應用程式的所有位置新增重新導向 URI。</span><span class="sxs-lookup"><span data-stu-id="33851-123">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="33851-124">如需詳細資訊，請參閱[使用 Azure 入口網站註冊 Web 應用程式](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)。</span><span class="sxs-lookup"><span data-stu-id="33851-124">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="33851-125">在該位置部署應用程式之後，立即為該位置新增重新導向 URI。</span><span class="sxs-lookup"><span data-stu-id="33851-125">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="33851-126">**我無法註冊足夠數量的回覆 URL**</span><span class="sxs-lookup"><span data-stu-id="33851-126">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="33851-127">您是 ISV，您的每個客戶都有一或多個重新導向 URI。</span><span class="sxs-lookup"><span data-stu-id="33851-127">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="33851-128">您想要從 ADAL/Azure AD v1.0 移轉到 MSAL/Microsoft 身分識別平台，並且您達到[重新導向 URI 的數量上限](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris)。</span><span class="sxs-lookup"><span data-stu-id="33851-128">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="33851-129">若要解決此問題，請[將重新導向 URI 新增至與每個客戶對應的服務主體](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals)。</span><span class="sxs-lookup"><span data-stu-id="33851-129">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
