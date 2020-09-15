---
title: 內容不會出現在 SharePoint 搜尋結果中
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713121"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="4becb-102">內容不會出現在 SharePoint 搜尋結果中</span><span class="sxs-lookup"><span data-stu-id="4becb-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="4becb-103">當預期的內容未出現在搜尋結果中時，請遵循下列疑難排解步驟：</span><span class="sxs-lookup"><span data-stu-id="4becb-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="4becb-104">檢查包含預期內容的 **網站** 是否設定為允許內容出現在搜尋結果中。</span><span class="sxs-lookup"><span data-stu-id="4becb-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="4becb-105">依照在 [搜尋結果中顯示網站內容](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)中的步驟進行。</span><span class="sxs-lookup"><span data-stu-id="4becb-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="4becb-106">檢查包含預期內容的 **清單** 或文檔 **庫** ，是否設定為允許內容出現在搜尋結果中。</span><span class="sxs-lookup"><span data-stu-id="4becb-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="4becb-107">依照在 [搜尋結果中顯示清單或文件庫](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)中的內容中的步驟進行。</span><span class="sxs-lookup"><span data-stu-id="4becb-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="4becb-108">請確認頁面、檔或自訂的版面配置已發佈為 **主要版本。**</span><span class="sxs-lookup"><span data-stu-id="4becb-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="4becb-109">請遵循搜尋中的步驟3， [不會傳回 SharePoint Online 中的所有結果](https://go.microsoft.com/fwlink/?linkid=874525)。</span><span class="sxs-lookup"><span data-stu-id="4becb-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="4becb-110">確認使用者具備查看內容的 **許可權** 。</span><span class="sxs-lookup"><span data-stu-id="4becb-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="4becb-111">遵循 [SharePoint 中瞭解許可權等級](https://docs.microsoft.com/sharepoint/understanding-permission-levels)的步驟。</span><span class="sxs-lookup"><span data-stu-id="4becb-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="4becb-112">如果已使用新增的 managed 屬性變更了搜尋架構、編輯 managed 屬性，或是移除 managed 屬性，則會需要要求編目及重新建立索引。</span><span class="sxs-lookup"><span data-stu-id="4becb-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="4becb-113">遵循[手動要求編目及重新編制網站、文件庫或清單的索引](https://docs.microsoft.com/sharepoint/crawl-site-content)中的步驟，以**重新編制內容索引**。</span><span class="sxs-lookup"><span data-stu-id="4becb-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="4becb-114">這可能需要一些時間，請等候24小時後檢查結果。</span><span class="sxs-lookup"><span data-stu-id="4becb-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="4becb-115">如需詳細資訊，請參閱 [讓網站上的內容](https://docs.microsoft.com/sharepoint/make-site-content-searchable)可供搜尋。</span><span class="sxs-lookup"><span data-stu-id="4becb-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
