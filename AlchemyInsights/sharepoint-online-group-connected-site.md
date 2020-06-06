---
title: 將群組新增至 SharePoint 網站
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582802"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="fb311-102">在 SharePoint 中建立群組連線的網站時發生問題</span><span class="sxs-lookup"><span data-stu-id="fb311-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="fb311-103">建立或重新建立群組連線的網站時，遇到的一些常見問題。</span><span class="sxs-lookup"><span data-stu-id="fb311-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="fb311-104">如果您已刪除群組及其連線的網站，且想要使用相同的 URL 建立另一個網站，則必須永久移除之前的網站。</span><span class="sxs-lookup"><span data-stu-id="fb311-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="fb311-105">下載[SPO 管理命令](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)介面</span><span class="sxs-lookup"><span data-stu-id="fb311-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="fb311-106">如需有關如何開始使用 Powershell 的詳細資訊，請參閱[SharePoint Online 管理命令介面快速](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)入門。</span><span class="sxs-lookup"><span data-stu-id="fb311-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="fb311-107">使用[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell Cmdlet，從刪除的網站中移除網站。</span><span class="sxs-lookup"><span data-stu-id="fb311-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="fb311-108">需要有 Powershell 才能永久刪除群組網站。</span><span class="sxs-lookup"><span data-stu-id="fb311-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="fb311-109">如果您正在建立群組連線的網站，並收到警告：**另一個具有相同別名的群組已存在**，請從[Microsoft 365 系統管理中心](https://admin.microsoft.com/AdminPortal/Home#/groups)檢查現有的群組。</span><span class="sxs-lookup"><span data-stu-id="fb311-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="fb311-110">若要解決此問題，請刪除現有的群組（如果不再需要的話），或建立網站並指派不同的別名。</span><span class="sxs-lookup"><span data-stu-id="fb311-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="fb311-111">有不同的方式可用來建立及使用 SharePoint 的現代群組。</span><span class="sxs-lookup"><span data-stu-id="fb311-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="fb311-112">您可以將現有的網站連接至 Microsoft 365 群組。</span><span class="sxs-lookup"><span data-stu-id="fb311-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="fb311-113">如需詳細資訊，請參閱[使用 SharePoint 使用者介面連接 Microsoft 365 群組](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)。</span><span class="sxs-lookup"><span data-stu-id="fb311-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="fb311-114">若要建立 Microsoft 365 群組連線的網站，您需要建立[小組網站](https://admin.microsoft.com/sharepoint)。</span><span class="sxs-lookup"><span data-stu-id="fb311-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
