---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: e7bff5f9fcf6f2f2c77e93c2f27f585f2cc18bea
ms.sourcegitcommit: 98231a228ecb2bf14ec3b96d4dd4ccf2507617a3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/01/2020
ms.locfileid: "43079251"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="e5004-102">封鎖舊版驗證</span><span class="sxs-lookup"><span data-stu-id="e5004-102">Blocking legacy authentication</span></span>

<span data-ttu-id="e5004-103">舊版驗證是指一種字詞，指的驗證要求是由下列專案所組成：</span><span class="sxs-lookup"><span data-stu-id="e5004-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="e5004-104">不使用新式驗證的舊版 Office 用戶端（例如，Office 2010 用戶端）。</span><span class="sxs-lookup"><span data-stu-id="e5004-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="e5004-105">任何使用舊版郵件通訊協定（如 IMAP/SMTP/POP3）的用戶端。</span><span class="sxs-lookup"><span data-stu-id="e5004-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="e5004-106">如需封鎖舊版驗證及啟用新式驗證的詳細資訊，請參閱[封鎖舊版驗證](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)。</span><span class="sxs-lookup"><span data-stu-id="e5004-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="e5004-107">Azure Active Directory （Azure AD）中的安全性預設值可讓您更容易安全，並協助保護您的組織。</span><span class="sxs-lookup"><span data-stu-id="e5004-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="e5004-108">安全性預設值包含常見攻擊的預先設定安全性設定。</span><span class="sxs-lookup"><span data-stu-id="e5004-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="e5004-109">如需安全性預設值的詳細資訊，請參閱[何謂安全性預設值？](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)。</span><span class="sxs-lookup"><span data-stu-id="e5004-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="e5004-110">**附注**：如果您的租使用者于22Nd 年10月或之後建立，請2019，您可能會遇到新的安全預設行為，且已在您的租使用者中啟用安全性預設值。</span><span class="sxs-lookup"><span data-stu-id="e5004-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="e5004-111">為了保護所有使用者的工作，安全性預設值會向所建立的所有新承租人推出。</span><span class="sxs-lookup"><span data-stu-id="e5004-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
