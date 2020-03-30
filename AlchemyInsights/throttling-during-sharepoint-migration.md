---
title: 在 SharePoint 移轉期間節流
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "9000353"
- "1987"
- "9000136"
- "2968"
ms.assetid: ''
ms.openlocfilehash: dc77c462fcf32817c92709852e2d03ab2086b9a4
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958889"
---
# <a name="sharepoint-throttling"></a><span data-ttu-id="92174-102">SharePoint 節流</span><span class="sxs-lookup"><span data-stu-id="92174-102">SharePoint throttling</span></span>

<span data-ttu-id="92174-103">**重要**：在這些前所未有的情況下，我們會採取下列步驟以確保 SharePoint Online 和 OneDrive 服務保持高度可用 – 請造訪 [SharePoint Online 暫時功能調整](https://aka.ms/ODSPAdjustments)以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="92174-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="92174-104">**SharePoint Online 節流**</span><span class="sxs-lookup"><span data-stu-id="92174-104">**SharePoint Online throttling**</span></span>

<span data-ttu-id="92174-105">SharePoint Online 會使用節流來維護 SharePoint Online 服務的最佳效能和可靠性。</span><span class="sxs-lookup"><span data-stu-id="92174-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="92174-106">節流會限制使用者動作或同時通話的數目 (藉由指令碼或程式碼)，以避免過度使用資源。</span><span class="sxs-lookup"><span data-stu-id="92174-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span>

<span data-ttu-id="92174-107">如需詳細資訊，請瀏覽以下連結：</span><span class="sxs-lookup"><span data-stu-id="92174-107">For more information please visit the links below:</span></span>

- [<span data-ttu-id="92174-108">如何避免在 SharePoint Online 中受到節流控制或封鎖</span><span class="sxs-lookup"><span data-stu-id="92174-108">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)
- [<span data-ttu-id="92174-109">資料移轉和 SPO 節流</span><span class="sxs-lookup"><span data-stu-id="92174-109">Data Migration and SPO Throttling</span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)
- [<span data-ttu-id="92174-110">SharePoint Online 和 OneDrive 的移轉速度</span><span class="sxs-lookup"><span data-stu-id="92174-110">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
- [<span data-ttu-id="92174-111">使用指數輪詢來處理 SharePoint Online 節流</span><span class="sxs-lookup"><span data-stu-id="92174-111">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)
- [<span data-ttu-id="92174-112">SharePoint Online 容量規劃和負載測試</span><span class="sxs-lookup"><span data-stu-id="92174-112">Capacity planning and load testing SharePoint Online</span></span>](https://support.office.com/article/Capacity-planning-and-load-testing-SharePoint-Online-c932bd9b-fb9a-47ab-a330-6979d03688c0)
- [<span data-ttu-id="92174-113">我在移轉期間遇到效能不佳或節流情況</span><span class="sxs-lookup"><span data-stu-id="92174-113">I am experiencing poor performance or throttling during migration</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed#faq-and-troubleshooting)