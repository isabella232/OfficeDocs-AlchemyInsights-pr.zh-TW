---
title: SharePoint 設計工具連接問題
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511535"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="e7ce0-102">SharePoint 設計工具連接問題</span><span class="sxs-lookup"><span data-stu-id="e7ce0-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="e7ce0-103">如果 SharePoint 設計工具遇到 SharePoint 網站的連線問題，請嘗試下列一般解決方案。</span><span class="sxs-lookup"><span data-stu-id="e7ce0-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="e7ce0-104">步驟1：確認 SharePoint 設計工具2013已使用[SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)和[8 月2日的2016更新（SharePoint Designer 2013）](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)進行更新。</span><span class="sxs-lookup"><span data-stu-id="e7ce0-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="e7ce0-105">步驟2：清除本機快取檔：</span><span class="sxs-lookup"><span data-stu-id="e7ce0-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="e7ce0-106">關閉 SharePoint 設計工具2013。</span><span class="sxs-lookup"><span data-stu-id="e7ce0-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="e7ce0-107">在本機電腦上，移除每個下列資料夾中找到的所有檔案。</span><span class="sxs-lookup"><span data-stu-id="e7ce0-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="e7ce0-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="e7ce0-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="e7ce0-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="e7ce0-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="e7ce0-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="e7ce0-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="e7ce0-111">開啟 SharePoint 設計工具2013，然後再次輸入帳戶，查看是否運作正常。</span><span class="sxs-lookup"><span data-stu-id="e7ce0-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="e7ce0-112">步驟3：[在 Windows 裝置上啟用 Office 2013 的新式驗證](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)。</span><span class="sxs-lookup"><span data-stu-id="e7ce0-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="e7ce0-113">步驟4：系統管理員必須允許 SharePoint 系統管理中心設定中的**自訂腳本**，才能允許 SharePoint Designer 連線。</span><span class="sxs-lookup"><span data-stu-id="e7ce0-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="e7ce0-114">如需詳細資訊，請參閱[Allow 或預防自訂腳本](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)。</span><span class="sxs-lookup"><span data-stu-id="e7ce0-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


