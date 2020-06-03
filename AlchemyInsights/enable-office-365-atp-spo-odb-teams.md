---
title: 為 SharePoint、OneDrive 和 Microsoft 團隊啟用 Office 365 ATP
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506909"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="5f1f9-102">針對 SharePoint 線上、OneDrive 和 Microsoft 團隊啟用 Office 365 的高級威脅防護</span><span class="sxs-lookup"><span data-stu-id="5f1f9-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="5f1f9-103">移至 https://protection.office.com 並登入。</span><span class="sxs-lookup"><span data-stu-id="5f1f9-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="5f1f9-104">選擇 [**威脅管理**  >  **原則**  >  **安全附件**]。</span><span class="sxs-lookup"><span data-stu-id="5f1f9-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="5f1f9-105">選取 [**開啟 SharePoint、OneDrive 和 Microsoft 小組的 ATP**]，然後按一下 [**儲存**]。</span><span class="sxs-lookup"><span data-stu-id="5f1f9-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="5f1f9-106">推薦以全域管理員或 SharePoint 線上管理員身分執行[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) Cmdlet，並將**DisallowInfectedFileDownload**參數設定為*true*。</span><span class="sxs-lookup"><span data-stu-id="5f1f9-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="5f1f9-107">推薦[設定](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)偵測到的檔案的警示。</span><span class="sxs-lookup"><span data-stu-id="5f1f9-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="5f1f9-108">ATP 只會掃描 SharePoint Online、OneDrive 或 Microsoft 小組中的每一個檔案。</span><span class="sxs-lookup"><span data-stu-id="5f1f9-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="5f1f9-109">檔案會透過使用共用和來賓活動事件的處理常式進行非同步掃描，並使用智慧試探法和威脅信號來識別惡意檔。</span><span class="sxs-lookup"><span data-stu-id="5f1f9-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="5f1f9-110">請參閱[ATP 的 SharePoint、OneDrive 和 Microsoft 團隊](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)。</span><span class="sxs-lookup"><span data-stu-id="5f1f9-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>