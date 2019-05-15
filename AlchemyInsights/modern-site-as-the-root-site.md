---
title: 新式網站作為根網站
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057679"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="f0a49-102">新式網站作為根網站</span><span class="sxs-lookup"><span data-stu-id="f0a49-102">Modern site as root site</span></span>

<span data-ttu-id="f0a49-103">[目標版本](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide)客戶現在可以啟用新式通訊的網站經驗，其 SharePoint 租用戶的傳統的根網站。</span><span class="sxs-lookup"><span data-stu-id="f0a49-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="f0a49-104">藉由執行簡單的 PowerShell cmdlet，就可以啟動這項功能。</span><span class="sxs-lookup"><span data-stu-id="f0a49-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="f0a49-105">在 PowerShell 命令執行成功，根網站會有新的通訊網站首頁。</span><span class="sxs-lookup"><span data-stu-id="f0a49-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="f0a49-106">關於 PowerShell 指令程式和功能需求的詳細資料可[啟用 SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps)」 文件中。</span><span class="sxs-lookup"><span data-stu-id="f0a49-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="f0a49-107">我們將會逐漸循環時，關閉依預設，在早期 2019 年，已設定目標發行客戶，首度發行將提供使用全球年 6 月 2019年結束。</span><span class="sxs-lookup"><span data-stu-id="f0a49-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="f0a49-108">若要參照在[訊息中心](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)的其他新功能與現代化繼續執行。</span><span class="sxs-lookup"><span data-stu-id="f0a49-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="f0a49-109">**重要**： 請不要刪除傳統的根網站以建立新式通訊網站。</span><span class="sxs-lookup"><span data-stu-id="f0a49-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="f0a49-110">Microsoft 不支援此。</span><span class="sxs-lookup"><span data-stu-id="f0a49-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="f0a49-111">刪除根網站會使所有的 SharePoint 網站組織中所有使用者，無法存取直到您還原的網站，或在相同的 URL 建立新的網站。</span><span class="sxs-lookup"><span data-stu-id="f0a49-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 