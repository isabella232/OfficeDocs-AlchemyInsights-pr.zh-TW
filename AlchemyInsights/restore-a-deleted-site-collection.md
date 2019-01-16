---
title: 還原刪除的網站集合
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: b3c72033dfcc093dd0c2837d2866c6a78d64449c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28278739"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="684c1-102">還原刪除的網站集合</span><span class="sxs-lookup"><span data-stu-id="684c1-102">Restore a deleted site collection</span></span>

<span data-ttu-id="684c1-p101">當系統管理員會刪除傳統的網站集合時，它會處於網站集合資源回收筒，它保留 93 天永久刪除之前。若要還原之網站集合：</span><span class="sxs-lookup"><span data-stu-id="684c1-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="684c1-105">在傳統 SharePoint 系統管理中心中，按一下 [功能區上的**資源回收筒**。</span><span class="sxs-lookup"><span data-stu-id="684c1-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="684c1-106">選取您想要還原之網站集合] 旁的核取方塊。</span><span class="sxs-lookup"><span data-stu-id="684c1-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="684c1-107">按一下 [**還原已刪除的項目**。</span><span class="sxs-lookup"><span data-stu-id="684c1-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="684c1-p102">若要還原已刪除的通訊的網站，您可以使用新的 SharePoint admin center 預覽。否則，您需要使用 PowerShell。若要還原到 Office 365 群組所屬的網站，您需要還原 Exchange 系統管理中心中的群組。群組可以還原他們正在刪除後的 30 天。</span><span class="sxs-lookup"><span data-stu-id="684c1-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  

