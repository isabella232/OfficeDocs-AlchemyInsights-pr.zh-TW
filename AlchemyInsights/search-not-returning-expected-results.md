---
title: 1491-搜尋-未傳回-預期結果
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355868"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="be78e-102">內容搜尋未傳回預期的結果</span><span class="sxs-lookup"><span data-stu-id="be78e-102">Content Search not returning expected results</span></span>

<span data-ttu-id="be78e-103">從 Office 365 安全性 & 規範中心執行內容搜尋時, 您可能會收到未預期的搜尋結果。</span><span class="sxs-lookup"><span data-stu-id="be78e-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="be78e-104">請考慮下列可能會影響搜尋結果的專案:</span><span class="sxs-lookup"><span data-stu-id="be78e-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="be78e-105">**內容位置和搜尋條件**: 請確定您已選取適當的內容位置和搜尋條件。</span><span class="sxs-lookup"><span data-stu-id="be78e-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="be78e-106">如果您執行大型搜尋 (有許多位置), 請考慮將它分割成多個搜尋。</span><span class="sxs-lookup"><span data-stu-id="be78e-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="be78e-107">**部分編制索引的專案**: 信箱中的[部分已編制索引的專案](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search)會包含在預估的搜尋結果中。</span><span class="sxs-lookup"><span data-stu-id="be78e-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="be78e-108">不過, 在 SharePoint 和 OneDrive 中的網站已部分編制索引的專案不會包含在搜尋預估中。</span><span class="sxs-lookup"><span data-stu-id="be78e-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="be78e-109">**搜尋失敗**: 搜尋大量信箱 (超過100000個信箱) 時, 您可能會收到搜尋錯誤, 如 CS008-009 和 CS012-002 等錯誤代碼。</span><span class="sxs-lookup"><span data-stu-id="be78e-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="be78e-110">在這種情況下, 請僅針對失敗的內容位置重試搜尋。</span><span class="sxs-lookup"><span data-stu-id="be78e-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="be78e-111">如需詳細資訊, 請參閱[本文](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)。</span><span class="sxs-lookup"><span data-stu-id="be78e-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
