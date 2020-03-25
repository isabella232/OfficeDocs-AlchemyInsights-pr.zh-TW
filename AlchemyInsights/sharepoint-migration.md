---
title: 將選項遷移至 SharePoint 線上
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932721"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="601d5-102">將選項遷移至 SharePoint 線上</span><span class="sxs-lookup"><span data-stu-id="601d5-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="601d5-103">**重要**：許多 SharePoint 線上及 OneDrive 客戶對在後臺執行的服務執行業務關鍵型應用程式。</span><span class="sxs-lookup"><span data-stu-id="601d5-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="601d5-104">包括內容遷移、資料遺失防護（DLP）及備份解決方案。</span><span class="sxs-lookup"><span data-stu-id="601d5-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="601d5-105">在這些空前的時間內，我們採取的步驟，確定在遠端工作案例中，線上和 OneDrive 服務的 SharePoint，都為您的使用者提供高可用性和更可靠的服務。</span><span class="sxs-lookup"><span data-stu-id="601d5-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="601d5-106">為了支援這專案標，我們已在星期幾的白天時段內，對背景應用程式（遷移、DLP 和備份解決方案）進行更為緊密的節流限制。</span><span class="sxs-lookup"><span data-stu-id="601d5-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="601d5-107">您應該會認為，這些應用程式在這段時間內可達到非常有限的輸送量。</span><span class="sxs-lookup"><span data-stu-id="601d5-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="601d5-108">不過，當地區的晚上和週末時，服務會準備好處理來自背景應用程式的大量要求。</span><span class="sxs-lookup"><span data-stu-id="601d5-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="601d5-109">**遷移選項**</span><span class="sxs-lookup"><span data-stu-id="601d5-109">**Migration options**</span></span>

<span data-ttu-id="601d5-110">您可以使用不同的選項，將內容遷移至 SharePoint 線上，具體取決於您需要移動的檔案大小與數量，請參閱[此處](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online)的選項清單。</span><span class="sxs-lookup"><span data-stu-id="601d5-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="601d5-111">如需有關內容遷移的詳細資訊，請流覽下列連結。</span><span class="sxs-lookup"><span data-stu-id="601d5-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="601d5-112">Sharepoint 遷移工具</span><span class="sxs-lookup"><span data-stu-id="601d5-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="601d5-113">開始使用移轉管理程式</span><span class="sxs-lookup"><span data-stu-id="601d5-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="601d5-114">Sharepoint Online 和 ODB 遷移速度</span><span class="sxs-lookup"><span data-stu-id="601d5-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="601d5-115">如何避免在 SharePoint Online 中受到節流控制或封鎖</span><span class="sxs-lookup"><span data-stu-id="601d5-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="601d5-116">SharePoint 遷移評估工具（SMAT）</span><span class="sxs-lookup"><span data-stu-id="601d5-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="601d5-117">**附注**：目前的 SharePoint 遷移工具僅支援從 SharePoint 2010 和2013進行遷移。</span><span class="sxs-lookup"><span data-stu-id="601d5-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="601d5-118">目前不支援版本2016或2019。</span><span class="sxs-lookup"><span data-stu-id="601d5-118">Version 2016 or 2019 are not supported at this time.</span></span>
