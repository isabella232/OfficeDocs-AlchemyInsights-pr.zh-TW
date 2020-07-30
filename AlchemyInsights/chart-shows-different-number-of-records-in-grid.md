---
title: 圖表顯示格線中不同數量的記錄
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431452"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="04ccb-102">圖表顯示格線中不同數量的記錄</span><span class="sxs-lookup"><span data-stu-id="04ccb-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="04ccb-103">**徵狀**</span><span class="sxs-lookup"><span data-stu-id="04ccb-103">**Symptom**</span></span>

<span data-ttu-id="04ccb-104">在儀表板頁面上，當您按一下 [圖表] “…” 並按一下 [查看記錄] 時，將瀏覽至格線頁查看所有記錄。有時候，記錄數會發變更。</span><span class="sxs-lookup"><span data-stu-id="04ccb-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="04ccb-105">**原因**</span><span class="sxs-lookup"><span data-stu-id="04ccb-105">**Cause**</span></span>

<span data-ttu-id="04ccb-106">這是因為原始儀表板頁面上的圖表與格線首頁上的圖表有所不同。</span><span class="sxs-lookup"><span data-stu-id="04ccb-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="04ccb-107">**解決方案**</span><span class="sxs-lookup"><span data-stu-id="04ccb-107">**Solution**</span></span>

1. <span data-ttu-id="04ccb-108">檢查原始頁面和格線中的視圖，查看它們是否不同。</span><span class="sxs-lookup"><span data-stu-id="04ccb-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="04ccb-109">變更格線中的視圖，使之與原始頁面中的視圖相符。</span><span class="sxs-lookup"><span data-stu-id="04ccb-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="04ccb-110">如果找不到正確的視圖，通常表示應用程式設計工具中沒有啟用該視圖。</span><span class="sxs-lookup"><span data-stu-id="04ccb-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="04ccb-111">移至特定應用程式的的 [應用程式設計工具]，選擇實體及其視圖，檢查您要啟用、儲存、發佈和關閉的視圖。</span><span class="sxs-lookup"><span data-stu-id="04ccb-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="04ccb-112">重新整理頁面。</span><span class="sxs-lookup"><span data-stu-id="04ccb-112">Refresh the page.</span></span>