---
title: 內容不會出現在 SharePoint 搜尋結果中
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363789"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="39720-102">內容不會出現在 SharePoint 搜尋結果中</span><span class="sxs-lookup"><span data-stu-id="39720-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="39720-103">如果預期的內容未出現在搜尋結果中, 請遵循下列疑難排解步驟:</span><span class="sxs-lookup"><span data-stu-id="39720-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="39720-104">檢查包含預期內容的**網站**是否設定為允許內容出現在搜尋結果中。</span><span class="sxs-lookup"><span data-stu-id="39720-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="39720-105">請依照在[搜尋結果中顯示網站內容](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)的步驟進行。</span><span class="sxs-lookup"><span data-stu-id="39720-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="39720-106">檢查包含預期內容的**清單**或文檔**庫**是否已設定為允許內容出現在搜尋結果中。</span><span class="sxs-lookup"><span data-stu-id="39720-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="39720-107">請依照 [在[搜尋結果中顯示清單](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)中的內容] 或 [文件庫] 中的步驟。</span><span class="sxs-lookup"><span data-stu-id="39720-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="39720-108">確認頁面、檔或自訂頁面配置已發佈為**主要版本。**</span><span class="sxs-lookup"><span data-stu-id="39720-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="39720-109">請遵循搜尋中的步驟 3,[不會傳回 SharePoint Online 中的所有結果](https://go.microsoft.com/fwlink/?linkid=874525)。</span><span class="sxs-lookup"><span data-stu-id="39720-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="39720-110">確認使用者具有查看內容的**許可權**。</span><span class="sxs-lookup"><span data-stu-id="39720-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="39720-111">請依照[瞭解 SharePoint 中的許可權層級](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels)中的步驟進行。</span><span class="sxs-lookup"><span data-stu-id="39720-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="39720-112">如果已透過新增 managed 屬性來變更搜尋架構、編輯 managed 屬性, 或是移除 managed 屬性, 則需要進行編目和重新編制索引。</span><span class="sxs-lookup"><span data-stu-id="39720-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="39720-113">[請依照手動要求編目和重新編制網站、文件庫或清單的索引](https://docs.microsoft.com/sharepoint/crawl-site-content)中的步驟,**重新編制內容索引**。</span><span class="sxs-lookup"><span data-stu-id="39720-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="39720-114">這可能需要一段時間, 請等候24小時後再檢查結果。</span><span class="sxs-lookup"><span data-stu-id="39720-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="39720-115">如需詳細資訊, 請參閱[啟用網站上的內容以](https://docs.microsoft.com/sharepoint/make-site-content-searchable)供搜尋。</span><span class="sxs-lookup"><span data-stu-id="39720-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
