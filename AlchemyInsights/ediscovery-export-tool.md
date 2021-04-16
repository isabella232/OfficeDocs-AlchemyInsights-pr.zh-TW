---
title: eDiscovery 匯出工具
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814579"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="939c9-102">無法安裝或執行 eDiscovery 匯出工具？</span><span class="sxs-lookup"><span data-stu-id="939c9-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="939c9-103">如果您無法安裝或執行 eDiscovery 匯出工具來下載搜尋結果，請檢查下列事項：</span><span class="sxs-lookup"><span data-stu-id="939c9-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="939c9-104">您所使用的電腦符合下列先決條件：</span><span class="sxs-lookup"><span data-stu-id="939c9-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="939c9-105">32或64位版本的 Windows 7 和更新版本</span><span class="sxs-lookup"><span data-stu-id="939c9-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="939c9-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="939c9-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="939c9-107">支援的瀏覽器：</span><span class="sxs-lookup"><span data-stu-id="939c9-107">A supported browser:</span></span>

  - <span data-ttu-id="939c9-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="939c9-108">Microsoft Edge</span></span>

    <span data-ttu-id="939c9-109">或</span><span class="sxs-lookup"><span data-stu-id="939c9-109">Or</span></span>

  - <span data-ttu-id="939c9-110">Internet Explorer 10 和更新版本</span><span class="sxs-lookup"><span data-stu-id="939c9-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="939c9-111">其他瀏覽器（如 Google Chrome 和 Mozilla Firefox）都不受支援。</span><span class="sxs-lookup"><span data-stu-id="939c9-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="939c9-112">您的組織可以連線到 Azure 中的端點，也就是 **\* blob.core.windows.net** (此萬用字元代表匯出工作) 的唯一識別碼。</span><span class="sxs-lookup"><span data-stu-id="939c9-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="939c9-113">您已在 Microsoft 365 安全性與合規性中心內指派「匯出」角色 &amp; 。</span><span class="sxs-lookup"><span data-stu-id="939c9-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="939c9-114">根據預設，此角色只會指派給 eDiscovery 管理員角色群組。</span><span class="sxs-lookup"><span data-stu-id="939c9-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="939c9-115">請參閱 [指派 eDiscovery 許可權](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)。</span><span class="sxs-lookup"><span data-stu-id="939c9-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="939c9-116">如需詳細資訊，請參閱 [匯出內容搜尋結果](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)。</span><span class="sxs-lookup"><span data-stu-id="939c9-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="939c9-117">若要匯出的信箱超過10個，您必須使用下列 Powershell 下載匯出結果：  [從超過100k 的信箱匯出結果](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)。</span><span class="sxs-lookup"><span data-stu-id="939c9-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>