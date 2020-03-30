---
title: 在 SharePoint 中永久刪除網站
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955107"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="ce0b0-102">在 SharePoint 中永久刪除網站</span><span class="sxs-lookup"><span data-stu-id="ce0b0-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="ce0b0-103">若要重複使用已刪除網站中的 URL (以重建網站)，或因為網站已不再使用而永久刪除網站，您可從新版 SharePoint 系統管理中心使用 [永久刪除]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="ce0b0-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="ce0b0-104">移至[新版 SharePoint 系統管理中心的 [已刪除網站]](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) 頁面，並使用具有組織系統管理員權限的帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="ce0b0-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="ce0b0-105">在左側資料行中，選取網站。</span><span class="sxs-lookup"><span data-stu-id="ce0b0-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="ce0b0-106">按一下 [永久刪除]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="ce0b0-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="ce0b0-107">**附註**：無法從新版 SharePoint 系統管理中心永久刪除群組連線的網站。</span><span class="sxs-lookup"><span data-stu-id="ce0b0-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="ce0b0-108">必須改用 [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite)。</span><span class="sxs-lookup"><span data-stu-id="ce0b0-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="ce0b0-109">如需詳細資訊，請參閱[永久刪除網站](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site)。</span><span class="sxs-lookup"><span data-stu-id="ce0b0-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
