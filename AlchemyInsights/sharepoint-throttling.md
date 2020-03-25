---
title: SharePoint 線上節流
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931433"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="f0b26-102">SharePoint 線上節流</span><span class="sxs-lookup"><span data-stu-id="f0b26-102">SharePoint Online throttling</span></span>

<span data-ttu-id="f0b26-103">**重要**：許多 SharePoint 線上及 OneDrive 客戶對在後臺執行的服務執行業務關鍵型應用程式。</span><span class="sxs-lookup"><span data-stu-id="f0b26-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f0b26-104">包括內容遷移、資料遺失防護（DLP）及備份解決方案。</span><span class="sxs-lookup"><span data-stu-id="f0b26-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f0b26-105">在這些空前的時間內，我們採取的步驟，確定在遠端工作案例中，線上和 OneDrive 服務的 SharePoint，都為您的使用者提供高可用性和更可靠的服務。</span><span class="sxs-lookup"><span data-stu-id="f0b26-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f0b26-106">為了支援這專案標，我們已在星期幾的白天時段內，對背景應用程式（遷移、DLP 和備份解決方案）進行更為緊密的節流限制。</span><span class="sxs-lookup"><span data-stu-id="f0b26-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f0b26-107">您應該會認為，這些應用程式在這段時間內可達到非常有限的輸送量。</span><span class="sxs-lookup"><span data-stu-id="f0b26-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f0b26-108">不過，當地區的晚上和週末時，服務會準備好處理來自背景應用程式的大量要求。</span><span class="sxs-lookup"><span data-stu-id="f0b26-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f0b26-109">**SharePoint 線上節流**</span><span class="sxs-lookup"><span data-stu-id="f0b26-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="f0b26-110">SharePoint 線上使用節流，以維持 SharePoint 線上服務的最佳效能和可靠性。</span><span class="sxs-lookup"><span data-stu-id="f0b26-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="f0b26-111">節流限制使用者動作數目或並行通話（按腳本或程式碼）以避免過度使用資源。</span><span class="sxs-lookup"><span data-stu-id="f0b26-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="f0b26-112">如需詳細資訊，請造訪下列連結。</span><span class="sxs-lookup"><span data-stu-id="f0b26-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="f0b26-113">如何避免在 SharePoint Online 中受到節流控制或封鎖</span><span class="sxs-lookup"><span data-stu-id="f0b26-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="f0b26-114">資料移轉和 SPO 節流</span><span class="sxs-lookup"><span data-stu-id="f0b26-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="f0b26-115">SharePoint Online 和 OneDrive 的移轉速度</span><span class="sxs-lookup"><span data-stu-id="f0b26-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="f0b26-116">使用指數回退來處理 SharePoint 線上節流</span><span class="sxs-lookup"><span data-stu-id="f0b26-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="f0b26-117">SharePoint Online 容量規劃和負載測試</span><span class="sxs-lookup"><span data-stu-id="f0b26-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

