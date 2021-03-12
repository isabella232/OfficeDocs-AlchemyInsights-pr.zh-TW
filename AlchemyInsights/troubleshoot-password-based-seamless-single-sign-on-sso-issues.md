---
title: 疑難排解以密碼為基礎的無縫單一登入 (SSO) 問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709492"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="fdcab-102">疑難排解以密碼為基礎的無縫單一登入 (SSO) 問題</span><span class="sxs-lookup"><span data-stu-id="fdcab-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="fdcab-103">若要瞭解密碼型 SSO 的基礎知識，請參閱以密碼為基礎的 [Azure Active Directory 驗證](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)。</span><span class="sxs-lookup"><span data-stu-id="fdcab-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="fdcab-104">**設定密碼型 SSO**</span><span class="sxs-lookup"><span data-stu-id="fdcab-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="fdcab-105">[設定密碼型單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) -本文將詳細說明密碼型 SSO 選項。</span><span class="sxs-lookup"><span data-stu-id="fdcab-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="fdcab-106">如果您要新增的應用程式需要自訂設定，而您需要使用以密碼為基礎的 SSO，則本文適用于您。</span><span class="sxs-lookup"><span data-stu-id="fdcab-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="fdcab-107">[針對部署的應用程式設定密碼型單一登入，](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) 應用程式 Proxy 支援數種單一登入模式。</span><span class="sxs-lookup"><span data-stu-id="fdcab-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="fdcab-108">密碼型登入適用于使用使用者名稱/密碼組合進行驗證的應用程式。</span><span class="sxs-lookup"><span data-stu-id="fdcab-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="fdcab-109">當您為應用程式設定密碼型簽入時，您的使用者必須登入內部部署應用程式一次。</span><span class="sxs-lookup"><span data-stu-id="fdcab-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="fdcab-110">之後，Azure Active Directory 會儲存登入資訊，並在使用者遠端存取它時，自動將其提供給應用程式。</span><span class="sxs-lookup"><span data-stu-id="fdcab-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="fdcab-111">您應該已經發佈並測試您的應用程式與應用程式 Proxy。</span><span class="sxs-lookup"><span data-stu-id="fdcab-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="fdcab-112">如果不是，請依照 [使用 AZURE AD 應用程式 Proxy 發行應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) 中的步驟，繼續設定部署應用程式的密碼型 SSO。</span><span class="sxs-lookup"><span data-stu-id="fdcab-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="fdcab-113">若要疑難排解以密碼為基礎的 SSO，請參閱 [在 AZURE AD 中疑難排解以密碼為基礎的單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="fdcab-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
