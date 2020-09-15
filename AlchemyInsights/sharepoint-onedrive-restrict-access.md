---
title: 在 SharePoint 或 OneDrive 中限制存取權
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700446"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="97911-102">在 SharePoint 或 OneDrive 中限制存取權</span><span class="sxs-lookup"><span data-stu-id="97911-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="97911-103">有許多方式可以限制存取 SharePoint 線上/OneDrive 服務。</span><span class="sxs-lookup"><span data-stu-id="97911-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="97911-104">下列列出各種訪問限制方法。</span><span class="sxs-lookup"><span data-stu-id="97911-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="97911-105">**許可權限制**</span><span class="sxs-lookup"><span data-stu-id="97911-105">**Permission Restriction**</span></span>

<span data-ttu-id="97911-106">在 SharePoint Online 和商務 OneDrive 中，我們只會將存取權授與網站、檔案和資料夾等專案的存取權授與應該具有存取權的那些群組/個人。</span><span class="sxs-lookup"><span data-stu-id="97911-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="97911-107">自訂 SharePoint 清單或文件庫的許可權</span><span class="sxs-lookup"><span data-stu-id="97911-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="97911-108">自訂 SharePoint 網站權限</span><span class="sxs-lookup"><span data-stu-id="97911-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="97911-109">變更子資料夾的權限</span><span class="sxs-lookup"><span data-stu-id="97911-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="97911-110">從未受控裝置中控制存取權</span><span class="sxs-lookup"><span data-stu-id="97911-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="97911-111">做為 SharePoint 或全域系統管理員，您可以封鎖或限制存取不受管理的裝置的 SharePoint 和 OneDrive 內容 (Intune) 中未結合的混合式廣告或相容性。</span><span class="sxs-lookup"><span data-stu-id="97911-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="97911-112">**網路位置限制**</span><span class="sxs-lookup"><span data-stu-id="97911-112">**Network Location Restriction**</span></span>

<span data-ttu-id="97911-113">做為 IT 管理員，您可以根據您信任的定義網路位置，控制對 SharePoint 和 OneDrive 資源的存取。</span><span class="sxs-lookup"><span data-stu-id="97911-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="97911-114">這也稱為位置型原則。</span><span class="sxs-lookup"><span data-stu-id="97911-114">This is also known as location-based policy.</span></span> <span data-ttu-id="97911-115">如需詳細資訊，請參閱 [以網路位置為基礎的 SharePoint 線上及 OneDrive 資料的控制存取權](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="97911-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="97911-116">**網站鎖定限制**</span><span class="sxs-lookup"><span data-stu-id="97911-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="97911-117">在 SharePoint Online 中，您可以鎖定網站集合，因此沒有人能夠存取。</span><span class="sxs-lookup"><span data-stu-id="97911-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="97911-118">這是透過 PowerShell 和使用[Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) LockState 屬性[SharePoint Online 管理命令](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)介面來設定。</span><span class="sxs-lookup"><span data-stu-id="97911-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="97911-119">**限制使用者建立網站或子網站**</span><span class="sxs-lookup"><span data-stu-id="97911-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="97911-120">做為 SharePoint 系統管理員或全域管理員，您可以讓您的使用者建立及管理自己的 SharePoint 網站、決定可以建立的網站類型，並指定網站的位置。</span><span class="sxs-lookup"><span data-stu-id="97911-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="97911-121">如需詳細資訊，請參閱 [在 SharePoint Online 中管理網站建立](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="97911-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

