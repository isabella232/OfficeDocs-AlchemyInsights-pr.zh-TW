---
title: 無縫 SSO 使用者登入問題
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
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/21/2021
ms.locfileid: "49919198"
---
# <a name="seamless-sso-user-sign-in-issues"></a><span data-ttu-id="75773-102">無縫 SSO 使用者登入問題</span><span class="sxs-lookup"><span data-stu-id="75773-102">Seamless SSO user sign-in issues</span></span>

<span data-ttu-id="75773-103">使用者驗證之後，瀏覽器將會快取使用者的認證，因此，在相同的瀏覽器上，應用程式會自動以相同的帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="75773-103">After the user is authenticated, the browser will cache the user's credentials, so that on the same browser, the application will automatically sign-in with the same account.</span></span> <span data-ttu-id="75773-104">這可能會使另一位使用者或單一使用者在一個裝置上登入多個帳戶變得很困難。</span><span class="sxs-lookup"><span data-stu-id="75773-104">This may make it difficult for another user or a single user to log into multiple accounts on one device.</span></span> <span data-ttu-id="75773-105">若要解決此事項：1。</span><span class="sxs-lookup"><span data-stu-id="75773-105">To solve this: 1.</span></span> <span data-ttu-id="75773-106">嘗試在另一個瀏覽器登入。</span><span class="sxs-lookup"><span data-stu-id="75773-106">Try signing in on another browser.</span></span> <span data-ttu-id="75773-107">2.</span><span class="sxs-lookup"><span data-stu-id="75773-107">2.</span></span> <span data-ttu-id="75773-108">請清除瀏覽器的快取和/或 cookie，然後再次嘗試登入。</span><span class="sxs-lookup"><span data-stu-id="75773-108">Clear the browser's cache and/or cookies and try signing in again.</span></span>

<span data-ttu-id="75773-109">如果您仍遇到登入問題，建議您先執行下列步驟，以診斷及自動化解決步驟：</span><span class="sxs-lookup"><span data-stu-id="75773-109">If you are still experiencing sign-in issues, we recommend the following to diagnose and automate the resolution steps:</span></span>

1. <span data-ttu-id="75773-110">安裝 [My Apps Secure Browser Extension](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) ，以協助 Azure Active Directory (azure AD) ，以在使用 Azure 入口網站中的測試體驗時，提供更好的診斷和解決方法。</span><span class="sxs-lookup"><span data-stu-id="75773-110">Install the [My Apps Secure Browser Extension](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) to help Azure Active Directory (Azure AD) to provide better diagnosis and resolutions when using the testing experience in the Azure portal.</span></span>
2. <span data-ttu-id="75773-111">使用 Azure 入口網站中 app configuration 頁面上的測試體驗，再現錯誤。</span><span class="sxs-lookup"><span data-stu-id="75773-111">Reproduce the error using the testing experience in the app configuration page in the Azure portal.</span></span> <span data-ttu-id="75773-112">若要深入瞭解，請參閱 [調試 SAML-based 單一登入應用程式](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)。</span><span class="sxs-lookup"><span data-stu-id="75773-112">To learn more, see [Debug SAML-based single sign-on applications](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).</span></span>
3. <span data-ttu-id="75773-113">如果您在 Azure 入口網站中使用 My Apps Secure Browser Extension 的測試體驗，您可以 **略過步驟 4**。</span><span class="sxs-lookup"><span data-stu-id="75773-113">If you use the testing experience in the Azure portal with the My Apps Secure Browser Extension, you can **skip step 4**.</span></span>
4. <span data-ttu-id="75773-114">若要開啟 [SAML-based 單一登入設定] 頁面：</span><span class="sxs-lookup"><span data-stu-id="75773-114">To open the SAML-based single sign-on configuration page:</span></span>
    - <span data-ttu-id="75773-115">開啟 [Azure 入口網站](https://portal.azure.com/) ，並以 **全域系統管理員** 或 **Coadmin** 登入。</span><span class="sxs-lookup"><span data-stu-id="75773-115">Open the [Azure portal](https://portal.azure.com/) and sign in as a **Global Administrator** or **Coadmin**.</span></span>
    - <span data-ttu-id="75773-116">選取主要左導覽功能表頂端的 [**所有服務**]，以開啟 **Azure Active Directory 擴充**。</span><span class="sxs-lookup"><span data-stu-id="75773-116">Open the **Azure Active Directory Extension** by selecting **All services** at the top of the main left-side navigation menu.</span></span>
    - <span data-ttu-id="75773-117">在 [篩選搜尋] 方塊中，輸入 "Azure Active Directory"，然後選取 **Azure Active directory** 專案。</span><span class="sxs-lookup"><span data-stu-id="75773-117">Type "Azure Active Directory" in the filter search box and select the **Azure Active Directory** item.</span></span>
    - <span data-ttu-id="75773-118">從 Azure Active Directory 左手手流覽功能表中選取 [ **企業應用程式** ]。</span><span class="sxs-lookup"><span data-stu-id="75773-118">Select **Enterprise Applications** from the Azure Active Directory left-hand navigation menu.</span></span>
    - <span data-ttu-id="75773-119">選取 [ **所有應用程式** ]，以查看所有應用程式的清單。</span><span class="sxs-lookup"><span data-stu-id="75773-119">Select **All Applications** to view a list of all your applications.</span></span> <span data-ttu-id="75773-120">如果您沒有看到您想要顯示的應用程式，請使用 [**所有應用程式] 清單** 頂端的 [**篩選**] 控制項，並將 [**顯示**] 選項設定為 [**所有應用程式**]。</span><span class="sxs-lookup"><span data-stu-id="75773-120">If you do not see the application you want show up here, use the **Filter** control at the top of the **All Applications List** and set the **Show** option to **All Applications**.</span></span>
    - <span data-ttu-id="75773-121">選取您要設定單一登入的應用程式。</span><span class="sxs-lookup"><span data-stu-id="75773-121">Select the application you want to configure for single sign-on.</span></span>
    - <span data-ttu-id="75773-122">在應用程式載入之後，從應用程式的左手流覽功能表中選取 [ **單一登入** ]。</span><span class="sxs-lookup"><span data-stu-id="75773-122">After the application loads, select **Single sign-on** from the application’s left-hand navigation menu.</span></span>
    - <span data-ttu-id="75773-123">選取 [ **SAML-BASED SSO**]。</span><span class="sxs-lookup"><span data-stu-id="75773-123">Select **SAML-based SSO**.</span></span>
5. <span data-ttu-id="75773-124">根據錯誤，若要深入瞭解建議遵循的步驟，請參閱登 [入 SAML-based 單一登入已設定之應用程式的問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)。</span><span class="sxs-lookup"><span data-stu-id="75773-124">Based on the error, to learn more about the recommended steps to follow, see [Problems signing in to SAML-based single sign-on configured apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).</span></span>
6. <span data-ttu-id="75773-125">若要疑難排解其他使用者簽署問題，請參閱下列指導：</span><span class="sxs-lookup"><span data-stu-id="75773-125">To troubleshoot other user sign-issues refer to the following guidance:</span></span>
    - [<span data-ttu-id="75773-126">單一 Sign-On SAML 通訊協定</span><span class="sxs-lookup"><span data-stu-id="75773-126">Single Sign-On SAML protocol</span></span>](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [<span data-ttu-id="75773-127">操作方法：使用 Azure Active Directory 報告疑難排解簽入錯誤</span><span class="sxs-lookup"><span data-stu-id="75773-127">How to: Troubleshoot sign-in errors using Azure Active Directory reports</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [<span data-ttu-id="75773-128">未預期的同意提示</span><span class="sxs-lookup"><span data-stu-id="75773-128">Unexpected consent prompt</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [<span data-ttu-id="75773-129">使用者同意錯誤</span><span class="sxs-lookup"><span data-stu-id="75773-129">User consent error</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [<span data-ttu-id="75773-130">從我的應用程式登入時發生問題</span><span class="sxs-lookup"><span data-stu-id="75773-130">Problems signing in from My Apps</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [<span data-ttu-id="75773-131">Application 登入頁面上的錯誤</span><span class="sxs-lookup"><span data-stu-id="75773-131">Error on application sign-in page</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [<span data-ttu-id="75773-132">登入 Microsoft 應用程式時的問題</span><span class="sxs-lookup"><span data-stu-id="75773-132">Problem signing into a Microsoft App</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
