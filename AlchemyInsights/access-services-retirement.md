---
title: Access services 淘汰網站
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973902"
---
# <a name="access-services-retirement"></a><span data-ttu-id="a51e2-102">Access services 淘汰網站</span><span class="sxs-lookup"><span data-stu-id="a51e2-102">Access services retirement</span></span>

<span data-ttu-id="a51e2-103">我們原本 March 2017 月所宣布 MC97576，並繼續透過過去一年通訊 Access Services 會被淘汰從 Office 365。</span><span class="sxs-lookup"><span data-stu-id="a51e2-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="a51e2-104">此程序的下一個階段將會使用 SharePoint 清單作為其基礎資料儲存區的 Access Web 資料庫移除。</span><span class="sxs-lookup"><span data-stu-id="a51e2-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="a51e2-105">這有什麼影響我？</span><span class="sxs-lookup"><span data-stu-id="a51e2-105">How does this affect me?</span></span>

<span data-ttu-id="a51e2-106">啟動年 6 月 2019年，我們將停止 SharePoint Online 中的新 Access 資料庫的建立，並由 2020 年 4 月關閉服務] 和 [任何其餘的應用程式。</span><span class="sxs-lookup"><span data-stu-id="a51e2-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="a51e2-107">是否需要什麼準備，這項變更？</span><span class="sxs-lookup"><span data-stu-id="a51e2-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="a51e2-108">我們鼓勵您建立轉換計劃為貴組織的 Access web 資料庫。</span><span class="sxs-lookup"><span data-stu-id="a51e2-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="a51e2-109">系統管理員可以使用[SharePoint 的 Access 應用程式掃描程式](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0)來取得站台均使用 Access 應用程式的詳細目錄。</span><span class="sxs-lookup"><span data-stu-id="a51e2-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="a51e2-110">有幾種方式可以將 Access web 資料庫資料移轉：</span><span class="sxs-lookup"><span data-stu-id="a51e2-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="a51e2-111">匯入至本機的 Access 資料庫 (。ACCDB) 或至 Excel 檔案。</span><span class="sxs-lookup"><span data-stu-id="a51e2-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="a51e2-112">我們也建議探索 Microsoft PowerApps 做為建立 web 和行動裝置的無程式碼商務解決方案替代平台。</span><span class="sxs-lookup"><span data-stu-id="a51e2-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>