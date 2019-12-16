---
title: 管理 SharePoint Online 中的搜尋結構描述
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042954"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="e02e8-102">管理 SharePoint Online 中的搜尋結構描述</span><span class="sxs-lookup"><span data-stu-id="e02e8-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="e02e8-103">搜尋結構描述可以控制使用者可以搜尋的使用者可以搜尋，您可以搜尋網站上顯示結果。</span><span class="sxs-lookup"><span data-stu-id="e02e8-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="e02e8-104">請參閱[管理 SharePoint Online 的搜尋結構描述](https://docs.microsoft.com/sharepoint/manage-search-schema)]，以了解如何：</span><span class="sxs-lookup"><span data-stu-id="e02e8-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="e02e8-105">變更搜尋結構描述。</span><span class="sxs-lookup"><span data-stu-id="e02e8-105">Change the search schema.</span></span>
- <span data-ttu-id="e02e8-106">建立 managed 的屬性。</span><span class="sxs-lookup"><span data-stu-id="e02e8-106">Create managed properties.</span></span>
- <span data-ttu-id="e02e8-107">對應編目的對應至 managed 屬性的編目屬性。</span><span class="sxs-lookup"><span data-stu-id="e02e8-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="e02e8-108">請注意下列有關管理搜尋結構描述中：</span><span class="sxs-lookup"><span data-stu-id="e02e8-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="e02e8-109">如果您收到警告，告知**應用程式已暫停**的結構描述變更時，這是只有暫時服務維護為發生。</span><span class="sxs-lookup"><span data-stu-id="e02e8-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="e02e8-110">如果已經過了超過 24 小時後，仍然會出現警告，請登支援案例。</span><span class="sxs-lookup"><span data-stu-id="e02e8-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="e02e8-111">當您變更 managed 的屬性，或新增新的時內容已重新編目之後才所做的變更才會生效。</span><span class="sxs-lookup"><span data-stu-id="e02e8-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="e02e8-112">在 SharePoint Online 中，編目會發生自動根據已定義的編目的排程。</span><span class="sxs-lookup"><span data-stu-id="e02e8-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="e02e8-113">若要確保您的變更進行編目，您可以特別[要求重新編製索引的清單或文件庫](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="e02e8-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="e02e8-114">搜尋結構描述的完整概觀，請參閱[介紹搜尋結構描述](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="e02e8-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


