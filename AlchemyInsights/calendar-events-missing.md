---
title: 行事曆事件遺失或未更新
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10932"
- "9001435"
ms.openlocfilehash: b114411d6285a68a41bbcbf64151c212ee2cf661
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819978"
---
# <a name="calendar-events-missing-or-not-updating"></a><span data-ttu-id="05ee4-102">行事曆事件遺失或未更新</span><span class="sxs-lookup"><span data-stu-id="05ee4-102">Calendar Events missing or not updating</span></span>

<span data-ttu-id="05ee4-103">如果行事曆事件遺失或未更新，請首先在 Outlook 中查看行事曆資料夾內容中的項目計數：</span><span class="sxs-lookup"><span data-stu-id="05ee4-103">If calendar items are missing or not updating, start by looking at the item count in your Calendar folder properties in Outlook:</span></span> 

1. <span data-ttu-id="05ee4-104">以滑鼠右鍵按一下受影響的使用者 **[行事曆]** 資料夾，然後選取 **[内容]**。</span><span class="sxs-lookup"><span data-stu-id="05ee4-104">Right-click on the affected user **Calendar** folder, and then select **Properties**.</span></span>

1. <span data-ttu-id="05ee4-105">選取 **[同步處理]** 索引標籤。</span><span class="sxs-lookup"><span data-stu-id="05ee4-105">Select the **Synchronization** tab.</span></span>

<span data-ttu-id="05ee4-106">如果伺服器資料夾和離線資料夾之間的項目計數不同：</span><span class="sxs-lookup"><span data-stu-id="05ee4-106">If the item count is not the same between the Server folder and the Offline Folder:</span></span>

1.  <span data-ttu-id="05ee4-107">醒目顯示 **[行事曆]** 資料夾。</span><span class="sxs-lookup"><span data-stu-id="05ee4-107">Highlight the **Calendar** folder.</span></span>

1.  <span data-ttu-id="05ee4-108">前往 **[傳送]**/**[接收]** 索引標籤，然後選取 **[更新資料夾]**。</span><span class="sxs-lookup"><span data-stu-id="05ee4-108">Go to the **Send**/**Receive** tab, and then select **Update Folder**.</span></span>

<span data-ttu-id="05ee4-109">如果仍未更新行事曆或遺失事件，請從 [Microsoft 下載中心](https://www.microsoft.com/download/details.aspx?id=28786)下載 Outlook 行事曆檢查工具。</span><span class="sxs-lookup"><span data-stu-id="05ee4-109">If your calendar is still not updating or events are missing, download the Calendar Checking Tool for Outlook from the [Microsoft download center](https://www.microsoft.com/download/details.aspx?id=28786).</span></span> <span data-ttu-id="05ee4-110">確定行事曆資料夾中的項目是否超過 5000 個，因為這可能導致行事曆會議未更新或會議錯誤等問題。</span><span class="sxs-lookup"><span data-stu-id="05ee4-110">Determine if there are more than 5000 items in the calendar folder as this can cause symptoms such as calendar meetings not updated or meeting errors.</span></span> 

<span data-ttu-id="05ee4-111">如需詳細資訊，請參閱[快取模式 .ost 或 .pst 檔案中的項目或資料夾過多時的 Outlook 效能問題](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders)。</span><span class="sxs-lookup"><span data-stu-id="05ee4-111">For more information, see [Outlook performance issues when there are too many items or folders in a cached mode .ost or .pst file](https://docs.microsoft.com/outlook/troubleshoot/performance/performance-issues-if-too-many-items-or-folders).</span></span>