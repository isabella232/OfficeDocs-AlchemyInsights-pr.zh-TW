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
ms.openlocfilehash: edf851da951e163f30660d524049abe0798a8314
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048787"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="21d04-102">還原刪除的網站</span><span class="sxs-lookup"><span data-stu-id="21d04-102">Restore a deleted site</span></span>

<span data-ttu-id="21d04-103">當系統管理員會刪除 SharePoint 網站時，就會處於網站集合資源回收筒，它會保留 93 天前就會永久刪除。</span><span class="sxs-lookup"><span data-stu-id="21d04-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="21d04-104">若要還原的網站：</span><span class="sxs-lookup"><span data-stu-id="21d04-104">To restore the site:</span></span>
  
1. <span data-ttu-id="21d04-105">在新的 SharePoint 系統管理中心，按一下功能區上的 [**資源回收筒**]。</span><span class="sxs-lookup"><span data-stu-id="21d04-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="21d04-106">選取您想要還原的網站集合旁的核取方塊。</span><span class="sxs-lookup"><span data-stu-id="21d04-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="21d04-107">按一下 [**還原已刪除的項目**。</span><span class="sxs-lookup"><span data-stu-id="21d04-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="21d04-108">若要還原已刪除的通訊網站，您可以使用新的 SharePoint 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="21d04-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="21d04-109">否則，您需要使用 Microsoft PowerShell。</span><span class="sxs-lookup"><span data-stu-id="21d04-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="21d04-110">若要還原至 Office 365 群組網站，您需要還原 Exchange 系統管理中心中的群組。</span><span class="sxs-lookup"><span data-stu-id="21d04-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="21d04-111">群組可以還原 30 天後在被刪除。</span><span class="sxs-lookup"><span data-stu-id="21d04-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

