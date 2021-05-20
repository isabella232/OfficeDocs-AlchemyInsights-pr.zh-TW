---
title: 啟用 SharePoint、OneDrive 和 Microsoft Teams 的 Office 365 ATP
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543919"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="18a96-102">針對 SharePoint 線上、OneDrive 和 Microsoft Teams 啟用 Microsoft Defender Office 365</span><span class="sxs-lookup"><span data-stu-id="18a96-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="18a96-103">移至 https://protection.office.com 並登入。</span><span class="sxs-lookup"><span data-stu-id="18a96-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="18a96-104">選擇 [**威脅管理**  >  **原則**  >  **安全附件**]。</span><span class="sxs-lookup"><span data-stu-id="18a96-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="18a96-105">**針對 SharePoint、OneDrive 及 Microsoft Teams，選取 [為 Office 365 開啟 Defender**]，然後按一下 [**儲存**]。</span><span class="sxs-lookup"><span data-stu-id="18a96-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="18a96-106"> (建議) 成為全域系統管理員或 SharePoint Online 管理員，請執行 [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) Cmdlet，並將 **DisallowInfectedFileDownload** 參數設定為 *true*。</span><span class="sxs-lookup"><span data-stu-id="18a96-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="18a96-107"> (建議的) 設定偵測到的檔案 [警示](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) 。</span><span class="sxs-lookup"><span data-stu-id="18a96-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="18a96-108">Microsoft Defender for Office 365 不會掃描 SharePoint Online、OneDrive 或 Microsoft Teams 中的每一個檔案。</span><span class="sxs-lookup"><span data-stu-id="18a96-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="18a96-109">檔案會透過使用共用和來賓活動事件的處理常式進行非同步掃描，並使用智慧試探法和威脅信號來識別惡意檔。</span><span class="sxs-lookup"><span data-stu-id="18a96-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="18a96-110">請參閱適用[于 SharePoint、OneDrive 和 Microsoft Teams 的 Microsoft Defender Office 365](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)。</span><span class="sxs-lookup"><span data-stu-id="18a96-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>