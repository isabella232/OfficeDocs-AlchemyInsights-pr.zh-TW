---
title: 1491-搜尋-未傳回-預期結果
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510563"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="d5c94-102">內容搜尋未傳回預期的結果</span><span class="sxs-lookup"><span data-stu-id="d5c94-102">Content Search not returning expected results</span></span>

<span data-ttu-id="d5c94-103">從 Microsoft 365 security & 合規性中心執行內容搜尋時，您可能會收到意外的搜尋結果。</span><span class="sxs-lookup"><span data-stu-id="d5c94-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="d5c94-104">請考慮可能影響搜尋結果的下列專案：</span><span class="sxs-lookup"><span data-stu-id="d5c94-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="d5c94-105">**內容位置和搜尋條件**：請確定您已選取適當的內容位置和搜尋條件。</span><span class="sxs-lookup"><span data-stu-id="d5c94-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="d5c94-106">如果您執行大型搜尋（有許多位置），請考慮將其分割為多個搜尋。</span><span class="sxs-lookup"><span data-stu-id="d5c94-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="d5c94-107">**部分索引項目目**：信箱中的[部分已編制索引的專案](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search)會包含在預估的搜尋結果中。</span><span class="sxs-lookup"><span data-stu-id="d5c94-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="d5c94-108">不過，搜尋評估中不會包含從 SharePoint 和 OneDrive 中的網站部分編制索引的專案。</span><span class="sxs-lookup"><span data-stu-id="d5c94-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="d5c94-109">**搜尋失敗**：搜尋大量信箱（超過100000個信箱）時，您可能會收到搜尋錯誤，例如 CS008-009 和 CS012-002 等錯誤代碼。</span><span class="sxs-lookup"><span data-stu-id="d5c94-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="d5c94-110">在此情況下，只會針對失敗的內容位置，重試搜尋。</span><span class="sxs-lookup"><span data-stu-id="d5c94-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="d5c94-111">如需詳細資訊，請參閱[本文](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search)。</span><span class="sxs-lookup"><span data-stu-id="d5c94-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
