---
title: 新式網站作為根網站
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 260048db6c439183da8e0bb0c2dfa3c7475fca79
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269367"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="292a2-102">新式網站作為根網站</span><span class="sxs-lookup"><span data-stu-id="292a2-102">Modern site as root site</span></span>

<span data-ttu-id="292a2-103">我們已開始導入可讓您將交換與新式網站您傳統網站的根網站的新功能。</span><span class="sxs-lookup"><span data-stu-id="292a2-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="292a2-104">使用[Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)封存原始網站時切換網站與其他網站的位置。</span><span class="sxs-lookup"><span data-stu-id="292a2-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="292a2-105">適用於小組網站 （未連線至群組） 及通訊網站。</span><span class="sxs-lookup"><span data-stu-id="292a2-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="292a2-106">請勿刪除傳統的根網站以建立新式通訊網站。</span><span class="sxs-lookup"><span data-stu-id="292a2-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="292a2-107">Microsoft 不支援此。</span><span class="sxs-lookup"><span data-stu-id="292a2-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="292a2-108">刪除根網站會使所有的 SharePoint 網站組織中所有使用者，無法存取直到您還原的網站，或在相同的 URL 建立新的網站。</span><span class="sxs-lookup"><span data-stu-id="292a2-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="292a2-109">我們將通訊透過訊息中心這項功能。</span><span class="sxs-lookup"><span data-stu-id="292a2-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="292a2-110">您應該會開啟在您的租用戶中短時間內的功能。</span><span class="sxs-lookup"><span data-stu-id="292a2-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="292a2-111">交換網站的已知的問題</span><span class="sxs-lookup"><span data-stu-id="292a2-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="292a2-112">目標網站可能會傳回 「 找不到 」 (HTTP 404) 錯誤的短時間內。</span><span class="sxs-lookup"><span data-stu-id="292a2-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="292a2-113">內容必須重新編目要更新的搜尋索引。</span><span class="sxs-lookup"><span data-stu-id="292a2-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="292a2-114">並沒有手動步驟是這裡所需，這將會自動完成。</span><span class="sxs-lookup"><span data-stu-id="292a2-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="292a2-115">取決於 「 靜態 」 連結 （例如檔案同步處理和 OneNote 檔案） 的任何項目將會需要手動修正。</span><span class="sxs-lookup"><span data-stu-id="292a2-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="292a2-116">Project Server 網站可能需要驗證，以確保其仍然關聯正確。</span><span class="sxs-lookup"><span data-stu-id="292a2-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
