---
title: 還原刪除的網站集合
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 1f9a66daf7bee43291b785b6260aec8725ee782f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753777"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="d50d2-102">還原刪除的網站集合</span><span class="sxs-lookup"><span data-stu-id="d50d2-102">Restore a deleted site collection</span></span>

<span data-ttu-id="d50d2-103">當系統管理員會刪除傳統網站集合時，它會處於網站集合資源回收筒，它會保留 93 天前就會永久刪除。</span><span class="sxs-lookup"><span data-stu-id="d50d2-103">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="d50d2-104">若要還原之網站集合：</span><span class="sxs-lookup"><span data-stu-id="d50d2-104">To restore the site collection:</span></span>
  
1. <span data-ttu-id="d50d2-105">在傳統的 SharePoint 系統管理中心，按一下功能區上的 [**資源回收筒**]。</span><span class="sxs-lookup"><span data-stu-id="d50d2-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="d50d2-106">選取您想要還原的網站集合旁的核取方塊。</span><span class="sxs-lookup"><span data-stu-id="d50d2-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="d50d2-107">按一下 [**還原已刪除的項目**。</span><span class="sxs-lookup"><span data-stu-id="d50d2-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="d50d2-108">若要還原已刪除的通訊網站，您可以使用新的 SharePoint 系統管理中心預覽。</span><span class="sxs-lookup"><span data-stu-id="d50d2-108">To restore a deleted communication site, you can use the new SharePoint admin center preview.</span></span> <span data-ttu-id="d50d2-109">否則，您必須使用 PowerShell。</span><span class="sxs-lookup"><span data-stu-id="d50d2-109">Otherwise, you need to use PowerShell.</span></span> <span data-ttu-id="d50d2-110">若要還原至 Office 365 群組網站，您需要還原 Exchange 系統管理中心中的群組。</span><span class="sxs-lookup"><span data-stu-id="d50d2-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="d50d2-111">群組可以還原 30 天後在被刪除。</span><span class="sxs-lookup"><span data-stu-id="d50d2-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

