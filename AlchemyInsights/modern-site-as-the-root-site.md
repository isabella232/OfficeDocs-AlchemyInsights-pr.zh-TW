---
title: 新式網站作為根網站
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666861"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="d043a-102">新式網站為根網站</span><span class="sxs-lookup"><span data-stu-id="d043a-102">Modern site as root site</span></span>

<span data-ttu-id="d043a-103">我們已開始推出新功能，可讓您將 [傳統網站根網站與現代網站交換](https://docs.microsoft.com/sharepoint/modern-root-site)。</span><span class="sxs-lookup"><span data-stu-id="d043a-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="d043a-104">使用 [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) 在封存原始網站時，將網站的位置交換為另一個網站。</span><span class="sxs-lookup"><span data-stu-id="d043a-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="d043a-105">可用於兩個小組網站 (未連接至群組) 和通訊網站。</span><span class="sxs-lookup"><span data-stu-id="d043a-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="d043a-106">請勿刪除傳統的根網站來建立新式的通訊網站。</span><span class="sxs-lookup"><span data-stu-id="d043a-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="d043a-107">Microsoft 不支援此功能。</span><span class="sxs-lookup"><span data-stu-id="d043a-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="d043a-108">刪除根網站會使所有的使用者都無法存取組織中的所有 SharePoint 網站，直到您還原網站或在相同 URL 上建立新網站為止。</span><span class="sxs-lookup"><span data-stu-id="d043a-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="d043a-109">我們將透過訊息中心來傳遞這項功能。</span><span class="sxs-lookup"><span data-stu-id="d043a-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="d043a-110">您應該會在您的租使用者中立即開啟此功能。</span><span class="sxs-lookup"><span data-stu-id="d043a-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="d043a-111">交換網站的已知問題</span><span class="sxs-lookup"><span data-stu-id="d043a-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="d043a-112">目標網站可能會在 HTTP 404) 錯誤的一小段時間內傳回「找不到」 (。</span><span class="sxs-lookup"><span data-stu-id="d043a-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="d043a-113">內容將需要重新編目更新搜尋索引。</span><span class="sxs-lookup"><span data-stu-id="d043a-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="d043a-114">沒有必要手動步驟，這將會自動完成。</span><span class="sxs-lookup"><span data-stu-id="d043a-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="d043a-115">任何依存于「靜態」連結 (（例如檔案同步處理及 OneNote 檔案）的內容，) 將需要手動修正。</span><span class="sxs-lookup"><span data-stu-id="d043a-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="d043a-116">可能需要驗證 Project Server 網站，以確保它們仍然有正確相關聯。</span><span class="sxs-lookup"><span data-stu-id="d043a-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
