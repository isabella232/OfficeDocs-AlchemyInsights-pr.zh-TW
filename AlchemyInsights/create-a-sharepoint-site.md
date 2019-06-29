---
title: 建立 SharePoint 網站
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: cc0218dd34844cc1fdeb55a6f84975311826c372
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364544"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="b4162-102">建立 SharePoint 網站</span><span class="sxs-lookup"><span data-stu-id="b4162-102">Create a SharePoint site</span></span>

<span data-ttu-id="b4162-103">請參閱在[新的 SharePoint 系統管理中心管理](https://docs.microsoft.com/sharepoint/manage-site-creation )網站建立選項。</span><span class="sxs-lookup"><span data-stu-id="b4162-103">See [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation ) for site creation options.</span></span> <span data-ttu-id="b4162-104">選取以建立[小組網站](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US)(這會建立 Office 365 群組) 或[通訊網站](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)。</span><span class="sxs-lookup"><span data-stu-id="b4162-104">Select to create a [team site](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US) (which will create an Office 365 group) or a [communication site](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb).</span></span> <span data-ttu-id="b4162-105">若要建立[傳統網站](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site), 或是不包含 Office 365 群組的新小組網站, 請按一下 [**其他選項**]。</span><span class="sxs-lookup"><span data-stu-id="b4162-105">To create a [classic site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site), or a new team site that doesn't include an Office 365 group, click **Other options**.</span></span>
  
<span data-ttu-id="b4162-106">筆尖</span><span class="sxs-lookup"><span data-stu-id="b4162-106">Tips:</span></span>
- <span data-ttu-id="b4162-107">*您無法使用現有網站的相同 URL 來建立網站。如果您刪除網站, 而且想要重新使用此 URL, 則可能是已刪除的網站仍然存在於 [**已刪除的網站**] 底下。若要管理刪除的網站, 請參閱,[刪除網站](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)。若要完全移除具有 Powershell 的網站, 請參閱[remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) Cmdlet 範例。*</span><span class="sxs-lookup"><span data-stu-id="b4162-107">*You cannot create a site with the same URL of an existing site. If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**. To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site). To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.*</span></span>
- <span data-ttu-id="b4162-108">*某些使用者可能無法建立網站。請參閱[管理 SharePoint Online 中的網站](https://docs.microsoft.com/sharepoint/manage-site-creation)架設。*</span><span class="sxs-lookup"><span data-stu-id="b4162-108">*Some users may not be able to create a site. See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).*</span></span>
- <span data-ttu-id="b4162-109">*網站可能會在**建立**比預期更長的時間停滯。如果在您第一次看到此問題後超過24小時, 請記錄支援票證。在許多情況下, 我們已經在處理解決方案。請至少為我們提供24小時的時間, 才可完成解決方案。*</span><span class="sxs-lookup"><span data-stu-id="b4162-109">*It's possible the site appears stuck at **Creating** longer than expected. If more than 24 hours have passed since you first saw this issue, please log a support ticket. In many cases, we're already working on a solution. Please give us at least 24 hours to complete a solution.*</span></span>
