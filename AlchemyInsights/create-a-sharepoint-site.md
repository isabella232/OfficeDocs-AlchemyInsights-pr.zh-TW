---
title: 建立 SharePoint 網站
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806930"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="b65d6-102">建立 SharePoint 網站</span><span class="sxs-lookup"><span data-stu-id="b65d6-102">Create a SharePoint site</span></span>

<span data-ttu-id="b65d6-103">從 SharePoint 系統管理中心的使用中 [網站](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) 建立或管理網站。</span><span class="sxs-lookup"><span data-stu-id="b65d6-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="b65d6-104">如需詳細資訊，請參閱 [Manage sites in new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation)。</span><span class="sxs-lookup"><span data-stu-id="b65d6-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="b65d6-105">技巧：</span><span class="sxs-lookup"><span data-stu-id="b65d6-105">Tips:</span></span>

- <span data-ttu-id="b65d6-106">您 **無法** 使用現有網站的相同 URL 來建立網站。</span><span class="sxs-lookup"><span data-stu-id="b65d6-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="b65d6-107">如果您已刪除網站，且想要重新使用 URL，則已刪除的網站可能仍然存在於 [ [已刪除的網站](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)] 底下。</span><span class="sxs-lookup"><span data-stu-id="b65d6-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="b65d6-108">網站必須永久刪除，才能重複使用 URL。</span><span class="sxs-lookup"><span data-stu-id="b65d6-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="b65d6-109">若要使用 Powershell 完全移除網站，請參閱 [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) Cmdlet 範例。</span><span class="sxs-lookup"><span data-stu-id="b65d6-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="b65d6-110">有些使用者可能無法建立網站。</span><span class="sxs-lookup"><span data-stu-id="b65d6-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="b65d6-111">[請參閱管理 SharePoint Online 中的網站建立](https://docs.microsoft.com/sharepoint/manage-site-creation)。</span><span class="sxs-lookup"><span data-stu-id="b65d6-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="b65d6-112">網站可能會在 **建立** 比預期更長的時間停滯。</span><span class="sxs-lookup"><span data-stu-id="b65d6-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="b65d6-113">如果從您第一次看到此問題起已經過去超過24小時，請記錄支援票證。</span><span class="sxs-lookup"><span data-stu-id="b65d6-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="b65d6-114">多數情況下，我們已經著手研究解決方案。</span><span class="sxs-lookup"><span data-stu-id="b65d6-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b65d6-115">請至少為我們提供24小時的時間來完成解決方案。</span><span class="sxs-lookup"><span data-stu-id="b65d6-115">Please give us at least 24 hours to complete a solution.</span></span>
