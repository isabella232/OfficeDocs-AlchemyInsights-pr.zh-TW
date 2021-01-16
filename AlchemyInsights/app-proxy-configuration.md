---
title: 應用程式 Proxy 設定
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876542"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="5ed87-102">應用程式 Proxy 設定</span><span class="sxs-lookup"><span data-stu-id="5ed87-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="5ed87-103">若要瞭解如何在 Azure AD 中設定應用程式 Proxy 應用程式，以將您的內部部署應用程式公開至雲端，請參閱 how [to configure An Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)。</span><span class="sxs-lookup"><span data-stu-id="5ed87-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="5ed87-104">單一登入 (SSO) 可讓您的使用者存取應用程式，而不需多次驗證。</span><span class="sxs-lookup"><span data-stu-id="5ed87-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="5ed87-105">它允許在雲端中進行單一驗證，針對 Azure Active Directory，並允許服務或連接器模擬使用者，以從應用程式中完成其他任何驗證挑戰。</span><span class="sxs-lookup"><span data-stu-id="5ed87-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="5ed87-106">若要深入瞭解，請參閱 how [to configure an single sign to An Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)。</span><span class="sxs-lookup"><span data-stu-id="5ed87-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="5ed87-107">使用 [本文](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) 來疑難排解在建立新的應用程式 proxy 應用程式時，人們面臨的常見問題。</span><span class="sxs-lookup"><span data-stu-id="5ed87-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="5ed87-108">如果您在設定應用程式的後端驗證時發生問題，您可能需要對 [應用程式 Proxy 的 Kerberos 限制委派設定進行疑難排解](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) ，或遵循 [使用 PingAccess 設定應用程式](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) 的指導方針來解決您的問題。</span><span class="sxs-lookup"><span data-stu-id="5ed87-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
