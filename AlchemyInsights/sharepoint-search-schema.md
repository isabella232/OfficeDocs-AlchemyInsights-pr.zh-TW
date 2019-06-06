---
title: 管理 SharePoint Online 中的搜尋字典
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 89db349189584a45c54c9c08d37ab669c3c7a39b
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716463"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="6b96d-102">管理 SharePoint Online 的搜尋結構描述</span><span class="sxs-lookup"><span data-stu-id="6b96d-102">Manage the search schema in SharePoint Online</span></span>

<span data-ttu-id="6b96d-103">搜尋結構描述能夠控制可以搜尋的內容、搜尋該內容的方法，以及結果呈現在搜尋網站上的方式。</span><span class="sxs-lookup"><span data-stu-id="6b96d-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="6b96d-104">若要變更搜尋結構描述、建立 Managed 屬性，並將編目屬性對應至 Managed 屬性。請參閱[管理 Sharepoint 的搜尋結構描述 (機器翻譯)](https://docs.microsoft.com/zh-TW/sharepoint/manage-search-schema)。</span><span class="sxs-lookup"><span data-stu-id="6b96d-104">To change the search schema, create managed properties, and map crawled properties to managed properties, see [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-search-schema).</span></span> <span data-ttu-id="6b96d-105">如果您進行結構描述變更時收到「暫停應用程式」的警告，應該只是發生暫時服務維修。</span><span class="sxs-lookup"><span data-stu-id="6b96d-105">If you receive a warning 'the application is paused' when making a schema change, this is only temporary there is service maintenance occurring.</span></span> 

<span data-ttu-id="6b96d-106">如果暫停 24 小時並且依然收到警告，請記錄支援案例。</span><span class="sxs-lookup"><span data-stu-id="6b96d-106">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>

<span data-ttu-id="6b96d-107">當您變更Managed 屬性或新增新屬性時，所做的變更只會在內容重新編目後才生效。</span><span class="sxs-lookup"><span data-stu-id="6b96d-107">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="6b96d-108">在 SharePoint Online 中，會根據已定義的編目排程進行自動編目。</span><span class="sxs-lookup"><span data-stu-id="6b96d-108">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>

<span data-ttu-id="6b96d-109">若要確保會對您的變更進行編目，可以明確[要求為清單或文件庫重新編製索引](https://docs.microsoft.com/zh-TW/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="6b96d-109">To make sure that your changes are crawled and reindexed, you can specifically request a reindexing of the list or library.</span></span> 

<span data-ttu-id="6b96d-110">如需完整搜尋結構描述的概觀，請參閱[簡介搜尋結構描述 (英文)](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="6b96d-110">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 

