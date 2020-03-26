---
title: SharePoint 移轉效能
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931882"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="cd181-102">SharePoint 移轉效能</span><span class="sxs-lookup"><span data-stu-id="cd181-102">SharePoint migration performance</span></span>

<span data-ttu-id="cd181-103">**重要**：許多 SharePoint Online 和 OneDrive 客戶都會對在背景中執行的服務執行關鍵應用程式。</span><span class="sxs-lookup"><span data-stu-id="cd181-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="cd181-104">其中包括內容移轉、資料遺失防護 (DLP) 及備份解決方案。</span><span class="sxs-lookup"><span data-stu-id="cd181-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="cd181-105">在這些前所未有的情況中，我們會採取一些步驟來確保 SharePoint Online 和 OneDrive 服務保持高度可用和可靠的狀態，以便在遠端工作情況下比以往更依賴服務的使用者使用。</span><span class="sxs-lookup"><span data-stu-id="cd181-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="cd181-106">為了支持這個目標，我們已在平日白天時段內對背景應用程式 (移轉、DLP 和備份解決方案) 上實施更嚴密的節流限制。</span><span class="sxs-lookup"><span data-stu-id="cd181-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="cd181-107">在這些情況中，您會認為這些應用程式的輸送量相當有限。</span><span class="sxs-lookup"><span data-stu-id="cd181-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="cd181-108">不過，在夜間和週末時段內，服務將會準備好處理來自背景應用程式的更大量要求。</span><span class="sxs-lookup"><span data-stu-id="cd181-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="cd181-109">**移轉效能**</span><span class="sxs-lookup"><span data-stu-id="cd181-109">**Migration performance**</span></span>

<span data-ttu-id="cd181-p103">移轉效能可能會受到網路基礎結構、檔案大小、移轉時間和節流的影響。了解這些可協助您規劃並最佳化您的移轉效能。</span><span class="sxs-lookup"><span data-stu-id="cd181-p103">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling. Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="cd181-112">如需詳細資訊，請瀏覽以下連結。</span><span class="sxs-lookup"><span data-stu-id="cd181-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="cd181-113">SharePoint Online 和 ODB 的移轉速度</span><span class="sxs-lookup"><span data-stu-id="cd181-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="cd181-114">如何避免在 SharePoint Online 中受到節流控制或封鎖</span><span class="sxs-lookup"><span data-stu-id="cd181-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="cd181-115">下載並安裝 SharePoint 移轉工具</span><span class="sxs-lookup"><span data-stu-id="cd181-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
