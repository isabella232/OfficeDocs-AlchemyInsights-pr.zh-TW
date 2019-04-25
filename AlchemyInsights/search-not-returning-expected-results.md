---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383826"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="4f134-102">未預期的結果傳回的內容搜尋</span><span class="sxs-lookup"><span data-stu-id="4f134-102">Content Search not returning expected results</span></span>

<span data-ttu-id="4f134-103">從 Office 365 安全性 & 合規性中心執行內容搜尋，您可能會收到未預期的搜尋結果。</span><span class="sxs-lookup"><span data-stu-id="4f134-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="4f134-104">請考慮下列事項，可能會影響您的搜尋結果：</span><span class="sxs-lookup"><span data-stu-id="4f134-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="4f134-105">**內容的位置和搜尋條件**： 請確定您已選取適當的內容位置和搜尋條件。</span><span class="sxs-lookup"><span data-stu-id="4f134-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="4f134-106">如果您執行大型搜尋 （使用許多位置），請考慮將它分割成多個搜尋。</span><span class="sxs-lookup"><span data-stu-id="4f134-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="4f134-107">**已局部編製索引的項目**： 預估的搜尋結果中隨附的信箱的[已局部編製索引的項目](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search)。</span><span class="sxs-lookup"><span data-stu-id="4f134-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="4f134-108">不過，SharePoint 和 OneDrive 中的網站中的已局部編製索引項目不包含在搜尋估計值。</span><span class="sxs-lookup"><span data-stu-id="4f134-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="4f134-109">**搜尋失敗**： 當您搜尋大量信箱 （超過 100000 信箱），您可能會收到搜尋錯誤，例如 CS008 009 和 CS012-002 錯誤碼)。</span><span class="sxs-lookup"><span data-stu-id="4f134-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="4f134-110">在此情況下，再試一次僅針對失敗的內容位置的搜尋。</span><span class="sxs-lookup"><span data-stu-id="4f134-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="4f134-111">請參閱[這篇文章](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)如需詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="4f134-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
