---
title: 在 SharePoint 或 OneDrive 中限制存取
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223703"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="eebef-102">在 SharePoint 或 OneDrive 中限制存取</span><span class="sxs-lookup"><span data-stu-id="eebef-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="eebef-103">有許多方法可以限制對 SharePoint Online/OneDrive 服務的存取。</span><span class="sxs-lookup"><span data-stu-id="eebef-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="eebef-104">下列各種訪問限制方法如下所示。</span><span class="sxs-lookup"><span data-stu-id="eebef-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="eebef-105">**許可權限制**</span><span class="sxs-lookup"><span data-stu-id="eebef-105">**Permission Restriction**</span></span>

<span data-ttu-id="eebef-106">在 SharePoint Online 和商務用 OneDrive 中, 我們只會授與應該具有存取權的群組/個人存取權, 以限制網站、檔案和資料夾等專案的存取權。</span><span class="sxs-lookup"><span data-stu-id="eebef-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="eebef-107">自訂 SharePoint 清單或文件庫的許可權</span><span class="sxs-lookup"><span data-stu-id="eebef-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- <span data-ttu-id="eebef-108">[自訂 SharePoint 網站的權限](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions) (機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="eebef-108">[Customize SharePoint site permissions](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)</span></span>

- [<span data-ttu-id="eebef-109">變更子資料夾的權限</span><span class="sxs-lookup"><span data-stu-id="eebef-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="eebef-110">從未受控裝置中控制存取權</span><span class="sxs-lookup"><span data-stu-id="eebef-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="eebef-111">在 Office 365 中為 SharePoint 或全域系統管理員, 您可以封鎖或限制存取未受管理裝置 (不是在 Intune 中加入或相容的使用者) 的 SharePoint 和 OneDrive 內容。</span><span class="sxs-lookup"><span data-stu-id="eebef-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="eebef-112">**網路位置限制**</span><span class="sxs-lookup"><span data-stu-id="eebef-112">**Network Location Restriction**</span></span>

<span data-ttu-id="eebef-113">作為 IT 系統管理員, 您可以根據您信任的定義網路位置, 來控制 SharePoint 和 OneDrive 資源的存取權。</span><span class="sxs-lookup"><span data-stu-id="eebef-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="eebef-114">這也稱為位置型原則。</span><span class="sxs-lookup"><span data-stu-id="eebef-114">This is also known as location-based policy.</span></span> <span data-ttu-id="eebef-115">如需詳細資訊, 請參閱[根據網路位置控制對 SharePoint Online 和 OneDrive 資料的存取](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="eebef-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="eebef-116">**網站鎖定限制**</span><span class="sxs-lookup"><span data-stu-id="eebef-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="eebef-117">在 SharePoint Online 中, 您可以鎖定網站集合, 讓任何人都無法存取。</span><span class="sxs-lookup"><span data-stu-id="eebef-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="eebef-118">這是透過 PowerShell 和使用[get-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState 屬性的[SharePoint Online 管理命令](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)介面進行設定。</span><span class="sxs-lookup"><span data-stu-id="eebef-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="eebef-119">**限制使用者建立網站或子網站**</span><span class="sxs-lookup"><span data-stu-id="eebef-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="eebef-120">作為 SharePoint 系統管理員或 Office 365 全域管理員, 您可以讓您的使用者建立及管理自己的 SharePoint 網站、決定他們可以建立的網站類型, 以及指定網站的位置。</span><span class="sxs-lookup"><span data-stu-id="eebef-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="eebef-121">如需詳細資訊, 請參閱[在 SharePoint Online 中管理網站建立](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="eebef-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

