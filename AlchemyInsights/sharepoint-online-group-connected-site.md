---
title: 新增群組至 SharePoint 網站
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758722"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a><span data-ttu-id="caacf-102">在 Sharepoint Online 中建立群組連結的網站</span><span class="sxs-lookup"><span data-stu-id="caacf-102">Create group connected site in SharePoint Online</span></span>

<span data-ttu-id="caacf-103">有幾個建立或重新建立一組連線網站時常見的問題。</span><span class="sxs-lookup"><span data-stu-id="caacf-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="caacf-104">如果您已刪除群組及其連結的網站，且想要使用的相同 URL 建立另一個網站，您必須永久移除舊版的網站。</span><span class="sxs-lookup"><span data-stu-id="caacf-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="caacf-105">下載[SPO 管理命令介面](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="caacf-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="caacf-106">如需開始使用 PowerShell 的詳細資訊，請參閱[開始使用 SharePoint Online 管理命令介面](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="caacf-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="caacf-107">使用[移除 SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell Cmdlet 移除已刪除的網站。</span><span class="sxs-lookup"><span data-stu-id="caacf-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="caacf-108">如果您正在建立群組連結的網站，卻收到具有相同別名的群組已存在的警告，請從[Office 365 的系統管理中心](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)查看現有的群組。</span><span class="sxs-lookup"><span data-stu-id="caacf-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="caacf-109">請刪除不再需要的現有群組或建立不同別名的網站來解決此問題。</span><span class="sxs-lookup"><span data-stu-id="caacf-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="caacf-110">建立及使用 SharePoint 的新式群組的方式有很多種。</span><span class="sxs-lookup"><span data-stu-id="caacf-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="caacf-111">您可以連線現有的網站至 Office 365 群組。</span><span class="sxs-lookup"><span data-stu-id="caacf-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="caacf-112">如需詳細資訊，請參閱[使用 SharePoint 使用者介面連線至 Office 365 群組](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)。</span><span class="sxs-lookup"><span data-stu-id="caacf-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="caacf-113">若要建立 Office 365 群組連結的網站，您必須建立小組網站。</span><span class="sxs-lookup"><span data-stu-id="caacf-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="caacf-114">如需詳細資訊，請參閱[在 SharePoint 中建立小組網站](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)。</span><span class="sxs-lookup"><span data-stu-id="caacf-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

