---
title: 驗證程式庫的問題
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/28/2021
ms.locfileid: "50037211"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="6e570-102">驗證程式庫的問題</span><span class="sxs-lookup"><span data-stu-id="6e570-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="6e570-103">[Microsoft 身分識別平臺驗證庫](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) 會列出 Microsoft 支援和相容的用戶端和中介軟體文件庫。</span><span class="sxs-lookup"><span data-stu-id="6e570-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="6e570-104">Microsoft 驗證程式庫 (MSAL) 支援數種 [驗證流量](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) ，以用於不同的應用程式案例。</span><span class="sxs-lookup"><span data-stu-id="6e570-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="6e570-105">若要驗證及取得標記，您可以在程式碼中初始化新的公用或機密用戶端應用程式。</span><span class="sxs-lookup"><span data-stu-id="6e570-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="6e570-106">在 [Microsoft 驗證程式庫] 中初始化用戶端應用程式時，您可以設定數個設定選項 (MSAL) 。</span><span class="sxs-lookup"><span data-stu-id="6e570-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="6e570-107">若要深入瞭解，請參閱 [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)。</span><span class="sxs-lookup"><span data-stu-id="6e570-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="6e570-108">**Azure Active Directory 驗證程式庫的支援終止 (ADAL) 和 Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="6e570-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="6e570-109">**從2020年6月30日起**，我們將不再將任何新功能新增至 ADAL 和 Azure AD Graph。</span><span class="sxs-lookup"><span data-stu-id="6e570-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="6e570-110">我們會繼續提供技術支援和安全性更新，但將不再提供功能更新。</span><span class="sxs-lookup"><span data-stu-id="6e570-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="6e570-111">**從2022年6月30日起**，我們將結束支援 ADAL 和 Azure AD Graph，而且將不再提供技術支援或安全性更新。</span><span class="sxs-lookup"><span data-stu-id="6e570-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="6e570-112">在此時間之後，使用 ADAL 的現有作業系統版本的應用程式仍可運作，但不會 *取得任何技術支援或安全性更新*。</span><span class="sxs-lookup"><span data-stu-id="6e570-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="6e570-113">在此時間之後使用 Azure AD Graph 的應用程式可能不再接收 Azure AD Graph 端點的回應。</span><span class="sxs-lookup"><span data-stu-id="6e570-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="6e570-114">**ADAL 遷移**</span><span class="sxs-lookup"><span data-stu-id="6e570-114">**ADAL Migration**</span></span>

<span data-ttu-id="6e570-115">我們建議您更新至 [Microsoft 驗證程式庫 (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) (部分機器翻譯)，其中包含最新的功能和安全性更新。</span><span class="sxs-lookup"><span data-stu-id="6e570-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="6e570-116">如果您使用的是 Microsoft 應用程式，請注意，Microsoft 正處於將其應用程式遷移至 MSAL 的程式，由支援期限終止，以確保它們能夠從 MSAL 的持續安全性和功能改進中受益。</span><span class="sxs-lookup"><span data-stu-id="6e570-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="6e570-117">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="6e570-117">For more information, see:</span></span>

1. [<span data-ttu-id="6e570-118">閱讀 ADAL 常見問題集</span><span class="sxs-lookup"><span data-stu-id="6e570-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="6e570-119">了解如何以每個平台為基礎移轉應用程式</span><span class="sxs-lookup"><span data-stu-id="6e570-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="6e570-120">如果您需要協助瞭解您使用 ADAL 的應用程式，建議您檢查您的所有應用程式原始程式碼，並在適用時，向內送出任何 Isv 或應用程式提供者。</span><span class="sxs-lookup"><span data-stu-id="6e570-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="6e570-121">Microsoft 支援服務也可提供您租用戶中所有非 Microsoft ADAL 應用程式清單。</span><span class="sxs-lookup"><span data-stu-id="6e570-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="6e570-122">**AAD Graph 移轉**</span><span class="sxs-lookup"><span data-stu-id="6e570-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="6e570-123">針對使用 Azure AD Graph 的應用程式，請遵循我們的指導，將 [AZURE AD Graph 應用程式遷移至 Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)。</span><span class="sxs-lookup"><span data-stu-id="6e570-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="6e570-124">我們的遷移檢查清單提供開始點。</span><span class="sxs-lookup"><span data-stu-id="6e570-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="6e570-125">您的 Azure 應用程式註冊入口網站顯示哪些應用程式正在使用 AAD Graph。</span><span class="sxs-lookup"><span data-stu-id="6e570-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="6e570-126">我們建議您檢閱所有應用程式的原始程式碼，如果適用的話，請向任何 ISV 或應用程式提供者諮詢。</span><span class="sxs-lookup"><span data-stu-id="6e570-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="6e570-127">Microsoft 支援也可以提供您租使用者中所有 AAD 圖形使用方式的清單。</span><span class="sxs-lookup"><span data-stu-id="6e570-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="6e570-128">若要讓您的應用程式存取 Microsoft Graph 中的資料，使用者或系統管理員必須透過同意程式授與其正確的許可權。</span><span class="sxs-lookup"><span data-stu-id="6e570-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="6e570-129">[Microsoft graph 許可權參考](https://docs.microsoft.com/graph/permissions-reference)會列出與每個主要 Microsoft Graph APIs 集合相關聯的許可權。</span><span class="sxs-lookup"><span data-stu-id="6e570-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="6e570-130">此外，它也提供如何使用許可權的指導方針。</span><span class="sxs-lookup"><span data-stu-id="6e570-130">It also provides guidance about how to use the permissions.</span></span>
