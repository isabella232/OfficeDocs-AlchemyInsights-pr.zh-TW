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
ms.openlocfilehash: d37fd903c91c8cd6ac6137e815cb253f7edb4494
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912666"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="069e0-102">還原刪除的網站</span><span class="sxs-lookup"><span data-stu-id="069e0-102">Restore a deleted site</span></span>

<span data-ttu-id="069e0-103">當系統管理員刪除 SharePoint 網站時，它會放在網站集合的回收站中，該回收站會在永久刪除之前于93天內保留。</span><span class="sxs-lookup"><span data-stu-id="069e0-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="069e0-104">若要還原網站：</span><span class="sxs-lookup"><span data-stu-id="069e0-104">To restore the site:</span></span>
  
1. <span data-ttu-id="069e0-105">在 [新增 SharePoint 系統管理中心] 中，按一下功能區上的 [**回收站**]。</span><span class="sxs-lookup"><span data-stu-id="069e0-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="069e0-106">選取您要還原之網站集合旁邊的核取方塊。</span><span class="sxs-lookup"><span data-stu-id="069e0-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="069e0-107">按一下 [**還原已刪除的郵件**]。</span><span class="sxs-lookup"><span data-stu-id="069e0-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="069e0-108">若要還原已刪除的通訊網站，您可以使用新的 SharePoint 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="069e0-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="069e0-109">否則，您必須使用 Microsoft PowerShell。</span><span class="sxs-lookup"><span data-stu-id="069e0-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="069e0-110">若要還原屬於 Microsoft 365 群組的網站，您必須在 Exchange 系統管理中心中還原該群組。</span><span class="sxs-lookup"><span data-stu-id="069e0-110">To restore a site that belongs to an Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="069e0-111">群組可在刪除之後30天內還原。</span><span class="sxs-lookup"><span data-stu-id="069e0-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

