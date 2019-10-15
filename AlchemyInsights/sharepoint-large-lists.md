---
title: SharePoint 大型清單
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488508"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="38149-102">用來處理大型清單和文件庫的 SharePoint</span><span class="sxs-lookup"><span data-stu-id="38149-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="38149-103">SharePoint 清單與文件庫可以包含最多 30 萬個項目，但是當他們有超過 5000 個項目時，您可能會看到一個清單檢視臨界值的錯誤時您嘗試進行處理。</span><span class="sxs-lookup"><span data-stu-id="38149-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="38149-104">這個臨界值是以維護服務的效能。</span><span class="sxs-lookup"><span data-stu-id="38149-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="38149-105">您無法變更。</span><span class="sxs-lookup"><span data-stu-id="38149-105">It can't be changed.</span></span> <span data-ttu-id="38149-106">若要避免此臨界值：</span><span class="sxs-lookup"><span data-stu-id="38149-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="38149-107">**使用新式**</span><span class="sxs-lookup"><span data-stu-id="38149-107">**Use modern**</span></span>

<span data-ttu-id="38149-108">檢視顯示許多項目的運作起來最順暢中的新式體驗。</span><span class="sxs-lookup"><span data-stu-id="38149-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="38149-109">若要避免的錯誤可能會看到傳統經驗中[使用的新式體驗](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9)。</span><span class="sxs-lookup"><span data-stu-id="38149-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="38149-110">**新增索引**</span><span class="sxs-lookup"><span data-stu-id="38149-110">**Add indexes**</span></span>

<span data-ttu-id="38149-111">當您篩選或排序都不會有索引欄中，您可能會看到一則錯誤訊息。</span><span class="sxs-lookup"><span data-stu-id="38149-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="38149-112">以手動方式從 [**清單設定**在 [設定] 功能表，然後**編製索引的資料行**中[新增的索引](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0)。</span><span class="sxs-lookup"><span data-stu-id="38149-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="38149-113">**編輯清單檢視**</span><span class="sxs-lookup"><span data-stu-id="38149-113">**Edit the list view**</span></span>

<span data-ttu-id="38149-114">如果使用大型清單，[編輯清單檢視](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)時，就會發生錯誤。</span><span class="sxs-lookup"><span data-stu-id="38149-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="38149-115">下列四個變更將會移除清單檢視臨界值錯誤。</span><span class="sxs-lookup"><span data-stu-id="38149-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="38149-116">變更所有四個要移除所有錯誤。</span><span class="sxs-lookup"><span data-stu-id="38149-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="38149-117">如果您仍會發生錯誤，請檢查[管理大型清單和文件庫](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)。</span><span class="sxs-lookup"><span data-stu-id="38149-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="38149-118">選取 [**無]** **先依欄排序**和**然後依欄排序**。</span><span class="sxs-lookup"><span data-stu-id="38149-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="38149-119">選取 [**無]** 從**依欄的第一個群組**，**然後依欄群組**。</span><span class="sxs-lookup"><span data-stu-id="38149-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="38149-120">選取 [**無]** 的 [**總計**] 區段中的所有欄。</span><span class="sxs-lookup"><span data-stu-id="38149-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="38149-121">取消選取所有但一欄，從 [**欄**] 區段中的顯示。</span><span class="sxs-lookup"><span data-stu-id="38149-121">Deselect all but one column for display from the **Columns** section.</span></span>

