---
title: 查詢 Microsoft Graph API
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950681"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="ce9bf-102">查詢 Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="ce9bf-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="ce9bf-103">本主題也適用于開發人員，但仍在使用 Azure AD Graph API。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="ce9bf-104">不過， **強烈** 建議您將 Microsoft Graph 用於所有目錄、身分識別和存取管理案例。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="ce9bf-105">**驗證或授權問題**</span><span class="sxs-lookup"><span data-stu-id="ce9bf-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="ce9bf-106">如果您的應用程式 **無法取得標記** 以撥打 Microsoft graph，請挑選) Microsoft graph 類別取得 **存取權杖 (驗證** ，以取得更多有關本主題的說明和支援的問題。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="ce9bf-107">當呼叫 Microsoft Graph 時，如果您的應用程式 **收到401或403授權錯誤** ，請選擇 [ **取得存取權被拒絕] 錯誤 (授權)** Microsoft Graph API 類別，以取得更多有關本主題的說明和支援。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="ce9bf-108">**我想要使用 Microsoft Graph，但不確定開始的位置**</span><span class="sxs-lookup"><span data-stu-id="ce9bf-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="ce9bf-109">若要深入瞭解 Microsoft Graph，請參閱：</span><span class="sxs-lookup"><span data-stu-id="ce9bf-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="ce9bf-110">Microsoft Graph 概觀</span><span class="sxs-lookup"><span data-stu-id="ce9bf-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="ce9bf-111">Microsoft Graph 中的身分識別與存取管理綜述</span><span class="sxs-lookup"><span data-stu-id="ce9bf-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="ce9bf-112">建立 Microsoft Graph 應用程式入門</span><span class="sxs-lookup"><span data-stu-id="ce9bf-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="ce9bf-113">**Microsoft Graph Explorer** -在您的租使用者或示範租使用者中測試 Microsoft graph APIs</span><span class="sxs-lookup"><span data-stu-id="ce9bf-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="ce9bf-114">**我想要使用 Microsoft Graph，但是它是否支援我需要的1.0 版目錄 APIs？**</span><span class="sxs-lookup"><span data-stu-id="ce9bf-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="ce9bf-115">Microsoft Graph 是目錄、身分識別和存取管理的建議 API。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="ce9bf-116">不過，Azure AD Graph 和 Microsoft Graph 中的可能仍然有一些間距。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="ce9bf-117">請參閱下列文章，這些文章會反白顯示最新的差異，以協助您選擇：</span><span class="sxs-lookup"><span data-stu-id="ce9bf-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="ce9bf-118">Azure AD Graph 和 Microsoft Graph 之間的資源類型差異</span><span class="sxs-lookup"><span data-stu-id="ce9bf-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="ce9bf-119">Azure AD Graph 和 Microsoft Graph 之間的屬性差異</span><span class="sxs-lookup"><span data-stu-id="ce9bf-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="ce9bf-120">Azure AD 和 Microsoft Graph 之間的方法差異</span><span class="sxs-lookup"><span data-stu-id="ce9bf-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="ce9bf-121">**當我查詢 *使用者* 物件時，它的許多屬性都缺失**</span><span class="sxs-lookup"><span data-stu-id="ce9bf-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="ce9bf-122">`GET https://graph.microsoft.com/v1.0/users` 只會傳回11個屬性，因為 Microsoft Graph 會自動選取一組要傳回的預設 *使用者* 屬性。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="ce9bf-123">如果您需要其他 *使用者* 屬性，請使用 $select 來挑選您的應用程式所需的屬性。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="ce9bf-124">請先在 **Microsoft Graph Explorer** 中嘗試。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="ce9bf-125">**部分使用者屬性值為 *null* ，即使我知道已經設定**</span><span class="sxs-lookup"><span data-stu-id="ce9bf-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="ce9bf-126">最可能的說明是已授與 *ReadBasic 所有* 許可權的應用程式。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="ce9bf-127">這可讓應用程式讀取一組有限的使用者屬性，將所有其他屬性都傳回 null，即使先前已經設定。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="ce9bf-128">嘗試授予應用程式 *使用者。* 請改為讀取權限。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="ce9bf-129">如需詳細資訊，請參閱 [Microsoft Graph 使用者許可權](https://docs.microsoft.com/graph/permissions-reference#user-permissions)。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="ce9bf-130">**在我的要求中使用 OData 查詢參數篩選資料時遇到問題**</span><span class="sxs-lookup"><span data-stu-id="ce9bf-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="ce9bf-131">雖然 Microsoft Graph 支援廣泛的 OData 查詢參數，但這些參數中的許多參數並未從 Microsoft Graph 中的 *directoryObject*) 繼承的目錄服務 (資源完全支援。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="ce9bf-132">Azure AD Graph 中所提供的限制，在 Microsoft Graph 中的大部分部分都存在：</span><span class="sxs-lookup"><span data-stu-id="ce9bf-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="ce9bf-133">**不支援：不支援** *null* 或 *非 null* 值的 $count、$search 及 $filter</span><span class="sxs-lookup"><span data-stu-id="ce9bf-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="ce9bf-134">**不支援**：在特定屬性 $filter (請參閱可篩選屬性的資源主題) </span><span class="sxs-lookup"><span data-stu-id="ce9bf-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="ce9bf-135">**不支援**：同時分頁、篩選和排序</span><span class="sxs-lookup"><span data-stu-id="ce9bf-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="ce9bf-136">**不支援**：在關聯上篩選。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="ce9bf-137">例如，尋找 UK 中工程群組的所有成員。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="ce9bf-138">**部分支援**： *user* (displayName 上的 $orderby，並只 userPrincipalName) 與 *群組*</span><span class="sxs-lookup"><span data-stu-id="ce9bf-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="ce9bf-139">**部分支援**： $filter (僅支援 *eq*、 *startswith*、  *and 和* 有限的 *任何*) 支援，$expand (擴充單一物件的關聯性會傳回所有關聯，但展開物件的關聯集合會受到限制) </span><span class="sxs-lookup"><span data-stu-id="ce9bf-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="ce9bf-140">如需詳細資訊，請參閱 [使用查詢參數自訂回應](https://docs.microsoft.com/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="ce9bf-141">**我所呼叫的 API 沒有作用-我可以在哪裡進行其他測試？**</span><span class="sxs-lookup"><span data-stu-id="ce9bf-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="ce9bf-142">**Microsoft Graph Explorer** -在您的租使用者或示範承租人中測試 Microsoft graph APIs，也請查看 Microsoft graph Explorer 中的 **範例查詢** 。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="ce9bf-143">**當我查詢資料時，我似乎沒有完整的資料集回復**</span><span class="sxs-lookup"><span data-stu-id="ce9bf-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="ce9bf-144">如果您正在查詢集合 (如 *使用者*) 所示，Microsoft Graph 會使用伺服器端的頁面限制，因此會永遠以預設頁面大小傳回結果。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="ce9bf-145">您的應用程式應該會永遠預計會從服務傳回的集合逐步分頁。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="ce9bf-146">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="ce9bf-146">For more information, see:</span></span>

- [<span data-ttu-id="ce9bf-147">Microsoft Graph 最佳作法</span><span class="sxs-lookup"><span data-stu-id="ce9bf-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="ce9bf-148">在您的應用程式中分頁 Microsoft Graph 資料</span><span class="sxs-lookup"><span data-stu-id="ce9bf-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="ce9bf-149">**我的應用程式速度太慢，也遭到節流。我可以進行哪些改進？**</span><span class="sxs-lookup"><span data-stu-id="ce9bf-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="ce9bf-150">視您的案例而定，您可以使用各種不同的選項，讓應用程式更具能力，在某些情況下，當您) 進行許多呼叫時，可能會降低服務 (的限制。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="ce9bf-151">若要深入了解，請參閱：</span><span class="sxs-lookup"><span data-stu-id="ce9bf-151">To learn more, see:</span></span>

- [<span data-ttu-id="ce9bf-152">Microsoft Graph 最佳作法</span><span class="sxs-lookup"><span data-stu-id="ce9bf-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="ce9bf-153">批次處理要求</span><span class="sxs-lookup"><span data-stu-id="ce9bf-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="ce9bf-154">透過增量查詢追蹤變更</span><span class="sxs-lookup"><span data-stu-id="ce9bf-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="ce9bf-155">透過 webhooks 取得變更的通知</span><span class="sxs-lookup"><span data-stu-id="ce9bf-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="ce9bf-156">節流指導</span><span class="sxs-lookup"><span data-stu-id="ce9bf-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="ce9bf-157">**在哪裡可以找到錯誤和已知問題的詳細資訊？**</span><span class="sxs-lookup"><span data-stu-id="ce9bf-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="ce9bf-158">Microsoft Graph 錯誤回應資訊</span><span class="sxs-lookup"><span data-stu-id="ce9bf-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="ce9bf-159">Microsoft Graph 的已知問題</span><span class="sxs-lookup"><span data-stu-id="ce9bf-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="ce9bf-160">**我可以在哪裡檢查服務可用性和線上狀態？**</span><span class="sxs-lookup"><span data-stu-id="ce9bf-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="ce9bf-161">可透過 Microsoft Graph 存取之基礎服務的服務可用性和連線能力會影響 Microsoft Graph 的整體可用性和效能。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="ce9bf-162">在 [Azure Active Directory 服務健康情況] 中，檢查 [ [azure 狀態] 頁面](https://azure.microsoft.com/status/)中所列的 [**安全性 + 身分識別** 服務] 狀態。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="ce9bf-163">針對參與 Microsoft Graph 的 Office 服務，請檢查 [Office 服務健康情況儀表板](https://portal.office.com/adminportal/home#/servicehealth)中所列服務的狀態。</span><span class="sxs-lookup"><span data-stu-id="ce9bf-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
