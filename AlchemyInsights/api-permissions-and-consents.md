---
title: API 許可權和同意
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
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951871"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="a8102-102">API 許可權和同意</span><span class="sxs-lookup"><span data-stu-id="a8102-102">API permissions and consent</span></span>

<span data-ttu-id="a8102-103">與 Microsoft identity platform 整合的應用程式遵循授權模式，可讓使用者和系統管理員控制資料的存取方式。</span><span class="sxs-lookup"><span data-stu-id="a8102-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="a8102-104">已在 Microsoft identity platform 端點上更新授權模型的實施。</span><span class="sxs-lookup"><span data-stu-id="a8102-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="a8102-105">它會變更應用程式必須與 Microsoft identity platform 互動的方式。</span><span class="sxs-lookup"><span data-stu-id="a8102-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="a8102-106">[Microsoft identity platform 端點中的許可權與同意](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 涵蓋此授權模型的基本概念，包括範圍、許可權和同意。</span><span class="sxs-lookup"><span data-stu-id="a8102-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="a8102-107">[Azure Active Directory (AZURE AD) 同意架構](https://docs.microsoft.com/azure/active-directory/develop/consent-framework)，可讓您輕鬆開發多承租人 web 和原生用戶端應用程式。</span><span class="sxs-lookup"><span data-stu-id="a8102-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="a8102-108">這些應用程式允許從 Azure AD 租使用者登入，而不是應用程式註冊的使用者帳戶。</span><span class="sxs-lookup"><span data-stu-id="a8102-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="a8102-109">他們可能也需要存取 web APIs 例如 Microsoft Graph API (，以存取 Microsoft 365) 和其他 Microsoft services APIs 中的 Azure AD、Intune 和服務，以及您自己的 web APIs。</span><span class="sxs-lookup"><span data-stu-id="a8102-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

