---
title: SharePoint 線上節流
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 2aca55ac2fefbb2035140a759a77730dc905a4e9
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958709"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="a07e2-102">SharePoint 線上節流</span><span class="sxs-lookup"><span data-stu-id="a07e2-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="a07e2-103">**重要**事項：在這些空前的時間內，我們採取步驟來確保 SharePoint 線上和 OneDrive 服務保持高可用性–請流覽[SharePoint 線上暫存功能](https://aka.ms/ODSPAdjustments)，以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="a07e2-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="a07e2-104">**503伺服器忙碌錯誤**</span><span class="sxs-lookup"><span data-stu-id="a07e2-104">**503 server is busy error**</span></span>

<span data-ttu-id="a07e2-105">嘗試流覽至 SharePoint 或 OneDrive 網站時，使用者可能會收到503伺服器繁忙的錯誤。</span><span class="sxs-lookup"><span data-stu-id="a07e2-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="a07e2-106">此錯誤可能是由 SharePoint 服務中的節流所造成。</span><span class="sxs-lookup"><span data-stu-id="a07e2-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="a07e2-107">SharePoint 線上使用節流，以維持 SharePoint 線上服務的最佳效能和可靠性。</span><span class="sxs-lookup"><span data-stu-id="a07e2-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="a07e2-108">節流限制使用者動作數目或並行通話（按腳本或程式碼）以避免過度使用資源。</span><span class="sxs-lookup"><span data-stu-id="a07e2-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="a07e2-109">如需節流的詳細資訊，請參閱，[避免在線上 SharePoint 遭到節流或封鎖](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)。</span><span class="sxs-lookup"><span data-stu-id="a07e2-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="a07e2-110">如果您認為此錯誤與節流不相關，您可以流覽至[消息中心](https://portal.office.com/adminportal/home#/MessageCenter)以檢查您租使用者上是否有使用中的維護。</span><span class="sxs-lookup"><span data-stu-id="a07e2-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="a07e2-111">最後，請確定您已造訪 [[服務健康](https://portal.office.com/adminportal/home#/servicehealth)情況] 頁面，檢查任何可能發生的諮詢/事件。</span><span class="sxs-lookup"><span data-stu-id="a07e2-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

