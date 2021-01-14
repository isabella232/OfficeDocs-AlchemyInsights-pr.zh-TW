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
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="02678-102">將無縫 SSO 與我的內部部署應用程式整合的問題</span><span class="sxs-lookup"><span data-stu-id="02678-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="02678-103">若要疑難排解與內部部署應用程式整合無縫 SSO 的問題，請執行下列操作：</span><span class="sxs-lookup"><span data-stu-id="02678-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="02678-104">**建議的步驟**</span><span class="sxs-lookup"><span data-stu-id="02678-104">**Recommended steps**</span></span>

1. <span data-ttu-id="02678-105">若要將 **內部部署應用程式** 設定為 **透過應用程式 proxy 進行單一登入**，請參閱 [密碼保險存儲搭配應用程式 proxy 的單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)。</span><span class="sxs-lookup"><span data-stu-id="02678-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="02678-106">**疑難排解應用程式 Proxy 問題**：建議您先開始檢查疑難排解流程（ [調試應用程式 proxy 連接器問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)），以判斷是否正確設定應用程式 proxy 連接器。</span><span class="sxs-lookup"><span data-stu-id="02678-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="02678-107">如果您在連線至應用程式時仍然有問題，請遵循 [調試應用程式 Proxy 應用程式問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)中的疑難排解步驟。</span><span class="sxs-lookup"><span data-stu-id="02678-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="02678-108">您可以使用下列瀏覽器調試工具來 [識別 CORS 問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) ：</span><span class="sxs-lookup"><span data-stu-id="02678-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="02678-109">啟動瀏覽器，並流覽至 web 應用程式。</span><span class="sxs-lookup"><span data-stu-id="02678-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="02678-110">按 **F12** 以顯示調試主控台。</span><span class="sxs-lookup"><span data-stu-id="02678-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="02678-111">請嘗試再現交易，並複查主控台訊息。</span><span class="sxs-lookup"><span data-stu-id="02678-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="02678-112">CORS 違規產生有關原創的主控台錯誤。</span><span class="sxs-lookup"><span data-stu-id="02678-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="02678-113">無法解析某些 CORS 問題，例如當您的應用程式重新導向至 login.microsoftonline.com 以進行驗證，以及存取權杖到期時。</span><span class="sxs-lookup"><span data-stu-id="02678-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="02678-114">否則，CORS 呼叫會失敗。</span><span class="sxs-lookup"><span data-stu-id="02678-114">The CORS call then fails.</span></span> <span data-ttu-id="02678-115">此案例的解決方法是擴充存取權杖的存留期，以防止在使用者會話期間到期。</span><span class="sxs-lookup"><span data-stu-id="02678-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="02678-116">如需如何執行此動作的詳細資訊，請參閱 [Microsoft identity platform 中的可設定權杖生命週期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。</span><span class="sxs-lookup"><span data-stu-id="02678-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="02678-117">**建議的檔**</span><span class="sxs-lookup"><span data-stu-id="02678-117">**Recommended documents**</span></span>

- [<span data-ttu-id="02678-118">如何設定單一登入至應用程式 Proxy 應用程式</span><span class="sxs-lookup"><span data-stu-id="02678-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="02678-119">具有應用程式 Proxy 之內部部署應用程式的 SAML 單一登入</span><span class="sxs-lookup"><span data-stu-id="02678-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="02678-120">瞭解並解決 Azure Active Directory 應用程式 Proxy CORS 問題</span><span class="sxs-lookup"><span data-stu-id="02678-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="02678-121">針對應用程式 Proxy 的 Kerberos 限制委派設定疑難排解</span><span class="sxs-lookup"><span data-stu-id="02678-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)