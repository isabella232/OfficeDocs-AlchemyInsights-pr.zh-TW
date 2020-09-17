---
title: 在共用連結上封鎖下載
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 5837013a71648d5d53cd215c3e3489f3de5528d5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685733"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="18cc9-102">在共用連結上封鎖下載</span><span class="sxs-lookup"><span data-stu-id="18cc9-102">Block download on sharing links</span></span>

<span data-ttu-id="18cc9-103">**[封鎖下載]** 可用於 Office 文件的**僅供檢視連結**。</span><span class="sxs-lookup"><span data-stu-id="18cc9-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="18cc9-104">當您選取此選項時，透過您建立的連結存取檔案的人員，將不會看到下載、列印或複製檔案的選項。</span><span class="sxs-lookup"><span data-stu-id="18cc9-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="18cc9-105">系統管理員可以透過更改 [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) 或 [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets 中的 `BlockDownloadLinksFileType` 設定，來控制是否僅針對 Office 檔案顯示「封鎖下載」設定。</span><span class="sxs-lookup"><span data-stu-id="18cc9-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
