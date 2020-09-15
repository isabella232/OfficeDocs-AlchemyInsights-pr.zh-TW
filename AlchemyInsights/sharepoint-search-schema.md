---
title: 在 SharePoint Online 中管理搜尋架構
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770542"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="191e7-102">在 SharePoint Online 中管理搜尋架構</span><span class="sxs-lookup"><span data-stu-id="191e7-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="191e7-103">搜尋架構會控制使用者可以搜尋的內容、使用者可搜尋的內容，以及在搜尋網站上顯示結果的方式。</span><span class="sxs-lookup"><span data-stu-id="191e7-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="191e7-104">請參閱 [管理 SharePoint Online 中的搜尋架構](https://docs.microsoft.com/sharepoint/manage-search-schema) ，瞭解如何：</span><span class="sxs-lookup"><span data-stu-id="191e7-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="191e7-105">變更搜尋架構。</span><span class="sxs-lookup"><span data-stu-id="191e7-105">Change the search schema.</span></span>
- <span data-ttu-id="191e7-106">建立 managed 屬性。</span><span class="sxs-lookup"><span data-stu-id="191e7-106">Create managed properties.</span></span>
- <span data-ttu-id="191e7-107">將編目編目屬性對應到 managed 屬性。</span><span class="sxs-lookup"><span data-stu-id="191e7-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="191e7-108">請注意下列有關管理搜尋架構的事項：</span><span class="sxs-lookup"><span data-stu-id="191e7-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="191e7-109">如果您收到一則警告，指出在進行架構變更時 **已暫停應用程式** ，這只是服務維護髮生時的暫時性。</span><span class="sxs-lookup"><span data-stu-id="191e7-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="191e7-110">超過24小時後，您仍會遇到警告，請記錄支援案例。</span><span class="sxs-lookup"><span data-stu-id="191e7-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="191e7-111">當您變更 managed 屬性或新增新的屬性時，只有重新編目內容之後，變更才會生效。</span><span class="sxs-lookup"><span data-stu-id="191e7-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="191e7-112">在線上 SharePoint 中，編目會根據定義的編目排程自動進行。</span><span class="sxs-lookup"><span data-stu-id="191e7-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="191e7-113">若要確定您的變更已編目，您可以特別 [要求重新建立清單或文件庫的索引](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="191e7-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="191e7-114">如需搜尋架構的完整綜述，請參閱 [簡介搜尋架構](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="191e7-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


