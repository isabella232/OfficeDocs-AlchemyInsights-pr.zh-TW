---
title: SharePoint Online 的權限等級
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760684"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="7e530-102">SharePoint Designer 連線問題</span><span class="sxs-lookup"><span data-stu-id="7e530-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="7e530-103">如果 SharePoint Designer 遇到至 SharePoint 網站的連線問題，請嘗試下列常見的解決方案。</span><span class="sxs-lookup"><span data-stu-id="7e530-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="7e530-104">步驟 1： 驗證已更新 SharePoint Designer。</span><span class="sxs-lookup"><span data-stu-id="7e530-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="7e530-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="7e530-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="7e530-106">SharePoint Designer Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="7e530-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="7e530-107">SharePoint Designer 2013 (KB3114721) 更新</span><span class="sxs-lookup"><span data-stu-id="7e530-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="7e530-108">步驟 2： 清除本機快取檔案</span><span class="sxs-lookup"><span data-stu-id="7e530-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="7e530-109">關閉 SharePoint Designer 2013。</span><span class="sxs-lookup"><span data-stu-id="7e530-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="7e530-110">本機電腦上，瀏覽至下列資料夾移除快取的檔案。</span><span class="sxs-lookup"><span data-stu-id="7e530-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="7e530-111">按一下 [開始]、 [執行] 和 [刪除所有檔案都位於 [每個位置下方。</span><span class="sxs-lookup"><span data-stu-id="7e530-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="7e530-112">%APPDATA%\Microsoft\Web 伺服器 Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="7e530-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="7e530-113">開啟 SharePoint Designer 2013，並輸入一次若要查看是否它的運作方式的帳戶。</span><span class="sxs-lookup"><span data-stu-id="7e530-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="7e530-114">步驟 3：[的 Windows 裝置上的 Office 2013 啟用新式驗證](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="7e530-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="7e530-115">步驟 4： 系統管理員必須允許自訂指令碼以允許 SharePoint Designer 連線。</span><span class="sxs-lookup"><span data-stu-id="7e530-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="7e530-116">如需詳細的步驟、 範例及考量請參閱[允許或防止自訂指令碼](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)。</span><span class="sxs-lookup"><span data-stu-id="7e530-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


