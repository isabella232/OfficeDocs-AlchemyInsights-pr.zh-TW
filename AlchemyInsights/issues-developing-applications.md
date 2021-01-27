---
title: 開發應用程式的問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950690"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="cc673-102">開發應用程式的問題</span><span class="sxs-lookup"><span data-stu-id="cc673-102">Issues developing applications</span></span>

<span data-ttu-id="cc673-103">若要針對建立 Azure Active Directory (AD) 應用程式時最常見的問題進行疑難排解，請參閱下列文章：</span><span class="sxs-lookup"><span data-stu-id="cc673-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="cc673-104">我只有在使用 Chrome 網頁瀏覽器登入應用程式時會發生問題</span><span class="sxs-lookup"><span data-stu-id="cc673-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="cc673-105">我不知道如何變更應用程式的權杖生命週期預設值</span><span class="sxs-lookup"><span data-stu-id="cc673-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="cc673-106">我對於應用程式同意的運作方式感到困惑</span><span class="sxs-lookup"><span data-stu-id="cc673-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="cc673-107">我不知道如何將權限授與我的應用程式</span><span class="sxs-lookup"><span data-stu-id="cc673-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="cc673-108">我不了解委派和應用程式權限之間的差異</span><span class="sxs-lookup"><span data-stu-id="cc673-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="cc673-109">\***Azure Active Directory 驗證程式庫 (ADAL) 和 Azure AD Graph API (AAD Graph) 的終止支援** _</span><span class="sxs-lookup"><span data-stu-id="cc673-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="cc673-110">從 2020 年 6 月 30 日起，我們不再將任何新功能新增至 Azure Active Directory 驗證程式庫 (ADAL) 和 Azure AD Graph API (AAD Graph)。</span><span class="sxs-lookup"><span data-stu-id="cc673-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="cc673-111">我們會繼續提供技術支援和安全性更新，但將不再提供功能更新。</span><span class="sxs-lookup"><span data-stu-id="cc673-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="cc673-112">從 2022 年 6 月 30 日起，我們將終止 ADAL 和 AAD Graph 的支援，並不再提供技術支援或安全性更新。</span><span class="sxs-lookup"><span data-stu-id="cc673-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="cc673-113">由於此情況，以下是一些影響：</span><span class="sxs-lookup"><span data-stu-id="cc673-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="cc673-114">在現有作業系統版本上使用 ADAL 的應用程式將在此時間後繼續運作，但不會取得任何技術支援或安全性更新。</span><span class="sxs-lookup"><span data-stu-id="cc673-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="cc673-115">在此時間之後使用 AAD Graph 的應用程式可能無法再收到 AAD Graph 端點的回應</span><span class="sxs-lookup"><span data-stu-id="cc673-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="cc673-116">_ *ADAL 移轉*\*</span><span class="sxs-lookup"><span data-stu-id="cc673-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="cc673-117">如果您使用 Microsoft 應用程式，建議您更新至 Microsoft 驗證程式庫 (MSAL)，其包含最新的功能和安全性更新。</span><span class="sxs-lookup"><span data-stu-id="cc673-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="cc673-118">本建議是由 Microsoft 在終止支援期限之前起始將其應用程式移轉至 MSAL 的程序。</span><span class="sxs-lookup"><span data-stu-id="cc673-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="cc673-119">Microsoft 將其應用程式移轉至 MSAL，可確保應用程式能夠從 MSAL 持續的安全性與功能增強中受益。</span><span class="sxs-lookup"><span data-stu-id="cc673-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="cc673-120">閱讀 ADAL 常見問題集</span><span class="sxs-lookup"><span data-stu-id="cc673-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="cc673-121">了解如何以每個平台為基礎移轉應用程式</span><span class="sxs-lookup"><span data-stu-id="cc673-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="cc673-122">如果您需要協助了解您的哪些應用程式使用 ADAL，建議您檢閱所有應用程式的原始程式碼，並且 (如適用) 向任何獨立軟體廠商 (ISV) 或應用程式提供者諮詢。</span><span class="sxs-lookup"><span data-stu-id="cc673-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="cc673-123">Microsoft 支援服務也可提供您租用戶中所有非 Microsoft ADAL 應用程式清單。</span><span class="sxs-lookup"><span data-stu-id="cc673-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="cc673-124">**AAD Graph 移轉**</span><span class="sxs-lookup"><span data-stu-id="cc673-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="cc673-125">針對使用 AAD Graph 的應用程式，請依照我們的指導方針，將 AAD Graph 應用程式移轉至 Microsoft Graph：</span><span class="sxs-lookup"><span data-stu-id="cc673-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="cc673-126">[我們的移轉檢查清單可做為起點](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。</span><span class="sxs-lookup"><span data-stu-id="cc673-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="cc673-127">您的 Azure 應用程式註冊入口網站會顯示哪些應用程式正在使用 AAD Graph。</span><span class="sxs-lookup"><span data-stu-id="cc673-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="cc673-128">建議您檢閱所有應用程式的原始程式碼，如果適用的話，請向任何獨立軟體廠商 (ISV) 或應用程式提供者諮詢。</span><span class="sxs-lookup"><span data-stu-id="cc673-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="cc673-129">Microsoft 支援服務也可為您提供租用戶中所有 AAD Graph 使用狀況的資訊。</span><span class="sxs-lookup"><span data-stu-id="cc673-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







