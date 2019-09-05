---
title: 限制存取 SharePoint 或 OneDrive 中
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750655"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="fdd36-102">限制存取 SharePoint 或 OneDrive 中</span><span class="sxs-lookup"><span data-stu-id="fdd36-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="fdd36-103">有許多方式可以限制存取 SharePoint Online/OneDrive 服務。</span><span class="sxs-lookup"><span data-stu-id="fdd36-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="fdd36-104">這些不同的存取限制方法概述如下。</span><span class="sxs-lookup"><span data-stu-id="fdd36-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="fdd36-105">**權限限制**</span><span class="sxs-lookup"><span data-stu-id="fdd36-105">**Permission Restriction**</span></span>

<span data-ttu-id="fdd36-106">在 SharePoint Online 和商務用 OneDrive，我們要限制存取網站、 檔案及資料夾等項目只授與存取這些群組/個人應該具有存取權。</span><span class="sxs-lookup"><span data-stu-id="fdd36-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="fdd36-107">自訂 SharePoint 清單或文件庫的權限</span><span class="sxs-lookup"><span data-stu-id="fdd36-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- <span data-ttu-id="fdd36-108">[自訂 SharePoint 網站的權限](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions) (機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="fdd36-108">[Customize SharePoint site permissions](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)</span></span>

- [<span data-ttu-id="fdd36-109">變更子資料夾的權限</span><span class="sxs-lookup"><span data-stu-id="fdd36-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="fdd36-110">從未受控裝置中控制存取權</span><span class="sxs-lookup"><span data-stu-id="fdd36-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="fdd36-111">為 SharePoint 或 Office 365 全域系統管理員，您可以封鎖或限制存取 SharePoint 和 OneDrive 內容來自未受管理的裝置 (這些混合式 AD 加入或相容 Intune 中)。</span><span class="sxs-lookup"><span data-stu-id="fdd36-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="fdd36-112">**網路位置限制**</span><span class="sxs-lookup"><span data-stu-id="fdd36-112">**Network Location Restriction**</span></span>

<span data-ttu-id="fdd36-113">身為 IT 系統管理員，您可以控制存取 SharePoint 和 OneDrive 的資源，根據您信任的已定義的網路位置。</span><span class="sxs-lookup"><span data-stu-id="fdd36-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="fdd36-114">這也稱為是位置為基礎的原則。</span><span class="sxs-lookup"><span data-stu-id="fdd36-114">This is also known as location-based policy.</span></span> <span data-ttu-id="fdd36-115">如需詳細資訊，請參閱[SharePoint Online 和 OneDrive 資料是根據網路位置控制存取](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="fdd36-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="fdd36-116">**網站鎖定限制**</span><span class="sxs-lookup"><span data-stu-id="fdd36-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="fdd36-117">在 SharePoint Online 中，您必須鎖定網站集合，因此沒有人有權存取的能力。</span><span class="sxs-lookup"><span data-stu-id="fdd36-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="fdd36-118">這是透過 PowerShell 和[SharePoint Online 管理命令介面](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)使用[Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState 屬性設定。</span><span class="sxs-lookup"><span data-stu-id="fdd36-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="fdd36-119">**限制使用者只能建立網站或子網站**</span><span class="sxs-lookup"><span data-stu-id="fdd36-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="fdd36-120">為 SharePoint 系統管理員或 Office 365 全域系統管理員，您可以讓您的使用者建立及管理自己的 SharePoint 網站，請決定何種網站他們可以建立，並指定網站的位置。</span><span class="sxs-lookup"><span data-stu-id="fdd36-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="fdd36-121">如需詳細資訊，請參閱[在 SharePoint Online 中的管理網站架設](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="fdd36-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

