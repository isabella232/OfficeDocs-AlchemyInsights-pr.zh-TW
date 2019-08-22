---
title: 搜尋 SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507622"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="868d4-102">內容編目和編製索引 SharePoint Online 中</span><span class="sxs-lookup"><span data-stu-id="868d4-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="868d4-103">內容必須被編目並新增至使用者尋找項目他們透過其中搜尋的 SharePoint Online 中的搜尋索引。</span><span class="sxs-lookup"><span data-stu-id="868d4-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="868d4-104">內容會自動編目根據預先定義的編目排程 （不能變更編目排程）。</span><span class="sxs-lookup"><span data-stu-id="868d4-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="868d4-105">編目程式挑選自前次編目以來已變更及更新的索引的內容。</span><span class="sxs-lookup"><span data-stu-id="868d4-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="868d4-106">若要確保編目內容，以及更新索引，請注意下列事項：</span><span class="sxs-lookup"><span data-stu-id="868d4-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="868d4-107">請確定可以找到內容[製作網站內容可供搜尋](https://docs.microsoft.com/sharepoint/make-site-content-searchable)。</span><span class="sxs-lookup"><span data-stu-id="868d4-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="868d4-108">當您已變更的 managed 的屬性，或您已變更的對應的編目及 managed 屬性，該網站必須在重新編目，才能變更會反映在搜尋索引中。</span><span class="sxs-lookup"><span data-stu-id="868d4-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="868d4-109">搜尋結構描述中，而非實際網站進行變更，因為編目程式將不會自動重新編製索引之網站。</span><span class="sxs-lookup"><span data-stu-id="868d4-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="868d4-110">如需詳細資訊，請參閱[手動要求編目和重新編製索引的網站、 文件庫或清單](https://docs.microsoft.com/sharepoint/crawl-site-conten)。</span><span class="sxs-lookup"><span data-stu-id="868d4-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="868d4-111">請至少等候 24 小時之後以手動方式要求編目和完整重新編製索引以查看是否仍有問題。</span><span class="sxs-lookup"><span data-stu-id="868d4-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="868d4-112">如果您起始的編目和完整重新編製索引以來超過 24 小時，請登支援案例。</span><span class="sxs-lookup"><span data-stu-id="868d4-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="868d4-113">在許多情況下，我們已使用的方案。</span><span class="sxs-lookup"><span data-stu-id="868d4-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="868d4-114">請讓我們至少 24 小時才能完成解決方案。</span><span class="sxs-lookup"><span data-stu-id="868d4-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="868d4-115">如果網站、 文件 （檔案庫） 或清單已遭刪除，仍會顯示在搜尋結果中，使用者應該會收到**錯誤 404 找不到檔案**時，嘗試對其進行存取。</span><span class="sxs-lookup"><span data-stu-id="868d4-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="868d4-116">這個問題應該記錄為進一步調查的支援案例。</span><span class="sxs-lookup"><span data-stu-id="868d4-116">This issue should be logged as a support case for further investigation.</span></span> 



