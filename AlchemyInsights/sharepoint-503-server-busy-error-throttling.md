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
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931217"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="497d7-102">SharePoint 線上節流</span><span class="sxs-lookup"><span data-stu-id="497d7-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="497d7-103">**重要**：許多 SharePoint 線上及 OneDrive 客戶對在後臺執行的服務執行業務關鍵型應用程式。</span><span class="sxs-lookup"><span data-stu-id="497d7-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="497d7-104">包括內容遷移、資料遺失防護（DLP）及備份解決方案。</span><span class="sxs-lookup"><span data-stu-id="497d7-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="497d7-105">在這些空前的時間內，我們採取的步驟，確定在遠端工作案例中，線上和 OneDrive 服務的 SharePoint，都為您的使用者提供高可用性和更可靠的服務。</span><span class="sxs-lookup"><span data-stu-id="497d7-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="497d7-106">為了支援這專案標，我們已在星期幾的白天時段內，對背景應用程式（遷移、DLP 和備份解決方案）進行更為緊密的節流限制。</span><span class="sxs-lookup"><span data-stu-id="497d7-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="497d7-107">您應該會認為，這些應用程式在這段時間內可達到非常有限的輸送量。</span><span class="sxs-lookup"><span data-stu-id="497d7-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="497d7-108">不過，當地區的晚上和週末時，服務會準備好處理來自背景應用程式的大量要求。</span><span class="sxs-lookup"><span data-stu-id="497d7-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="497d7-109">**503伺服器忙碌錯誤**</span><span class="sxs-lookup"><span data-stu-id="497d7-109">**503 server is busy error**</span></span>

<span data-ttu-id="497d7-110">嘗試流覽至 SharePoint 或 OneDrive 網站時，使用者可能會收到503伺服器繁忙的錯誤。</span><span class="sxs-lookup"><span data-stu-id="497d7-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="497d7-111">此錯誤可能是由 SharePoint 服務中的節流所造成。</span><span class="sxs-lookup"><span data-stu-id="497d7-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="497d7-112">SharePoint 線上使用節流，以維持 SharePoint 線上服務的最佳效能和可靠性。</span><span class="sxs-lookup"><span data-stu-id="497d7-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="497d7-113">節流限制使用者動作數目或並行通話（按腳本或程式碼）以避免過度使用資源。</span><span class="sxs-lookup"><span data-stu-id="497d7-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="497d7-114">如需節流的詳細資訊，請參閱，[避免在線上 SharePoint 遭到節流或封鎖](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)。</span><span class="sxs-lookup"><span data-stu-id="497d7-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="497d7-115">如果您認為此錯誤與節流不相關，您可以流覽至[消息中心](https://portal.office.com/adminportal/home#/MessageCenter)以檢查您租使用者上是否有使用中的維護。</span><span class="sxs-lookup"><span data-stu-id="497d7-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="497d7-116">最後，請確定您已造訪 [[服務健康](https://portal.office.com/adminportal/home#/servicehealth)情況] 頁面，檢查任何可能發生的諮詢/事件。</span><span class="sxs-lookup"><span data-stu-id="497d7-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

