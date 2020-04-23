---
title: 將傳統的根網站與現代網站交換
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741535"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="262f5-102">將傳統的根網站與現代網站交換</span><span class="sxs-lookup"><span data-stu-id="262f5-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="262f5-103">如果您的環境是在2019年4月之前設定，您可以使用 Microsoft PowerShell: 將您的根網站變更為現代網站。</span><span class="sxs-lookup"><span data-stu-id="262f5-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="262f5-104">如果您有不同的網站，您想要用來作為根網站，您可以將[根網站取代（換用）](https://docs.microsoft.com/sharepoint/modern-root-site) 。</span><span class="sxs-lookup"><span data-stu-id="262f5-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="262f5-105">使用[SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)在封存原始網站時，將網站的位置交換為另一個網站。</span><span class="sxs-lookup"><span data-stu-id="262f5-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="262f5-106">可用於兩個小組網站（未連接至群組）和通訊網站。</span><span class="sxs-lookup"><span data-stu-id="262f5-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="262f5-107">將會很快引進其他功能，讓您繼續使用網站上的內容，但將現有網站轉換為通訊網站。</span><span class="sxs-lookup"><span data-stu-id="262f5-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="262f5-108">這些功能將會逐步向之外進行匯總。</span><span class="sxs-lookup"><span data-stu-id="262f5-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="262f5-109">繼續檢查訊息中心是否有更新。</span><span class="sxs-lookup"><span data-stu-id="262f5-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="262f5-110">交換網站的已知問題</span><span class="sxs-lookup"><span data-stu-id="262f5-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="262f5-111">目標網站可能會傳回一小段時間的「找不到」（HTTP 404）錯誤。</span><span class="sxs-lookup"><span data-stu-id="262f5-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="262f5-112">內容將需要重新編目更新搜尋索引。</span><span class="sxs-lookup"><span data-stu-id="262f5-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="262f5-113">不需要手動步驟，這將會自動完成。</span><span class="sxs-lookup"><span data-stu-id="262f5-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="262f5-114">任何依存于「靜態」連結的專案（例如，檔案同步處理及 OneNote 檔案）都必須手動修正。</span><span class="sxs-lookup"><span data-stu-id="262f5-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="262f5-115">如果來源網站為組織新聞網站，請更新 URL。</span><span class="sxs-lookup"><span data-stu-id="262f5-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="262f5-116">取得所有組織新聞網站的清單。</span><span class="sxs-lookup"><span data-stu-id="262f5-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="262f5-117">可能需要驗證 Project Server 網站，以確保它們仍然有正確相關聯。</span><span class="sxs-lookup"><span data-stu-id="262f5-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
