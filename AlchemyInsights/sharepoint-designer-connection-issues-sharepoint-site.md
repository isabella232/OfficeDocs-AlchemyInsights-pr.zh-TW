---
title: SharePoint Designer 連線問題
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
ms.openlocfilehash: 9730bd66afd494385db3de605f5fe68d0f274ed3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051704"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="7c106-102">SharePoint Designer 連線問題</span><span class="sxs-lookup"><span data-stu-id="7c106-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="7c106-103">如果 SharePoint Designer 遇到至 SharePoint 網站的連線問題，請嘗試下列常見的解決方案。</span><span class="sxs-lookup"><span data-stu-id="7c106-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="7c106-104">步驟 1： 確認 SharePoint Designer 2013 會更新為[SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)和[2016 年 8 月 2 日更新的 SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)。</span><span class="sxs-lookup"><span data-stu-id="7c106-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="7c106-105">步驟 2： 清除本機快取檔案：</span><span class="sxs-lookup"><span data-stu-id="7c106-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="7c106-106">關閉 SharePoint Designer 2013。</span><span class="sxs-lookup"><span data-stu-id="7c106-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="7c106-107">本機電腦上，移除在每個下列資料夾中找到的所有檔案。</span><span class="sxs-lookup"><span data-stu-id="7c106-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="7c106-108">%APPDATA%\Microsoft\Web 伺服器 Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="7c106-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="7c106-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="7c106-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="7c106-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="7c106-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="7c106-111">開啟 SharePoint Designer 2013，並輸入一次若要查看是否它的運作方式的帳戶。</span><span class="sxs-lookup"><span data-stu-id="7c106-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="7c106-112">步驟 3：[的 Windows 裝置上的 Office 2013 啟用新式驗證](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="7c106-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="7c106-113">步驟 4： 系統管理員必須**允許自訂指令碼**中的 SharePoint 系統管理中心設定以允許 SharePoint Designer 連線。</span><span class="sxs-lookup"><span data-stu-id="7c106-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="7c106-114">請參閱[允許或防止自訂指令碼](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)如需詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="7c106-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


