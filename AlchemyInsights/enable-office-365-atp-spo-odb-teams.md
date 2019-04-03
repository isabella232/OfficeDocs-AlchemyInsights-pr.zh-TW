---
title: 啟用 Office 365 ATP SharePoint、 OneDrive 及 Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030902"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="b60e5-102">啟用 SharePoint Online、 OneDrive 及 Microsoft Teams 的 Office 365 進階的威脅防護</span><span class="sxs-lookup"><span data-stu-id="b60e5-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="b60e5-103">移至 [https://protection.office.com並登入。</span><span class="sxs-lookup"><span data-stu-id="b60e5-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="b60e5-104">選擇 [**威脅管理** > **原則** > **安全附件**。</span><span class="sxs-lookup"><span data-stu-id="b60e5-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="b60e5-105">選取 [**開啟 ATP SharePoint、 OneDrive 及 Microsoft Teams**，，然後按一下 [**儲存**。</span><span class="sxs-lookup"><span data-stu-id="b60e5-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="b60e5-106">（建議使用）以全域管理員或 SharePoint Online 系統管理員，執行[Set-spotenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps)指令程式搭配**DisallowInfectedFileDownload**參數設為*true*。</span><span class="sxs-lookup"><span data-stu-id="b60e5-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="b60e5-107">（建議使用）[設定提醒](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)偵測到的檔案。</span><span class="sxs-lookup"><span data-stu-id="b60e5-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="b60e5-108">ATP 會 nto 掃描 SharePoint Online、 OneDrive 或 Microsoft Teams 中每一個檔案。</span><span class="sxs-lookup"><span data-stu-id="b60e5-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="b60e5-109">掃描檔案有以非同步方式，透過使用共用和來賓活動事件，以及智慧啟發和威脅訊號，以識別惡意檔案的程序。</span><span class="sxs-lookup"><span data-stu-id="b60e5-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="b60e5-110">請參閱[https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)。</span><span class="sxs-lookup"><span data-stu-id="b60e5-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>