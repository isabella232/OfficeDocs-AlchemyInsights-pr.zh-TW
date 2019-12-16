---
title: 交換傳統根網站與新式網站
ms.author: pebaum
author: pebaum
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: fe1f0f662c49de2bd0b5b997697c98309cb7983f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042918"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="41e36-102">交換傳統根網站與新式網站</span><span class="sxs-lookup"><span data-stu-id="41e36-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="41e36-103">如果您的環境設定成 [年 4 月 2019年之前，您可以變更至新式網站的根網站使用 Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="41e36-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="41e36-104">如果您有不同的網站，您想要作為根網站時，您可以將[（分頁） 的根網站](https://docs.microsoft.com/sharepoint/modern-root-site)取代它。</span><span class="sxs-lookup"><span data-stu-id="41e36-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="41e36-105">使用[Invoke SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)封存原始網站時切換網站與其他網站的位置。</span><span class="sxs-lookup"><span data-stu-id="41e36-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="41e36-106">適用於小組網站 （未連線至群組） 及通訊網站。</span><span class="sxs-lookup"><span data-stu-id="41e36-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="41e36-107">額外的功能將會引進推出，可讓您保留網站上，使用內容，但是在通訊網站轉換現有的網站。</span><span class="sxs-lookup"><span data-stu-id="41e36-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="41e36-108">這些功能會逐步導入。</span><span class="sxs-lookup"><span data-stu-id="41e36-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="41e36-109">繼續進行若要檢查 Office 365 訊息中心的更新。</span><span class="sxs-lookup"><span data-stu-id="41e36-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="41e36-110">交換網站的已知的問題</span><span class="sxs-lookup"><span data-stu-id="41e36-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="41e36-111">目標網站可能會傳回 「 找不到 」 (HTTP 404) 錯誤的短時間內。</span><span class="sxs-lookup"><span data-stu-id="41e36-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="41e36-112">內容必須重新編目要更新的搜尋索引。</span><span class="sxs-lookup"><span data-stu-id="41e36-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="41e36-113">沒有任何所需的手動步驟-這會自動完成。</span><span class="sxs-lookup"><span data-stu-id="41e36-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="41e36-114">取決於 「 靜態 」 連結 （例如檔案同步處理和 OneNote 檔案） 的任何項目將會需要手動修正。</span><span class="sxs-lookup"><span data-stu-id="41e36-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="41e36-115">如果來源網站組織新聞網站，更新 URL。</span><span class="sxs-lookup"><span data-stu-id="41e36-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="41e36-116">取得所有組織新聞網站的清單。</span><span class="sxs-lookup"><span data-stu-id="41e36-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="41e36-117">Project Server 網站可能需要驗證，以確保其仍然關聯正確。</span><span class="sxs-lookup"><span data-stu-id="41e36-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





