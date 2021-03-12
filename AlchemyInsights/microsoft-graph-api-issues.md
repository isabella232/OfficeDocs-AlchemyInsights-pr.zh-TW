---
title: Microsoft Graph API 問題
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/29/2021
ms.locfileid: "50716194"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="01b9b-102">Microsoft Graph API 問題</span><span class="sxs-lookup"><span data-stu-id="01b9b-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="01b9b-103">本主題也適用于開發人員，但仍在使用 Azure AD Graph API。</span><span class="sxs-lookup"><span data-stu-id="01b9b-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="01b9b-104">不過， **強烈** 建議您將 Microsoft Graph 用於所有目錄、身分識別和存取管理案例。</span><span class="sxs-lookup"><span data-stu-id="01b9b-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="01b9b-105">**驗證或授權問題**</span><span class="sxs-lookup"><span data-stu-id="01b9b-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="01b9b-106">如果您的應用程式 **無法取得標記** 以撥打 Microsoft graph，請挑選) Microsoft graph 類別取得 **存取權杖 (驗證** ，以取得更多有關本主題的說明和支援的問題。</span><span class="sxs-lookup"><span data-stu-id="01b9b-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="01b9b-107">當呼叫 Microsoft Graph 時，如果您的應用程式 **收到401或403授權錯誤** ，請選擇 [ **取得存取權被拒絕] 錯誤 (授權)** Microsoft Graph API 類別，以取得更多有關本主題的說明和支援。</span><span class="sxs-lookup"><span data-stu-id="01b9b-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="01b9b-108">**我想要使用 Microsoft Graph，但不確定開始的位置**</span><span class="sxs-lookup"><span data-stu-id="01b9b-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="01b9b-109">Microsoft Graph 概觀</span><span class="sxs-lookup"><span data-stu-id="01b9b-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="01b9b-110">Microsoft Graph 中的身分識別與存取管理綜述</span><span class="sxs-lookup"><span data-stu-id="01b9b-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="01b9b-111">建立 Microsoft Graph 應用程式入門</span><span class="sxs-lookup"><span data-stu-id="01b9b-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="01b9b-112">**Microsoft Graph Explorer** -在您的租使用者或示範租使用者中測試 Microsoft graph APIs</span><span class="sxs-lookup"><span data-stu-id="01b9b-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="01b9b-113">**我想要使用 Microsoft Graph，但是它是否支援我需要的1.0 版目錄 APIs？**</span><span class="sxs-lookup"><span data-stu-id="01b9b-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="01b9b-114">Microsoft Graph 是目錄、身分識別和存取管理的建議 API。</span><span class="sxs-lookup"><span data-stu-id="01b9b-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="01b9b-115">不過，Azure AD Graph 和 Microsoft Graph 中的可能仍然有一些間距。</span><span class="sxs-lookup"><span data-stu-id="01b9b-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="01b9b-116">請參閱下列文章，這些文章會反白顯示最新的差異，以協助您選擇：</span><span class="sxs-lookup"><span data-stu-id="01b9b-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="01b9b-117">Azure AD Graph 和 Microsoft Graph 之間的資源類型差異</span><span class="sxs-lookup"><span data-stu-id="01b9b-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="01b9b-118">Azure AD Graph 和 Microsoft Graph 之間的屬性差異</span><span class="sxs-lookup"><span data-stu-id="01b9b-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="01b9b-119">Azure AD 和 Microsoft Graph 之間的方法差異</span><span class="sxs-lookup"><span data-stu-id="01b9b-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="01b9b-120">**我正在通話的 API 無法運作-我可以在哪裡進行其他測試？**</span><span class="sxs-lookup"><span data-stu-id="01b9b-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="01b9b-121">**Microsoft Graph Explorer** -在您的租使用者或示範承租人中測試 Microsoft graph APIs，也請查看 Microsoft graph Explorer 中的 **範例查詢** 。</span><span class="sxs-lookup"><span data-stu-id="01b9b-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="01b9b-122">**我的應用程式速度太慢，也遭到節流。我可以進行哪些改進？**</span><span class="sxs-lookup"><span data-stu-id="01b9b-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="01b9b-123">視您的案例而定，有許多選項可讓您的應用程式更具能力，在某些情況下，當您) 進行許多呼叫時，可能會降低服務 (的限制。</span><span class="sxs-lookup"><span data-stu-id="01b9b-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="01b9b-124">Microsoft Graph 最佳作法</span><span class="sxs-lookup"><span data-stu-id="01b9b-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="01b9b-125">批次處理要求</span><span class="sxs-lookup"><span data-stu-id="01b9b-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="01b9b-126">透過增量查詢追蹤變更</span><span class="sxs-lookup"><span data-stu-id="01b9b-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="01b9b-127">透過 webhooks 取得變更的通知</span><span class="sxs-lookup"><span data-stu-id="01b9b-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="01b9b-128">節流指導</span><span class="sxs-lookup"><span data-stu-id="01b9b-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="01b9b-129">**在哪裡可以找到錯誤和已知問題的詳細資訊？**</span><span class="sxs-lookup"><span data-stu-id="01b9b-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="01b9b-130">Microsoft Graph 錯誤回應資訊</span><span class="sxs-lookup"><span data-stu-id="01b9b-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="01b9b-131">Microsoft Graph 的已知問題</span><span class="sxs-lookup"><span data-stu-id="01b9b-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="01b9b-132">**我可以在哪裡檢查服務可用性和線上狀態？**</span><span class="sxs-lookup"><span data-stu-id="01b9b-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="01b9b-133">可透過 Microsoft Graph 存取之基礎服務的服務可用性和連線能力會影響 Microsoft Graph 的整體可用性和效能。</span><span class="sxs-lookup"><span data-stu-id="01b9b-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="01b9b-134">在 [Azure Active Directory 服務健康情況] 中，檢查 [ [azure 狀態] 頁面](https://azure.microsoft.com/status/)中所列的 [**安全性 + 身分識別** 服務] 狀態。</span><span class="sxs-lookup"><span data-stu-id="01b9b-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="01b9b-135">針對參與 Microsoft Graph 的 Office 服務，請檢查 [Office 服務健康情況儀表板](https://portal.office.com/adminportal/home#/servicehealth)中所列服務的狀態。</span><span class="sxs-lookup"><span data-stu-id="01b9b-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="01b9b-136">Microsoft Graph 授權錯誤可能是幾個不同問題的結果，大部分會產生401或403錯誤。</span><span class="sxs-lookup"><span data-stu-id="01b9b-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="01b9b-137">例如，下列各項會導致授權錯誤：</span><span class="sxs-lookup"><span data-stu-id="01b9b-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="01b9b-138">不正確的[存取權杖取得流程](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios) (部分機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="01b9b-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="01b9b-139">設定錯誤的 [權限範圍](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) (部分機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="01b9b-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="01b9b-140">缺少[同意](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) (部分機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="01b9b-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="01b9b-141">\**_Azure Active Directory 驗證程式庫 (ADAL)和 Azure AD Graph API (AAD Graph) 的終止支援_* _</span><span class="sxs-lookup"><span data-stu-id="01b9b-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="01b9b-142">_ \* 從2020年6月30日起，\* \*，我們將不再將任何新功能新增至 ADAL 和 Azure AD Graph。</span><span class="sxs-lookup"><span data-stu-id="01b9b-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="01b9b-143">我們會繼續提供技術支援和安全性更新，但將不再提供功能更新。</span><span class="sxs-lookup"><span data-stu-id="01b9b-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="01b9b-144">**從2022年6月30日起**，我們將結束支援 ADAL 和 Azure AD Graph，而且將不再提供技術支援或安全性更新。</span><span class="sxs-lookup"><span data-stu-id="01b9b-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="01b9b-145">在此時間之後，使用 ADAL 的現有作業系統版本的應用程式仍可運作，但不會 *取得任何技術支援或安全性更新*。</span><span class="sxs-lookup"><span data-stu-id="01b9b-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="01b9b-146">在此時間之後使用 Azure AD Graph 的應用程式可能不再接收 Azure AD Graph 端點的回應。</span><span class="sxs-lookup"><span data-stu-id="01b9b-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="01b9b-147">**ADAL 遷移**</span><span class="sxs-lookup"><span data-stu-id="01b9b-147">**ADAL Migration**</span></span>

<span data-ttu-id="01b9b-148">我們建議您更新至 [Microsoft 驗證程式庫 (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) (部分機器翻譯)，其中包含最新的功能和安全性更新。</span><span class="sxs-lookup"><span data-stu-id="01b9b-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="01b9b-149">如果您使用的是 Microsoft 應用程式，請知道 Microsoft 正在將其應用程式遷移至 MSAL 的程式，以在支援的期限內進行遷移，以確保他們能夠從 MSAL 的持續安全性和功能改進中受益。</span><span class="sxs-lookup"><span data-stu-id="01b9b-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="01b9b-150">閱讀 ADAL 常見問題集</span><span class="sxs-lookup"><span data-stu-id="01b9b-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="01b9b-151">了解如何以每個平台為基礎移轉應用程式</span><span class="sxs-lookup"><span data-stu-id="01b9b-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="01b9b-152">如果您需要協助瞭解您使用 ADAL 的應用程式，建議您檢查您的所有應用程式原始程式碼，並在適用時，向內送出任何 Isv 或應用程式提供者。</span><span class="sxs-lookup"><span data-stu-id="01b9b-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="01b9b-153">Microsoft 支援服務也可提供您租用戶中所有非 Microsoft ADAL 應用程式清單。</span><span class="sxs-lookup"><span data-stu-id="01b9b-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="01b9b-154">**AAD Graph 移轉**</span><span class="sxs-lookup"><span data-stu-id="01b9b-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="01b9b-155">針對使用 Azure AD Graph 的應用程式，請遵循我們的指導，將 [AZURE AD Graph 應用程式遷移至 Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)。</span><span class="sxs-lookup"><span data-stu-id="01b9b-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="01b9b-156">[我們的移轉檢查清單可做為起點](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。</span><span class="sxs-lookup"><span data-stu-id="01b9b-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="01b9b-157">您的 Azure 應用程式註冊入口網站顯示哪些應用程式正在使用 AAD Graph。</span><span class="sxs-lookup"><span data-stu-id="01b9b-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="01b9b-158">我們建議您檢閱所有應用程式的原始程式碼，如果適用的話，請向任何 ISV 或應用程式提供者諮詢。</span><span class="sxs-lookup"><span data-stu-id="01b9b-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="01b9b-159">Microsoft 支援也可以提供您租使用者中所有 AAD 圖形使用方式的清單。</span><span class="sxs-lookup"><span data-stu-id="01b9b-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="01b9b-160">若要讓您的應用程式存取 Microsoft Graph 中的資料，使用者或系統管理員必須透過同意程式授與其正確的許可權。</span><span class="sxs-lookup"><span data-stu-id="01b9b-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="01b9b-161">[Microsoft graph 許可權參考](https://docs.microsoft.com/graph/permissions-reference)會列出與每個主要 Microsoft Graph APIs 集合相關聯的許可權。</span><span class="sxs-lookup"><span data-stu-id="01b9b-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="01b9b-162">此外，它也提供如何使用許可權的指導方針。</span><span class="sxs-lookup"><span data-stu-id="01b9b-162">It also provides guidance about how to use the permissions.</span></span>
