---
title: 效能問題-SharePoint 或 OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771892"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="f291f-102">SharePoint 或 OneDrive 多個使用者的慢速、無法存取或無法使用</span><span class="sxs-lookup"><span data-stu-id="f291f-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="f291f-103">SharePoint 或 OneDrive 可能會變慢、無法存取或無法使用，或顯示服務無法使用或503錯誤，其原因有多種：</span><span class="sxs-lookup"><span data-stu-id="f291f-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="f291f-104">如果您的 SharePoint 或 OneDrive 網站的執行速度很慢或延遲多個使用者，則在存取 SharePoint 網站或 OneDrive 內容時，使用者可能會遇到延遲延遲或流覽錯誤的暫時性服務問題。</span><span class="sxs-lookup"><span data-stu-id="f291f-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="f291f-105">請查看[服務健康情況儀表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)，了解您的組織是否受到影響。</span><span class="sxs-lookup"><span data-stu-id="f291f-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="f291f-106">嘗試流覽至 SharePoint 或 OneDrive 網站時，使用者可能會收到 *503 伺服器繁忙* 的錯誤。</span><span class="sxs-lookup"><span data-stu-id="f291f-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="f291f-107">此錯誤可能是由 SharePoint 服務中的節流所造成。</span><span class="sxs-lookup"><span data-stu-id="f291f-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="f291f-108">SharePoint Online 會使用節流來維護 SharePoint Online 服務的最佳效能和可靠性。</span><span class="sxs-lookup"><span data-stu-id="f291f-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="f291f-109">節流會限制使用者動作或同時通話的數目 (藉由指令碼或程式碼)，以避免過度使用資源。</span><span class="sxs-lookup"><span data-stu-id="f291f-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="f291f-110">如需節流的詳細資訊，請參閱， [避免在線上 SharePoint 遭到節流或封鎖](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)。</span><span class="sxs-lookup"><span data-stu-id="f291f-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="f291f-111">如果您使用 **傳統** 或 **新式** SharePoint 網站或頁面時速度變慢，請利用 [頁面診斷工具](https://aka.ms/perftool) 來分析頁面。</span><span class="sxs-lookup"><span data-stu-id="f291f-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="f291f-112">如果您仍遇到一般緩慢效能，請參閱本文底部的資源： [SharePoint 線上的效能調整簡介](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="f291f-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  