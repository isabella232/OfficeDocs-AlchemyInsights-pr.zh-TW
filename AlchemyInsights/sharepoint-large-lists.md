---
title: SharePoint 大型清單
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767276"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="2fe79-102">使用 SharePoint 中的大型清單和文件庫</span><span class="sxs-lookup"><span data-stu-id="2fe79-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="2fe79-103">SharePoint 清單和文件庫最多可以包含30000000個專案，但是當其具有超過5000個專案時，當您嘗試使用這些專案時，可能會看到清單檢視閾值錯誤。</span><span class="sxs-lookup"><span data-stu-id="2fe79-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="2fe79-104">此閾值存在的目的是為了維持服務效能。</span><span class="sxs-lookup"><span data-stu-id="2fe79-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="2fe79-105">您無法對它進行變更。</span><span class="sxs-lookup"><span data-stu-id="2fe79-105">It can't be changed.</span></span> <span data-ttu-id="2fe79-106">若要避免達到此臨界值：</span><span class="sxs-lookup"><span data-stu-id="2fe79-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="2fe79-107">**使用現代**</span><span class="sxs-lookup"><span data-stu-id="2fe79-107">**Use modern**</span></span>

<span data-ttu-id="2fe79-108">顯示許多專案在新式體驗中最適合運作的視圖。</span><span class="sxs-lookup"><span data-stu-id="2fe79-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="2fe79-109">[使用現代化的經驗](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9)，避免您在傳統體驗中所看到的錯誤。</span><span class="sxs-lookup"><span data-stu-id="2fe79-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="2fe79-110">**新增索引**</span><span class="sxs-lookup"><span data-stu-id="2fe79-110">**Add indexes**</span></span>

<span data-ttu-id="2fe79-111">當您以沒有索引的資料行篩選或排序時，可能會看到錯誤訊息。</span><span class="sxs-lookup"><span data-stu-id="2fe79-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="2fe79-112">從 [設定] 功能表中的 [**清單設定**] 手動[新增索引](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0)，然後再以**索引欄**。</span><span class="sxs-lookup"><span data-stu-id="2fe79-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="2fe79-113">**編輯清單視圖**</span><span class="sxs-lookup"><span data-stu-id="2fe79-113">**Edit the list view**</span></span>

<span data-ttu-id="2fe79-114">如果使用大型清單時發生錯誤，請[編輯清單視圖](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)。</span><span class="sxs-lookup"><span data-stu-id="2fe79-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="2fe79-115">下列四項變更將會移除清單視圖臨界值錯誤。</span><span class="sxs-lookup"><span data-stu-id="2fe79-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="2fe79-116">進行四個變更，以移除所有的錯誤。</span><span class="sxs-lookup"><span data-stu-id="2fe79-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="2fe79-117">如果仍有錯誤，請參閱[管理大型清單和文件庫](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)。</span><span class="sxs-lookup"><span data-stu-id="2fe79-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="2fe79-118">從**欄的第一個排序選取 [** **無**]，**然後依資料行排序**。</span><span class="sxs-lookup"><span data-stu-id="2fe79-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="2fe79-119">從**第一個群組**中選取 [**無**]，**然後按該列進行群組**。</span><span class="sxs-lookup"><span data-stu-id="2fe79-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="2fe79-120">選取 [**總計**] 區段中所有欄的 [**無**]。</span><span class="sxs-lookup"><span data-stu-id="2fe79-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="2fe79-121">取消選取 [**欄**] 區段中的 [所有] （顯示一欄）。</span><span class="sxs-lookup"><span data-stu-id="2fe79-121">Deselect all but one column for display from the **Columns** section.</span></span>

