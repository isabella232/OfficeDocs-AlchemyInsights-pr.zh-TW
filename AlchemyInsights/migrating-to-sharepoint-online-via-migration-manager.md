---
title: 透過移轉管理器遷移至 SharePoint Online
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
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931870"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="b62cb-102">透過移轉管理器遷移至 SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b62cb-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="b62cb-103">**重要**：許多 SharePoint Online 和 OneDrive 客戶都會對在背景中執行的服務執行關鍵應用程式。</span><span class="sxs-lookup"><span data-stu-id="b62cb-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b62cb-104">其中包括內容移轉、資料遺失防護 (DLP) 及備份解決方案。</span><span class="sxs-lookup"><span data-stu-id="b62cb-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b62cb-105">在這些前所未有的情況中，我們會採取一些步驟來確保 SharePoint Online 和 OneDrive 服務保持高度可用和可靠的狀態，以便在遠端工作情況下比以往更依賴服務的使用者使用。</span><span class="sxs-lookup"><span data-stu-id="b62cb-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b62cb-106">為了支持這個目標，我們已在平日白天時段內對背景應用程式 (移轉、DLP 和備份解決方案) 上實施更嚴密的節流限制。</span><span class="sxs-lookup"><span data-stu-id="b62cb-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b62cb-107">在這些情況中，您會認為這些應用程式的輸送量相當有限。</span><span class="sxs-lookup"><span data-stu-id="b62cb-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b62cb-108">不過，在夜間和週末時段內，服務將會準備好處理來自背景應用程式的更大量要求。</span><span class="sxs-lookup"><span data-stu-id="b62cb-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b62cb-109">**移轉管理員**</span><span class="sxs-lookup"><span data-stu-id="b62cb-109">**Migration Manager**</span></span>

<span data-ttu-id="b62cb-110">移轉管理員位於新式 SharePoint 系統管理中心，可引導您完成用戶端的設定以及工作的建立。</span><span class="sxs-lookup"><span data-stu-id="b62cb-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="b62cb-111">您可以指定全域或工作層級設定、檢視所有進行中工作進度，以及下載彙總摘要和工作層級報告。</span><span class="sxs-lookup"><span data-stu-id="b62cb-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="b62cb-112">開始使用移轉管理員</span><span class="sxs-lookup"><span data-stu-id="b62cb-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="b62cb-113">設定移轉管理員用戶端</span><span class="sxs-lookup"><span data-stu-id="b62cb-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="b62cb-114">移轉管理員設定</span><span class="sxs-lookup"><span data-stu-id="b62cb-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
