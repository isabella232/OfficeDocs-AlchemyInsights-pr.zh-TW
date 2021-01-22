---
title: 設定和延長權杖存留期
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/20/2021
ms.locfileid: "49911979"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="fb14c-102">設定和延長權杖存留期</span><span class="sxs-lookup"><span data-stu-id="fb14c-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="fb14c-103">您可以指定由 Microsoft 身分識別平台發出的存取、SAML 或識別碼權杖的存留期。</span><span class="sxs-lookup"><span data-stu-id="fb14c-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="fb14c-104">您可以為組織中的所有應用程式、多租用戶 (多組織) 應用程式或組織中的特定服務主體設定權杖存留期。</span><span class="sxs-lookup"><span data-stu-id="fb14c-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="fb14c-105">有關更多資訊，請閱讀[可設定權杖存留期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。</span><span class="sxs-lookup"><span data-stu-id="fb14c-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="fb14c-106">例如，閱讀[如何設定權杖存留期的範例](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)。</span><span class="sxs-lookup"><span data-stu-id="fb14c-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="fb14c-107">要了解如何在 Azure Active Directory B2C (Azure AD B2C) 中設定權杖的存留期和相容性，請參閱[在 Azure Active Directory B2C 中設定權杖](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)。</span><span class="sxs-lookup"><span data-stu-id="fb14c-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="fb14c-108">文章[在 Azure Active Directory B2C 中設定工作階段行為](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow)描述了 Azure AD B2C 中使用的單一登入 (SSO) 方法，並協助您在設定原則時選擇最合適的 SSO 方法。</span><span class="sxs-lookup"><span data-stu-id="fb14c-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="fb14c-109">**權杖能用多久？有效期是多久？**</span><span class="sxs-lookup"><span data-stu-id="fb14c-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="fb14c-110">權杖存留期為 1 小時，工作階段存留期為 24 小時。</span><span class="sxs-lookup"><span data-stu-id="fb14c-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="fb14c-111">這意味著，如果 24 小時內沒有任何要求，則需要在要求新權杖之前再次登入。</span><span class="sxs-lookup"><span data-stu-id="fb14c-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="fb14c-112">2020 年 5 月 30 日之後，新租用戶將無法使用可設定權杖存留期原則來設定工作階段和重新整理權杖。</span><span class="sxs-lookup"><span data-stu-id="fb14c-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="fb14c-113">取代將在之後的幾個月內發生，這意味著我們將停止執行現有工作階段並重新整理權杖原則。</span><span class="sxs-lookup"><span data-stu-id="fb14c-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="fb14c-114">仍然可以在取代之後設定存取權杖存留期。</span><span class="sxs-lookup"><span data-stu-id="fb14c-114">You can still configure access token lifetimes after the deprecation.</span></span>






