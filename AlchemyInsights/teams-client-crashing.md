---
title: Teams 用戶端當機？
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
- "9002323"
- "4512"
ms.openlocfilehash: 39310233eae83ceb18c6ff82451ae747f3c50048
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691098"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="66387-102">Teams 用戶端當機？</span><span class="sxs-lookup"><span data-stu-id="66387-102">Teams client crashing?</span></span>

<span data-ttu-id="66387-103">如果您的 Teams 用戶端當機，請嘗試下列操作：</span><span class="sxs-lookup"><span data-stu-id="66387-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="66387-104">如果您使用的是 Teams 傳統型應用程式，請[確定應用程式已完全更新](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。</span><span class="sxs-lookup"><span data-stu-id="66387-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="66387-105">請確定所有 [Microsoft 365 URL 和位址範圍](https://docs.microsoft.com/microsoftteams/connectivity-issues)皆可存取。</span><span class="sxs-lookup"><span data-stu-id="66387-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="66387-106">使用您的租用戶系統管理員帳戶登入，並檢查您的[服務健康情況儀表板](https://docs.microsoft.com/office365/enterprise/view-service-health)，確認沒有中斷或服務降級。</span><span class="sxs-lookup"><span data-stu-id="66387-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="66387-107">解除安裝後重新安裝 Teams 應用程式 (連結)</span><span class="sxs-lookup"><span data-stu-id="66387-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="66387-108">在電腦上瀏覽至 %appdata%\Microsoft\teams\ 資料夾，刪除該目錄中的所有檔案。</span><span class="sxs-lookup"><span data-stu-id="66387-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="66387-109">[下載並安裝 Teams 應用程式](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)，如果可能，請以系統管理員身分安裝 Teams (先以滑鼠右鍵按一下 Teams 安裝程式，如果有的話，接著請選取 [以系統管理員身分執行])。</span><span class="sxs-lookup"><span data-stu-id="66387-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="66387-110">如果 Teams 用戶端仍然當機，您是否能重現問題？</span><span class="sxs-lookup"><span data-stu-id="66387-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="66387-111">如果可以：</span><span class="sxs-lookup"><span data-stu-id="66387-111">If so:</span></span>

1. <span data-ttu-id="66387-112">使用步驟收錄程式擷取您的步驟。</span><span class="sxs-lookup"><span data-stu-id="66387-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="66387-113">關閉所有不必要或機密的應用程式。</span><span class="sxs-lookup"><span data-stu-id="66387-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="66387-114">啟動步驟收錄程式，然後在以受影響使用者帳戶登入時重現問題。</span><span class="sxs-lookup"><span data-stu-id="66387-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="66387-115">[收集擷取記錄之重現步驟的 Teams 記錄檔](https://docs.microsoft.com/microsoftteams/log-files)。</span><span class="sxs-lookup"><span data-stu-id="66387-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="66387-116">**備註**：務必擷取受影響使用者的登入位址。</span><span class="sxs-lookup"><span data-stu-id="66387-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="66387-117">收集傾印和/或錯誤容器資訊 (Windows)。</span><span class="sxs-lookup"><span data-stu-id="66387-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="66387-118">在發生當機的電腦上啟動 Windows Powershell，並執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="66387-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="66387-119">將檔案附加到您的支援案例。</span><span class="sxs-lookup"><span data-stu-id="66387-119">Attach the file to your support case.</span></span>
