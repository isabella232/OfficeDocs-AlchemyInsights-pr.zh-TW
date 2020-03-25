---
title: SharePoint 含503錯誤的遷移節流
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931649"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="a7b34-102">SharePoint 含503錯誤的遷移節流</span><span class="sxs-lookup"><span data-stu-id="a7b34-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="a7b34-103">**重要**：許多 SharePoint 線上及 OneDrive 客戶對在後臺執行的服務執行業務關鍵型應用程式。</span><span class="sxs-lookup"><span data-stu-id="a7b34-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a7b34-104">包括內容遷移、資料遺失防護（DLP）及備份解決方案。</span><span class="sxs-lookup"><span data-stu-id="a7b34-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a7b34-105">在這些空前的時間內，我們採取的步驟，確定在遠端工作案例中，線上和 OneDrive 服務的 SharePoint，都為您的使用者提供高可用性和更可靠的服務。</span><span class="sxs-lookup"><span data-stu-id="a7b34-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a7b34-106">為了支援這專案標，我們已在星期幾的白天時段內，對背景應用程式（遷移、DLP 和備份解決方案）進行更為緊密的節流限制。</span><span class="sxs-lookup"><span data-stu-id="a7b34-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a7b34-107">您應該會認為，這些應用程式在這段時間內可達到非常有限的輸送量。</span><span class="sxs-lookup"><span data-stu-id="a7b34-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a7b34-108">不過，當地區的晚上和週末時，服務會準備好處理來自背景應用程式的大量要求。</span><span class="sxs-lookup"><span data-stu-id="a7b34-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="a7b34-109">**遷移至 SharePoint Online 時的503錯誤**</span><span class="sxs-lookup"><span data-stu-id="a7b34-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="a7b34-110">它似乎您正在遷移至 SharePoint 線上，且收到503錯誤。</span><span class="sxs-lookup"><span data-stu-id="a7b34-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="a7b34-111">請依照下列步驟進行，讓我們能夠儘快協助您。</span><span class="sxs-lookup"><span data-stu-id="a7b34-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="a7b34-112">按一下 [**連絡人支援**]，然後按一下 [**新增服務要求**]。</span><span class="sxs-lookup"><span data-stu-id="a7b34-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="a7b34-113">在 [標題與描述] 中，輸入**SharePoint 含503的遷移節流**。</span><span class="sxs-lookup"><span data-stu-id="a7b34-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="a7b34-114">送出票證後，請使用下列資訊更新它：</span><span class="sxs-lookup"><span data-stu-id="a7b34-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="a7b34-115">遷移的左側量（例如，多少 Tb？）。</span><span class="sxs-lookup"><span data-stu-id="a7b34-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="a7b34-116">遷移開始和結束日期。</span><span class="sxs-lookup"><span data-stu-id="a7b34-116">Migration start and end date.</span></span>
    - <span data-ttu-id="a7b34-117">描述您要從何處遷移內容，例如 SharePoint Server、Box、GDrive、檔案共用等等。</span><span class="sxs-lookup"><span data-stu-id="a7b34-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="a7b34-118">估計節流錯誤的數目（例如，每小時 x 節流？）以及節流的發生時間。</span><span class="sxs-lookup"><span data-stu-id="a7b34-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="a7b34-119">您正在使用哪個遷移工具（例如，SPMT 或 ShareGate）。</span><span class="sxs-lookup"><span data-stu-id="a7b34-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


