---
title: 還原刪除的網站
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 7c2ae754c86a3502092b622c55d18f3f4006bf8b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582226"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="c80db-102">還原刪除的網站</span><span class="sxs-lookup"><span data-stu-id="c80db-102">Restore a deleted site</span></span>

<span data-ttu-id="c80db-103">當系統管理員刪除 SharePoint 網站時，它會放在網站集合的回收站中，該回收站會在永久刪除之前于93天內保留。</span><span class="sxs-lookup"><span data-stu-id="c80db-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="c80db-104">若要還原網站：</span><span class="sxs-lookup"><span data-stu-id="c80db-104">To restore the site:</span></span>
  
1. <span data-ttu-id="c80db-105">在 [新增 SharePoint 系統管理中心] 中，按一下功能區上的 [**回收站**]。</span><span class="sxs-lookup"><span data-stu-id="c80db-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="c80db-106">選取您要還原之網站集合旁邊的核取方塊。</span><span class="sxs-lookup"><span data-stu-id="c80db-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="c80db-107">按一下 [**還原已刪除的郵件**]。</span><span class="sxs-lookup"><span data-stu-id="c80db-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="c80db-108">若要還原已刪除的通訊網站，您可以使用新的 SharePoint 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="c80db-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="c80db-109">否則，您必須使用 Microsoft PowerShell。</span><span class="sxs-lookup"><span data-stu-id="c80db-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="c80db-110">若要還原屬於 Microsoft 365 群組的網站，您必須在 Exchange 系統管理中心中還原群組。</span><span class="sxs-lookup"><span data-stu-id="c80db-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="c80db-111">群組可在刪除之後30天內還原。</span><span class="sxs-lookup"><span data-stu-id="c80db-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

