---
title: 一般移轉效能指引
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
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932470"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="04d14-102">一般移轉效能指引</span><span class="sxs-lookup"><span data-stu-id="04d14-102">General migration performance guidance</span></span>

<span data-ttu-id="04d14-103">**重要**：許多 SharePoint Online 和 OneDrive 客戶都會對在背景中執行的服務執行關鍵應用程式。</span><span class="sxs-lookup"><span data-stu-id="04d14-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="04d14-104">其中包括內容移轉、資料遺失防護 (DLP) 及備份解決方案。</span><span class="sxs-lookup"><span data-stu-id="04d14-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="04d14-105">在這些前所未有的情況中，我們會採取一些步驟來確保 SharePoint Online 和 OneDrive 服務保持高度可用和可靠的狀態，以便在遠端工作情況下比以往更依賴服務的使用者使用。</span><span class="sxs-lookup"><span data-stu-id="04d14-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="04d14-106">為了支持這個目標，我們已在平日白天時段內對背景應用程式 (移轉、DLP 和備份解決方案) 上實施更嚴密的節流限制。</span><span class="sxs-lookup"><span data-stu-id="04d14-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="04d14-107">在這些情況中，您會認為這些應用程式的輸送量相當有限。</span><span class="sxs-lookup"><span data-stu-id="04d14-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="04d14-108">不過，在夜間和週末時段內，服務將會準備好處理來自背景應用程式的更大量要求。</span><span class="sxs-lookup"><span data-stu-id="04d14-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="04d14-109">**移轉效能指引**</span><span class="sxs-lookup"><span data-stu-id="04d14-109">**Migration performance guidance**</span></span>

<span data-ttu-id="04d14-p103">移轉效能可能會受到網路基礎結構、檔案大小、移轉時間和節流的影響。了解這些可協助您規劃並最佳化您的移轉效能。</span><span class="sxs-lookup"><span data-stu-id="04d14-p103">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling. Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="04d14-112">一般移轉效能指引</span><span class="sxs-lookup"><span data-stu-id="04d14-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
