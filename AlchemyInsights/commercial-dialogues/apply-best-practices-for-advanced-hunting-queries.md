---
title: 套用高級搜尋查詢的最佳作法
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736018"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="9538b-102">套用高級搜尋查詢的最佳作法</span><span class="sxs-lookup"><span data-stu-id="9538b-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="9538b-103">若要更快地取得結果，並避免執行複雜查詢時超時，請套用下列最佳作法：</span><span class="sxs-lookup"><span data-stu-id="9538b-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="9538b-104">嘗試新的查詢時，一定要使用限制，以避免取得極大的結果集。</span><span class="sxs-lookup"><span data-stu-id="9538b-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="9538b-105">此外，您也 `count` 可以使用來進行初始評估結果集的大小。</span><span class="sxs-lookup"><span data-stu-id="9538b-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="9538b-106">首先使用時間篩選。</span><span class="sxs-lookup"><span data-stu-id="9538b-106">Use time filters first.</span></span> <span data-ttu-id="9538b-107">理想狀況下，將您的查詢限制為七天。</span><span class="sxs-lookup"><span data-stu-id="9538b-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="9538b-108">在查詢的開頭，在時間篩選器之後，新增預期的篩選，以移除大部分的資料。</span><span class="sxs-lookup"><span data-stu-id="9538b-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="9538b-109">尋找完整的標記時，請使用 `has` 運算子而非 `contains` 。</span><span class="sxs-lookup"><span data-stu-id="9538b-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="9538b-110">針對特定欄執行搜尋，而不是在所有欄上執行搜尋。</span><span class="sxs-lookup"><span data-stu-id="9538b-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="9538b-111">當加入資料表時，請先以較少的列指定資料表。</span><span class="sxs-lookup"><span data-stu-id="9538b-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="9538b-112">`project` 只從您已加入之資料表的必要欄。</span><span class="sxs-lookup"><span data-stu-id="9538b-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="9538b-113">若要深入瞭解，請參閱 [高級搜尋查詢最佳作法](https://go.microsoft.com/fwlink/?linkid=2144812)。</span><span class="sxs-lookup"><span data-stu-id="9538b-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
